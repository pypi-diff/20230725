# Comparing `tmp/setuptools-github-0.3.0b60.tar.gz` & `tmp/setuptools-github-0.3.0b61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.0b60.tar", last modified: Tue Jul 25 14:17:49 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.0b61.tar", last modified: Tue Jul 25 18:45:41 2023, max compression
```

## Comparing `setuptools-github-0.3.0b60.tar` & `setuptools-github-0.3.0b61.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.608185 setuptools-github-0.3.0b60/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.604185 setuptools-github-0.3.0b60/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.608185 setuptools-github-0.3.0b60/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:45:41.079402 setuptools-github-0.3.0b61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 18:45:41.079402 setuptools-github-0.3.0b61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:45:41.079402 setuptools-github-0.3.0b61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:45:41.075402 setuptools-github-0.3.0b61/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 18:45:41.000000 setuptools-github-0.3.0b61/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 18:45:41.000000 setuptools-github-0.3.0b61/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:45:41.000000 setuptools-github-0.3.0b61/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 18:45:41.000000 setuptools-github-0.3.0b61/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 18:45:41.000000 setuptools-github-0.3.0b61/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 18:45:41.000000 setuptools-github-0.3.0b61/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:45:41.071402 setuptools-github-0.3.0b61/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:45:41.079402 setuptools-github-0.3.0b61/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 18:45:41.000000 setuptools-github-0.3.0b61/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:45:41.079402 setuptools-github-0.3.0b61/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 18:45:08.000000 setuptools-github-0.3.0b61/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.0b60/LICENSE` & `setuptools-github-0.3.0b61/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/PKG-INFO` & `setuptools-github-0.3.0b61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b60
+Version: 0.3.0b61
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.0b60/README.md` & `setuptools-github-0.3.0b61/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/setup.py` & `setuptools-github-0.3.0b61/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.0b61/setuptools_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b60
+Version: 0.3.0b61
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.0b60/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.0b61/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/src/setuptools_github/checks.py` & `setuptools-github-0.3.0b61/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/src/setuptools_github/cli.py` & `setuptools-github-0.3.0b61/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/src/setuptools_github/scm.py` & `setuptools-github-0.3.0b61/src/setuptools_github/scm.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,32 @@
 import re
 import dataclasses as dc
 import subprocess
 from pathlib import Path
 
 
 from typing_extensions import TypeAlias
-from typing import Union, List
+from typing import Union, List, Any
 
 
 ListOfArgs: TypeAlias = Union[str, Path, List[Union[str, Path]]]
 
 
 def to_list_of_paths(paths: ListOfArgs) -> list[Path]:
     return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
 
+class NA:
+    pass
+
+
+class GitError(Exception):
+    pass
+
+
 @dc.dataclass
 class GitRepoBranches:
     local: list[str]
     remote: list[str]
 
 
 @dc.dataclass
@@ -72,35 +80,64 @@
 
         buf = io.StringIO()
         print("\n".join([line.rstrip() for line in lines.split("\n")]), file=buf)
         return buf.getvalue()
 
 
 class GitRepo(GitRepoBase):
-    # COMMANDS FOR THE REPO HERE
+    @property
+    def config(self):
+        @dc.dataclass
+        class X:
+            repo: GitRepo
+
+            def __getitem__(self, item: str):
+                return self.repo(["config", item]).strip()
+
+            def __setitem__(self, item: str, value: Any):
+                self.repo(["config", item, str(value)])
+
+            def __contains__(self, item: str):
+                return item in self.repo(
+                    [
+                        "config",
+                        "--list",
+                        "--name-only",
+                    ]
+                ).split("\n")
+
+        return X(self)
+
     def revert(self, paths: ListOfArgs | None = None):
         sources = to_list_of_paths(paths or self.workdir)
         self(["checkout", *sources])
 
     @property
     def head(self):
         name = self(["symbolic-ref", "HEAD"]).strip()
-        txt = self(["rev-parse", name]).strip()
+        try:
+            txt = self(["rev-parse", name]).strip()
+        except subprocess.CalledProcessError as exc:
+            raise GitError(f"no branch '{name}'") from exc
         return GitRepoHead(name=name, target=GitRepoHead.GitRepoHeadHex(txt))
 
     def status(
         self, untracked_files: str = "all", ignored: bool = False
     ) -> dict[str, int]:
         mapper = {
             "??": 128 if untracked_files == "all" else None,
             " D": 512,
             " M": 256,
         }
         result = {}
-        for line in self(["status", "--porcelain"]).split("\n"):
+        try:
+            txt = self(["status", "--porcelain"])
+        except subprocess.CalledProcessError as exc:
+            raise GitError("invalid repo") from exc
+        for line in txt.split("\n"):
             if not line.strip():
                 continue
             tag, filename = line[:2], line[3:]
             value = mapper[tag]
             if value:
                 result[filename] = value
         return result
```

### Comparing `setuptools-github-0.3.0b60/src/setuptools_github/script.py` & `setuptools-github-0.3.0b61/src/setuptools_github/script.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 """
 from __future__ import annotations
 import logging
 import re
 from pathlib import Path
 import argparse
-from . import cli, tools
-import pygit2  # type: ignore
+from . import cli, tools, scm
 
 
 log = logging.getLogger(__name__)
 
 
 def add_arguments(parser: argparse.ArgumentParser):
     parser.add_argument("--master", help="the 'master' branch")
@@ -34,26 +33,27 @@
     parser.add_argument("mode", choices=["micro", "minor", "major", "make-beta"])
 
 
 def process_options(
     options: argparse.Namespace, error: cli.ErrorFn
 ) -> argparse.Namespace:
     try:
-        options.repo = repo = pygit2.Repository(options.workdir)
-    except pygit2.GitError:
+        options.repo = repo = scm.GitRepo(options.workdir)
+        repo.status()
+    except scm.GitError:
         error(
             "no git directory",
             "It looks the repository is not a git repo",
             hint="init the git directory",
         )
     log.info("working dir set to '%s'", options.workdir)
     try:
         branch = repo.head.shorthand
         log.info("current branch set to '%s'", branch)
-    except pygit2.GitError:
+    except scm.GitError:
         error(
             "invalid git repository",
             """
               It looks the repository doesn't have any branch,
               you should:
                 git checkout --orphan <branch-name>
               """,
@@ -77,74 +77,55 @@
         options.error(f"cannot find version file {options.initfile}")
 
     version = tools.get_module_var(options.initfile, "__version__")
     assert version
     log.info("got version %s for branch '{options.repo.head.name}'", version)
 
     # fetching all remotes
-    [remote.fetch() for remote in options.repo.remotes]
+    options.repo(["fetch", "--all"])
 
     if options.mode == "make-beta":
         if options.repo.head.name != f"refs/heads/{master}":
             options.error(
                 f"wrong branch '{options.repo.head.name}', expected '{master}'"
             )
 
         for branch in [*options.repo.branches.local, *options.repo.branches.remote]:
             if not branch.endswith(f"beta/{version}"):
                 continue
             options.error(f"branch '{branch}' already present")
         log.info("creating branch '%s'", f"/beta/{version}")
-        commit = options.repo.revparse_single("HEAD")
-        options.repo.branches.local.create(f"/beta/{version}", commit)
+        options.repo.branch(f"beta/{version}", master)
+        options.repo(["checkout", master])
     elif options.mode in {"micro", "minor", "major"}:
         # we need to be in the beta/N.M.O branch
         expr = re.compile(r"refs/heads/beta/(?P<beta>\d+([.]\d+)*)$")
         if not (match := expr.search(options.repo.head.name)):
             options.error(
                 f"wrong branch '{options.repo.head.name}' "
                 f"expected 'refs/heads/beta/{version}'"
             )
             return
         local = match.group("beta")
         if local != version:
             options.error(f"wrong version file {version=} != {local}")
 
         # tag
-        obj = options.repo.get(options.repo.head.target)
-        options.repo.create_tag(
-            f"release/{version}",
-            obj.oid,
-            pygit2.GIT_OBJ_COMMIT,
-            obj.author,
-            f"release {version}",
-        )
+        options.repo(["tag", "-a", f"release/{version}", "-m", f"released {version}"])
 
         # switch to master
-        branch = options.repo.lookup_branch(master)
-        head = options.repo.lookup_reference(branch.name)
-        options.repo.checkout(head.name)
+        options.repo(["checkout", master])
 
         # bump version
-        tools.set_module_var(
-            options.initfile, "__version__", tools.bump_version(version, options.mode)
-        )
+        new_version = tools.bump_version(version, options.mode)
+        tools.set_module_var(options.initfile, "__version__", new_version)
 
         # commit
-        ref = options.repo.head.name
-        parents = [options.repo.head.target]
-        obj = options.repo.get(options.repo.head.target)
-        index = options.repo.index
-        index.add(
-            str(options.initfile.relative_to(options.repo.workdir)).replace("\\", "/")
-        )
-        index.write()
-        tree = index.write_tree()
-        options.repo.create_commit(
-            ref, obj.author, obj.author, "release", tree, parents
+        options.repo.commit(
+            options.initfile, f"version bump {version} -> {new_version}"
         )
 
     else:
         options.error(f"unsupported mode {options.mode=}")
         raise RuntimeError(f"unsupported mode {options.mode=}")
```

### Comparing `setuptools-github-0.3.0b60/src/setuptools_github/tools.py` & `setuptools-github-0.3.0b61/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/tests/conftest.py` & `setuptools-github-0.3.0b61/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/tests/test_checks.py` & `setuptools-github-0.3.0b61/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/tests/test_cli.py` & `setuptools-github-0.3.0b61/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/tests/test_conftest.py` & `setuptools-github-0.3.0b61/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b60/tests/test_scm.py` & `setuptools-github-0.3.0b61/tests/test_scm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import subprocess
 
 import pytest
-import pygit2
 
 from setuptools_github import scm
 
 
 def test_lookup(git_project_factory):
     repo = git_project_factory().create("0.0.0")
     dstdir = repo.workdir / "a" / "b" / "c"
@@ -17,29 +16,21 @@
 
 
 def test_handle_remote_and_local_repos(git_project_factory):
     "test branch handling across repos"
 
     def check_branches(repo):
         srepo = scm.GitRepo(repo.workdir)
-        grepo = pygit2.Repository(repo.workdir)
         assert set(repo.branches.local) == set(srepo.branches.local)
-        assert set(srepo.branches.local) == set(grepo.branches.local)
         assert set(repo.branches.remote) == set(srepo.branches.remote)
-        assert set(srepo.branches.remote) == set(grepo.branches.remote)
 
     # Create a repository with two beta branches tagged
     repo = git_project_factory("test_check_version-repo").create("0.0.0")
     repo.branch("beta/0.0.3")
-    # repo(["tag", "-m", "release", "release/0.0.3"])
-    rx = pygit2.Repository(repo.workdir)
-    obj = rx.get(rx.head.target)
-    rx.create_tag(
-        "release/0.0.3", obj.oid, pygit2.GIT_OBJ_COMMIT, obj.author, "release"
-    )
+    repo(["tag", "-m", "release", "release/0.0.3"])
 
     repo.branch("beta/0.0.4")
     repo(["tag", "-m", "release", "release/0.0.4"])
     repo(["checkout", "master"])
     assert (
         repo.dumps(mask=True)
         == f"""\
```

### Comparing `setuptools-github-0.3.0b60/tests/test_script.py` & `setuptools-github-0.3.0b61/tests/test_script.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from argparse import Namespace
 from setuptools_github import script
 
-import pytest
-
-import pygit2
-
 
 class MyError(Exception):
     pass
 
 
 def errorfn(message, explain="", hint=""):
     raise MyError(message, explain, hint)
@@ -33,34 +29,33 @@
     options = Namespace(workdir=repo.workdir)
     try:
         script.process_options(options, error=errorfn)  # , error=error)
     except MyError as e:
         assert e.args[0] == "invalid git repository"
 
 
-@pytest.mark.skipif(not pygit2, reason="pygit2 not installed")
 def test_main_make_beta(git_project_factory):
     repo = git_project_factory().create(force=True)
 
     options = Namespace(
         initfile=repo.workdir / "src" / "__init__.py",
-        repo=pygit2.Repository(repo.workdir),
+        repo=repo,
         mode="make-beta",
         error=errorfn,
         master=None
     )
     try:
         script.main.__wrapped__(options)
     except MyError as exc:
         assert exc.args[0].startswith("cannot find version file")
 
     repo = git_project_factory().create(version="0.0.0")
     options = Namespace(
         initfile=repo.workdir / "src" / "__init__.py",
-        repo=pygit2.Repository(repo.workdir),
+        repo=repo,
         mode="make-beta",
         error=errorfn,
         master="master"
     )
     script.main.__wrapped__(options)
     assert set(repo.branches.local) == {"master", "beta/0.0.0"}
 
@@ -74,15 +69,15 @@
 
     repo = git_project_factory().create(version="0.0.0")
     old = repo.branch("beta/0.0.0", "master")
     repo(["checkout", old])
 
     options = Namespace(
         initfile=repo.workdir / "src" / "__init__.py",
-        repo=pygit2.Repository(repo.workdir),
+        repo=repo,
         mode="micro",
         error=errorfn,
         master="master"
     )
     try:
         script.main.__wrapped__(options)
     except MyError as exc:
```

### Comparing `setuptools-github-0.3.0b60/tests/test_tools.py` & `setuptools-github-0.3.0b61/tests/test_tools.py`

 * *Files identical despite different names*

