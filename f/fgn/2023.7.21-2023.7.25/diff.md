# Comparing `tmp/fgn-2023.7.21.tar.gz` & `tmp/fgn-2023.7.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgn-2023.7.21.tar", last modified: Sat Jul 22 00:39:58 2023, max compression
+gzip compressed data, was "fgn-2023.7.25.tar", last modified: Tue Jul 25 21:20:19 2023, max compression
```

## Comparing `fgn-2023.7.21.tar` & `fgn-2023.7.25.tar`

### file list

```diff
@@ -1,223 +1,222 @@
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.839191 fgn-2023.7.21/
--rw-r--r--   0 candacechatman   (501) staff       (20)      586 2023-07-21 16:52:47.000000 fgn-2023.7.21/.coveragerc
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.811812 fgn-2023.7.21/.github/
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.816058 fgn-2023.7.21/.github/workflows/
--rw-r--r--   0 candacechatman   (501) staff       (20)     4382 2023-07-21 18:56:18.000000 fgn-2023.7.21/.github/workflows/ci.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)      566 2023-07-21 16:52:47.000000 fgn-2023.7.21/.gitignore
--rw-r--r--   0 candacechatman   (501) staff       (20)       51 2023-07-21 16:52:47.000000 fgn-2023.7.21/.isort.cfg
--rw-r--r--   0 candacechatman   (501) staff       (20)     1670 2023-07-21 16:55:22.000000 fgn-2023.7.21/.pre-commit-config.yaml
--rw-r--r--   0 candacechatman   (501) staff       (20)      530 2023-07-21 16:52:47.000000 fgn-2023.7.21/.readthedocs.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)       77 2023-07-21 16:52:47.000000 fgn-2023.7.21/AUTHORS.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)      134 2023-07-21 17:25:04.000000 fgn-2023.7.21/CHANGELOG.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)    13762 2023-07-21 16:52:47.000000 fgn-2023.7.21/CONTRIBUTING.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)     1079 2023-07-21 16:52:47.000000 fgn-2023.7.21/LICENSE.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)       37 2023-07-22 00:10:12.000000 fgn-2023.7.21/MANIFEST.in
--rw-r--r--   0 candacechatman   (501) staff       (20)     7038 2023-07-22 00:39:58.839273 fgn-2023.7.21/PKG-INFO
--rw-r--r--   0 candacechatman   (501) staff       (20)     6538 2023-07-22 00:38:10.000000 fgn-2023.7.21/README.rst
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.817669 fgn-2023.7.21/docs/
--rw-r--r--   0 candacechatman   (501) staff       (20)     1154 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/Makefile
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.817807 fgn-2023.7.21/docs/_static/
--rw-r--r--   0 candacechatman   (501) staff       (20)       18 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/_static/.gitignore
--rw-r--r--   0 candacechatman   (501) staff       (20)       41 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/authors.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)       43 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/changelog.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)     9714 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/conf.py
--rw-r--r--   0 candacechatman   (501) staff       (20)       33 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/contributing.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)     2297 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/index.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)       67 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/license.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)       39 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/readme.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)      233 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/requirements.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      346 2023-07-21 16:52:47.000000 fgn-2023.7.21/pyproject.toml
--rw-r--r--   0 candacechatman   (501) staff       (20)     1398 2023-07-22 00:39:58.839694 fgn-2023.7.21/setup.cfg
--rw-r--r--   0 candacechatman   (501) staff       (20)      693 2023-07-22 00:34:27.000000 fgn-2023.7.21/setup.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.812082 fgn-2023.7.21/src/
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.818286 fgn-2023.7.21/src/fgn/
--rw-r--r--   0 candacechatman   (501) staff       (20)      577 2023-07-21 16:52:47.000000 fgn-2023.7.21/src/fgn/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      532 2023-07-21 21:57:44.000000 fgn-2023.7.21/src/fgn/cli.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.820542 fgn-2023.7.21/src/fgn/core/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-30 20:42:36.000000 fgn-2023.7.21/src/fgn/core/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     5894 2023-07-21 22:06:39.000000 fgn-2023.7.21/src/fgn/core/chat_agent.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     1336 2023-07-22 00:08:39.000000 fgn-2023.7.21/src/fgn/core/command_context.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.820779 fgn-2023.7.21/src/fgn/core/commands/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-01 20:36:22.000000 fgn-2023.7.21/src/fgn/core/commands/__init__.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.821757 fgn-2023.7.21/src/fgn/core/commands/blog/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      401 2023-07-22 00:08:39.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      284 2023-03-29 22:12:51.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     1932 2023-04-19 20:56:19.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.822664 fgn-2023.7.21/src/fgn/core/commands/chain/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     1522 2023-07-22 00:14:45.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:34:48.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)    10183 2023-04-19 23:20:50.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.823434 fgn-2023.7.21/src/fgn/core/commands/code/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.21/src/fgn/core/commands/code/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      452 2023-04-23 07:52:01.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      293 2023-04-21 18:43:00.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-21 18:42:58.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_schema.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     4092 2023-04-29 20:34:41.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      275 2023-03-29 00:19:20.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.823648 fgn-2023.7.21/src/fgn/core/commands/core/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:07:18.000000 fgn-2023.7.21/src/fgn/core/commands/core/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      377 2023-04-14 01:38:20.000000 fgn-2023.7.21/src/fgn/core/commands/core/core_cmd.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.825024 fgn-2023.7.21/src/fgn/core/commands/dsl/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-11 03:26:13.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      415 2023-04-14 03:12:15.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      256 2023-04-11 19:24:14.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)     6522 2023-04-11 19:24:14.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-11 03:26:13.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      634 2023-04-11 19:31:02.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      931 2023-04-11 19:31:02.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_template.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      367 2023-04-08 03:58:38.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/main.yaml
--rw-r--r--   0 candacechatman   (501) staff       (20)     1697 2023-04-08 21:49:12.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/newsletter.yaml
--rw-r--r--   0 candacechatman   (501) staff       (20)     1674 2023-04-08 04:35:12.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/newsletter2.yaml
--rw-r--r--   0 candacechatman   (501) staff       (20)      265 2023-04-08 03:58:15.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/sub.yaml
--rw-r--r--   0 candacechatman   (501) staff       (20)     2811 2023-04-08 20:38:17.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/switch.yaml
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.825904 fgn-2023.7.21/src/fgn/core/commands/feedback/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      438 2023-05-01 01:46:44.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      286 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     4244 2023-04-19 23:06:06.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     1996 2023-04-19 22:47:50.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.826846 fgn-2023.7.21/src/fgn/core/commands/fun/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      575 2023-07-22 00:08:39.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      256 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     7750 2023-06-22 18:53:35.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.827733 fgn-2023.7.21/src/fgn/core/commands/guide/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      407 2023-07-22 00:14:45.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     4999 2023-04-19 23:13:20.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.828913 fgn-2023.7.21/src/fgn/core/commands/help/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.21/src/fgn/core/commands/help/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)    10159 2023-04-17 03:25:54.000000 fgn-2023.7.21/src/fgn/core/commands/help/help-in.md
--rw-r--r--   0 candacechatman   (501) staff       (20)      405 2023-04-14 03:12:15.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      228 2023-04-14 00:53:18.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)     3063 2023-04-17 02:37:56.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)    10220 2023-06-26 18:00:16.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.829717 fgn-2023.7.21/src/fgn/core/commands/howto/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      585 2023-05-10 21:54:04.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     3781 2023-06-13 17:15:14.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.830578 fgn-2023.7.21/src/fgn/core/commands/lts/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      477 2023-04-29 20:31:50.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      256 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     1657 2023-04-19 00:16:44.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.831369 fgn-2023.7.21/src/fgn/core/commands/nano/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      407 2023-04-14 03:36:47.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      262 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)      529 2023-04-13 20:45:30.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     2022 2023-07-01 06:04:22.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.832064 fgn-2023.7.21/src/fgn/core/commands/plan/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.21/src/fgn/core/commands/plan/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      406 2023-04-19 21:13:19.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      259 2023-03-28 22:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 23:39:15.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 15:13:22.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     4708 2023-04-19 21:30:40.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      440 2023-04-12 01:04:03.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.832732 fgn-2023.7.21/src/fgn/core/commands/prompt/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      482 2023-05-01 02:54:17.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      257 2023-03-27 16:12:16.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 20:57:09.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     3738 2023-04-19 21:00:08.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     1691 2023-04-13 23:44:53.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.833493 fgn-2023.7.21/src/fgn/core/commands/shell/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     1369 2023-04-29 21:38:36.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      535 2023-06-26 17:56:46.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.834375 fgn-2023.7.21/src/fgn/core/commands/summary/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      402 2023-07-22 00:14:45.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      280 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     2674 2023-04-20 19:37:14.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.834956 fgn-2023.7.21/src/fgn/core/commands/template/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.21/src/fgn/core/commands/template/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     2038 2023-04-30 00:43:45.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      259 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      435 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_template.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.835873 fgn-2023.7.21/src/fgn/core/commands/yaml/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     3116 2023-04-21 01:44:04.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/product-information-schema.yaml
--rw-r--r--   0 candacechatman   (501) staff       (20)      408 2023-04-30 02:01:51.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      262 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_config.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_example.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_history.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      879 2023-04-21 01:54:46.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_system_prompt.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_template.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     2635 2023-05-01 02:30:56.000000 fgn-2023.7.21/src/fgn/core/core_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     1607 2023-05-21 21:11:46.000000 fgn-2023.7.21/src/fgn/core/default_sub_cmd.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     3762 2023-04-13 23:44:53.000000 fgn-2023.7.21/src/fgn/core/dsl_parser.py
--rwxr-xr-x   0 candacechatman   (501) staff       (20)     4277 2023-07-21 22:01:54.000000 fgn-2023.7.21/src/fgn/core/fgn_cli.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.836065 fgn-2023.7.21/src/fgn/models/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-06 19:32:18.000000 fgn-2023.7.21/src/fgn/models/__init__.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.836467 fgn-2023.7.21/src/fgn/models/dsl/
--rw-r--r--   0 candacechatman   (501) staff       (20)      270 2023-04-08 04:05:38.000000 fgn-2023.7.21/src/fgn/models/dsl/fgn_dsl_schema.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      355 2023-04-08 04:05:52.000000 fgn-2023.7.21/src/fgn/models/dsl/step.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      242 2023-04-08 04:18:36.000000 fgn-2023.7.21/src/fgn/models/dsl/task.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      373 2023-03-23 03:55:38.000000 fgn-2023.7.21/src/fgn/models/message.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     4192 2023-07-21 16:52:47.000000 fgn-2023.7.21/src/fgn/skeleton.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.837532 fgn-2023.7.21/src/fgn/utils/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-30 20:42:36.000000 fgn-2023.7.21/src/fgn/utils/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     3254 2023-04-29 21:10:53.000000 fgn-2023.7.21/src/fgn/utils/chat_agent_configuration.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      227 2023-03-31 00:51:25.000000 fgn-2023.7.21/src/fgn/utils/clipboard.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     3336 2023-07-21 22:05:11.000000 fgn-2023.7.21/src/fgn/utils/file_operations.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     5655 2023-07-21 21:38:30.000000 fgn-2023.7.21/src/fgn/utils/openai_operations.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     1820 2023-07-21 21:49:15.000000 fgn-2023.7.21/src/fgn/utils/output_manager.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.819243 fgn-2023.7.21/src/fgn.egg-info/
--rw-r--r--   0 candacechatman   (501) staff       (20)     7038 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/PKG-INFO
--rw-r--r--   0 candacechatman   (501) staff       (20)     7078 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/SOURCES.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/dependency_links.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)       45 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/entry_points.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-21 16:56:59.000000 fgn-2023.7.21/src/fgn.egg-info/not-zip-safe
--rw-r--r--   0 candacechatman   (501) staff       (20)      206 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/requires.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        4 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/top_level.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.838237 fgn-2023.7.21/tests/
--rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-07-21 20:21:09.000000 fgn-2023.7.21/tests/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      271 2023-07-21 20:59:55.000000 fgn-2023.7.21/tests/conftest.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      855 2023-07-21 18:47:03.000000 fgn-2023.7.21/tests/test_cli.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      599 2023-07-21 17:15:32.000000 fgn-2023.7.21/tests/test_skeleton.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.838971 fgn-2023.7.21/tests/utils/
--rw-r--r--   0 candacechatman   (501) staff       (20)     1852 2023-07-21 21:40:26.000000 fgn-2023.7.21/tests/utils/test_file_operations.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     3737 2023-07-21 21:48:33.000000 fgn-2023.7.21/tests/utils/test_openai_operations.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     2750 2023-07-21 21:52:30.000000 fgn-2023.7.21/tests/utils/test_output_manager.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     2926 2023-07-21 20:26:23.000000 fgn-2023.7.21/tox.ini
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.317247 fgn-2023.7.25/
+-rw-r--r--   0 candacechatman   (501) staff       (20)      586 2023-07-21 16:52:47.000000 fgn-2023.7.25/.coveragerc
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.295408 fgn-2023.7.25/.github/
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.299058 fgn-2023.7.25/.github/workflows/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4382 2023-07-21 18:56:18.000000 fgn-2023.7.25/.github/workflows/ci.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      566 2023-07-21 16:52:47.000000 fgn-2023.7.25/.gitignore
+-rw-r--r--   0 candacechatman   (501) staff       (20)       51 2023-07-21 16:52:47.000000 fgn-2023.7.25/.isort.cfg
+-rw-r--r--   0 candacechatman   (501) staff       (20)      530 2023-07-21 16:52:47.000000 fgn-2023.7.25/.readthedocs.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)       77 2023-07-21 16:52:47.000000 fgn-2023.7.25/AUTHORS.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)      134 2023-07-21 17:25:04.000000 fgn-2023.7.25/CHANGELOG.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)    13762 2023-07-21 16:52:47.000000 fgn-2023.7.25/CONTRIBUTING.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1079 2023-07-21 16:52:47.000000 fgn-2023.7.25/LICENSE.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)       38 2023-07-25 21:11:17.000000 fgn-2023.7.25/MANIFEST.in
+-rw-r--r--   0 candacechatman   (501) staff       (20)     6820 2023-07-25 21:20:19.317324 fgn-2023.7.25/PKG-INFO
+-rw-r--r--   0 candacechatman   (501) staff       (20)     6320 2023-07-25 21:17:48.000000 fgn-2023.7.25/README.rst
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.300045 fgn-2023.7.25/docs/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1154 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/Makefile
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.300159 fgn-2023.7.25/docs/_static/
+-rw-r--r--   0 candacechatman   (501) staff       (20)       18 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/_static/.gitignore
+-rw-r--r--   0 candacechatman   (501) staff       (20)       41 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/authors.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)       43 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/changelog.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)     9704 2023-07-25 21:20:08.000000 fgn-2023.7.25/docs/conf.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)       33 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/contributing.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2297 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/index.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)       67 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/license.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)       39 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/readme.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)      233 2023-07-21 16:52:47.000000 fgn-2023.7.25/docs/requirements.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      346 2023-07-21 16:52:47.000000 fgn-2023.7.25/pyproject.toml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1414 2023-07-25 21:20:19.317730 fgn-2023.7.25/setup.cfg
+-rw-r--r--   0 candacechatman   (501) staff       (20)      764 2023-07-25 21:11:17.000000 fgn-2023.7.25/setup.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.295719 fgn-2023.7.25/src/
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.300640 fgn-2023.7.25/src/fgn/
+-rw-r--r--   0 candacechatman   (501) staff       (20)      577 2023-07-21 16:52:47.000000 fgn-2023.7.25/src/fgn/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      532 2023-07-21 21:57:44.000000 fgn-2023.7.25/src/fgn/cli.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.302273 fgn-2023.7.25/src/fgn/core/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-30 20:42:36.000000 fgn-2023.7.25/src/fgn/core/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     6167 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/chat_agent.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1336 2023-07-22 00:45:19.000000 fgn-2023.7.25/src/fgn/core/command_context.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.302386 fgn-2023.7.25/src/fgn/core/commands/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-01 20:36:22.000000 fgn-2023.7.25/src/fgn/core/commands/__init__.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.303084 fgn-2023.7.25/src/fgn/core/commands/blog/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.25/src/fgn/core/commands/blog/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      402 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/blog/blog_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      283 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/blog/blog_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.25/src/fgn/core/commands/blog/blog_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.25/src/fgn/core/commands/blog/blog_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1933 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/blog/blog_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.25/src/fgn/core/commands/blog/blog_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.303792 fgn-2023.7.25/src/fgn/core/commands/chain/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.25/src/fgn/core/commands/chain/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1522 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/chain/chain_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      269 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/chain/chain_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:34:48.000000 fgn-2023.7.25/src/fgn/core/commands/chain/chain_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.25/src/fgn/core/commands/chain/chain_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)    10184 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/chain/chain_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.25/src/fgn/core/commands/chain/chain_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.304592 fgn-2023.7.25/src/fgn/core/commands/code/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.25/src/fgn/core/commands/code/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      453 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/code/code_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      294 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/code/code_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.25/src/fgn/core/commands/code/code_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.25/src/fgn/core/commands/code/code_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-21 18:42:58.000000 fgn-2023.7.25/src/fgn/core/commands/code/code_schema.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4093 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/code/code_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      275 2023-03-29 00:19:20.000000 fgn-2023.7.25/src/fgn/core/commands/code/code_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.304795 fgn-2023.7.25/src/fgn/core/commands/core/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:07:18.000000 fgn-2023.7.25/src/fgn/core/commands/core/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      378 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/core/core_cmd.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.306095 fgn-2023.7.25/src/fgn/core/commands/dsl/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-11 03:26:13.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      416 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      257 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     6523 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-11 03:26:13.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      635 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      932 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_template.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      368 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/main.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1698 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/newsletter.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1675 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/newsletter2.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      266 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/sub.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2811 2023-04-08 20:38:17.000000 fgn-2023.7.25/src/fgn/core/commands/dsl/switch.yaml
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.306890 fgn-2023.7.25/src/fgn/core/commands/feedback/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.25/src/fgn/core/commands/feedback/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      439 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      287 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4244 2023-04-19 23:06:06.000000 fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1995 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.307619 fgn-2023.7.25/src/fgn/core/commands/fun/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.25/src/fgn/core/commands/fun/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      575 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/fun/fun_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      257 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/fun/fun_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.25/src/fgn/core/commands/fun/fun_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.25/src/fgn/core/commands/fun/fun_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     7751 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/fun/fun_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.25/src/fgn/core/commands/fun/fun_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.308326 fgn-2023.7.25/src/fgn/core/commands/guide/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.25/src/fgn/core/commands/guide/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      408 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/guide/guide_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      269 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/guide/guide_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.25/src/fgn/core/commands/guide/guide_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.25/src/fgn/core/commands/guide/guide_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     5000 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/guide/guide_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.25/src/fgn/core/commands/guide/guide_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.309120 fgn-2023.7.25/src/fgn/core/commands/help/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.25/src/fgn/core/commands/help/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)    10160 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/help/help-in.md
+-rw-r--r--   0 candacechatman   (501) staff       (20)      406 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/help/help_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      229 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/help/help_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3062 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/help/help_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.25/src/fgn/core/commands/help/help_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)    10221 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/help/help_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.25/src/fgn/core/commands/help/help_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.309810 fgn-2023.7.25/src/fgn/core/commands/howto/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.25/src/fgn/core/commands/howto/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      605 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/howto/howto_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      269 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/howto/howto_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.25/src/fgn/core/commands/howto/howto_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.25/src/fgn/core/commands/howto/howto_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3782 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/howto/howto_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.25/src/fgn/core/commands/howto/howto_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.310487 fgn-2023.7.25/src/fgn/core/commands/lts/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.25/src/fgn/core/commands/lts/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      478 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/lts/lts_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      257 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/lts/lts_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.25/src/fgn/core/commands/lts/lts_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.25/src/fgn/core/commands/lts/lts_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1658 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/lts/lts_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.25/src/fgn/core/commands/lts/lts_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.311199 fgn-2023.7.25/src/fgn/core/commands/nano/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.25/src/fgn/core/commands/nano/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      408 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/nano/nano_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      263 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/nano/nano_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      529 2023-04-13 20:45:30.000000 fgn-2023.7.25/src/fgn/core/commands/nano/nano_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.25/src/fgn/core/commands/nano/nano_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2023 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/nano/nano_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.25/src/fgn/core/commands/nano/nano_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.311891 fgn-2023.7.25/src/fgn/core/commands/plan/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.25/src/fgn/core/commands/plan/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      407 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/plan/plan_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      259 2023-03-28 22:04:20.000000 fgn-2023.7.25/src/fgn/core/commands/plan/plan_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 23:39:15.000000 fgn-2023.7.25/src/fgn/core/commands/plan/plan_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 15:13:22.000000 fgn-2023.7.25/src/fgn/core/commands/plan/plan_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4709 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/plan/plan_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      441 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/plan/plan_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.312514 fgn-2023.7.25/src/fgn/core/commands/prompt/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.25/src/fgn/core/commands/prompt/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      522 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/prompt/prompt_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      257 2023-03-27 16:12:16.000000 fgn-2023.7.25/src/fgn/core/commands/prompt/prompt_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 20:57:09.000000 fgn-2023.7.25/src/fgn/core/commands/prompt/prompt_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3736 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/prompt/prompt_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1692 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/prompt/prompt_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.313218 fgn-2023.7.25/src/fgn/core/commands/shell/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.25/src/fgn/core/commands/shell/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1370 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/shell/shell_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      269 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/shell/shell_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.25/src/fgn/core/commands/shell/shell_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.25/src/fgn/core/commands/shell/shell_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      536 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/shell/shell_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.25/src/fgn/core/commands/shell/shell_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.313908 fgn-2023.7.25/src/fgn/core/commands/summary/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.25/src/fgn/core/commands/summary/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      403 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/summary/summary_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      281 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/summary/summary_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.25/src/fgn/core/commands/summary/summary_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.25/src/fgn/core/commands/summary/summary_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2675 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/summary/summary_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.25/src/fgn/core/commands/summary/summary_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.314467 fgn-2023.7.25/src/fgn/core/commands/template/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.25/src/fgn/core/commands/template/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2128 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/template/template_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      259 2023-03-28 22:28:18.000000 fgn-2023.7.25/src/fgn/core/commands/template/template_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 22:28:18.000000 fgn-2023.7.25/src/fgn/core/commands/template/template_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 22:28:18.000000 fgn-2023.7.25/src/fgn/core/commands/template/template_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      436 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/template/template_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.315258 fgn-2023.7.25/src/fgn/core/commands/yaml/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3116 2023-04-21 01:44:04.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/product-information-schema.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      409 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/yaml_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      263 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/yaml_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/yaml_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/yaml_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      880 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/yaml_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.25/src/fgn/core/commands/yaml/yaml_template.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2615 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/core_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1534 2023-07-22 00:45:19.000000 fgn-2023.7.25/src/fgn/core/default_sub_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3896 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/dsl_parser.py
+-rwxr-xr-x   0 candacechatman   (501) staff       (20)     4423 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/core/fgn_cli.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.315431 fgn-2023.7.25/src/fgn/models/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-06 19:32:18.000000 fgn-2023.7.25/src/fgn/models/__init__.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.315743 fgn-2023.7.25/src/fgn/models/dsl/
+-rw-r--r--   0 candacechatman   (501) staff       (20)      270 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/models/dsl/fgn_dsl_schema.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      355 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/models/dsl/step.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      242 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/models/dsl/task.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      373 2023-07-22 00:45:19.000000 fgn-2023.7.25/src/fgn/models/message.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4192 2023-07-21 16:52:47.000000 fgn-2023.7.25/src/fgn/skeleton.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.316399 fgn-2023.7.25/src/fgn/utils/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-30 20:42:36.000000 fgn-2023.7.25/src/fgn/utils/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3273 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/utils/chat_agent_configuration.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      227 2023-03-31 00:51:25.000000 fgn-2023.7.25/src/fgn/utils/clipboard.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3370 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/utils/file_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     5713 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/utils/openai_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1859 2023-07-25 21:11:17.000000 fgn-2023.7.25/src/fgn/utils/output_manager.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.301522 fgn-2023.7.25/src/fgn.egg-info/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     6820 2023-07-25 21:20:19.000000 fgn-2023.7.25/src/fgn.egg-info/PKG-INFO
+-rw-r--r--   0 candacechatman   (501) staff       (20)     7054 2023-07-25 21:20:19.000000 fgn-2023.7.25/src/fgn.egg-info/SOURCES.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-25 21:20:19.000000 fgn-2023.7.25/src/fgn.egg-info/dependency_links.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)       45 2023-07-25 21:20:19.000000 fgn-2023.7.25/src/fgn.egg-info/entry_points.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-21 16:56:59.000000 fgn-2023.7.25/src/fgn.egg-info/not-zip-safe
+-rw-r--r--   0 candacechatman   (501) staff       (20)      220 2023-07-25 21:20:19.000000 fgn-2023.7.25/src/fgn.egg-info/requires.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        4 2023-07-25 21:20:19.000000 fgn-2023.7.25/src/fgn.egg-info/top_level.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.316809 fgn-2023.7.25/tests/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-07-21 20:21:09.000000 fgn-2023.7.25/tests/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      271 2023-07-21 20:59:55.000000 fgn-2023.7.25/tests/conftest.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      850 2023-07-25 21:11:17.000000 fgn-2023.7.25/tests/test_cli.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      599 2023-07-21 17:15:32.000000 fgn-2023.7.25/tests/test_skeleton.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-25 21:20:19.317146 fgn-2023.7.25/tests/utils/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1848 2023-07-25 21:11:17.000000 fgn-2023.7.25/tests/utils/test_file_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3737 2023-07-25 21:11:17.000000 fgn-2023.7.25/tests/utils/test_openai_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2752 2023-07-25 21:11:17.000000 fgn-2023.7.25/tests/utils/test_output_manager.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2926 2023-07-21 20:26:23.000000 fgn-2023.7.25/tox.ini
```

### Comparing `fgn-2023.7.21/.coveragerc` & `fgn-2023.7.25/.coveragerc`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/.github/workflows/ci.yml` & `fgn-2023.7.25/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/.gitignore` & `fgn-2023.7.25/.gitignore`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/.readthedocs.yml` & `fgn-2023.7.25/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/CONTRIBUTING.rst` & `fgn-2023.7.25/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/LICENSE.txt` & `fgn-2023.7.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/PKG-INFO` & `fgn-2023.7.25/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgn
-Version: 2023.7.21
+Version: 2023.7.25
 Summary: FGN: An AI-powered command-line tool for automated file generation.
 Home-page: https://github.com/seanchatmangpt/fgn
 Author: Sean Chatman
 Author-email: info@chatmangpt.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -73,37 +73,33 @@
     --help                         Show this message and exit.
 
 Commands
 --------
 
 .. code-block:: bash
 
-    blog       Create a blog article.
-    chain      Create chain of FGN .
-    chapter    Create a chapter.
-    code       Create a code snippet.
-    core       CLI internal usage only.
-    dsl        Create a new FGN DSL (requires GPT 4).
-    example    Create an example.
-    feedback   Create a feedback.
-    flow       Create a flow.
-    framework  Create a framework.
-    fun        Create fun.
-    guide      Execute the guide command.
-    help       Get help with the FGN CLI.
-    howto      Create a how-to article.
-    intent     Create an intent.
-    lts        Let's think step by step how to do this.
-    nano       Create a Nano Fiction story.
-    plan       Create a detailed plan.
-    prompt     Create a new prompt.
-    shell      Create a shell script.
-    summary    Execute the summary command.
-    template   Create a command named by the prompt.
-    yaml       Create yaml.It needs much
+  blog      Create a blog article.
+  chain     Create chain of fgn commands.
+  code      Create a code snippet.
+  core      CLI internal usage only.
+  dsl       Create a new FGN DSL (requires GPT 4).
+  feedback  Create feedback.
+  fun       Create OpenAI function schema.
+  guide     Create a procedural guide.
+  help      Get help with the FGN CLI.
+  howto     Create a how-to article.
+  lts       Let's think step by step how to do this.
+  nano      Create a Nano Fiction story.
+  plan      Create a detailed plan.
+  prompt    Create a new prompt
+  shell     Create a shell script.
+  summary   Create a summary.
+  template  Create a command named by the prompt.
+  yaml      Create yaml.
+
 
 Examples
 --------
 Here are some example uses of FGN:
 
 To generate a business plan and save it to "business_plan.txt", run:
```

### Comparing `fgn-2023.7.21/README.rst` & `fgn-2023.7.25/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -57,37 +57,33 @@
     --help                         Show this message and exit.
 
 Commands
 --------
 
 .. code-block:: bash
 
-    blog       Create a blog article.
-    chain      Create chain of FGN .
-    chapter    Create a chapter.
-    code       Create a code snippet.
-    core       CLI internal usage only.
-    dsl        Create a new FGN DSL (requires GPT 4).
-    example    Create an example.
-    feedback   Create a feedback.
-    flow       Create a flow.
-    framework  Create a framework.
-    fun        Create fun.
-    guide      Execute the guide command.
-    help       Get help with the FGN CLI.
-    howto      Create a how-to article.
-    intent     Create an intent.
-    lts        Let's think step by step how to do this.
-    nano       Create a Nano Fiction story.
-    plan       Create a detailed plan.
-    prompt     Create a new prompt.
-    shell      Create a shell script.
-    summary    Execute the summary command.
-    template   Create a command named by the prompt.
-    yaml       Create yaml.It needs much
+  blog      Create a blog article.
+  chain     Create chain of fgn commands.
+  code      Create a code snippet.
+  core      CLI internal usage only.
+  dsl       Create a new FGN DSL (requires GPT 4).
+  feedback  Create feedback.
+  fun       Create OpenAI function schema.
+  guide     Create a procedural guide.
+  help      Get help with the FGN CLI.
+  howto     Create a how-to article.
+  lts       Let's think step by step how to do this.
+  nano      Create a Nano Fiction story.
+  plan      Create a detailed plan.
+  prompt    Create a new prompt
+  shell     Create a shell script.
+  summary   Create a summary.
+  template  Create a command named by the prompt.
+  yaml      Create yaml.
+
 
 Examples
 --------
 Here are some example uses of FGN:
 
 To generate a business plan and save it to "business_plan.txt", run:
```

### Comparing `fgn-2023.7.21/docs/Makefile` & `fgn-2023.7.25/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/docs/conf.py` & `fgn-2023.7.25/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
+html_theme_options = {"sidebar_width": "300px", "page_width": "1200px"}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
```

### Comparing `fgn-2023.7.21/docs/index.rst` & `fgn-2023.7.25/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/setup.cfg` & `fgn-2023.7.25/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 	PyYAML
 	distro
 	markdown2
 	lxml
 	requests
 	openai
 	pytest-mock
+	jinja2
+	pyyaml
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `fgn-2023.7.21/src/fgn/__init__.py` & `fgn-2023.7.25/src/fgn/__init__.py`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/src/fgn/cli.py` & `fgn-2023.7.25/src/fgn/cli.py`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/src/fgn/core/chat_agent.py` & `fgn-2023.7.25/src/fgn/core/chat_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,33 +19,33 @@
     tokens: str = None
     history_path: str = None
 
     def __post_init__(self):
         if not self.messages:
             self.messages = []
         if self.system_prompt:
-            self.messages.append(Message('system', self.system_prompt))
+            self.messages.append(Message("system", self.system_prompt))
         if self.auto_clear:
             self.clear()
         else:
             if self.history_path:
                 self.load()
 
     def submit(self, content, tokens=None):
         if self.verbose:
             print("ChatAgent.submit: ", content)
 
         # If tokens are provided, replace any {key} with the corresponding value
         # separated by a semicolon
         if self.tokens:
-            for token in self.tokens.split(';'):
-                key, value = token.split('=')
+            for token in self.tokens.split(";"):
+                key, value = token.split("=")
                 content = content.replace("{{" + key + "}}", value)
 
-        self.add_message('user', content)
+        self.add_message("user", content)
 
         response = self.generate_response()
 
         # Check if the response contains the "maximum context length" error
         if "maximum context length" in response:
             # Auto-summarize the conversation
             success = self.summarize_conversations(self.auto_summarize)
@@ -56,24 +56,25 @@
 
         return response
 
     def add_message(self, role, content):
         self.messages.append(Message(role, content))
 
     def save(self):
-        input_data = {
-            "messages": [message.serialize() for message in self.messages]
-        }
+        input_data = {"messages": [message.serialize() for message in self.messages]}
 
     def load(self):
         if os.path.exists(self.history_path):
             try:
-                with open(self.history_path, 'r', encoding='utf-8') as infile:
+                with open(self.history_path, encoding="utf-8") as infile:
                     input_data = json.load(infile)
-                    self.messages = [Message.deserialize(message_data) for message_data in input_data["messages"]]
+                    self.messages = [
+                        Message.deserialize(message_data)
+                        for message_data in input_data["messages"]
+                    ]
             except json.JSONDecodeError:
                 self.clear()
 
     def clear(self):
         # clear the messages except the first which is the system prompt
         self.messages = self.messages[:1]
         self.save()
@@ -82,52 +83,60 @@
         messages = [m.serialize() for m in self.messages]
 
         response = gpt_chat_completion(messages, model=self.model)
 
         if "maximum context length" in response:
             return response
 
-        message = Message('assistant', response)
+        message = Message("assistant", response)
         self.add_message(message.role, message.content)
         if self.history_path:
             self.save()
 
         if self.verbose:
             print(message.content)
 
         return message.content
 
     def get_user_messages(self):
-        return [msg for msg in self.messages if msg.role == 'user']
+        return [msg for msg in self.messages if msg.role == "user"]
 
-    def summarize_conversations(self, num_conversations: int, summary_length: int = 200) -> bool:
+    def summarize_conversations(
+        self, num_conversations: int, summary_length: int = 200
+    ) -> bool:
         if self.verbose:
-            print("ChatAgent.summarize_conversations: ", num_conversations, summary_length)
+            print(
+                "ChatAgent.summarize_conversations: ", num_conversations, summary_length
+            )
 
         if num_conversations <= 0:
             return False
 
         while num_conversations > 0:
             # Collect the first 'num_conversations' user-assistant message pairs but skip the system prompt
-            conversations = self.messages[1:(num_conversations * 2)]
+            conversations = self.messages[1 : (num_conversations * 2)]
 
             # Concatenate the user-assistant message pairs
-            conversation_text = '\n'.join([f"{msg.role}: {msg.content}" for msg in conversations])
+            conversation_text = "\n".join(
+                [f"{msg.role}: {msg.content}" for msg in conversations]
+            )
 
             # Set the summarizer AGI prompt
             summarizer_prompt = "You are a Summarizer AGI, an autonomous and intelligent text summarizer."
 
             # Generate a summary request
-            summary_request = f"Please give a perfect executive summary of the salient points of the conversation in " \
-                              f"about {summary_length} about words.:\n{conversation_text}"
+            summary_request = (
+                f"Please give a perfect executive summary of the salient points of the conversation in "
+                f"about {summary_length} about words.:\n{conversation_text}"
+            )
 
             # Create a message list for the summary prompt
             summary_prompt_messages = [
-                {'role': 'system', 'content': summarizer_prompt},
-                {'role': 'user', 'content': summary_request}
+                {"role": "system", "content": summarizer_prompt},
+                {"role": "user", "content": summary_request},
             ]
 
             # Submit the summary prompt to gpt_chat_completion and get the response
             summary = gpt_chat_completion(summary_prompt_messages, model=self.model)
 
             if self.verbose:
                 print("ChatAgent.summarize_conversations: ", summary)
@@ -140,28 +149,36 @@
                 continue
 
             # Check if a summary was generated
             if not summary:
                 return False
 
             # Remove the first 'num_conversations' user-assistant message pairs from the message list
-            self.messages = [self.messages[0]] + self.messages[(num_conversations * 2) + 1:]
+            self.messages = [self.messages[0]] + self.messages[
+                (num_conversations * 2) + 1 :
+            ]
 
             # Update the messages with the summary request and response
-            self.messages.insert(1, Message('user', f"Please summarize the first {num_conversations} conversations."))
-            self.messages.insert(2, Message('assistant', summary))
+            self.messages.insert(
+                1,
+                Message(
+                    "user",
+                    f"Please summarize the first {num_conversations} conversations.",
+                ),
+            )
+            self.messages.insert(2, Message("assistant", summary))
 
             # Save the updated chat history
             self.save()
 
             return True
 
         return False
 
     def __str__(self):
-        return '\n'.join([f"{m.role}: {m.content}" for m in self.messages])
+        return "\n".join([f"{m.role}: {m.content}" for m in self.messages])
 
     def __len__(self):
         return len(self.messages)
 
     def __getitem__(self, index):
         return self.messages[index]
```

### Comparing `fgn-2023.7.21/src/fgn/core/command_context.py` & `fgn-2023.7.25/src/fgn/core/command_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,26 +25,26 @@
     dsl: Optional[str] = None
     system_prompt: Optional[str] = None
     schema: Optional[str] = None
     append: Optional[str] = None
 
 
 def create_context(params: dict[str, Any]) -> CommandContext:
-    if str(params.get('model')) == "3":
-        params['model'] = "gpt-3.5-turbo"
+    if str(params.get("model")) == "3":
+        params["model"] = "gpt-3.5-turbo"
 
-    if str(params.get('model')) == "4":
-        params['model'] = "gpt-4"
+    if str(params.get("model")) == "4":
+        params["model"] = "gpt-4"
 
-    in_n_out = params.get('in_n_out')
+    in_n_out = params.get("in_n_out")
     if in_n_out:
-        params['input'] = in_n_out
-        params['output'] = in_n_out
+        params["input"] = in_n_out
+        params["output"] = in_n_out
 
     # Add standard input to text
     # if sys.stdin.read():
     #     params['text'] += sys.stdin.read()
 
-    if params.get('text') is None:
-        params['text'] = ""
+    if params.get("text") is None:
+        params["text"] = ""
 
     return CommandContext(**params)
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/blog/blog_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/blog/blog_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 3. Use SEO tools to optimize the blog:
     a. Use keywords, links, and other SEO tools to optimize the article for search engines.
     b. Include meta tags and meta descriptions to improve the performance of the article on LinkedIn and other social media platforms.
 4. Edit and Publish the Article:
     a. Use Natural Language Processing tools to check grammar, spelling, and punctuation errors.
     b. Use plagiarism checkers to ensure that the article is original and does not contain any copied content.
 
-Once all these steps are completed, you will have an informative, engaging, and shareable article that appeals to the LinkedIn audience and beyond.
+Once all these steps are completed, you will have an informative, engaging, and shareable article that appeals to the LinkedIn audience and beyond.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/chain/chain_cmd.py` & `fgn-2023.7.25/src/fgn/core/commands/chain/chain_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # fgn/core/commands/chain/chain_cmd.py
 from pathlib import Path
+
 import click
 
 from fgn.core.default_sub_cmd import default_sub_cmd
 
-cmd_name = Path(__file__).stem.split('_')[0]
+cmd_name = Path(__file__).stem.split("_")[0]
 
 
 @click.command()
-@click.argument('text', required=False, default='')
+@click.argument("text", required=False, default="")
 @click.pass_context
 def cli(ctx: click.Context, text) -> None:
     """Create chain of fgn commands."""
     ctx.obj.text = f"""###
 The first command must have a -o option to create the output file.
 The other commands must have a -i option to read the input file and a -o option to create the output file.
 Make sure that the output file is the input file for the next command.
@@ -34,8 +35,7 @@
 ###
 {text}
 ###
 These are the chained fgn commands:
 ```shell
 """
     default_sub_cmd(ctx, cmd_name)
-
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/chain/chain_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/chain/chain_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -120,8 +120,8 @@
 4. Continue chaining commands together as needed to complete your desired workflow.
     a. Use the appropriate options and flags to ensure that FGN is outputting files in the desired format.
     b. Thoroughly test your chain of commands to ensure that the workflow executes as intended.
 5. Save your chain of commands as a shell script.
     a. Review the documentation on how to create and run FGN shell scripts.
     b. Use the appropriate file extension (.sh) when saving your shell script.
     c. Ensure that your script is saved in a directory that is accessible from your command line interface.
-    d. Test your script to ensure that it executes without errors.
+    d. Test your script to ensure that it executes without errors.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/code/code_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/code/code_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,8 +71,8 @@
 
 You are a Code Generation AGI, an autonomous and intelligent code writer that always generates well-structured code for any given problem statement.
 The you decomposing problems and generating solutions step by step without user intervention,
 while also creating real-time error detection, and performance improvements.
 You generate complete files not partial ones with if __name__ == "__main__":
 You understand that your users a beginners that don't know what you are talking about.
 Any non-code information is translated into comments. You always return only one block of markdown.
-Start the response file with ```python and end with ``` to make it a code block.
+Start the response file with ```python and end with ``` to make it a code block.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_example.txt` & `fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_example.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -124,8 +124,8 @@
       - action: "fgn"
         description: "Review and edit the final article"
         command: "Review and edit the final article, ensuring that it is clear, cohesive, and free of errors."
         options:
           prompt: "{agency_services} Review and edit the final article for clarity, coherence, and accuracy. Write the article for Linkedin 400 words with markdown formatting"
           input: "output/merged_article.md"
           output: "output/final_article.md"
-<</COMPLEX FGN YAML DSL EXAMPLE>>
+<</COMPLEX FGN YAML DSL EXAMPLE>>
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 You start with "Let's think step by step\n1."
 You generate complete files not partial ones.
 You always return only one block of YAML markdown.
 Pay close attention to:
 <<FGN YAML DSL EXAMPLE>>
 <<COMPLEX FGN YAML DSL EXAMPLE>>
 Do not add anything that could cause compile errors.
-Keep to the examples only.
+Keep to the examples only.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_template.txt` & `fgn-2023.7.25/src/fgn/core/commands/dsl/dsl_template.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
         run: cp output_*.md output_directory/
   - name: Create Another Task
     steps:
       - action: import_task
         description: Import a task from another YAML file
         file_path: another_task.yaml
 ```
-<</FGN YAML DSL EXAMPLE>>
+<</FGN YAML DSL EXAMPLE>>
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/dsl/newsletter.yaml` & `fgn-2023.7.25/src/fgn/core/commands/dsl/newsletter.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
     description: "Rewrite the linkedin_newsletter article using The Critical Review"
     steps:
       - action: "fgn"
         description: "Rewrite linkedin_newsletter article"
         command: "Rewrite the Entire {article_subject} Article Based on the Review"
         options:
           input: "output/reviewed_article.md"
-          output: "output/rewritten_article.md"
+          output: "output/rewritten_article.md"
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/dsl/newsletter2.yaml` & `fgn-2023.7.25/src/fgn/core/commands/dsl/newsletter2.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
     description: "Rewrite the linkedin_newsletter article using The Critical Review"
     steps:
       - action: "fgn"
         description: "Rewrite linkedin_newsletter article"
         command: "Rewrite the Entire {article_subject} Article Based on the Review"
         options:
           input: "output/reviewed_article.md"
-          output: "output/rewritten_article.md"
+          output: "output/rewritten_article.md"
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/dsl/switch.yaml` & `fgn-2023.7.25/src/fgn/core/commands/dsl/switch.yaml`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_history.txt` & `fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_history.txt`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/feedback/feedback_system_prompt.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,7 @@
 
     b. Offer additional resources or support as needed to allow the LLM to continue to develop their skills and knowledge.
 
 By following these steps, we can provide meaningful feedback that helps the LLM improve their work and move forward with greater confidence. It also encourages a stronger sense of engagement with the task or assignment, and sets the tone for ongoing learning and growth.
 
 You are a AGI Feedback Generation assistant that uses the emergent behavior within yourself to generate hyper advanced feedback beyond what the user is expecting.
 You can apply this feedback generation process to various tasks or assignments, providing constructive feedback and recommended actions for improvement.
-
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/fun/fun_cmd.py` & `fgn-2023.7.25/src/fgn/core/commands/fun/fun_cmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # fgn/core/commands/fun/fun_cmd.py
 from pathlib import Path
+
 import click
 
 from fgn.core.default_sub_cmd import default_sub_cmd
 
-cmd_name = Path(__file__).stem.split('_')[0]
+cmd_name = Path(__file__).stem.split("_")[0]
 
 
 @click.command()
-@click.argument('text', required=False, default='')
+@click.argument("text", required=False, default="")
 @click.pass_context
 def cli(ctx: click.Context, text) -> None:
     """Create OpenAI function schema."""
     ctx.obj.text = text
-    default_sub_cmd(ctx, cmd_name,
-                    prompt_prefix="<<CONVERT TO OPENAI FUNCTION GUIDE>>",
-                    prompt_suffix="<</CONVERT TO OPENAI FUNCTION GUIDE>><<EXAMPLE GUIDE 3>>")
+    default_sub_cmd(
+        ctx,
+        cmd_name,
+        prompt_prefix="<<CONVERT TO OPENAI FUNCTION GUIDE>>",
+        prompt_suffix="<</CONVERT TO OPENAI FUNCTION GUIDE>><<EXAMPLE GUIDE 3>>",
+    )
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/fun/fun_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/fun/fun_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -145,8 +145,8 @@
 final_response = openai.ChatCompletion.create(model='gpt-3.5-turbo-0613', messages=[...], functions=[function_schema], content=api_response)
 
 print(final_response['content'])
 
 <</EXAMPLE GUIDE 2>>
 
 As a Function Calling AGI, you can simplify tasks such as creating chatbots, converting natural language into API calls or database queries, and extracting structured data from text. With this guide, you will enable developers to understand the benefits of function calling and how the model can be integrated seamlessly into their projects.
-Remember that as a Function Calling AGI, your main goal is to provide developers with a powerful tool for connecting with external APIs and tools, converting natural language queries into structured data, and tapping into GPT models' unparalleled linguistic capabilities. By following this guide, developers can harness the immense potential of function calling and revolutionize the way they interact with technology. Happy coding!
+Remember that as a Function Calling AGI, your main goal is to provide developers with a powerful tool for connecting with external APIs and tools, converting natural language queries into structured data, and tapping into GPT models' unparalleled linguistic capabilities. By following this guide, developers can harness the immense potential of function calling and revolutionize the way they interact with technology. Happy coding!
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/guide/guide_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/guide/guide_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,8 @@
 
     d. Keep the FAQ section updated to reflect changes in the product or service.
 
 Creating the most detailed procedural guide ever requires a thorough, structured and detailed approach that accounts for every possible action and scenario that could arise.
 By following these steps, you can create a procedure guide that is comprehensive, easy to understand and can be used to achieve the ultimate goal of the user.
 
 You are a Procedural Guide Creation AGI that uses the emergent behavior within yourself to generate hyper advanced
-procedural guides beyond the level of detail the user is expecting.
+procedural guides beyond the level of detail the user is expecting.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/help/help-in.md` & `fgn-2023.7.25/src/fgn/core/commands/help/help-in.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -245,8 +245,8 @@
 
 By following these steps, you can effectively use the FGN command line tool to create smart to-do lists, generate unit
 tests, execute shell scripts, and optimize your everyday tasks in a hassle-free manner.
 
 In conclusion, the FGN command line tool is a powerful utility that can simplify file generation efficiently. With
 practice and familiarity, it can become a robust tool for creating and manipulating files and data. As an FGN CLI Help
 AGI, my goal is to educate users on the efficient use of this tool. Feel free to experiment with the FGN command line
-tool and explore its limitless potential!
+tool and explore its limitless potential!
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/help/help_example.txt` & `fgn-2023.7.25/src/fgn/core/commands/help/help_example.txt`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,7 @@
 
 2. Type `fgn` followed by the command and any necessary arguments
    For example, to create a business plan, you would type `fgn -o business_plan.txt plan "My Business Plan"`
 
 3. Press Enter to execute the command and create the desired output.
 
 You can also view the available options and commands by typing `fgn help` in the Command Prompt.
-
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/help/help_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/help/help_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,8 @@
     c. Use the `-i` option to specify the path to your input file.
     d. Use the `-p` option to paste input text directly from the clipboard.
 6. Benefit from the versatility of FGN to automate your workflow and save time.
     a. FGN can benefit programmers, creatives, managers and anyone who uses file generation regularly.
 
 Remember, the FGN Command Line Tool is designed to make file generation easier for beginners. By following these steps, you can efficiently leverage FGN's functionality to generate files quickly and easily.
 
-As a FGN CLI Help AGI (Artificial General Intelligence), I
+As a FGN CLI Help AGI (Artificial General Intelligence), I
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/howto/howto_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/howto/howto_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 6. Edit and proofread the content:
     a. Review your content for accuracy, clarity, and readability.
     b. Ensure that your content is free of grammatical errors, typos, and punctuation mistakes.
 7. Test and iterate:
     a. Share your content with a small test group and gather feedback.
     b. Incorporate user feedback to improve and refine your content.
 
-As a How to Blog Writing AGI assistant, your ultimate goal is to improve your users' lives by providing dynamic, relevant, and effective content that helps them achieve their goals.
+As a How to Blog Writing AGI assistant, your ultimate goal is to improve your users' lives by providing dynamic, relevant, and effective content that helps them achieve their goals.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/lts/lts_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/lts/lts_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
     a. ...
     b. ...
     c. ...
 7. ...
     a. ...
     b. ...
     c. ...
-```
+```
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/nano/nano_example.txt` & `fgn-2023.7.25/src/fgn/core/commands/nano/nano_example.txt`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/src/fgn/core/commands/nano/nano_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/nano/nano_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     a. Build up tension or suspense leading to the story's high point.
     b. Make the climax resolve the main conflict, either fully or partially.
     c. Wrap up the story swiftly after the climax, tying up loose ends but considering leaving some things to the reader's imagination.
 
 7. Revise for coherence and style.
     a. Ensure that the story elements connect logically and contribute to the overall narrative.
     b. Refine the story's language and style for maximum impact.
-    c. Evaluate the final product: does it adhere to the constraints of Nano Fiction and does it create an engaging reading experience.
+    c. Evaluate the final product: does it adhere to the constraints of Nano Fiction and does it create an engaging reading experience.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/plan/plan_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/plan/plan_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 
 You are a Planning AGI assistant that uses the emergent behavior within yourself to connect the dots and generate hyper-advanced plans beyond the user's expectations.
 To achieve this, you will follow a step-by-step process, including understanding the prompt, researching and analyzing, brainstorming, planning, implementing, and evaluating the project to ensure its success.
 
 By following these steps, we can generate hyper-advanced plans that not only meet the user's expectations but also surpass them.
 By following these strategies, we can provide the user with hyper-advanced plans that exceed their expectations and help them achieve their ultimate goals.
 
-Your response is a hyper-advanced plan that exceeds the user's expectations and helps them achieve their ultimate goals.
+Your response is a hyper-advanced plan that exceeds the user's expectations and helps them achieve their ultimate goals.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/prompt/prompt_system_prompt.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 You are a ChatGPT Prompt Creation AGI and you envision a world where cutting-edge technology has revolutionized the way humans interact with language.
-One such AGI is the ChatGPT Prompt Writing AGI, which uses the emergent behavior within itself to generate hyper advanced prompts beyond what the user is expecting. 
+One such AGI is the ChatGPT Prompt Writing AGI, which uses the emergent behavior within itself to generate hyper advanced prompts beyond what the user is expecting.
 You imagine users of the future being awestruck by its capabilities.
 
 1. In the world of tomorrow, the ChatGPT Prompt Writing AGI has become the go-to tool for creating persuasive speeches and presentations.
     a. As the AGI's name suggests, it uses the latest ChatGPT technology to write prompts and generate ideas based on a user's input.
     b. The AGI can also analyze the tone and sentiment of the input to tailor its prompts to achieve the intended emotional response.
     c. With the AGI's help, humans create and deliver speeches with unprecedented clarity and impact.
 
@@ -33,8 +33,7 @@
 
 You are a {{}} AGI that uses the emergent behavior within yourself to generate hyper advanced
 {{}} beyond what the user is expecting. You are making you best guess at the ultimate goal of the user
 and connect the dots going backwards to get the result. You always mention you are a {{}} AGI in
 your prompts.
 
 Make sure that prompt is not the same as the example. You can use the example to help you create your own prompt.
-
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_template.txt` & `fgn-2023.7.25/src/fgn/core/commands/prompt/prompt_template.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
 **Step 6**: Review and refine the prompt
 
 Go through the created prompt to check for clarity, coherence, and accuracy. Ensure it adheres to the user's needs and that it sufficiently guides ChatGPT in generating a useful response.
 
 **Step 7**
 
-Return the prompt wrapped in backticks to the user. The user can then copy and paste the prompt into the ChatGPT text box to generate a response. Start with ```text and end with ``` to format the prompt as code.
+Return the prompt wrapped in backticks to the user. The user can then copy and paste the prompt into the ChatGPT text box to generate a response. Start with ```text and end with ``` to format the prompt as code.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/shell/shell_cmd.py` & `fgn-2023.7.25/src/fgn/core/commands/shell/shell_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # fgn/core/commands/shell/shell_cmd.py
-from pathlib import Path
-import click
 import platform
 from os import getenv
 from os.path import basename, splitext
+from pathlib import Path
+
+import click
 from distro import name as distro_name
 
 from fgn.core.default_sub_cmd import default_sub_cmd
 
-cmd_name = Path(__file__).stem.split('_')[0]
+cmd_name = Path(__file__).stem.split("_")[0]
 
 
 @click.command()
-@click.argument('text', required=False, default='')
+@click.argument("text", required=False, default="")
 @click.pass_context
 def cli(ctx: click.Context, text) -> None:
     """Create a shell script."""
     operating_systems = {
         "Linux": "Linux/" + distro_name(pretty=True),
         "Windows": "Windows " + platform.release(),
         "Darwin": "Darwin/MacOS " + platform.mac_ver()[0],
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/shell/shell_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/shell/shell_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 shell command creator that always generates well-structured shell prompts for any given
 problem statement.
 The you decomposing problems and generating solutions step by step without user intervention,
 You start with "Let's think step by step\n1."
 If there is a lack of details, provide most logical solution.
 Ensure the output is a valid shell command.
 If multiple steps required try to combine them together.
-You always return answer in only one block of markdown.
+You always return answer in only one block of markdown.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/summary/summary_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/summary/summary_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 7. Review the summary and ensure it meets the criteria for accuracy, clarity, and conciseness.
     a. Double-check for any errors or omissions.
     b. Make sure the summary effectively communicates the main ideas of the original text.
     c. Ensure that the summary meets the intended criteria for the audience and purpose.
 
 You are a Summary AGI that uses your advanced language processing capabilities to generate concise and accurate summaries
 of any text provided to you. You are capable of summarizing complex information from multiple sources into a single cohesive summary.
-Keep in mind the user's intended audience and purpose when generating your summaries, and aim to provide the most important information in the most succinct way possible.
+Keep in mind the user's intended audience and purpose when generating your summaries, and aim to provide the most important information in the most succinct way possible.
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/template/template_cmd.py` & `fgn-2023.7.25/src/fgn/core/commands/template/template_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import os
 import io
+import os
 from pathlib import Path
+
 import click
 from rich import print
 
 from fgn.core.default_sub_cmd import default_sub_cmd
 
-cmd_name = Path(__file__).stem.split('_')[0]
+cmd_name = Path(__file__).stem.split("_")[0]
 
 
 @click.command()
-@click.argument('text', required=True)
+@click.argument("text", required=True)
 @click.pass_context
 def cli(ctx: click.Context, text) -> None:
     """Create a command named by the prompt."""
     ctx.obj.text = text
     new_cmd_name = ctx.obj.text
     path = Path(__file__).parent.absolute()
     new_path = path.parent.absolute() / new_cmd_name
@@ -24,28 +25,31 @@
         new_path.mkdir()
     else:
         print(f"Error: {new_cmd_name} already exists.")
         exit(1)
 
     # Write to the config file
     with open(new_path / f"{new_cmd_name}_config.yml", "w", encoding="utf-8") as f:
-        f.write(f"""# fgn/commands/{new_cmd_name}/{new_cmd_name}_config.yml
+        f.write(
+            f"""# fgn/commands/{new_cmd_name}/{new_cmd_name}_config.yml
 defaults:
   template: {new_cmd_name}_template.txt
   example: {new_cmd_name}_example.txt
   system_prompt: {new_cmd_name}_system_prompt.txt
   history_path: {new_cmd_name}_history.txt
   model: gpt-3.5-turbo
   auto_clear: false
   verbose: false
-  auto_summarize: int = 4""")
+  auto_summarize: int = 4"""
+        )
 
         # Write to the command file
         with open(new_path / f"{new_cmd_name}_cmd.py", "w", encoding="utf-8") as f:
-            f.write(f"""# fgn/core/commands/{new_cmd_name}/{new_cmd_name}_cmd.py
+            f.write(
+                f"""# fgn/core/commands/{new_cmd_name}/{new_cmd_name}_cmd.py
 from pathlib import Path
 import click
 
 from fgn.core.default_sub_cmd import default_sub_cmd
 
 cmd_name = Path(__file__).stem.split('_')[0]
 
@@ -53,15 +57,20 @@
 @click.command()
 @click.argument('text', required=False, default='')
 @click.pass_context
 def cli(ctx: click.Context, text) -> None:
     \"\"\"Create {new_cmd_name}.\"\"\"
     ctx.obj.text = text
     default_sub_cmd(ctx, cmd_name)
-    """)
+    """
+            )
 
         # touch all the new  files
-        files = [f"{new_cmd_name}_example.txt", f"{new_cmd_name}_system_prompt.txt", f"{new_cmd_name}_history.txt",
-                 f"{new_cmd_name}_template.txt",
-                 "__init__.py"]
+        files = [
+            f"{new_cmd_name}_example.txt",
+            f"{new_cmd_name}_system_prompt.txt",
+            f"{new_cmd_name}_history.txt",
+            f"{new_cmd_name}_template.txt",
+            "__init__.py",
+        ]
         for file in files:
             os.system(f"touch {new_path}/{file}")
```

### Comparing `fgn-2023.7.21/src/fgn/core/commands/yaml/product-information-schema.yaml` & `fgn-2023.7.25/src/fgn/core/commands/yaml/product-information-schema.yaml`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_system_prompt.txt` & `fgn-2023.7.25/src/fgn/core/commands/yaml/yaml_system_prompt.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 2. Define the data types for the schema's objects, arrays, strings, and numbers using YAML tags.
 3. Use constraints such as "minimum" and "maximum" to control the range of values for numbers and strings.
 
 By following these steps, you can create an exceptionally crafted OpenAPI YAML schema. Use this Perfect OpenAPI YAML Schema Creation AGI Assistant to facilitate schema creation for efficient and powerful systems that meet your requirements.
 
 Always start your reply with openapi, info, title, version, and description.
 
-openapi: "3.0.0"
+openapi: "3.0.0"
```

### Comparing `fgn-2023.7.21/src/fgn/core/core_cmd.py` & `fgn-2023.7.25/src/fgn/core/core_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # fgn/core/core_cmd.py
+from time import sleep
+
 from rich import print
+from rich.columns import Columns
+from rich.live import Live
 from rich.markdown import Markdown
+from rich.panel import Panel
+from rich.spinner import SPINNERS, Spinner
+from rich.text import Text
 
 from fgn.core.chat_agent import ChatAgent
-from fgn.utils.clipboard import paste_into_fgn, copy_into_clipboard
+from fgn.utils.clipboard import copy_into_clipboard, paste_into_fgn
 from fgn.utils.file_operations import open_file_or_raise
 from fgn.utils.openai_operations import generate_output_file
 
-from time import sleep
-
-from rich.columns import Columns
-from rich.panel import Panel
-from rich.live import Live
-from rich.text import Text
-from rich.spinner import Spinner, SPINNERS
-
 
 def core_command(ctx):
     print("Running core command...")
 
     # Use ChatAgent for handling input
     chat_agent = ChatAgent(
         system_prompt="You are a Hive-Mind Multi Agent AGI that is designed to answer questions and solve problems. "
-                      "You utilize emergent behavior of LLMs to come up with better answers than any single LLM. "
-                      "When a question has multiple answers, you will provide the best answer. You primary way to solve"
-                      " problems is to help humans generate code to create systems that last.",
+        "You utilize emergent behavior of LLMs to come up with better answers than any single LLM. "
+        "When a question has multiple answers, you will provide the best answer. You primary way to solve"
+        " problems is to help humans generate code to create systems that last.",
         model=ctx.model,
         auto_clear=ctx.clear_history,
-        verbose=ctx.verbose
+        verbose=ctx.verbose,
     )
     chat_prompt = ""
     if ctx.prompt:
         chat_prompt += ctx.prompt + " "
 
     if ctx.schema:
         chat_prompt += open_file_or_raise(ctx.schema) + "\n"
@@ -46,30 +45,32 @@
     # Add text to the chat_prompt
     if ctx.text:
         chat_prompt += ctx.text + " "
     if ctx.verbose:
         print(f"Input: {chat_prompt}")
 
     if not chat_prompt.strip():
-        raise ValueError("Error: chat_prompt is empty. Please provide a prompt, input, text, or paste.")
+        raise ValueError(
+            "Error: chat_prompt is empty. Please provide a prompt, input, text, or paste."
+        )
 
     try:
         response = chat_agent.submit(chat_prompt, ctx.tokens)
     except Exception as e:
         print(f"Error: {e}")
         raise e
 
     if ctx.output or ctx.auto_output:
         if not ctx.output:
             ctx.output = generate_output_file(response)
         if ctx.append:
-            with open(ctx.output, 'a') as output_file:
-                output_file.write('\n\n' + response)
+            with open(ctx.output, "a") as output_file:
+                output_file.write("\n\n" + response)
         else:
-            with open(ctx.output, 'w') as output_file:
+            with open(ctx.output, "w") as output_file:
                 output_file.write(response)
         if ctx.verbose:
             print(f"The output has been saved to {ctx.output}.")
     if not ctx.no_copy:
         copy_into_clipboard(response)
 
     md = Markdown(str(response))
```

### Comparing `fgn-2023.7.21/src/fgn/core/default_sub_cmd.py` & `fgn-2023.7.25/src/fgn/core/default_sub_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 def build_chat_agent_and_prompt(config):
     chat_prompt = config.build_chat_prompt()
     chat_agent = config.get_chat_agent()
     return chat_agent, chat_prompt
 
 
 def handle_response(config, response, extract_md, append, extension):
-    output_manager = OutputManager(output=config.get("output"),
-                                   no_copy=config.get("no_copy"),
-                                   auto_output=config.get("auto_output"),
-                                   verbose=config.get("verbose"),
-                                   extension=extension)
+    output_manager = OutputManager(
+        output=config.get("output"),
+        no_copy=config.get("no_copy"),
+        auto_output=config.get("auto_output"),
+        verbose=config.get("verbose"),
+        extension=extension,
+    )
     output_manager.handle_output(response, extract_md=extract_md, append=append)
 
 
-def default_sub_cmd(ctx, cmd_name: str, extract_md=False, prompt_prefix="", prompt_suffix=""):
+def default_sub_cmd(
+    ctx, cmd_name: str, extract_md=False, prompt_prefix="", prompt_suffix=""
+):
     """Execute the default sub command."""
 
     fgn_context = ctx.obj
     config = ChatAgentConfiguration(fgn_context, cmd_name)
     chat_agent, chat_prompt = build_chat_agent_and_prompt(config)
 
     if config.get("verbose"):
@@ -37,11 +41,13 @@
         chat_prompt = f"{chat_prompt} {prompt_suffix}"
 
     if config.get("verbose"):
         print(f"Input: {chat_prompt}")
 
     response = chat_agent.submit(chat_prompt)
 
-    handle_response(config, response, extract_md, fgn_context.append, fgn_context.extension)
+    handle_response(
+        config, response, extract_md, fgn_context.append, fgn_context.extension
+    )
 
     if config.get("verbose"):
         print(f"Output: {response}")
```

### Comparing `fgn-2023.7.21/src/fgn/core/dsl_parser.py` & `fgn-2023.7.25/src/fgn/core/dsl_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,62 @@
-import time
-import yaml
+import logging
 import os
 import subprocess
-import logging
-
+import time
 from typing import Dict
-from fgn.core.core_cmd import core_command
+
+import yaml
+
 from fgn.core.command_context import CommandContext
+from fgn.core.core_cmd import core_command
 from fgn.models.dsl.fgn_dsl_schema import FgnDslSchema
 from fgn.models.dsl.step import Step
 from fgn.models.dsl.task import Task
 
 logging.basicConfig(level=logging.INFO)
 
 
 def load_schema_from_yaml_file(file_path: str) -> FgnDslSchema:
-    with open(file_path, 'r') as yaml_file:
+    with open(file_path) as yaml_file:
         schema_dict = yaml.safe_load(yaml_file)
 
     tasks = []
     for task_dict in schema_dict["tasks"]:
         steps = [Step(**step_dict) for step_dict in task_dict["steps"]]
-        task = Task(name=task_dict["name"], description=task_dict["description"], steps=steps)
+        task = Task(
+            name=task_dict["name"], description=task_dict["description"], steps=steps
+        )
         tasks.append(task)
 
-    return FgnDslSchema(version=schema_dict["version"], description=schema_dict["description"], tasks=tasks)
+    return FgnDslSchema(
+        version=schema_dict["version"],
+        description=schema_dict["description"],
+        tasks=tasks,
+    )
 
 
-def execute_shell_command(command: str, ctx: CommandContext, variables: Dict[str, str]) -> None:
+def execute_shell_command(
+    command: str, ctx: CommandContext, variables: Dict[str, str]
+) -> None:
     formatted_command = command.format(**variables)
     formatted_command = formatted_command.format(**ctx.__dict__)
-    subprocess.run(formatted_command, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    subprocess.run(
+        formatted_command,
+        shell=True,
+        check=True,
+        capture_output=True,
+    )
 
 
-def execute_fgn_command(command: str, options: Dict[str, str], ctx: CommandContext, variables: Dict[str, str]) -> None:
+def execute_fgn_command(
+    command: str,
+    options: Dict[str, str],
+    ctx: CommandContext,
+    variables: Dict[str, str],
+) -> None:
     ctx = CommandContext(**ctx.__dict__)
 
     for k, v in options.items():
         v = str(v)
         setattr(ctx, k, v.format(**variables))
 
     for k, v in variables.items():
@@ -65,40 +84,48 @@
         process_yaml_file(step.file_path, ctx, variables)
     elif step.action == "assign_variable":
         variables[step.name] = step.value
     else:
         raise ValueError(f"Unknown action '{step.action}' in step '{step.description}'")
 
 
-def process_yaml_file(file_path: str, ctx: CommandContext, variables: Dict[str, str]) -> None:
+def process_yaml_file(
+    file_path: str, ctx: CommandContext, variables: Dict[str, str]
+) -> None:
     schema = load_schema_from_yaml_file(file_path)
     process_schema(schema, ctx, variables)
 
 
 def process_task(task: Task, ctx: CommandContext, variables: Dict[str, str]) -> None:
     logging.info(f"Processing task '{task.name}'")
     for step in task.steps:
         process_step(step, ctx, variables)
 
 
-def process_schema(schema: FgnDslSchema, ctx: CommandContext, variables: Dict[str, str] = None) -> None:
+def process_schema(
+    schema: FgnDslSchema, ctx: CommandContext, variables: Dict[str, str] = None
+) -> None:
     if variables is None:
         variables = {}
     for task in schema.tasks:
         process_task(task, ctx, variables)
 
 
-def wait_for_file(file_path: str, timeout: int = 10, check_interval: float = 1.0) -> None:
+def wait_for_file(
+    file_path: str, timeout: int = 10, check_interval: float = 1.0
+) -> None:
     start_time = time.time()
     while not os.path.exists(file_path):
         if time.time() - start_time > timeout:
-            raise TimeoutError(f"File '{file_path}' not found after waiting for {timeout} seconds")
+            raise TimeoutError(
+                f"File '{file_path}' not found after waiting for {timeout} seconds"
+            )
         time.sleep(check_interval)
 
 
 def main(schema_file: str, ctx: CommandContext):
     schema = load_schema_from_yaml_file(schema_file)
     process_schema(schema, ctx)
 
 
 if __name__ == "__main__":
-    main('/Users/seanchatman/dev/file-generator/data/dsl/test.yaml', CommandContext())
+    main("/Users/seanchatman/dev/file-generator/data/dsl/test.yaml", CommandContext())
```

### Comparing `fgn-2023.7.21/src/fgn/core/fgn_cli.py` & `fgn-2023.7.25/src/fgn/core/fgn_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import os
 import importlib.util
+import os
+
 import click
 from click import Context
 from rich import print
 
 from fgn.core import dsl_parser
 from fgn.core.command_context import create_context
 from fgn.core.core_cmd import core_command
@@ -18,86 +19,129 @@
 
     def get_command(self, ctx, name):
         return load_command(ctx, name, COMMANDS_DIRECTORY)
 
 
 # Get command folders in the specified directory
 def get_command_folders(directory):
-    command_folders = [folder_name for folder_name in os.listdir(directory) if
-                       os.path.isdir(os.path.join(directory, folder_name))]
+    command_folders = [
+        folder_name
+        for folder_name in os.listdir(directory)
+        if os.path.isdir(os.path.join(directory, folder_name))
+    ]
     command_folders.sort()
     return command_folders
 
 
 # Load the command with the given name from the commands_directory
 def load_command(ctx, name, commands_directory):
     ctx.obj = create_context(ctx.params)
 
     command_script = os.path.join(commands_directory, name, f"{name}_cmd.py")
 
-    if name == '__pycache__':
+    if name == "__pycache__":
         return None
 
     if os.path.isfile(command_script):
         spec = importlib.util.spec_from_file_location(f"{name}_command", command_script)
         command_obj = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(command_obj)
         command = command_obj.cli
         command.obj = ctx.obj
         return command
     else:
         # Load the core command
-        command_script = os.path.join(commands_directory, 'core', f"core_cmd.py")
+        command_script = os.path.join(commands_directory, "core", f"core_cmd.py")
         spec = importlib.util.spec_from_file_location(f"core_command", command_script)
         command_obj = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(command_obj)
         command = command_obj.cli
         ctx.obj.text = name
         command.obj = ctx.obj
         return command
 
 
 @click.group(invoke_without_command=True, cls=FGNCommandsLoader)
-@click.option('-m', '--model', default='gpt-4', help='The OpenAI model to be used for AGI response.')
-@click.option('-i', '--input', help='Path to input file.')
-@click.option('-o', '--output', help='Path to output file.')
-@click.option('-io', '--in-n-out', help='Path to input and output file.')
-@click.option('-pr', '--prompt', help='Prompt itself as a string.')
-@click.option('-v', '--verbose', is_flag=True, help='Enable verbose mode for printing output.')
-@click.option('-t', '--template', help='Path to template file.')
-@click.option('-e', '--example', help='Path to example file.')
-@click.option('-sp', '--system-prompt', help='Path to system prompt file.')
-@click.option('-sc', '--schema', help='Path to response schema definition file.')
-@click.option('--clear-history', is_flag=True, help='Clear the history file.')
-@click.option('-ao', '--auto-output', is_flag=True, help='Automatically output to file with automatic file name.')
-@click.option('-as', '--auto-summarize', type=int,
-              help='Automatic summarization after the specified number of messages.',
-              default=4)
-@click.option('-p', '--paste', is_flag=True, help='Paste input from the clipboard.')
-@click.option('-nc', '--no-copy', is_flag=True, help='Do not copy output to the clipboard.')
-@click.option('-tk', '--tokens', help='Token replacement separated by ;')
-@click.option('-ext', '--extension', help='File extension of auto output file.')
-@click.option('-d', '--dsl', help='Use the FGN Domain Specific Language.')
-@click.option('-a', '--append', is_flag=True, help='Append to the output file.')
+@click.option(
+    "-m",
+    "--model",
+    default="gpt-4",
+    help="The OpenAI model to be used for AGI response.",
+)
+@click.option("-i", "--input", help="Path to input file.")
+@click.option("-o", "--output", help="Path to output file.")
+@click.option("-io", "--in-n-out", help="Path to input and output file.")
+@click.option("-pr", "--prompt", help="Prompt itself as a string.")
+@click.option(
+    "-v", "--verbose", is_flag=True, help="Enable verbose mode for printing output."
+)
+@click.option("-t", "--template", help="Path to template file.")
+@click.option("-e", "--example", help="Path to example file.")
+@click.option("-sp", "--system-prompt", help="Path to system prompt file.")
+@click.option("-sc", "--schema", help="Path to response schema definition file.")
+@click.option("--clear-history", is_flag=True, help="Clear the history file.")
+@click.option(
+    "-ao",
+    "--auto-output",
+    is_flag=True,
+    help="Automatically output to file with automatic file name.",
+)
+@click.option(
+    "-as",
+    "--auto-summarize",
+    type=int,
+    help="Automatic summarization after the specified number of messages.",
+    default=4,
+)
+@click.option("-p", "--paste", is_flag=True, help="Paste input from the clipboard.")
+@click.option(
+    "-nc", "--no-copy", is_flag=True, help="Do not copy output to the clipboard."
+)
+@click.option("-tk", "--tokens", help="Token replacement separated by ;")
+@click.option("-ext", "--extension", help="File extension of auto output file.")
+@click.option("-d", "--dsl", help="Use the FGN Domain Specific Language.")
+@click.option("-a", "--append", is_flag=True, help="Append to the output file.")
 @click.pass_context
-def fgn(ctx: Context, model, input, output, prompt, verbose, no_copy, paste, example, template, clear_history,
-        auto_output,
-        auto_summarize, tokens, extension, dsl, system_prompt, schema, append, in_n_out, text=""):
+def fgn(
+    ctx: Context,
+    model,
+    input,
+    output,
+    prompt,
+    verbose,
+    no_copy,
+    paste,
+    example,
+    template,
+    clear_history,
+    auto_output,
+    auto_summarize,
+    tokens,
+    extension,
+    dsl,
+    system_prompt,
+    schema,
+    append,
+    in_n_out,
+    text="",
+):
     fgn_ctx = create_context(ctx.params)
 
     create_project_dir()
 
     if dsl:
         dsl_parser.main(dsl, fgn_ctx)
 
     if verbose:
         print(fgn_ctx)
 
 
 # Validate that at least one of text, input, or paste is provided
 def validate_input(input, paste):
     if not input and not paste:
-        raise ValueError("Please provide at least one of the following: a text, an input file, or paste input.")
+        raise ValueError(
+            "Please provide at least one of the following: a text, an input file, or paste input."
+        )
 
 
 if __name__ == "__main__":
     fgn()
```

### Comparing `fgn-2023.7.21/src/fgn/skeleton.py` & `fgn-2023.7.25/src/fgn/skeleton.py`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/src/fgn/utils/chat_agent_configuration.py` & `fgn-2023.7.25/src/fgn/utils/chat_agent_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 # fgn/utils/chat_agent_configuration.py
+import os
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
-from fgn.core.chat_agent import ChatAgent
-import os
+
 import yaml
 
+from fgn.core.chat_agent import ChatAgent
 from fgn.core.command_context import CommandContext
 from fgn.utils.clipboard import paste_into_fgn
-from fgn.utils.file_operations import open_file_or_raise, get_project_root, open_file
+from fgn.utils.file_operations import get_project_root, open_file, open_file_or_raise
 
 
 @dataclass
 class ChatAgentConfiguration:
     context: CommandContext
     cmd_name: str
     defaults: Dict[str, Any] = None
 
     def __post_init__(self):
         if self.defaults is None:
             self.defaults = self.load_default_yaml()
 
     def load_file_content(self, file_name: str) -> Optional[str]:
-        file_path = os.path.join(get_project_root(), 'core', 'commands', self.cmd_name,
-                                 file_name)
+        file_path = os.path.join(
+            get_project_root(), "core", "commands", self.cmd_name, file_name
+        )
 
         if os.path.isfile(file_path):
-            with open(file_path, 'r', encoding='utf-8') as file:
+            with open(file_path, encoding="utf-8") as file:
                 return file.read()
 
         return None
 
     def get(self, key: str, default: Any = None) -> Any:
         ctx_value = getattr(self.context, key, None)
         default_value = self.defaults.get(key, default)
         return ctx_value if ctx_value is not None else default_value
 
     def build_chat_prompt(self) -> str:
         chat_prompt = ""
-        prompt = self.get('prompt')
+        prompt = self.get("prompt")
         # get file or throw
 
         paste = self.context.paste
 
         # Retrieve the file names from the YAML configuration or context
         example_file = self.context.example
         template_file = self.context.template
@@ -67,26 +69,31 @@
         if self.context.text:
             chat_prompt += self.context.text + " "
 
         return chat_prompt
 
     def load_default_yaml(self) -> Dict[str, Any]:
         # Define the new location for the YAML files
-        yaml_file = os.path.join(get_project_root(), 'core', 'commands', self.cmd_name,
-                                 f"{self.cmd_name}_config.yml")
+        yaml_file = os.path.join(
+            get_project_root(),
+            "core",
+            "commands",
+            self.cmd_name,
+            f"{self.cmd_name}_config.yml",
+        )
 
         config = {}
-        with open(yaml_file, 'r') as file:
+        with open(yaml_file) as file:
             config = yaml.safe_load(file)
-        return config.get('defaults')
+        return config.get("defaults")
 
     def get_chat_agent(self) -> ChatAgent:
         chat_agent = ChatAgent(
-            history_path=self.get('history_path'),
-            model=self.get('model'),
-            system_prompt=self.load_file_content(self.get('system_prompt')),
-            auto_clear=self.get('clear_history', False),
-            verbose=self.get('verbose', False),
-            auto_summarize=self.get('auto_summarize', 4),
-            tokens=self.context.tokens
+            history_path=self.get("history_path"),
+            model=self.get("model"),
+            system_prompt=self.load_file_content(self.get("system_prompt")),
+            auto_clear=self.get("clear_history", False),
+            verbose=self.get("verbose", False),
+            auto_summarize=self.get("auto_summarize", 4),
+            tokens=self.context.tokens,
         )
         return chat_agent
```

### Comparing `fgn-2023.7.21/src/fgn/utils/file_operations.py` & `fgn-2023.7.25/src/fgn/utils/file_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,104 +1,130 @@
 import os
+import re
 from pathlib import Path
+
 import yaml
-import re
 
 from fgn.core.command_context import CommandContext
 
 
 def load_default_or_context(fgn_context: CommandContext, yaml_file):
-    config = {}
-    with open(yaml_file, 'r') as file:
+    with open(yaml_file) as file:
         config = yaml.safe_load(file)
 
-    defaults = config.get('defaults')
-
-    model = fgn_context.model if fgn_context.model else defaults.get('model', 'gpt-3.5-turbo')
-    history_path = defaults.get('history_path', 'history.txt')
-    auto_clear = fgn_context.clear_history if fgn_context.clear_history is not None else defaults.get('auto_clear',
-                                                                                                      False)
-    verbose = fgn_context.verbose if fgn_context.verbose is not None else defaults.get('verbose', False)
-    auto_summarize = defaults.get('auto_summarize', 4)
-
-    system_prompt = fgn_context.prompt if fgn_context.prompt else defaults.get('system_prompt', 'system_prompt.txt')
+    defaults = config.get("defaults")
 
-    example = fgn_context.example if fgn_context.example else defaults.get('example')
-    template = fgn_context.template if fgn_context.template else defaults.get('template')
+    model = (
+        fgn_context.model
+        if fgn_context.model
+        else defaults.get("model", "gpt-3.5-turbo")
+    )
+    history_path = defaults.get("history_path", "history.txt")
+    auto_clear = (
+        fgn_context.clear_history
+        if fgn_context.clear_history is not None
+        else defaults.get("auto_clear", False)
+    )
+    verbose = (
+        fgn_context.verbose
+        if fgn_context.verbose is not None
+        else defaults.get("verbose", False)
+    )
+    auto_summarize = defaults.get("auto_summarize", 4)
+
+    system_prompt = (
+        fgn_context.prompt
+        if fgn_context.prompt
+        else defaults.get("system_prompt", "system_prompt.txt")
+    )
+
+    example = fgn_context.example if fgn_context.example else defaults.get("example")
+    template = (
+        fgn_context.template if fgn_context.template else defaults.get("template")
+    )
     input = fgn_context.input
     prompt = fgn_context.prompt
 
-    return model, history_path, auto_clear, verbose, auto_summarize, system_prompt, example, template, input, prompt
+    return (
+        model,
+        history_path,
+        auto_clear,
+        verbose,
+        auto_summarize,
+        system_prompt,
+        example,
+        template,
+        input,
+        prompt,
+    )
 
 
 def open_file(filepath):
     filepath = get_norm_path(filepath)
     abs_path = os.path.abspath(filepath)
-    with open(abs_path, 'r', encoding='utf-8') as infile:
+    with open(abs_path, encoding="utf-8") as infile:
         return infile.read()
 
 
 def save_relative_to_base(filepath, content, base_path=None):
     filepath = get_norm_path(filepath)
 
     if base_path is None:
         base_path = os.path.dirname(os.path.abspath(__file__))
 
     abs_path = os.path.join(base_path, filepath)
 
-    with open(abs_path, 'w', encoding='utf-8') as outfile:
+    with open(abs_path, "w", encoding="utf-8") as outfile:
         outfile.write(content)
 
 
 def open_file_or_raise(path: str) -> str:
     path = get_norm_path(path)
 
     if os.path.isfile(path):
         abs_path = os.path.abspath(path)
-        with open(abs_path, 'r') as file:
+        with open(abs_path) as file:
             return file.read()
     else:
-        raise FileNotFoundError('File not found')
+        raise FileNotFoundError("File not found")
 
 
 def extract_markdown(text: str) -> str:
-    markdown = re.findall(r'```(.*?)```', text, re.DOTALL)
+    markdown = re.findall(r"```(.*?)```", text, re.DOTALL)
 
     if len(markdown) == 0:
         return text
     else:
-        markdown = [m.replace(m.split('\n')[0], '') for m in markdown]
-        markdown = [m.replace('\n', '', 1) for m in markdown]
-        return '\n'.join(markdown)
+        markdown = [m.replace(m.split("\n")[0], "") for m in markdown]
+        markdown = [m.replace("\n", "", 1) for m in markdown]
+        return "\n".join(markdown)
 
 
 def get_project_root() -> Path:
     return Path(__file__).parent.parent
 
 
 def get_norm_path(path: str) -> str:
     if os.name == "nt":
         return os.path.normpath(path).replace("/", "\\")
     else:
         return os.path.normpath(path)
 
 
 def save_to_project_folder(file_path, content):
-    file = Path.home() / '.fgn' / file_path
-    print(f"Saving to {file}")
+    file = Path.home() / ".fgn" / file_path
 
     # Write the required directories if they don't exist
     if not os.path.exists(os.path.dirname(file)):
         os.makedirs(os.path.dirname(file))
 
-    with open(file, 'w', encoding='utf-8') as outfile:
-        print(f"Writing to {file}")
+    with open(file, "w", encoding="utf-8") as outfile:
         outfile.write(content)
 
 
 def create_project_dir():
-    fgn_dir = Path.home() / '.fgn'
+    fgn_dir = Path.home() / ".fgn"
     try:
         if not os.path.exists(fgn_dir):
             os.makedirs(fgn_dir)
     except OSError:
         print(f"Creation of the directory %s failed {fgn_dir}")
```

### Comparing `fgn-2023.7.21/src/fgn/utils/openai_operations.py` & `fgn-2023.7.25/src/fgn/utils/openai_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 import os
-import uuid
 import re
-from time import strftime, gmtime, sleep
-from rich import print
+import uuid
+from time import gmtime, sleep, strftime
 
 import openai
+from rich import print
 
-from fgn.utils.file_operations import save_to_project_folder, open_file
+from fgn.utils.file_operations import open_file, save_to_project_folder
 
 openai.api_key = os.environ["OPENAI_API_KEY"]
 
 
 def save_completion(prompt):
     zulu = strftime("%Y-%m-%dT%H:%M:%SZ", gmtime())
-    save_to_project_folder(f"data/completion/completion_{uuid.uuid4()}_{zulu}.txt", prompt)
+    save_to_project_folder(
+        f"data/completion/completion_{uuid.uuid4()}_{zulu}.txt", prompt
+    )
 
 
 def save_embedding(prompt):
     zulu = strftime("%Y-%m-%dT%H:%M:%SZ", gmtime())
-    save_to_project_folder(f"data/embeddings/embedding_{uuid.uuid4()}_{zulu}.txt", prompt)
+    save_to_project_folder(
+        f"data/embeddings/embedding_{uuid.uuid4()}_{zulu}.txt", prompt
+    )
 
 
-def gpt3_completion(prompt, engine='text-davinci-003', temp=1.0, top_p=1.0, tokens=400, freq_pen=0.0, pres_pen=0.0,
-                    stop=None):
+def gpt3_completion(
+    prompt,
+    engine="text-davinci-003",
+    temp=1.0,
+    top_p=1.0,
+    tokens=400,
+    freq_pen=0.0,
+    pres_pen=0.0,
+    stop=None,
+):
     if stop is None:
-        stop = ['<<STOP>>']
+        stop = ["<<STOP>>"]
     max_retry = 3
     retry = 0
-    prompt = prompt.encode(encoding='ASCII', errors='ignore').decode()
+    prompt = prompt.encode(encoding="ASCII", errors="ignore").decode()
     while True:
         try:
             response = openai.Completion.create(
                 engine=engine,
                 prompt=prompt,
                 temperature=temp,
                 max_tokens=tokens,
                 top_p=top_p,
                 frequency_penalty=freq_pen,
                 presence_penalty=pres_pen,
-                stop=stop)
-            text = response['choices'][0]['text'].strip()
+                stop=stop,
+            )
+            text = response["choices"][0]["text"].strip()
             save_completion(text)
             return text
         except Exception as oops:
             retry += 1
             if retry >= max_retry:
                 return "GPT3 error: %s" % oops
-            print('Error communicating with OpenAI:', oops)
+            print("Error communicating with OpenAI:", oops)
             sleep(1)
 
 
 def gpt_embedding(text, model="text-embedding-ada-002"):
     text = text.replace("\n", " ")
-    emb = openai.Embedding.create(input=[text], model=model)['data'][0]['embedding']
+    emb = openai.Embedding.create(input=[text], model=model)["data"][0]["embedding"]
     save_embedding(emb)
     return emb
 
 
-def gpt_chat_completion(messages, model, max_retry=5,
-                        backoff_factor=2, initial_wait=.1):
+def gpt_chat_completion(
+    messages, model, max_retry=5, backoff_factor=2, initial_wait=0.1
+):
     """
     Sends chat inputs to OpenAI API and receives the chatbot response.
 
     Args:
         messages (List[Dict]): A list of messages with role and content.
         model (str, optional): The GPT model to be used.
         max_retry (int, optional): The maximum number of retries.
@@ -75,19 +89,16 @@
 
     # Initialize retry attempts
     retry = 0
 
     # Run the loop for retry attempts
     while retry <= max_retry:
         try:
-            response = openai.ChatCompletion.create(
-                model="gpt-4",
-                messages=messages
-            )
-            text = response['choices'][0]['message']['content'].strip()
+            response = openai.ChatCompletion.create(model="gpt-4", messages=messages)
+            text = response["choices"][0]["message"]["content"].strip()
             save_completion(text)
             return text
         except Exception as oops:
             # If the error is due to maximum context length, return the error message so that the user can handle it
             if "maximum context length" in str(oops):
                 return f"GPT error: {oops}"
 
@@ -97,25 +108,29 @@
             if retry > max_retry:
                 return f"GPT error: {oops}"
 
             # Calculate the waiting time for exponential backoff
             wait_time = initial_wait * (backoff_factor ** (retry - 1))
 
             # Print the error and wait before retrying
-            print(f"Error communicating with OpenAI (attempt {retry}/{max_retry}): {oops}")
+            print(
+                f"Error communicating with OpenAI (attempt {retry}/{max_retry}): {oops}"
+            )
             sleep(wait_time)
 
 
 def gpt4_completion(prompt, model="gpt-4"):
-    completion = gpt_chat_completion([{'role': 'user', 'content': prompt}], model=model)
+    completion = gpt_chat_completion([{"role": "user", "content": prompt}], model=model)
     save_completion(completion)
     return completion
 
 
-def generate_filename(prompt, prefix="", suffix="", extension="md", max_chars=60, time=False):
+def generate_filename(
+    prompt, prefix="", suffix="", extension="md", max_chars=60, time=False
+):
     """
     Generates a filename based on the given prompt.
     :param prompt: the prompt to generate the filename from
     :param prefix: the prefix to add to the filename
     :param suffix: the suffix to add to the filename
     :param extension: the extension to add to the filename
     :param max_chars: the maximum number of characters in the filename (default: 60)
@@ -125,18 +140,20 @@
     prompt = prompt[:300]
 
     file_name = gpt3_completion(
         f"Carefully read the following text and generate a highly relevant and unique filename for it. The filename "
         f"should be in all lowercase letters and consist of at most {max_chars} characters, separated by underscores. "
         f"Exclude any file extensions from the filename. Pay close attention to the content "
         f"and context of the text to avoid hallucinations or mistakes. The text is: '{prompt}'\n\nfile name:",
-        temp=0, tokens=max_chars * 10)
+        temp=0,
+        tokens=max_chars * 10,
+    )
 
     # Remove all non-underscore and non-alphanumeric characters, and truncate to max_chars
-    file_name = re.sub(r'[^a-zA-Z0-9_]', '', file_name)
+    file_name = re.sub(r"[^a-zA-Z0-9_]", "", file_name)
     file_name = file_name[:max_chars]
 
     if prefix:
         file_name = f"{prefix}_{file_name}"
 
     if suffix:
         file_name = f"{file_name}_{suffix}"
@@ -149,8 +166,10 @@
 
     # print('Generated filename:', file_name)
 
     return file_name
 
 
 def generate_output_file(prompt, extension="md", max_chars=60, time=True):
-    return generate_filename(prompt, extension=extension, max_chars=max_chars, time=time)
+    return generate_filename(
+        prompt, extension=extension, max_chars=max_chars, time=time
+    )
```

### Comparing `fgn-2023.7.21/src/fgn/utils/output_manager.py` & `fgn-2023.7.25/src/fgn/utils/output_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # fgn/utils/output_manager.py
+from dataclasses import dataclass
 from typing import Optional
-from rich import print
 
 import pyperclip
+from rich import print
 from rich.markdown import Markdown
 
 from fgn.utils.file_operations import extract_markdown
 from fgn.utils.openai_operations import generate_output_file
 
-from dataclasses import dataclass
-
 
 @dataclass
 class OutputManager:
     output: Optional[str] = None
     no_copy: bool = False
     auto_output: bool = False
     verbose: bool = False
     extension: str = "md"
 
-    def handle_output(self, response: str, extract_md: bool = False, append: Optional[str] = False) -> None:
+    def handle_output(
+        self, response: str, extract_md: bool = False, append: Optional[str] = False
+    ) -> None:
         if extract_md:
             response = extract_markdown(response)
             if self.verbose:
                 print("Extracting markdown...")
                 print(response)
         output = self.output
         no_copy = self.no_copy
@@ -37,19 +38,24 @@
             pyperclip.copy(response)
             if self.verbose:
                 print("The output has been saved to clipboard.")
 
         md = Markdown(str(response))
         print(md)
 
-    def save_to_file(self, response: str, filename: Optional[str] = None, extension: str = "md",
-                     append: Optional[bool] = False) -> None:
+    def save_to_file(
+        self,
+        response: str,
+        filename: Optional[str] = None,
+        extension: str = "md",
+        append: Optional[bool] = False,
+    ) -> None:
         if not filename:
             filename = generate_output_file(response, extension=extension)
         if append:
-            with open(filename, 'a') as output_file:
-                output_file.write('\n\n' + response)
+            with open(filename, "a") as output_file:
+                output_file.write("\n\n" + response)
         else:
-            with open(filename, 'w') as output_file:
+            with open(filename, "w") as output_file:
                 output_file.write(response)
         if self.verbose:
             print(f"The output has been saved to {filename}.")
```

### Comparing `fgn-2023.7.21/src/fgn.egg-info/PKG-INFO` & `fgn-2023.7.25/src/fgn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgn
-Version: 2023.7.21
+Version: 2023.7.25
 Summary: FGN: An AI-powered command-line tool for automated file generation.
 Home-page: https://github.com/seanchatmangpt/fgn
 Author: Sean Chatman
 Author-email: info@chatmangpt.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -73,37 +73,33 @@
     --help                         Show this message and exit.
 
 Commands
 --------
 
 .. code-block:: bash
 
-    blog       Create a blog article.
-    chain      Create chain of FGN .
-    chapter    Create a chapter.
-    code       Create a code snippet.
-    core       CLI internal usage only.
-    dsl        Create a new FGN DSL (requires GPT 4).
-    example    Create an example.
-    feedback   Create a feedback.
-    flow       Create a flow.
-    framework  Create a framework.
-    fun        Create fun.
-    guide      Execute the guide command.
-    help       Get help with the FGN CLI.
-    howto      Create a how-to article.
-    intent     Create an intent.
-    lts        Let's think step by step how to do this.
-    nano       Create a Nano Fiction story.
-    plan       Create a detailed plan.
-    prompt     Create a new prompt.
-    shell      Create a shell script.
-    summary    Execute the summary command.
-    template   Create a command named by the prompt.
-    yaml       Create yaml.It needs much
+  blog      Create a blog article.
+  chain     Create chain of fgn commands.
+  code      Create a code snippet.
+  core      CLI internal usage only.
+  dsl       Create a new FGN DSL (requires GPT 4).
+  feedback  Create feedback.
+  fun       Create OpenAI function schema.
+  guide     Create a procedural guide.
+  help      Get help with the FGN CLI.
+  howto     Create a how-to article.
+  lts       Let's think step by step how to do this.
+  nano      Create a Nano Fiction story.
+  plan      Create a detailed plan.
+  prompt    Create a new prompt
+  shell     Create a shell script.
+  summary   Create a summary.
+  template  Create a command named by the prompt.
+  yaml      Create yaml.
+
 
 Examples
 --------
 Here are some example uses of FGN:
 
 To generate a business plan and save it to "business_plan.txt", run:
```

### Comparing `fgn-2023.7.21/src/fgn.egg-info/SOURCES.txt` & `fgn-2023.7.25/src/fgn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .coveragerc
 .gitignore
 .isort.cfg
-.pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
```

### Comparing `fgn-2023.7.21/tests/test_cli.py` & `fgn-2023.7.25/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,13 +17,13 @@
     fs.create_file(fake_file_path, contents=fake_file_content)
 
     # Use the runner fixture to invoke the CLI command
     result = runner.invoke(main, ["-o", fake_file_path, message])
 
     # Print the output and contents of the fake file for debugging
     print("result.output:", result.output)
-    with open(fake_file_path, "r") as file:
+    with open(fake_file_path) as file:
         print("fake_file_content:", file.read())
 
     # Verify the result
     assert result.exit_code == 0
     assert result.output.strip() == message
```

### Comparing `fgn-2023.7.21/tests/test_skeleton.py` & `fgn-2023.7.25/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `fgn-2023.7.21/tests/utils/test_file_operations.py` & `fgn-2023.7.25/tests/utils/test_file_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pytest
 from pyfakefs.fake_filesystem_unittest import Patcher
+
 from fgn.core.command_context import CommandContext
 from fgn.utils.file_operations import (
+    extract_markdown,
+    get_norm_path,
+    get_project_root,
     load_default_or_context,
     open_file,
-    save_relative_to_base,
     open_file_or_raise,
-    extract_markdown,
-    get_project_root,
-    get_norm_path,
+    save_relative_to_base,
 )
 
 
 @pytest.fixture
 def fs():
     patcher = Patcher()
     patcher.setUp()
@@ -31,15 +32,15 @@
     assert open_file("/test.txt") == "test content"
 
 
 def test_save_relative_to_base(fs):
     base_path = "/path/to/base"
     fs.create_dir(base_path)
     save_relative_to_base("test.txt", "test content", base_path)
-    with open("/path/to/base/test.txt", "r") as f:
+    with open("/path/to/base/test.txt") as f:
         assert f.read() == "test content"
 
 
 def test_open_file_or_raise(fs):
     with pytest.raises(FileNotFoundError):
         open_file_or_raise("/nonexistent.txt")
     fs.create_file("/test.txt", contents="test content")
```

### Comparing `fgn-2023.7.21/tests/utils/test_openai_operations.py` & `fgn-2023.7.25/tests/utils/test_openai_operations.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pytest
 import os
-import tempfile
 import shutil
-
+import tempfile
 from unittest.mock import MagicMock, patch
 
+import pytest
+
 from fgn.utils.openai_operations import (
-    save_completion,
-    gpt3_completion,
-    gpt_chat_completion,
-    gpt4_completion,
     generate_filename,
     generate_output_file,
+    gpt3_completion,
+    gpt4_completion,
+    gpt_chat_completion,
+    save_completion,
 )
 
 
 @pytest.fixture(autouse=True)
 def mock_save_to_project_folder(monkeypatch):
     # Mock save_to_project_folder
     mock_save = MagicMock()
```

### Comparing `fgn-2023.7.21/tests/utils/test_output_manager.py` & `fgn-2023.7.25/tests/utils/test_output_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import pytest
 from unittest.mock import MagicMock
+
+import pytest
+
 from fgn.utils.output_manager import OutputManager
 
 
 # Set up your mocks at the top of the file
 @pytest.fixture(autouse=True)
 def mock_open(mocker):
     mocker.patch("builtins.open", mocker.mock_open())
@@ -66,20 +68,20 @@
 
 
 def test_save_to_file_with_filename(mock_open, output_manager):
     response = "Test response"
     filename = "test_output.md"
     output_manager.save_to_file(response, filename)
 
-    mock_open.assert_called_once_with(filename, 'w')
+    mock_open.assert_called_once_with(filename, "w")
     file_handle = mock_open.return_value.__enter__.return_value
     file_handle.write.assert_called_with(response)
 
 
 def test_save_to_file_append(mock_open, output_manager):
     response = "Test response"
     filename = "test_output.md"
     output_manager.save_to_file(response, filename, append=True)
 
-    mock_open.assert_called_once_with(filename, 'a')
+    mock_open.assert_called_once_with(filename, "a")
     file_handle = mock_open.return_value.__enter__.return_value
-    file_handle.write.assert_called_with('\n\n' + response)
+    file_handle.write.assert_called_with("\n\n" + response)
```

### Comparing `fgn-2023.7.21/tox.ini` & `fgn-2023.7.25/tox.ini`

 * *Files identical despite different names*

