# Comparing `tmp/libretro_finder-0.1.0.tar.gz` & `tmp/libretro_finder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretro_finder-0.1.0.tar", max compression
+gzip compressed data, was "libretro_finder-0.1.1.tar", max compression
```

## Comparing `libretro_finder-0.1.0.tar` & `libretro_finder-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-05 19:33:27.530061 libretro_finder-0.1.0/libretro_finder/__init__.py
--rw-r--r--   0        0        0     3653 2023-07-25 09:51:01.027591 libretro_finder-0.1.0/libretro_finder/main.py
--rw-r--r--   0        0        0     1716 2023-07-25 09:22:57.544045 libretro_finder-0.1.0/libretro_finder/utils.py
--rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.1.0/LICENSE
--rw-r--r--   0        0        0      856 2023-07-25 11:18:21.174665 libretro_finder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2355 2023-07-06 09:26:25.948609 libretro_finder-0.1.0/README.md
--rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 libretro_finder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1760 2023-07-25 09:53:52.648295 libretro_finder-0.1.1/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:33:27.530061 libretro_finder-0.1.1/libretro_finder/__init__.py
+-rw-r--r--   0        0        0     3667 2023-07-25 12:41:28.893089 libretro_finder-0.1.1/libretro_finder/main.py
+-rw-r--r--   0        0        0     1716 2023-07-25 09:22:57.544045 libretro_finder-0.1.1/libretro_finder/utils.py
+-rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.1.1/LICENSE
+-rw-r--r--   0        0        0      869 2023-07-25 13:31:25.789129 libretro_finder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3931 2023-07-25 13:22:21.422636 libretro_finder-0.1.1/README.md
+-rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 libretro_finder-0.1.1/PKG-INFO
```

### Comparing `libretro_finder-0.1.0/libretro_finder/main.py` & `libretro_finder-0.1.1/libretro_finder/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from libretro_finder.utils import match_arrays, recursive_hash
 
 
 def organize(
     search_dir: pathlib.Path, output_dir: pathlib.Path, glob: str = "*"
 ) -> None:
     """
-    Non-destructive function that finds, copies and refactors files to the format expected by 
-    libretro (and its cores). This is useful if you source your BIOS files from many different 
+    Non-destructive function that finds, copies and refactors files to the format expected by
+    libretro (and its cores). This is useful if you source your BIOS files from many different
     places and have them saved them under different names (often with duplicates).
 
     :param search_dir:
     :param output_dir:
     :param glob:
     :param overwrite:
     :return:
@@ -45,15 +45,15 @@
     # np.unique and indexing doesn't merit a dedicated function but it should still be tested
     assert np.array_equal(np.array(system_subset["md5"].values), hashes)
     assert system_subset["name"].size == system_subset["name"].unique().size
 
     # printing matches per system
     matches = system_subset.groupby("system").count()
     print(
-        f"{matches['name'].sum()} matching BIOS files were found for {matches.shape[0]}" \
+        f"{matches['name'].sum()} matching BIOS files were found for {matches.shape[0]}"
         "unique systems:"
     )
     for name, row in matches.iterrows():
         print(f"\t{name} ({row['name']})")
 
     # copying matching files to output_dir using structure specified by libretro
     dsts = system_subset["name"].values
@@ -68,34 +68,36 @@
             continue
         if parent != output_dir:
             parent.mkdir(parents=True, exist_ok=True)
 
         shutil.copy(src=srcs[i], dst=dst)
 
 
-if __name__ == "__main__":
+def main() -> None:
+    """Simple argparse wrapper for packaging."""
     parser = argparse.ArgumentParser(
-        description="CLI that finds, copies and refactors BIOS files" \
-        "to the format expected by libretro.",
+        description="CLI that finds, copies and refactors BIOS files "
+        "to the format expected by libretro (i.e. name and directory structure).",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("search_dir", help="Directory to look for BIOS files", type=str)
     parser.add_argument(
-        "output_dir", help="Directory to copy found BIOS files to", type=str
+        "output_dir", help="Directory to refactor found BIOS files to", type=str
     )
     parser.add_argument(
         "-g",
         "--glob",
         help="Glob pattern to use for file matching",
         type=str,
         default="*",
     )
-    parser.add_argument(
-        "-o", "--overwrite", help="Overwrite output", action="store_true"
-    )
     args = vars(parser.parse_args())
 
     search_directory = pathlib.Path(args["search_dir"])
     output_directory = pathlib.Path(args["output_dir"])
     search_glob = args["glob"]
 
     organize(search_dir=search_directory, output_dir=output_directory, glob=search_glob)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `libretro_finder-0.1.0/libretro_finder/utils.py` & `libretro_finder-0.1.1/libretro_finder/utils.py`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.0/LICENSE` & `libretro_finder-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.0/pyproject.toml` & `libretro_finder-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 [tool.poetry]
 name = "libretro-finder"
-version = "0.1.0"
-description = "Command line utility that looks for specific BIOS files for libretro cores and, if found, refactors them to the expected format as documented [here](https://github.com/libretro/libretro-database/blob/4a98ea9726b3954a4e5a940d255bd14c307ddfba/dat/System.dat)."
+version = "0.1.1"
+description = "Command line utility that looks for specific BIOS files for libretro cores and, if found, refactors them to the expected format (i.e. name and directory structure)."
 authors = ["Jasper <j.siebring92@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
-packages = [{include = "libretro_finder"}]
+packages = [
+    {include = "libretro_finder"},
+    {include = "config"},
+]
+
+[tool.poetry.scripts]
+libretro_finder = "libretro_finder.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.25.1"
 pandas = "^2.0.3"
 tqdm = "^4.65.0"
 
@@ -20,8 +26,8 @@
 mypy = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint.'MESSAGES CONTROL']
-disable = "C0114"
+disable = "C0114"
```

