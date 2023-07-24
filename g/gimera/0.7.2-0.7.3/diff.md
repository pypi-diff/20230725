# Comparing `tmp/gimera-0.7.2.tar.gz` & `tmp/gimera-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.7.2.tar", last modified: Mon Jul 17 10:17:10 2023, max compression
+gzip compressed data, was "gimera-0.7.3.tar", last modified: Mon Jul 24 22:29:47 2023, max compression
```

## Comparing `gimera-0.7.2.tar` & `gimera-0.7.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:17:10.113565 gimera-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 10:16:19.000000 gimera-0.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-17 10:17:10.113565 gimera-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-17 10:16:19.000000 gimera-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:17:10.113565 gimera-0.7.2/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37461 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:17:10.113565 gimera-0.7.2/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 10:17:10.113565 gimera-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-17 10:16:19.000000 gimera-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:47.524883 gimera-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 22:29:00.000000 gimera-0.7.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-24 22:29:47.524883 gimera-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-24 22:29:00.000000 gimera-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:47.524883 gimera-0.7.3/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28893 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:47.524883 gimera-0.7.3/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 22:29:47.524883 gimera-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-24 22:29:00.000000 gimera-0.7.3/setup.py
```

### Comparing `gimera-0.7.2/LICENSE.txt` & `gimera-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.7.2/PKG-INFO` & `gimera-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.2
+Version: 0.7.3
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.2/README.md` & `gimera-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.7.2/gimera/config.py` & `gimera-0.7.3/gimera/config.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.2/gimera/gimera.py` & `gimera-0.7.3/gimera/gimera.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 #!/usr/bin/env python3
 import time
 import tempfile
 import re
 from contextlib import contextmanager
-import shutil
 import os
 from datetime import datetime
 import inquirer
 import click
 import json
 import yaml
 import sys
 import subprocess
 from pathlib import Path
 from .repo import Repo, Remote
 from .gitcommands import GitCommands
 from .tools import _raise_error, safe_relative_to, is_empty_dir, _strip_paths
 from .tools import yieldlist
+from .tools import rsync
 from .consts import gitcmd as git
-from .consts import inquirer_theme
 from .tools import prepare_dir
 from .tools import wait_git_lock
 from .tools import rmtree
-from .tools import confirm
-from .tools import temppath
-from .tools import path1inpath2
 from .consts import REPO_TYPE_INT, REPO_TYPE_SUB
 from .config import Config
+from .patches import make_patches
+from .patches import _apply_patches
+from .patches import _apply_patchfile
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -193,15 +192,15 @@
     recursive,
     no_patches,
     missing,
     remove_invalid_branches,
     non_interactive,
 ):
     if non_interactive:
-        os.environ['GIMERA_NON_INTERACTIVE'] = '1'
+        os.environ["GIMERA_NON_INTERACTIVE"] = "1"
     if all_integrated and all_submodule:
         _raise_error("Please set either -I or -S")
     ttype = None
     ttype = REPO_TYPE_INT if all_integrated else ttype
     ttype = REPO_TYPE_SUB if all_submodule else ttype
 
     repos = list(_expand_repos(repos))
@@ -286,15 +285,15 @@
         _turn_into_correct_repotype(main_repo, repo, config)
         if repo.type == REPO_TYPE_SUB:
             _make_sure_subrepo_is_checked_out(main_repo, repo)
             _fetch_latest_commit_in_submodule(main_repo, repo, update=update)
         elif repo.type == REPO_TYPE_INT:
             if not no_patches:
                 try:
-                    _make_patches(main_repo, repo)
+                    make_patches(main_repo, repo)
                 except Exception as ex:
                     msg = f"Error making patches for: {repo.path}"
                     _raise_error(msg)
 
             try:
                 _update_integrated_module(
                     main_repo, repo, update, parallel_safe, **options
@@ -375,264 +374,48 @@
     main_repo.X(
         *(git + ["submodule", "update", "--init", "--recursive", repo_yml.path])
     )
     if not path.exists():
         _raise_error("After submodule update the path {repo_yml['path']} did not exist")
 
 
-def _technically_make_patch(repo, path):
-    repo.X("git", "add", path)
-    repo.X("git", "commit", "-m", "for patch")
-
-    patch_content = Repo(path).out(
-        "git", "format-patch", "HEAD~1", "--stdout", "--relative"
-    )
-    repo.X("git", "reset", "HEAD~1")
-    return patch_content
-
-
-def _make_patches(main_repo, repo_yml):
-    subrepo_path = main_repo.path / repo_yml.path
-    if not subrepo_path.exists():
-        return
-    subrepo = main_repo.get_submodule(repo_yml.path, force=True)
-    changed_files = subrepo.filterout_submodules(subrepo.all_dirty_files)
-    untracked_files = subrepo.filterout_submodules(subrepo.untracked_files)
-    if not changed_files:
-        return
-
-    files_in_lines = "\n".join(map(str, sorted(changed_files)))
-    if os.getenv("GIMERA_NON_INTERACTIVE") == "1":
-        correct = True
-    else:
-        choice_yes = "Yes - make a patch"
-        if repo_yml.edit_patchfile:
-            choice_yes = f"Merge all changes into patchfile {repo_yml.edit_patchfile}"
-        questions = [
-            inquirer.List(
-                "correct",
-                message=f"Continue making patches for: {files_in_lines}",
-                default="no",
-                choices=[
-                    choice_yes,
-                    "Abort",
-                    "Ignore",
-                ],
-            )
-        ]
-        answers = inquirer.prompt(questions, theme=inquirer_theme)
-        correct = answers["correct"][0]
-        if correct == "Y":
-            correct = True
-        elif correct == "A":
-            correct = False
-    if not correct:
+def _get_cache_dir(main_repo, repo_yml):
+    url = repo_yml.url
+    if not url:
+        click.secho(f"Missing url: {json.dumps(repo_yml, indent=4)}")
         sys.exit(-1)
-    if correct == "I":
-        return
-
-    to_reset = []
-    if repo_yml.type == REPO_TYPE_INT:
-        cwd = main_repo.working_dir
-    else:
-        raise NotImplementedError(repo_yml.type)
-    # TODO does this work in subgimeras? because now we have parent_config stored
-    repo = Repo(cwd)
-    for untracked_file in untracked_files:
-        # add with empty blob to index, appears like that then:
-        """
-        Changes not staged for commit:
-        (use "git add <file>..." to update what will be committed)
-        (use "git restore <file>..." to discard changes in working directory)
-                modified:   roles2/sub1/file2.txt
-                new file:   roles2/sub1/file3.txt
-        """
-        repo.X("git", "add", "-N", untracked_file)
-        to_reset.append(untracked_file)
-        del untracked_file
-
-    subdir_path = Path(main_repo.working_dir) / repo_yml.path
-    patch_content = _technically_make_patch(repo, subdir_path)
-
-    if not repo_yml.all_patch_dirs(rel_or_abs="relative"):
-        _raise_error(
-            "Please define at least one directory, "
-            f"where patches are stored for {repo_yml.path}"
-        )
-
-    remove_edit_patchfile = False
-    patch_filename = datetime.now().strftime("%Y%m%d_%H%M%S")
-    if repo_yml.edit_patchfile:
+    path = Path(os.path.expanduser("~/.cache/gimera")) / url.replace(":", "_").replace(
+        "/", "_"
+    )
+    path.parent.mkdir(exist_ok=True, parents=True)
+    if not path.exists():
         click.secho(
-            "Editing a patch is in progress - continuing for "
-            f"{repo_yml.edit_patchfile}",
+            f"Caching the repository {repo_yml.url} for quicker reuse",
             fg="yellow",
         )
-        ttype = repo_yml._get_type_of_patchfolder(Path(repo_yml.edit_patchfile).parent)
-        if (ttype) == "from_outside":
-            edit_patchfile = (
-                repo_yml.config.config_file.parent / repo_yml.edit_patchfile
-            )
-        elif ttype == "internal":
-            edit_patchfile = (
-                repo_yml.config.config_file.parent
-                / repo_yml.path
-                / repo_yml.edit_patchfile
-            )
-        else:
-            raise NotImplementedError(ttype)
-        patch_dir = [
-            x
-            for x in repo_yml.all_patch_dirs("absolute")
-            if x._path == edit_patchfile.parent
-        ][0]
-        patch_filename = Path(repo_yml.edit_patchfile).name
-        remove_edit_patchfile = True
-    else:
-        patchdirs = repo_yml.all_patch_dirs(rel_or_abs="absolute")
-        if len(patchdirs) == 1:
-            patch_dir = patchdirs[0]
-        else:
-            questions = [
-                inquirer.List(
-                    "path",
-                    message="Please choose a directory where to put the patch file.",
-                    # choices=["Type directory"] + patchdirs,
-                    choices=patchdirs,
-                )
-            ]
-            answers = inquirer.prompt(questions, theme=inquirer_theme)
-            # if answers["path"] == "Type directory":
-            #     questions = [
-            #         inquirer.Text(
-            #             "path",
-            #             message="Where shall i put the patch file? (directory)",
-            #             default="./",
-            #         )
-            #     ]
-            #     answers = inquirer.prompt(questions, theme=inquirer_theme)
-            patch_dir = answers["path"]
-
-    patch_dir._path.mkdir(exist_ok=True, parents=True)
-
-    if os.getenv("GIMERA_NON_INTERACTIVE") != "1" and not repo_yml.edit_patchfile:
-        questions = [
-            inquirer.Text(
-                "filename",
-                message="Please give the patch-file a name",
-            )
-        ]
-        answers = inquirer.prompt(questions, theme=inquirer_theme)
-        if not answers:
-            sys.exit(-1)
-        patch_filename = answers["filename"]
-    if not patch_filename:
-        _raise_error("No filename provided")
-
-    if not patch_filename.endswith(".patch"):
-        patch_filename += ".patch"
-
-    patch_location = None
-    if path1inpath2(patch_dir._path, subrepo.path):
-        # case: patch must be put within patches folder of the integrated module
-        # so it must be uploaded via a temp path; and the latest version must be
-        # pulled
-        patch_location = "internal"
-
-        hex = _clone_directory_and_add_patch_file(
-            branch=repo_yml.branch,
-            repo_url=repo_yml.url,
-            patch_path=patch_dir._path.relative_to(subrepo_path) / patch_filename,
-            content=patch_content,
-        )
-        # write latest hex to gimera
-        repo_yml.config._store(
-            repo_yml,
-            {
-                "sha": hex,
-            },
-        )
-        repo_yml.sha = hex
-
-    else:
-        # case: patch file is in main repo and can be committed there
-        (patch_dir._path / patch_filename).write_text(patch_content)
-        patch_location = "outside"
-
-    for to_reset in to_reset:
-        main_repo.X("git", "reset", to_reset)
-
-    if patch_location == "outside":
-        # commit the patches - do NOT - could lie in submodule - is hard to do
-        subprocess.check_call(["git", "add", repo_yml.path], cwd=main_repo.working_dir)
-        subprocess.check_call(
-            ["git", "add", patch_dir._path], cwd=main_repo.working_dir
-        )
-        subprocess.check_call(
-            ["git", "commit", "-m", f"added patch {patch_filename}"],
-            cwd=main_repo.working_dir,
-        )
-
-    if remove_edit_patchfile:
-        repo_yml.config._store(
-            repo_yml,
-            {
-                "edit_patchfile": "",
-            },
-        )
-
-
-def _clone_directory_and_add_patch_file(branch, repo_url, patch_path, content):
-    with temppath() as path:
-        path = path / "repo"
-        subprocess.check_call(["git", "clone", repo_url, path])
-        repo = Repo(path)
-        repo.X("git", "checkout", branch)
-        patch_path = path / patch_path
-        assert patch_path.relative_to(path)
-        patch_path.parent.mkdir(exist_ok=True, parents=True)
-        patch_path.write_text(content)
-        repo.X("git", "add", patch_path.relative_to(path))
-        repo.X("git", "commit", "-m", f"added patchfile: {patch_path}")
-        repo.X("git", "push")
-        return repo.hex
+        with prepare_dir(path) as _path:
+            Repo(main_repo.path).X("git", "clone", url, _path)
+    return path
 
 
 def _update_integrated_module(
     main_repo,
     repo_yml,
     update,
     parallel_safe,
     **options,
 ):
     """
     Put contents of a git repository inside the main repository.
     """
 
     # TODO eval parallelsafe
-    def _get_cache_dir():
-        url = repo_yml.url
-        if not url:
-            click.secho(f"Missing url: {json.dumps(repo_yml, indent=4)}")
-            sys.exit(-1)
-        path = Path(os.path.expanduser("~/.cache/gimera")) / url.replace(
-            ":", "_"
-        ).replace("/", "_")
-        path.parent.mkdir(exist_ok=True, parents=True)
-        if not path.exists():
-            click.secho(
-                f"Caching the repository {repo_yml.url} for quicker reuse",
-                fg="yellow",
-            )
-            with prepare_dir(path) as _path:
-                Repo(main_repo.path).X("git", "clone", url, _path)
-        return path
 
     # use a cache directory for pulling the repository and updating it
-    local_repo_dir = _get_cache_dir()
+    local_repo_dir = _get_cache_dir(main_repo, repo_yml)
     with wait_git_lock(local_repo_dir):
         if not os.access(local_repo_dir, os.W_OK):
             _raise_error(f"No R/W rights on {local_repo_dir}")
         repo = Repo(local_repo_dir)
         repo.X("git", "remote", "set-url", "origin", repo_yml.url)
         repo.X("git", "fetch", "--all")
         branch = str(repo_yml.branch)
@@ -672,25 +455,15 @@
         with _apply_merges(repo, repo_yml, parallel_safe) as (repo, remote_refs):
             dest_path = Path(main_repo.path) / repo_yml.path
             dest_path.parent.mkdir(exist_ok=True, parents=True)
             # BTW: delete-after cannot removed unused directories - cool to know; is
             # just standarded out
             if dest_path.exists():
                 rmtree(dest_path)
-            subprocess.check_call(
-                [
-                    "rsync",
-                    "-ar",
-                    "--exclude=.git",
-                    "--delete-after",
-                    str(repo.path) + "/",
-                    str(dest_path) + "/",
-                ],
-                cwd=main_repo.working_dir,
-            )
+            rsync(repo.path, dest_path, exclude=[".git"])
             msg = [f"Merged: {repo_yml.url}"]
             for remote, ref in remote_refs:
                 msg.append(f"Merged {remote.url}:{ref}")
             main_repo.commit_dir_if_dirty(repo_yml.path, "\n".join(msg))
 
         del repo
 
@@ -809,27 +582,14 @@
         ):
             if not error_ok:
                 _raise_error(f"Error applying patch: {file}")
     except Exception as ex:  # pylint: disable=broad-except
         _raise_error(str(ex))
 
 
-def _apply_patches(repo_yml):
-    for patchdir in repo_yml.all_patch_dirs(rel_or_abs="absolute") or []:
-        # with patchdir.path as dir:
-        if not patchdir._path.exists():
-            patchdir._path.mkdir(parents=True)
-        for file in sorted(patchdir._path.rglob("*.patch")):
-            if repo_yml.ignore_patchfile(file):
-                continue
-            click.secho((f"Applying patch {file}"), fg="blue")
-            # Git apply fails silently if applied within local repos
-            _apply_patchfile(file, patchdir.apply_from_here_dir, error_ok=False)
-
-
 def _commit_submodule_inside_clean_but_not_linked_to_parent(main_repo, subrepo):
     """
     If the submodule is clean inside but is not committed to the parent
     repository, this module does that.
     """
     if subrepo.dirty:
         return False
@@ -849,15 +609,15 @@
             f"gimera: updated submodule at {subrepo.path.relative_to(main_repo.path)} "
             f"to latest version {sha}"
         ),
     )
 
 
 def _fetch_latest_commit_in_submodule(main_repo, repo_yml, update=False):
-    path = Path(main_repo.working_dir) / repo_yml.path
+    path = Path(main_repo.path) / repo_yml.path
     if not path.exists():
         return
     subrepo = main_repo.get_submodule(repo_yml.path)
     if subrepo.dirty:
         _raise_error(
             f"Directory {repo_yml.path} contains modified "
             "files. Please commit or purge before!"
```

### Comparing `gimera-0.7.2/gimera/gitcommands.py` & `gimera-0.7.3/gimera/gitcommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             if str(path.relative_to(self.path)) == "gimera.yml":
                 continue
             files.append(path)
         return bool(files)
 
     def simple_commit_all(self, msg="."):
         self.X("git", "add", ".")
-        self.X("git", "commit", "-am", msg)
+        self.X("git", "commit", "--allow-empty","-am", msg)
 
     @property
     def hex(self):
         return self.out("git", "log", "-n", "1", "--pretty=%H")
 
     def checkout(self, ref, force=False):
         self.X("git", "checkout", "-f" if force else None, ref)
```

### Comparing `gimera-0.7.2/gimera/repo.py` & `gimera-0.7.3/gimera/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .tools import yieldlist, X, safe_relative_to, _raise_error, rmtree
 from .consts import gitcmd as git
 
 
 class Repo(GitCommands):
     def __init__(self, path):
         self.path = Path(path)
-        self.working_dir = Path(path)
 
     def __repr__(self):
         return f"{self.path}"
 
     def __str__(self):
         return f"{self.path}"
 
@@ -127,14 +126,22 @@
     @yieldlist
     def get_submodules(self):
         submodules = self.out("git", "submodule", "status").splitlines()
         for line in submodules:
             splitted = line.strip().split(" ")
             yield Submodule(self.next_module_root / splitted[1], self.next_module_root)
 
+    def check_ignore(self, path):
+        try:
+            self.X("git", "check-ignore", "-q", path, allow_error=False)
+        except subprocess.CalledProcessError:
+            return False
+        else:
+            return True
+
     def _fix_to_remove_subdirectories(self, config):
         # https://stackoverflow.com/questions/4185365/no-submodule-mapping-found-in-gitmodule-for-a-path-thats-not-a-submodule
         # commands may block
         # git submodule--helper works and shows something
         # git submodule says: fatal: no submodule mapping found in .gitmodules
         # there is special folder with id 16000 then, then must be removed with git rm
         # then; not tested, because then it suddenly worked
```

### Comparing `gimera-0.7.2/gimera/tools.py` & `gimera-0.7.3/gimera/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -147,7 +147,20 @@
 
 def path1inpath2(path1, path2):
     try:
         path1.relative_to(path2)
         return True
     except:
         return False
+
+def rsync(dir1, dir2, exclude=None, delete_after=True):
+    cmd = [
+                "rsync",
+                "-ar",
+    ]
+    if delete_after:
+        cmd += ["--delete-after"]
+    for X in (exclude or []):
+        cmd += [f"--exclude={X}"]
+    cmd.append(str(dir1) + "/")
+    cmd.append(str(dir2) + "/")
+    subprocess.check_call(cmd)
```

### Comparing `gimera-0.7.2/gimera.egg-info/PKG-INFO` & `gimera-0.7.3/gimera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.2
+Version: 0.7.3
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.2/setup.py` & `gimera-0.7.3/setup.py`

 * *Files identical despite different names*

