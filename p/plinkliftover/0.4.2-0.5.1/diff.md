# Comparing `tmp/plinkliftover-0.4.2.tar.gz` & `tmp/plinkliftover-0.5.1.tar.gz`

## Comparing `plinkliftover-0.4.2.tar` & `plinkliftover-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.dockerignore
--rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.editorconfig
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.flake8
--rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     2819 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/CHANGELOG.md
--rwxr-xr-x   0        0        0     3352 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     2889 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/Makefile
--rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/SECURITY.md
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/cookiecutter-config-file.yml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/renovate.json
--rwxr-xr-x   0        0        0     1265 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/setup.cfg
--rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/.stale.yml
--rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/PULL_REQUEST_TEMPLATE.md
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/dependabot.yml
--rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/release-drafter.yml
--rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/config.yml
--rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/workflows/greetings.yml
--rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/workflows/release-drafter.yml
--rwxr-xr-x   0        0        0     1524 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.vscode/launch.json
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/docker/Dockerfile
--rwxr-xr-x   0        0        0      776 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/docker/README.md
--rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/__init__.py
--rwxr-xr-x   0        0        0     4767 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/__main__.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/bed2map.py
--rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/liftover.py
--rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/logger.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/map2bed.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/py.typed
--rwxr-xr-x   0        0        0    10552 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.gitignore
--rwxr-xr-x   0        0        0    34902 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/LICENSE.md
--rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/README.md
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.dockerignore
+-rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.editorconfig
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.flake8
+-rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     3363 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0     3352 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     2889 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/Makefile
+-rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/SECURITY.md
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/cookiecutter-config-file.yml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/renovate.json
+-rwxr-xr-x   0        0        0     1265 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/setup.cfg
+-rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/.stale.yml
+-rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/dependabot.yml
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/release-drafter.yml
+-rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/workflows/greetings.yml
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.github/workflows/release-drafter.yml
+-rwxr-xr-x   0        0        0     1524 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.vscode/launch.json
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/docker/Dockerfile
+-rwxr-xr-x   0        0        0      776 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/docker/README.md
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/src/plinkliftover/__init__.py
+-rwxr-xr-x   0        0        0     4789 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/src/plinkliftover/__main__.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/src/plinkliftover/bed2map.py
+-rwxr-xr-x   0        0        0     4229 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/src/plinkliftover/liftover.py
+-rwxr-xr-x   0        0        0      827 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/src/plinkliftover/logger.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/src/plinkliftover/map2bed.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/src/plinkliftover/py.typed
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/tests/test_map2bed.py
+-rwxr-xr-x   0        0        0    10552 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/.gitignore
+-rwxr-xr-x   0        0        0    34902 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/LICENSE.md
+-rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/README.md
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 plinkliftover-0.5.1/PKG-INFO
```

### Comparing `plinkliftover-0.4.2/.pre-commit-config.yaml` & `plinkliftover-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/CHANGELOG.md` & `plinkliftover-0.5.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+** [0.5.1] - 2023-07-18
+
+*** Change
+
+- Remove ProgressParallel class. Replace all uses of this class with `joblib.Parallel`, passing "return_as=generator"
+  to speed things up/reduce memory usage
+
+
+** [0.5.0] - 2023-07-17
+
+*** Change
+
+- Overhaul how the conversions and writing work so that they are now
+  performed using a modified form of `joblib.Parallel`
+  - Replaced all for loops with using the Parallel/delayed combo
+- Replace `typer.progressbar` with `tqdm.rich` (because the latter works with the modified 
+  `joblib.Parallel` class)
+
 ** [0.4.2] - 2023-07-17
 
 *** Fix
 
 - Minimum python version
 - running `plinkliftover` with no arguments now shows the help
```

### Comparing `plinkliftover-0.4.2/CODE_OF_CONDUCT.md` & `plinkliftover-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/CONTRIBUTING.md` & `plinkliftover-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/Makefile` & `plinkliftover-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/SECURITY.md` & `plinkliftover-0.5.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/setup.cfg` & `plinkliftover-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/.stale.yml` & `plinkliftover-0.5.1/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/PULL_REQUEST_TEMPLATE.md` & `plinkliftover-0.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/dependabot.yml` & `plinkliftover-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/release-drafter.yml` & `plinkliftover-0.5.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `plinkliftover-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `plinkliftover-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/workflows/build.yml` & `plinkliftover-0.5.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.github/workflows/greetings.yml` & `plinkliftover-0.5.1/.github/workflows/greetings.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/.vscode/launch.json` & `plinkliftover-0.5.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/docker/Dockerfile` & `plinkliftover-0.5.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/docker/README.md` & `plinkliftover-0.5.1/docker/README.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/src/plinkliftover/__main__.py` & `plinkliftover-0.5.1/src/plinkliftover/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from plinkliftover import app, console, verbosity_level, version_callback
 from plinkliftover.bed2map import bed2map
 from plinkliftover.liftover import lift_bed, lift_dat, lift_ped
 from plinkliftover.logger import init_logger
 from plinkliftover.map2bed import map2bed
 
 
-@app.command(name="liftover")
+@app.command(name="liftover", no_args_is_help=True)
 def liftover(
     mapfile: Annotated[
         Path,
         typer.Argument(help="The plink MAP file to `liftOver`."),
     ],
     chainfile: Annotated[Path, typer.Argument(help="The location of the chain files to provide to `liftOver`.")],
     pedfile: Annotated[
```

### Comparing `plinkliftover-0.4.2/src/plinkliftover/bed2map.py` & `plinkliftover-0.5.1/src/plinkliftover/bed2map.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+from multiprocessing import cpu_count
 from pathlib import Path
 from typing import Annotated, Optional
 
 import typer
+from joblib import Parallel, delayed
 from loguru import logger
+from tqdm.rich import tqdm
 
 from plinkliftover import app, console, verbosity_level, version_callback
 from plinkliftover.logger import init_logger
 
 BED_LINES_LENGTH: int = 4
 
 
 def bed2map(fin: Path, fout: Path) -> bool:
     init_logger(verbosity_level)
     logger.info(f"fin: {fin}, fout: {fout}")
     console.print(
         f"Converting lifted [green]BED[/] [blue]{fin.name}[/] file back to [green]MAP[/] [yellow]{fout.name}[/]..."
     )
     lines = fin.read_text().split("\n")
-    output = []
-    with typer.progressbar(lines) as bed_lines:
-        for line in bed_lines:
-            if len(x := line.split()) == BED_LINES_LENGTH:
-                chrom, _, pos1, rs = x
-                chrom = chrom.replace("chr", "")
-                output.append(f"{chrom}\t{rs}\t0.0\t{pos1}")
-    fout.write_text("\n".join(output))
+
+    parallel = Parallel(n_jobs=cpu_count(), return_as="generator")
+    output = parallel(delayed(bedlinesplit)(x) for line in tqdm(lines) if len(x := line.split()) == BED_LINES_LENGTH)
+
+    with fout.open("w") as lines_out:
+        lines_out.writelines(output)
     return True
 
 
-@app.command(name="bed2map")
+def bedlinesplit(line: str) -> str:
+    chrom, _, pos1, rs = line
+    chrom = chrom.replace("chr", "")
+    return f"{chrom}\t{rs}\t0.0\t{pos1}\n"
+
+
+@app.command(name="bed2map", no_args_is_help=True)
 def bed2mapapp(
     bedfile: Annotated[Path, typer.Argument(help="A BED file.")],
     output: Annotated[
         Optional[Path],  # noqa UP007
         typer.Option(
             "-o",
             "--output",
```

### Comparing `plinkliftover-0.4.2/src/plinkliftover/logger.py` & `plinkliftover-0.5.1/src/plinkliftover/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def init_logger(verbose: int, msg_format: str | None = None) -> None:
     if msg_format is None:
         msg_format = "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan>·-·<level>{message}</level>"
 
     timezone = datetime.datetime.now(datetime.timezone.utc).astimezone().tzinfo
-    logger.add(f"readcounts_{datetime.datetime.now(tz=timezone).strftime('%d-%m-%Y--%H-%M-%S')}.log", level="DEBUG")
+    logger.add(f"plinkliftover_{datetime.datetime.now(tz=timezone).strftime('%d-%m-%Y--%H-%M-%S')}.log", level="DEBUG")
 
     match verbose:
         case 3:
             logger.add(stderr, format=msg_format, level="DEBUG")
         case 2:
             logger.add(stderr, format=msg_format, level="INFO")
         case 1:
```

### Comparing `plinkliftover-0.4.2/src/plinkliftover/map2bed.py` & `plinkliftover-0.5.1/src/plinkliftover/map2bed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+from multiprocessing import cpu_count
 from pathlib import Path
 from typing import Annotated, Optional
 
 import typer
+from joblib import Parallel, delayed
 from loguru import logger
+from tqdm.rich import tqdm
 
 from plinkliftover import app, console, verbosity_level, version_callback
 from plinkliftover.logger import init_logger
 
 MAP_LINE_LENGTH: int = 4
 
 
 def map2bed(fin: Path, fout: Path) -> bool:
     logger.info(f"fin: {fin}, fout: {fout}")
     console.print(
         f"Converting [green]MAP[/] file [yellow]{fin.name}[/] file to [green]UCSC BED[/] file [blue]{fout.name}[/]..."
     )
     init_logger(verbosity_level)
     lines = fin.read_text().split("\n")
-    output = []
-    with typer.progressbar(lines) as map_lines:
-        for line in map_lines:
-            if len(x := line.split()) == MAP_LINE_LENGTH:
-                chrom, rs, _, pos = x
-                output.append(f"chr{chrom}\t{int(pos)-1}\t{int(pos)}\t{rs}")
-    fout.write_text("\n".join(output))
+    parallel = Parallel(n_jobs=cpu_count(), return_as="generator")
+    output = parallel(delayed(maplinesplit)(x) for line in tqdm(lines) if len(x := line.split()) == MAP_LINE_LENGTH)
+
+    with fout.open("w") as lines_out:
+        lines_out.writelines(output)
     return True
 
 
-@app.command(name="map2bed")
+def maplinesplit(line: str) -> str:
+    chrom, rs, _, pos = line
+    return f"chr{chrom}\t{int(pos)-1}\t{int(pos)}\t{rs}\n"
+
+
+@app.command(name="map2bed", no_args_is_help=True)
 def map2bedapp(
     mapfile: Annotated[Path, typer.Argument(help="A PLINK MAP file.")],
     output: Annotated[
         Optional[Path],  # noqa UP007
         typer.Option(
             "-o",
             "--output",
```

### Comparing `plinkliftover-0.4.2/.gitignore` & `plinkliftover-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/LICENSE.md` & `plinkliftover-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/README.md` & `plinkliftover-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.2/pyproject.toml` & `plinkliftover-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "plinkliftover"
-version = "0.4.2"
+version = "0.5.1"
 description = "Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver"
 readme = "README.md"
+requires-python = ">=3.10"
 keywords = []
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-requires-python = ">=3.10"
 dependencies = [
     "psutil ==5.9.5",
     "rich ==13.4.2",
     "typer ==0.9.0",
     "loguru ==0.7.0",
+    "joblib ==1.3.1",
+    "better_exceptions",
+    "tqdm ==4.65.0",
 ]
 
 [[project.authors]]
 name = "Miles Smith"
 email = "miles-smith@omrf.org"
 
 [project.urls]
@@ -51,14 +54,15 @@
     "pyflakes ==3.0.1",
     "pylint ==2.17.4",
     "pytest ==7.4.0",
     "pyupgrade ==3.9.0",
     "safety ==2.3.4",
     "twine ==4.0.2",
     "build ==0.10.0",
+    "ruff ==0.0.278",
 ]
 
 [tool.isort]
 known_typing = "typing,types,typing_extensions,mypy,mypy_extensions"
 sections = "FUTURE,TYPING,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 include_trailing_comma = true
 default_section = "FIRSTPARTY"
```

### Comparing `plinkliftover-0.4.2/PKG-INFO` & `plinkliftover-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: plinkliftover
-Version: 0.4.2
+Version: 0.5.1
 Summary: Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver
 Project-URL: repository, https://github.com/milescsmith/plinkliftover
 Project-URL: homepage, https://github.com/milescsmith/plinkliftover
 Author-email: Miles Smith <miles-smith@omrf.org>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
+Requires-Dist: better-exceptions
+Requires-Dist: joblib==1.3.1
 Requires-Dist: loguru==0.7.0
 Requires-Dist: psutil==5.9.5
 Requires-Dist: rich==13.4.2
+Requires-Dist: tqdm==4.65.0
 Requires-Dist: typer==0.9.0
 Provides-Extra: dev
 Requires-Dist: bandit==1.7.5; extra == 'dev'
 Requires-Dist: black==23.7.0; extra == 'dev'
 Requires-Dist: build==0.10.0; extra == 'dev'
 Requires-Dist: darglint==1.8.1; extra == 'dev'
 Requires-Dist: flakehell==0.9.0; extra == 'dev'
@@ -28,14 +31,15 @@
 Requires-Dist: pre-commit==3.3.3; extra == 'dev'
 Requires-Dist: pycodestyle==2.10.0; extra == 'dev'
 Requires-Dist: pydocstyle==6.3.0; extra == 'dev'
 Requires-Dist: pyflakes==3.0.1; extra == 'dev'
 Requires-Dist: pylint==2.17.4; extra == 'dev'
 Requires-Dist: pytest==7.4.0; extra == 'dev'
 Requires-Dist: pyupgrade==3.9.0; extra == 'dev'
+Requires-Dist: ruff==0.0.278; extra == 'dev'
 Requires-Dist: safety==2.3.4; extra == 'dev'
 Requires-Dist: twine==4.0.2; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # PLINKLiftOver
 
 [![Build status](https://github.com/milescsmith/plinkliftover/workflows/build/badge.svg?branch=master&event=push)](https://github.com/milescsmith/plinkliftover/actions?query=workflow%3Abuild)
```

