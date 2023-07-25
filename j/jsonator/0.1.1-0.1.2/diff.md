# Comparing `tmp/jsonator-0.1.1.tar.gz` & `tmp/jsonator-0.1.2.tar.gz`

## Comparing `jsonator-0.1.1.tar` & `jsonator-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jsonator-0.1.1/jsonator/__init__.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jsonator-0.1.1/jsonator/jsonator.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jsonator-0.1.1/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 jsonator-0.1.1/LICENSE
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jsonator-0.1.1/README.rst
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 jsonator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 jsonator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 jsonator-0.1.2/jsonator/__init__.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 jsonator-0.1.2/jsonator/jsonator.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jsonator-0.1.2/jsonator/output.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jsonator-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jsonator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jsonator-0.1.2/README.rst
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jsonator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 jsonator-0.1.2/PKG-INFO
```

### Comparing `jsonator-0.1.1/jsonator/__init__.py` & `jsonator-0.1.2/jsonator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,37 @@
 
 from jsonator.jsonator import ReturnCode, format_json_file
 
 
 def main() -> int:
     """Main function"""
     arg_parser = argparse.ArgumentParser(
-        prog="run_mode", formatter_class=argparse.RawTextHelpFormatter
+        prog="jsonator", formatter_class=argparse.RawTextHelpFormatter
     )
     arg_parser.add_argument("path", type=Path, help="Path to the JSON file or directory")
     arg_parser.add_argument("--recursive", "-r", action="store_true", help="Scan subdirectories")
     arg_parser.add_argument(
         "--check",
         action="store_true",
         help="""Don't write the files back, just return the status.
 Return code 0 means nothing would change. 
 Return code 1 means some files would be reformatted.
 Return code 122 means file not found.
 Return code 123 means there was an internal error.""",
     )
+    arg_parser.add_argument(
+        "--diff",
+        action="store_true",
+        help="Don't write the files back, just output a diff for each file on stdout.",
+    )
+    arg_parser.add_argument(
+        "--color",
+        action="store_true",
+        help="Show colored diff. Only applies when `--diff` is given.",
+    )
 
     args = arg_parser.parse_args()
 
     if not args.path.exists():
         return ReturnCode.FILE_NOT_FOUND.value
 
     if args.path.is_dir():
@@ -42,8 +52,8 @@
 
         return (
             ReturnCode.NOTHING_WOULD_CHANGE.value
             if all_files_identical
             else ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED.value
         )
 
-    return format_json_file(args.path, args.check).value
+    return format_json_file(args.path, args.check, args.diff, args.color).value
```

### Comparing `jsonator-0.1.1/jsonator/jsonator.py` & `jsonator-0.1.2/jsonator/jsonator.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 import random
 import string
 import sys
 from enum import Enum
 from pathlib import Path
 from tempfile import gettempdir
 
+from jsonator import output
+
 INTERPRETER = Path(sys.executable).stem
+FILES_ENCODING = "utf-8"
 
 
 class ReturnCode(Enum):
     """Set of possible return codes"""
 
     NOTHING_WOULD_CHANGE = 0
     SOME_FILES_WOULD_BE_REFORMATTED = 1
@@ -34,36 +37,48 @@
 
     while temp_file.exists():
         temp_file = temp_dir / random_str()
 
     return temp_file
 
 
-def format_json_file(json_file: Path, check: bool) -> ReturnCode:
+def format_json_file(json_file: Path, check: bool, diff: bool, color: bool) -> ReturnCode:
     """
     This function formats the file in JSON format.
     It uses the json.tool module, built into Python, to create a readable JSON format.
     """
-    if check:
+    if check or diff:
         print(f"Comparing {json_file} - ", end="")
     else:
         print(f"Formatting {json_file}")
 
     tmp_file = make_temp_file()
     os.system(f"{INTERPRETER} -m json.tool {json_file} {tmp_file}")
 
-    if check:
+    if check or diff:
         is_identical = filecmp.cmp(json_file, tmp_file, shallow=False)
 
         if is_identical:
             print("Ok")
             os.unlink(tmp_file)
             return ReturnCode.NOTHING_WOULD_CHANGE
 
         print("Need to format")
+        found_diff = output.diff(
+            json_file.read_text(encoding=FILES_ENCODING),
+            tmp_file.read_text(encoding=FILES_ENCODING),
+            json_file.name,
+            tmp_file.name,
+        )
+
+        if color:
+            found_diff = output.color_diff(found_diff)
+
+        print(found_diff)
+
         os.unlink(tmp_file)
         return ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED
 
     if tmp_file.exists():
         os.unlink(json_file)
         os.rename(tmp_file, json_file)
     else:
```

### Comparing `jsonator-0.1.1/LICENSE` & `jsonator-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `jsonator-0.1.1/README.rst` & `jsonator-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.1/pyproject.toml` & `jsonator-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=0.25.1",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonator"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Sergey Fomin", email="sergiusnn@gmail.com" },
 ]
 description = "JSON formatting and validating tool"
 readme = "README.rst"
 requires-python = ">=3.5"
 classifiers = [
@@ -31,8 +31,14 @@
     "/jsonator/*",
 ]
 
 [project.scripts]
 jsonator = "jsonator:main"
 
 [tool.poetry]
-readme = "README.rst"
+readme = "README.rst"
+name = "jsonator"
+version = "0.1.2"
+authors = [
+  "Sergey Fomin <sergiusnn@gmail.com>",
+]
+description = "JSON formatting and validating tool"
```

### Comparing `jsonator-0.1.1/PKG-INFO` & `jsonator-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonator
-Version: 0.1.1
+Version: 0.1.2
 Summary: JSON formatting and validating tool
 Project-URL: Homepage, https://github.com/sfominx/jsonator
 Author-email: Sergey Fomin <sergiusnn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
```

