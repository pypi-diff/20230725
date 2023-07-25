# Comparing `tmp/git_timemachine-1.4.0.tar.gz` & `tmp/git_timemachine-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_timemachine-1.4.0.tar", max compression
+gzip compressed data, was "git_timemachine-1.5.0.tar", max compression
```

## Comparing `git_timemachine-1.4.0.tar` & `git_timemachine-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35147 2023-07-21 12:05:00.981408 git_timemachine-1.4.0/COPYING
--rw-r--r--   0        0        0      846 2023-07-21 12:05:00.981408 git_timemachine-1.4.0/README.md
--rw-r--r--   0        0        0     1661 2023-07-22 06:36:00.935006 git_timemachine-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       87 2023-07-21 12:05:00.984741 git_timemachine-1.4.0/src/git_timemachine/__init__.py
--rw-r--r--   0        0        0     1751 2023-07-22 06:26:02.154988 git_timemachine-1.4.0/src/git_timemachine/__main__.py
--rw-r--r--   0        0        0      228 2023-07-21 12:05:00.984741 git_timemachine-1.4.0/src/git_timemachine/commands/__init__.py
--rw-r--r--   0        0        0     5230 2023-07-22 06:34:14.001670 git_timemachine-1.4.0/src/git_timemachine/commands/commit.py
--rw-r--r--   0        0        0     1179 2023-07-21 12:05:00.984741 git_timemachine-1.4.0/src/git_timemachine/commands/log.py
--rw-r--r--   0        0        0      703 2023-07-21 12:05:00.984741 git_timemachine-1.4.0/src/git_timemachine/commands/review.py
--rw-r--r--   0        0        0      600 2023-07-21 12:05:00.984741 git_timemachine-1.4.0/src/git_timemachine/commands/switch_date.py
--rw-r--r--   0        0        0       41 2023-07-22 06:34:14.001670 git_timemachine-1.4.0/src/git_timemachine/config.py
--rw-r--r--   0        0        0      994 2023-07-21 12:05:00.984741 git_timemachine-1.4.0/src/git_timemachine/types.py
--rw-r--r--   0        0        0     1283 2023-07-21 12:05:00.984741 git_timemachine-1.4.0/src/git_timemachine/utils.py
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 git_timemachine-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-25 11:45:33.024640 git_timemachine-1.5.0/COPYING
+-rw-r--r--   0        0        0      846 2023-07-25 11:45:33.025639 git_timemachine-1.5.0/README.md
+-rw-r--r--   0        0        0     1661 2023-07-25 11:45:33.026643 git_timemachine-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-07-25 11:45:33.027646 git_timemachine-1.5.0/src/git_timemachine/__init__.py
+-rw-r--r--   0        0        0     1792 2023-07-25 11:45:33.027646 git_timemachine-1.5.0/src/git_timemachine/__main__.py
+-rw-r--r--   0        0        0      273 2023-07-25 11:45:33.028643 git_timemachine-1.5.0/src/git_timemachine/commands/__init__.py
+-rw-r--r--   0        0        0     5417 2023-07-25 11:45:33.028643 git_timemachine-1.5.0/src/git_timemachine/commands/commit.py
+-rw-r--r--   0        0        0      495 2023-07-25 11:45:33.028643 git_timemachine-1.5.0/src/git_timemachine/commands/init.py
+-rw-r--r--   0        0        0     1179 2023-07-25 11:45:33.029642 git_timemachine-1.5.0/src/git_timemachine/commands/log.py
+-rw-r--r--   0        0        0      703 2023-07-25 11:45:33.029642 git_timemachine-1.5.0/src/git_timemachine/commands/review.py
+-rw-r--r--   0        0        0      600 2023-07-25 11:45:33.030646 git_timemachine-1.5.0/src/git_timemachine/commands/switch_date.py
+-rw-r--r--   0        0        0       41 2023-07-25 11:45:33.030646 git_timemachine-1.5.0/src/git_timemachine/config.py
+-rw-r--r--   0        0        0      994 2023-07-25 11:45:33.030646 git_timemachine-1.5.0/src/git_timemachine/types.py
+-rw-r--r--   0        0        0     1283 2023-07-25 11:45:33.030646 git_timemachine-1.5.0/src/git_timemachine/utils.py
+-rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 git_timemachine-1.5.0/PKG-INFO
```

### Comparing `git_timemachine-1.4.0/COPYING` & `git_timemachine-1.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.4.0/README.md` & `git_timemachine-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.4.0/pyproject.toml` & `git_timemachine-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-timemachine"
-version = "1.4.0"
+version = "1.5.0"
 description = "A command-line tool that helps you record commits on Git repositories at any time node."
 license = "GPL-3.0"
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/git-timemachine"
 repository = "https://github.com/he-yaowen/git-timemachine.git"
 keywords = ["git", "timemachine", "committing"]
```

### Comparing `git_timemachine-1.4.0/src/git_timemachine/__main__.py` & `git_timemachine-1.5.0/src/git_timemachine/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 @click.pass_context
 def cli(ctx: click.Context, repo_dir: str, cache_dir: str, config_file: str):
     """A command-line tool that helps you record commits on Git repositories at any time node."""
 
     ctx.ensure_object(dict)
     ctx.obj['repo_dir'] = repo_dir
     ctx.obj['states'] = StateManager(Path(cache_dir, 'states'))
+    ctx.obj['config_file'] = config_file
 
     config = default.copy()
 
     if os.path.exists(config_file):
         with open(config_file, 'r', encoding='utf-8') as fp:
             config.update(ini.parse(fp.read()))
```

### Comparing `git_timemachine-1.4.0/src/git_timemachine/commands/commit.py` & `git_timemachine-1.5.0/src/git_timemachine/commands/commit.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         commit_env = commit_time.replace(microsecond=0).astimezone().isoformat()
         subprocess.run(
             shlex.split(external) + list(args),
             cwd=repo_dir,
             env={**os.environ, 'GIT_AUTHOR_DATE': commit_env, 'GIT_COMMITTER_DATE': commit_env}
         )
 
+        states.set('commit-time', commit_time)
+
         return
 
     parents = []
     if repo.head_is_unborn:
         try:
             git_config = repo.config.get_global_config()
             ref_name = git_config['init.defaultBranch'] if 'init.defaultBranch' in git_config else 'main'
@@ -71,21 +73,24 @@
             ref_name = 'main'
 
         ref_name = f'refs/heads/{ref_name}'
     else:
         parents.append(repo.head.target)
         ref_name = repo.head.name
 
-    signature = Signature(
-        name=repo.default_signature.name,
-        email=repo.default_signature.email,
-        time=int(commit_time.replace(microsecond=0).timestamp()),
-        encoding='utf-8',
-        offset=int(commit_time.tzinfo.utcoffset(commit_time).seconds / 60)
-    )
+    try:
+        signature = Signature(
+            name=repo.default_signature.name,
+            email=repo.default_signature.email,
+            time=int(commit_time.replace(microsecond=0).timestamp()),
+            encoding='utf-8',
+            offset=0 if commit_time.tzinfo is None else int(commit_time.tzinfo.utcoffset(commit_time).seconds / 60)
+        )
+    except KeyError:
+        ctx.fail('Author identity unknown')
 
     tree = repo.index.write_tree()
     if tree is None:
         ctx.fail('Failed to write index tree.')
 
     if message is None:
         raise click.exceptions.MissingParameter(ctx=ctx, param=next(param for param in ctx.command.params if param.name == 'message'))
```

### Comparing `git_timemachine-1.4.0/src/git_timemachine/commands/log.py` & `git_timemachine-1.5.0/src/git_timemachine/commands/log.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.4.0/src/git_timemachine/commands/review.py` & `git_timemachine-1.5.0/src/git_timemachine/commands/review.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.4.0/src/git_timemachine/commands/switch_date.py` & `git_timemachine-1.5.0/src/git_timemachine/commands/switch_date.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.4.0/src/git_timemachine/types.py` & `git_timemachine-1.5.0/src/git_timemachine/types.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.4.0/src/git_timemachine/utils.py` & `git_timemachine-1.5.0/src/git_timemachine/utils.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.4.0/PKG-INFO` & `git_timemachine-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-timemachine
-Version: 1.4.0
+Version: 1.5.0
 Summary: A command-line tool that helps you record commits on Git repositories at any time node.
 Home-page: https://github.com/he-yaowen/git-timemachine
 License: GPL-3.0
 Keywords: git,timemachine,committing
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
```

