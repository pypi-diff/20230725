# Comparing `tmp/dvc-3.7.0.tar.gz` & `tmp/dvc-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-3.7.0.tar", last modified: Fri Jul 21 16:06:25 2023, max compression
+gzip compressed data, was "dvc-3.8.0.tar", last modified: Tue Jul 25 17:05:32 2023, max compression
```

## Comparing `dvc-3.7.0.tar` & `dvc-3.8.0.tar`

### file list

```diff
@@ -1,661 +1,661 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.517655 dvc-3.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.445654 dvc-3.7.0/.dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 16:06:09.000000 dvc-3.7.0/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/.dvc/config
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 16:06:09.000000 dvc-3.7.0/.dvcignore
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-21 16:06:09.000000 dvc-3.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-21 16:06:09.000000 dvc-3.7.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 16:06:09.000000 dvc-3.7.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-21 16:06:09.000000 dvc-3.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.445654 dvc-3.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.445654 dvc-3.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/ISSUE_TEMPLATE/epic_story.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.449654 dvc-3.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/workflows/plugin_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-21 16:06:09.000000 dvc-3.7.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-21 16:06:09.000000 dvc-3.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 16:06:09.000000 dvc-3.7.0/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-21 16:06:09.000000 dvc-3.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-21 16:06:09.000000 dvc-3.7.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-21 16:06:09.000000 dvc-3.7.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-21 16:06:09.000000 dvc-3.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-21 16:06:09.000000 dvc-3.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-07-21 16:06:09.000000 dvc-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-07-21 16:06:25.517655 dvc-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-07-21 16:06:09.000000 dvc-3.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.453654 dvc-3.7.0/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.453654 dvc-3.7.0/dvc/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/hook-asyncssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/hook-celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/hook-dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/hook-dvc.utils.flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/hook-dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/hook-fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/__pyinstaller/hook-pydrive2.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 16:06:18.000000 dvc-3.7.0/dvc/_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 16:06:25.000000 dvc-3.7.0/dvc/_dvc_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.453654 dvc-3.7.0/dvc/api/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/api/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/api/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/api/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/api/show.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/cachemgr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.453654 dvc-3.7.0/dvc/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.457654 dvc-3.7.0/dvc/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.461654 dvc-3.7.0/dvc/commands/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/exec_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/git_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/imp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.461654 dvc-3.7.0/dvc/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/ls/ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/ls_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/move.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.461654 dvc-3.7.0/dvc/commands/queue/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/queue/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/queue/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/queue/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/queue/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/queue/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/repro.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/unprotect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/dagascii.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/data_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.461654 dvc-3.7.0/dvc/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/dependency/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/dependency/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.461654 dvc-3.7.0/dvc/fs/
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/fs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/fs/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/fs/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/fs/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.461654 dvc-3.7.0/dvc/machine/
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.465654 dvc-3.7.0/dvc/machine/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/machine/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/machine/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/machine/backend/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46718 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.465654 dvc-3.7.0/dvc/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/parsing/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/parsing/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.465654 dvc-3.7.0/dvc/render/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/render/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.465654 dvc-3.7.0/dvc/render/converter/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/render/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/render/converter/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/render/converter/vega.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/render/match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.469654 dvc-3.7.0/dvc/repo/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/brancher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.473654 dvc-3.7.0/dvc/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/brancher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.473654 dvc-3.7.0/dvc/repo/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/executor/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/executor/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.473654 dvc-3.7.0/dvc/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/queue/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/refs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/stash.py
--rw-r--r--   0 runner    (1001) docker     (123)    24907 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/imp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/ls_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.473654 dvc-3.7.0/dvc/repo/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/metrics/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/metrics/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/move.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/open_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.473654 dvc-3.7.0/dvc/repo/params/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/params/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/params/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.473654 dvc-3.7.0/dvc/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (123)    17028 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/plots/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/scm_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/trie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/repo/worktree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.477654 dvc-3.7.0/dvc/stage/
--rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/stage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.477654 dvc-3.7.0/dvc/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/api_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.477654 dvc-3.7.0/dvc/testing/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.477654 dvc-3.7.0/dvc/testing/benchmarks/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.477654 dvc-3.7.0/dvc/testing/benchmarks/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.481654 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_exp_show.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_push.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.481654 dvc-3.7.0/dvc/testing/benchmarks/cli/stories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.481654 dvc-3.7.0/dvc/testing/benchmarks/cli/stories/use_cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/benchmarks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/remote_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/tmp_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/testing/workspace_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.481654 dvc-3.7.0/dvc/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/ui/_rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/ui/pager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/ui/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.481654 dvc-3.7.0/dvc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.485654 dvc-3.7.0/dvc/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/serialize/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/serialize/_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/serialize/_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/serialize/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/utils/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 16:06:09.000000 dvc-3.7.0/dvc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.453654 dvc-3.7.0/dvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-07-21 16:06:25.000000 dvc-3.7.0/dvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16386 2023-07-21 16:06:25.000000 dvc-3.7.0/dvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:06:25.000000 dvc-3.7.0/dvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-21 16:06:25.000000 dvc-3.7.0/dvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 16:06:25.000000 dvc-3.7.0/dvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-21 16:06:25.000000 dvc-3.7.0/dvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-21 16:06:09.000000 dvc-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:06:25.517655 dvc-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.485654 dvc-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/dir_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.489654 dvc-3.7.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/api/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/api/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/api/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/artifacts/test_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/data/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/data/db/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/executor/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_set_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_stash_exp.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/machine/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/machine/test_machine_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/machine/test_machine_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/metrics/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/metrics/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.493654 dvc-3.7.0/tests/func/params/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/params/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/params/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/func/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/parsing/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/parsing/test_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/parsing/test_interpolated_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/parsing/test_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/func/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/plots/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/plots/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/func/repro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/repro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/repro/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/repro/test_repro_allow_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/repro/test_repro_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)    30224 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)    22833 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16589 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_data_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    16348 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14156 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_merge_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_root.py
--rw-r--r--   0 runner    (1001) docker     (123)    20611 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_run_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_scm_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_stage_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_unprotect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_used_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/test_virtual_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/func/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/utils/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/func/utils/test_strict_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/integration/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/integration/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/integration/plots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/integration/plots/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/integration/plots/test_repo_plots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/integration/test_studio_live_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/remotes/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/remotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.497654 dvc-3.7.0/tests/remotes/git-init/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/remotes/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/remotes/git_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/remotes/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/remotes/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/remotes_env.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.501654 dvc-3.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.501654 dvc-3.7.0/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/cli/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.505654 dvc-3.7.0/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.505654 dvc-3.7.0/tests/unit/command/ls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/ls/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/ls/test_ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_compat_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_git_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_imp_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/command/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.505654 dvc-3.7.0/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.505654 dvc-3.7.0/tests/unit/data/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/data/db/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.505654 dvc-3.7.0/tests/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/dependency/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/dependency/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.509654 dvc-3.7.0/tests/unit/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_dvc_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/fs/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.509654 dvc-3.7.0/tests/unit/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.509654 dvc-3.7.0/tests/unit/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/output/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/output/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/output/test_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/output/test_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.509654 dvc-3.7.0/tests/unit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/remote/test_oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/remote/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/remote/test_webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/remote/test_webhdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.509654 dvc-3.7.0/tests/unit/render/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/render/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/render/test_image_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/render/test_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/render/test_vega_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.509654 dvc-3.7.0/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.509654 dvc-3.7.0/tests/unit/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/unit/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/queue/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/queue/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/test_executor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/unit/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/test_open_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/test_reproduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/repo/test_scm_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/unit/scm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/scm/test_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/unit/stage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/test_loader_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/test_serialize_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/test_serialize_pipeline_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/stage/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_hashinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_rwlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_tabular_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/unit/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/ui/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/ui/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/ui/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/unit/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/serialize/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/serialize/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/serialize/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/test_cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:06:25.513654 dvc-3.7.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-21 16:06:09.000000 dvc-3.7.0/tests/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.593780 dvc-3.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.529777 dvc-3.8.0/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 17:05:16.000000 dvc-3.8.0/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/.dvc/config
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 17:05:16.000000 dvc-3.8.0/.dvcignore
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-25 17:05:16.000000 dvc-3.8.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-25 17:05:16.000000 dvc-3.8.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 17:05:16.000000 dvc-3.8.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 17:05:16.000000 dvc-3.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.529777 dvc-3.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.529777 dvc-3.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/ISSUE_TEMPLATE/epic_story.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.529777 dvc-3.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/workflows/plugin_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-25 17:05:16.000000 dvc-3.8.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-25 17:05:16.000000 dvc-3.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 17:05:16.000000 dvc-3.8.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-25 17:05:16.000000 dvc-3.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-25 17:05:16.000000 dvc-3.8.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-25 17:05:16.000000 dvc-3.8.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-25 17:05:16.000000 dvc-3.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 17:05:16.000000 dvc-3.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-07-25 17:05:16.000000 dvc-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-07-25 17:05:32.593780 dvc-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-07-25 17:05:16.000000 dvc-3.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.533777 dvc-3.8.0/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.537778 dvc-3.8.0/dvc/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/hook-asyncssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/hook-celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/hook-dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/hook-dvc.utils.flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/hook-dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/hook-fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/__pyinstaller/hook-pydrive2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 17:05:25.000000 dvc-3.8.0/dvc/_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 17:05:32.000000 dvc-3.8.0/dvc/_dvc_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.537778 dvc-3.8.0/dvc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/api/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/api/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/api/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/api/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/cachemgr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.537778 dvc-3.8.0/dvc/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.541778 dvc-3.8.0/dvc/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.541778 dvc-3.8.0/dvc/commands/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/exec_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.541778 dvc-3.8.0/dvc/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/ls/ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.541778 dvc-3.8.0/dvc/commands/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/queue/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/queue/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/queue/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/queue/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/queue/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/repro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/dagascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/data_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.545778 dvc-3.8.0/dvc/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/dependency/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/dependency/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.545778 dvc-3.8.0/dvc/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/fs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/fs/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/fs/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/fs/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.545778 dvc-3.8.0/dvc/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.545778 dvc-3.8.0/dvc/machine/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/machine/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/machine/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/machine/backend/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46843 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.545778 dvc-3.8.0/dvc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/parsing/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/parsing/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.545778 dvc-3.8.0/dvc/render/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/render/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.545778 dvc-3.8.0/dvc/render/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/render/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/render/converter/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/render/converter/vega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/render/match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.549778 dvc-3.8.0/dvc/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.553778 dvc-3.8.0/dvc/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.553778 dvc-3.8.0/dvc/repo/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/executor/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/executor/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.553778 dvc-3.8.0/dvc/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/queue/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/refs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24907 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/ls_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.553778 dvc-3.8.0/dvc/repo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/metrics/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/metrics/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/open_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.553778 dvc-3.8.0/dvc/repo/params/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/params/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/params/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.553778 dvc-3.8.0/dvc/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)    17028 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/plots/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/repo/worktree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.557778 dvc-3.8.0/dvc/stage/
+-rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/stage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.557778 dvc-3.8.0/dvc/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/api_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.557778 dvc-3.8.0/dvc/testing/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.557778 dvc-3.8.0/dvc/testing/benchmarks/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.557778 dvc-3.8.0/dvc/testing/benchmarks/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.561778 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_exp_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.561778 dvc-3.8.0/dvc/testing/benchmarks/cli/stories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.561778 dvc-3.8.0/dvc/testing/benchmarks/cli/stories/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/benchmarks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/remote_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/tmp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/testing/workspace_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.561778 dvc-3.8.0/dvc/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/ui/_rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/ui/pager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/ui/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.565779 dvc-3.8.0/dvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.565779 dvc-3.8.0/dvc/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/serialize/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/serialize/_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/serialize/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/serialize/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/utils/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 17:05:16.000000 dvc-3.8.0/dvc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.533777 dvc-3.8.0/dvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-07-25 17:05:32.000000 dvc-3.8.0/dvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16386 2023-07-25 17:05:32.000000 dvc-3.8.0/dvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:05:32.000000 dvc-3.8.0/dvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 17:05:32.000000 dvc-3.8.0/dvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-25 17:05:32.000000 dvc-3.8.0/dvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 17:05:32.000000 dvc-3.8.0/dvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-25 17:05:16.000000 dvc-3.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:05:32.593780 dvc-3.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.565779 dvc-3.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/dir_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.569779 dvc-3.8.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.569779 dvc-3.8.0/tests/func/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/api/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/api/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/api/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.569779 dvc-3.8.0/tests/func/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/artifacts/test_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.569779 dvc-3.8.0/tests/func/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.569779 dvc-3.8.0/tests/func/data/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/data/db/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.573779 dvc-3.8.0/tests/func/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.573779 dvc-3.8.0/tests/func/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/executor/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_set_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_stash_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.573779 dvc-3.8.0/tests/func/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/machine/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/machine/test_machine_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/machine/test_machine_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.573779 dvc-3.8.0/tests/func/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/metrics/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/metrics/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.573779 dvc-3.8.0/tests/func/params/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/params/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/params/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.573779 dvc-3.8.0/tests/func/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/parsing/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/parsing/test_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/parsing/test_interpolated_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/parsing/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.577779 dvc-3.8.0/tests/func/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/plots/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/plots/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.577779 dvc-3.8.0/tests/func/repro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/repro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/repro/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/repro/test_repro_allow_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/repro/test_repro_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30224 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22833 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16623 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_data_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16348 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_merge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20611 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_run_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_stage_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_used_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/test_virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.577779 dvc-3.8.0/tests/func/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/utils/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/func/utils/test_strict_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.577779 dvc-3.8.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.577779 dvc-3.8.0/tests/integration/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/integration/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/integration/plots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/integration/plots/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/integration/plots/test_repo_plots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/integration/test_studio_live_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.577779 dvc-3.8.0/tests/remotes/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/remotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.577779 dvc-3.8.0/tests/remotes/git-init/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/remotes/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/remotes/git_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/remotes/user.key
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/remotes/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/remotes_env.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.581779 dvc-3.8.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.581779 dvc-3.8.0/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/cli/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.585780 dvc-3.8.0/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.585780 dvc-3.8.0/tests/unit/command/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/ls/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/ls/test_ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_compat_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/command/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.585780 dvc-3.8.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.585780 dvc-3.8.0/tests/unit/data/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/data/db/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.585780 dvc-3.8.0/tests/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/dependency/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/dependency/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.585780 dvc-3.8.0/tests/unit/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_dvc_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/fs/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.585780 dvc-3.8.0/tests/unit/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/output/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/output/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/output/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/output/test_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/remote/test_oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/remote/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/remote/test_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/remote/test_webhdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/render/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/render/test_image_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/render/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/render/test_vega_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/queue/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/queue/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/test_executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/test_open_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/test_reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/repo/test_scm_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.589780 dvc-3.8.0/tests/unit/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/scm/test_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.593780 dvc-3.8.0/tests/unit/stage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/test_loader_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/test_serialize_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/test_serialize_pipeline_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/stage/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_hashinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_tabular_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.593780 dvc-3.8.0/tests/unit/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/ui/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/ui/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/ui/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.593780 dvc-3.8.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.593780 dvc-3.8.0/tests/unit/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/serialize/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/serialize/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/serialize/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/test_cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:05:32.593780 dvc-3.8.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 17:05:16.000000 dvc-3.8.0/tests/utils/plots.py
```

### Comparing `dvc-3.7.0/.git-blame-ignore-revs` & `dvc-3.8.0/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvc-3.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.github/ISSUE_TEMPLATE/epic_story.md` & `dvc-3.8.0/.github/ISSUE_TEMPLATE/epic_story.md`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.github/workflows/build.yaml` & `dvc-3.8.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.github/workflows/codeql.yml` & `dvc-3.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.github/workflows/plugin_tests.yaml` & `dvc-3.8.0/.github/workflows/plugin_tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.github/workflows/tests.yaml` & `dvc-3.8.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.pre-commit-config.yaml` & `dvc-3.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/.pre-commit-hooks.yaml` & `dvc-3.8.0/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/CODE_OF_CONDUCT.md` & `dvc-3.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/LICENSE` & `dvc-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/PKG-INFO` & `dvc-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.7.0
+Version: 3.8.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.7.0/README.rst` & `dvc-3.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/__pyinstaller/hook-dvc.py` & `dvc-3.8.0/dvc/__pyinstaller/hook-dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/_debug.py` & `dvc-3.8.0/dvc/_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/analytics.py` & `dvc-3.8.0/dvc/analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/annotations.py` & `dvc-3.8.0/dvc/annotations.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/api/data.py` & `dvc-3.8.0/dvc/api/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/api/experiments.py` & `dvc-3.8.0/dvc/api/experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/api/scm.py` & `dvc-3.8.0/dvc/api/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/api/show.py` & `dvc-3.8.0/dvc/api/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/cachemgr.py` & `dvc-3.8.0/dvc/cachemgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     **kwargs,
 ):
     from dvc.fs import get_cloud_fs
 
     if not settings:
         return None
 
-    cls, config, fs_path = get_cloud_fs(repo, **settings)
+    cls, config, fs_path = get_cloud_fs(repo.config, **settings)
     fs = fs or cls(**config)
     if prefix:
         fs_path = fs.path.join(fs_path, *prefix)
     if hash_name:
         config["hash_name"] = hash_name
     return get_odb(fs, fs_path, state=repo.state, **config)
```

### Comparing `dvc-3.7.0/dvc/cli/__init__.py` & `dvc-3.8.0/dvc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/cli/command.py` & `dvc-3.8.0/dvc/cli/command.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/cli/completion.py` & `dvc-3.8.0/dvc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/cli/parser.py` & `dvc-3.8.0/dvc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/cli/utils.py` & `dvc-3.8.0/dvc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/add.py` & `dvc-3.8.0/dvc/commands/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/cache.py` & `dvc-3.8.0/dvc/commands/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/check_ignore.py` & `dvc-3.8.0/dvc/commands/check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/checkout.py` & `dvc-3.8.0/dvc/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/commit.py` & `dvc-3.8.0/dvc/commands/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/completion.py` & `dvc-3.8.0/dvc/commands/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/config.py` & `dvc-3.8.0/dvc/commands/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/daemon.py` & `dvc-3.8.0/dvc/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/dag.py` & `dvc-3.8.0/dvc/commands/dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/data.py` & `dvc-3.8.0/dvc/commands/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/data_sync.py` & `dvc-3.8.0/dvc/commands/data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/destroy.py` & `dvc-3.8.0/dvc/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/diff.py` & `dvc-3.8.0/dvc/commands/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/__init__.py` & `dvc-3.8.0/dvc/commands/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/apply.py` & `dvc-3.8.0/dvc/commands/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/branch.py` & `dvc-3.8.0/dvc/commands/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/clean.py` & `dvc-3.8.0/dvc/commands/experiments/clean.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/diff.py` & `dvc-3.8.0/dvc/commands/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/exec_run.py` & `dvc-3.8.0/dvc/commands/experiments/exec_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/ls.py` & `dvc-3.8.0/dvc/commands/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/pull.py` & `dvc-3.8.0/dvc/commands/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/push.py` & `dvc-3.8.0/dvc/commands/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/queue_worker.py` & `dvc-3.8.0/dvc/commands/experiments/queue_worker.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/remove.py` & `dvc-3.8.0/dvc/commands/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/run.py` & `dvc-3.8.0/dvc/commands/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/save.py` & `dvc-3.8.0/dvc/commands/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/experiments/show.py` & `dvc-3.8.0/dvc/commands/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/freeze.py` & `dvc-3.8.0/dvc/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/gc.py` & `dvc-3.8.0/dvc/commands/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/get.py` & `dvc-3.8.0/dvc/commands/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/get_url.py` & `dvc-3.8.0/dvc/commands/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/git_hook.py` & `dvc-3.8.0/dvc/commands/git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/imp.py` & `dvc-3.8.0/dvc/commands/imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/imp_url.py` & `dvc-3.8.0/dvc/commands/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/init.py` & `dvc-3.8.0/dvc/commands/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/install.py` & `dvc-3.8.0/dvc/commands/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/ls/__init__.py` & `dvc-3.8.0/dvc/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/ls/ls_colors.py` & `dvc-3.8.0/dvc/commands/ls/ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/ls_url.py` & `dvc-3.8.0/dvc/commands/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/machine.py` & `dvc-3.8.0/dvc/commands/machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/metrics.py` & `dvc-3.8.0/dvc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/move.py` & `dvc-3.8.0/dvc/commands/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/params.py` & `dvc-3.8.0/dvc/commands/params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/plots.py` & `dvc-3.8.0/dvc/commands/plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/queue/__init__.py` & `dvc-3.8.0/dvc/commands/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/queue/kill.py` & `dvc-3.8.0/dvc/commands/queue/kill.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/queue/logs.py` & `dvc-3.8.0/dvc/commands/queue/logs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/queue/remove.py` & `dvc-3.8.0/dvc/commands/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/queue/start.py` & `dvc-3.8.0/dvc/commands/queue/start.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/queue/status.py` & `dvc-3.8.0/dvc/commands/queue/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/queue/stop.py` & `dvc-3.8.0/dvc/commands/queue/stop.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/remote.py` & `dvc-3.8.0/dvc/commands/remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/remove.py` & `dvc-3.8.0/dvc/commands/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/repro.py` & `dvc-3.8.0/dvc/commands/repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/root.py` & `dvc-3.8.0/dvc/commands/root.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/stage.py` & `dvc-3.8.0/dvc/commands/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/status.py` & `dvc-3.8.0/dvc/commands/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/unprotect.py` & `dvc-3.8.0/dvc/commands/unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/update.py` & `dvc-3.8.0/dvc/commands/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/commands/version.py` & `dvc-3.8.0/dvc/commands/version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/compare.py` & `dvc-3.8.0/dvc/compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/config.py` & `dvc-3.8.0/dvc/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/config_schema.py` & `dvc-3.8.0/dvc/config_schema.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/daemon.py` & `dvc-3.8.0/dvc/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/dagascii.py` & `dvc-3.8.0/dvc/dagascii.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/data_cloud.py` & `dvc-3.8.0/dvc/data_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     ) -> "Remote":
         if not name:
             name = self.repo.config["core"].get("remote")
 
         if name:
             from dvc.fs import get_cloud_fs
 
-            cls, config, fs_path = get_cloud_fs(self.repo, name=name)
+            cls, config, fs_path = get_cloud_fs(self.repo.config, name=name)
 
             if config.get("worktree"):
                 version_aware = config.get("version_aware")
                 if version_aware is False:
                     raise RemoteConfigError(
                         "worktree remotes require version_aware cloud"
                     )
```

### Comparing `dvc-3.7.0/dvc/dependency/__init__.py` & `dvc-3.8.0/dvc/dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/dependency/base.py` & `dvc-3.8.0/dvc/dependency/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             self.meta = self.get_meta()
             self.def_path = self.fs.path.version_path(
                 self.def_path, self.meta.version_id
             )
             self.fs_path = self.fs.path.version_path(self.fs_path, self.meta.version_id)
 
     def download(self, to, jobs=None):
-        fs_download(self.fs, self.fs_path, to, jobs=jobs)
+        fs_download(self.fs, self.fs_path, to.fs_path, jobs=jobs)
 
     def save(self):
         super().save()
         if self.fs.version_aware:
             self.fs_path = self.fs.path.version_path(self.fs_path, self.meta.version_id)
 
     def dumpd(self, **kwargs):
```

### Comparing `dvc-3.7.0/dvc/dependency/param.py` & `dvc-3.8.0/dvc/dependency/param.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/dependency/repo.py` & `dvc-3.8.0/dvc/dependency/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/dirs.py` & `dvc-3.8.0/dvc/dirs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/dvcfile.py` & `dvc-3.8.0/dvc/dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/env.py` & `dvc-3.8.0/dvc/env.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/exceptions.py` & `dvc-3.8.0/dvc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/fs/__init__.py` & `dvc-3.8.0/dvc/fs/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from urllib.parse import urlparse
 
 from dvc_http import HTTPFileSystem, HTTPSFileSystem  # noqa: F401
 
 from dvc.config import ConfigError as RepoConfigError
 from dvc.config_schema import SCHEMA, Invalid
 
@@ -14,15 +15,15 @@
     get_fs_cls,
     known_implementations,
     localfs,
     registry,
     system,
     utils,
 )
-from dvc_objects.fs.base import AnyFSPath, FileSystem  # noqa: F401
+from dvc_objects.fs.base import AnyFSPath, FileSystem  # noqa: F401, TCH001
 from dvc_objects.fs.errors import (  # noqa: F401
     AuthError,
     ConfigError,
     RemoteMissingDepsError,
 )
 from dvc_objects.fs.path import Path  # noqa: F401
 
@@ -44,26 +45,53 @@
     }
 )
 
 
 # pylint: enable=unused-import
 
 
-def download(fs, fs_path, to, jobs=None):
+def download(fs: "FileSystem", fs_path: str, to: str, jobs: Optional[int] = None):
     with Callback.as_tqdm_callback(
         desc=f"Downloading {fs.path.name(fs_path)}",
         unit="files",
     ) as cb:
-        fs.get(fs_path, to.fs_path, batch_size=jobs, callback=cb)
+        # NOTE: We use dvc-objects generic.copy over fs.get since it makes file
+        # download atomic and avoids fsspec glob/regex path expansion.
+        if fs.isdir(fs_path):
+            from_infos = [
+                path
+                for path in fs.find(fs_path)
+                if not path.endswith(fs.path.flavour.sep)
+            ]
+            if not from_infos:
+                return localfs.makedirs(to, exist_ok=True)
+            to_infos = [
+                localfs.path.join(to, *fs.path.relparts(info, fs_path))
+                for info in from_infos
+            ]
+        else:
+            from_infos = [fs_path]
+            to_infos = [to]
+
+        cb.set_size(len(from_infos))
+        jobs = jobs or fs.jobs
+        generic.copy(
+            fs,
+            from_infos,
+            localfs,
+            to_infos,
+            callback=cb,
+            batch_size=jobs,
+        )
 
 
 def parse_external_url(url, config=None):
     remote_config = dict(config) if config else {}
     remote_config["url"] = url
-    fs_cls, fs_config, fs_path = get_cloud_fs(None, **remote_config)
+    fs_cls, fs_config, fs_path = get_cloud_fs({}, **remote_config)
     fs = fs_cls(**fs_config)
     return fs, fs_path
 
 
 def get_fs_config(config, **kwargs):
     name = kwargs.get("name")
     if name:
@@ -101,26 +129,22 @@
     #           "ask_password": False,
     #       }
     parsed = urlparse(remote_conf["url"])
     if parsed.scheme != "remote":
         return remote_conf
 
     base = get_fs_config(config, name=parsed.netloc)
-    cls, _, _ = _get_cloud_fs(config, **base)
+    cls, _, _ = get_cloud_fs(config, **base)
     relpath = parsed.path.lstrip("/").replace("/", cls.sep)
     url = cls.sep.join((base["url"], relpath))
     return {**base, **remote_conf, "url": url}
 
 
-def get_cloud_fs(repo, **kwargs):
-    repo_config = repo.config if repo else {}
-    return _get_cloud_fs(repo_config, **kwargs)
-
-
-def _get_cloud_fs(repo_config, **kwargs):
+def get_cloud_fs(repo_config, **kwargs):
+    repo_config = repo_config or {}
     core_config = repo_config.get("core", {})
 
     remote_conf = get_fs_config(repo_config, **kwargs)
     try:
         remote_conf = SCHEMA["remote"][str](remote_conf)  # type: ignore[index]
     except Invalid as exc:
         raise RepoConfigError(str(exc)) from None
```

### Comparing `dvc-3.7.0/dvc/fs/callbacks.py` & `dvc-3.8.0/dvc/fs/callbacks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/fs/data.py` & `dvc-3.8.0/dvc/fs/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/fs/dvc.py` & `dvc-3.8.0/dvc/fs/dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/fs/git.py` & `dvc-3.8.0/dvc/fs/git.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/ignore.py` & `dvc-3.8.0/dvc/ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/info.py` & `dvc-3.8.0/dvc/info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/lock.py` & `dvc-3.8.0/dvc/lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/logger.py` & `dvc-3.8.0/dvc/logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/machine/__init__.py` & `dvc-3.8.0/dvc/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/machine/backend/base.py` & `dvc-3.8.0/dvc/machine/backend/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/machine/backend/terraform.py` & `dvc-3.8.0/dvc/machine/backend/terraform.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/output.py` & `dvc-3.8.0/dvc/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,19 @@
         fs_kwargs = {}
         if meta.version_id or files:
             fs_kwargs["version_aware"] = True
 
         if fs_config is not None:
             fs_kwargs.update(**fs_config)
 
-        fs_cls, fs_config, fs_path = get_cloud_fs(self.repo, url=path, **fs_kwargs)
+        fs_cls, fs_config, fs_path = get_cloud_fs(
+            self.repo.config if self.repo else {},
+            url=path,
+            **fs_kwargs,
+        )
         self.fs = fs_cls(**fs_config)
 
         if (
             self.fs.protocol == "local"
             and stage
             and isinstance(stage.repo.fs, LocalFileSystem)
             and path_isin(path, stage.repo.root_dir)
@@ -1013,15 +1017,17 @@
 
     def transfer(
         self, source, odb=None, jobs=None, update=False, no_progress_bar=False
     ):
         if odb is None:
             odb = self.cache
 
-        cls, config, from_info = get_cloud_fs(self.repo, url=source)
+        cls, config, from_info = get_cloud_fs(
+            self.repo.config if self.repo else {}, url=source
+        )
         from_fs = cls(**config)
 
         # When running import-url --to-remote / add --to-remote/-o ... we
         # assume that it is unlikely that the odb will contain majority of the
         # hashes, so we transfer everything as is (even if that file might
         # already be in the cache) and don't waste an upload to scan the layout
         # of the source location. But when doing update --to-remote, there is
```

### Comparing `dvc-3.7.0/dvc/parsing/__init__.py` & `dvc-3.8.0/dvc/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/parsing/context.py` & `dvc-3.8.0/dvc/parsing/context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/parsing/interpolate.py` & `dvc-3.8.0/dvc/parsing/interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/pathspec_math.py` & `dvc-3.8.0/dvc/pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/progress.py` & `dvc-3.8.0/dvc/progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/prompt.py` & `dvc-3.8.0/dvc/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/render/convert.py` & `dvc-3.8.0/dvc/render/convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/render/converter/__init__.py` & `dvc-3.8.0/dvc/render/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/render/converter/image.py` & `dvc-3.8.0/dvc/render/converter/image.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/render/converter/vega.py` & `dvc-3.8.0/dvc/render/converter/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/render/match.py` & `dvc-3.8.0/dvc/render/match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/__init__.py` & `dvc-3.8.0/dvc/repo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
         uninitialized: bool = False,
         config: Optional["DictStrAny"] = None,
         url: Optional[str] = None,
         repo_factory: Optional[Callable] = None,
         scm: Optional[Union["Git", "NoSCM"]] = None,
     ):
         from dvc.cachemgr import CacheManager
-        from dvc.config import Config
         from dvc.data_cloud import DataCloud
         from dvc.fs import GitFileSystem, LocalFileSystem, localfs
         from dvc.lock import LockNoop, make_lock
         from dvc.repo.artifacts import Artifacts
         from dvc.repo.metrics import Metrics
         from dvc.repo.params import Params
         from dvc.repo.plots import Plots
@@ -159,14 +158,15 @@
         from dvc.stage.cache import StageCache
         from dvc_data.hashfile.state import State, StateNoop
 
         self.url = url
         self._fs_conf = {"repo_factory": repo_factory}
         self._fs = fs or localfs
         self._scm = scm
+        self._config = config
         self._data_index = None
 
         if rev and not fs:
             self._scm = scm = SCM(root_dir or os.curdir)
             root_dir = "/"
             self._fs = GitFileSystem(scm=self._scm, rev=rev)
 
@@ -178,15 +178,14 @@
         ) = self._get_repo_dirs(
             root_dir=root_dir,
             fs=self.fs,
             uninitialized=uninitialized,
             scm=scm,
         )
 
-        self.config: Config = Config(self.dvc_dir, fs=self.fs, config=config)
         self._uninitialized = uninitialized
 
         # used by DVCFileSystem to determine if it should traverse subrepos
         self.subrepos = subrepos
 
         self.cloud: "DataCloud" = DataCloud(self)
         self.stage: "StageLoad" = StageLoad(self)
@@ -231,14 +230,20 @@
         ] = None
         self._lock_depth: int = 0
 
     def __str__(self):
         return self.url or self.root_dir
 
     @cached_property
+    def config(self):
+        from dvc.config import Config
+
+        return Config(self.dvc_dir, fs=self.fs, config=self._config)
+
+    @cached_property
     def local_dvc_dir(self):
         from dvc.fs import GitFileSystem, LocalFileSystem
 
         if not self.dvc_dir:
             return None
 
         if isinstance(self.fs, LocalFileSystem):
@@ -625,13 +630,14 @@
         self.state.close()
         if "dvcfs" in self.__dict__:
             self.dvcfs.close()
         self.__dict__.pop("index", None)
         self.__dict__.pop("dvcignore", None)
         self.__dict__.pop("dvcfs", None)
         self.__dict__.pop("datafs", None)
+        self.__dict__.pop("config", None)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
```

### Comparing `dvc-3.7.0/dvc/repo/add.py` & `dvc-3.8.0/dvc/repo/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/artifacts.py` & `dvc-3.8.0/dvc/repo/artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/brancher.py` & `dvc-3.8.0/dvc/repo/brancher.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
     cwd_parts = ()
     if self.fs.path.isin(self.fs.path.getcwd(), self.scm.root_dir):
         cwd_parts = self.fs.path.relparts(self.fs.path.getcwd(), self.scm.root_dir)
 
     saved_fs = self.fs
     saved_root = self.root_dir
+    saved_dvc_dir = self.dvc_dir
 
     scm = self.scm
 
     logger.trace("switching fs to workspace")  # type: ignore[attr-defined]
     self.fs = LocalFileSystem(url=self.root_dir)
     yield "workspace"
 
@@ -97,14 +98,16 @@
             except NotDvcRepoError:
                 # ignore revs that don't contain repo root
                 # (i.e. revs from before a subdir=True repo was init'ed)
                 pass
     finally:
         self.fs = saved_fs
         self.root_dir = saved_root
+        self.dvc_dir = saved_dvc_dir
+        self._reset()  # pylint: disable=protected-access
 
 
 def _switch_fs(
     repo: "Repo",
     rev: str,
     repo_root_parts: Tuple[str, ...],
     cwd_parts: Tuple[str, ...],
@@ -121,14 +124,16 @@
     fs = GitFileSystem(scm=repo.scm, rev=rev)
     root_dir = repo.fs.path.join("/", *repo_root_parts)
     if not fs.exists(root_dir):
         raise NotDvcRepoError(f"Commit '{rev[:7]}' does not contain a DVC repo")
 
     repo.fs = fs
     repo.root_dir = root_dir
+    repo.dvc_dir = fs.path.join(root_dir, repo.DVC_DIR)
+    repo._reset()  # pylint: disable=protected-access
 
     if cwd_parts:
         cwd = repo.fs.path.join("/", *cwd_parts)
         repo.fs.path.chdir(cwd)
 
 
 @contextmanager
@@ -145,13 +150,16 @@
 
     cwd_parts = ()
     if repo.fs.path.isin(repo.fs.path.getcwd(), repo.scm.root_dir):
         cwd_parts = repo.fs.path.relparts(repo.fs.path.getcwd(), repo.scm.root_dir)
 
     saved_fs = repo.fs
     saved_root = repo.root_dir
+    saved_dvc_dir = repo.dvc_dir
     try:
         _switch_fs(repo, rev, repo_root_parts, cwd_parts)
         yield rev
     finally:
         repo.fs = saved_fs
         repo.root_dir = saved_root
+        repo.dvc_dir = saved_dvc_dir
+        repo._reset()  # pylint: disable=protected-access
```

### Comparing `dvc-3.7.0/dvc/repo/checkout.py` & `dvc-3.8.0/dvc/repo/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/collect.py` & `dvc-3.8.0/dvc/repo/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/commit.py` & `dvc-3.8.0/dvc/repo/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/data.py` & `dvc-3.8.0/dvc/repo/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/destroy.py` & `dvc-3.8.0/dvc/repo/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/diff.py` & `dvc-3.8.0/dvc/repo/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/__init__.py` & `dvc-3.8.0/dvc/repo/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/apply.py` & `dvc-3.8.0/dvc/repo/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/branch.py` & `dvc-3.8.0/dvc/repo/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/brancher.py` & `dvc-3.8.0/dvc/repo/experiments/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/cache.py` & `dvc-3.8.0/dvc/repo/experiments/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/collect.py` & `dvc-3.8.0/dvc/repo/experiments/collect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import itertools
 import logging
 import os
+from dataclasses import fields
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Collection,
     Dict,
     Iterable,
     Iterator,
@@ -148,15 +149,31 @@
         baseline_revs: Resolved baseline Git SHAs.
 
     Returns:
         Dict mapping baseline revision to list of queued experiments.
     """
     if not baseline_revs:
         return {}
-    return repo.experiments.celery_queue.collect_queued_data(baseline_revs, **kwargs)
+    queued_data = {}
+    for rev, ranges in repo.experiments.celery_queue.collect_queued_data(
+        baseline_revs, **kwargs
+    ).items():
+        for exp_range in ranges:
+            for exp_state in exp_range.revs:
+                if exp_state.data:
+                    attrs = [f.name for f in fields(SerializableExp)]
+                    exp_state.data = SerializableExp(
+                        **{
+                            attr: getattr(exp_state.data, attr)
+                            for attr in attrs
+                            if attr != "metrics"
+                        }
+                    )
+        queued_data[rev] = ranges
+    return queued_data
 
 
 def collect_active(
     repo: "Repo",
     baseline_revs: Collection[str],
     **kwargs,
 ) -> Dict[str, List["ExpRange"]]:
```

### Comparing `dvc-3.7.0/dvc/repo/experiments/diff.py` & `dvc-3.8.0/dvc/repo/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/exceptions.py` & `dvc-3.8.0/dvc/repo/experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/executor/base.py` & `dvc-3.8.0/dvc/repo/experiments/executor/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/executor/local.py` & `dvc-3.8.0/dvc/repo/experiments/executor/local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/executor/ssh.py` & `dvc-3.8.0/dvc/repo/experiments/executor/ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/ls.py` & `dvc-3.8.0/dvc/repo/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/pull.py` & `dvc-3.8.0/dvc/repo/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/push.py` & `dvc-3.8.0/dvc/repo/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/queue/base.py` & `dvc-3.8.0/dvc/repo/experiments/queue/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/queue/celery.py` & `dvc-3.8.0/dvc/repo/experiments/queue/celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/queue/remove.py` & `dvc-3.8.0/dvc/repo/experiments/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/queue/tasks.py` & `dvc-3.8.0/dvc/repo/experiments/queue/tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/queue/tempdir.py` & `dvc-3.8.0/dvc/repo/experiments/queue/tempdir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/queue/utils.py` & `dvc-3.8.0/dvc/repo/experiments/queue/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/queue/workspace.py` & `dvc-3.8.0/dvc/repo/experiments/queue/workspace.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/refs.py` & `dvc-3.8.0/dvc/repo/experiments/refs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/remove.py` & `dvc-3.8.0/dvc/repo/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/run.py` & `dvc-3.8.0/dvc/repo/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/save.py` & `dvc-3.8.0/dvc/repo/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/serialize.py` & `dvc-3.8.0/dvc/repo/experiments/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/show.py` & `dvc-3.8.0/dvc/repo/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/stash.py` & `dvc-3.8.0/dvc/repo/experiments/stash.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/experiments/utils.py` & `dvc-3.8.0/dvc/repo/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/fetch.py` & `dvc-3.8.0/dvc/repo/fetch.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,42 +17,45 @@
     with_deps=False,
     all_tags=False,
     recursive=False,
     all_commits=False,
     revs=None,
     max_size=None,
     types=None,
+    config=None,
 ):
     indexes = {}
     collection_exc = None
+
+    config = config or {}
+    if remote:
+        core = config.get("core") or {}
+        core["remote"] = remote
+        config["core"] = core
+
     for rev in repo.brancher(
         revs=revs,
         all_branches=all_branches,
         all_tags=all_tags,
         all_commits=all_commits,
     ):
-        saved_remote = repo.config["core"].get("remote")
         try:
-            if remote:
-                repo.config["core"]["remote"] = remote
+            repo.config.update(config)
 
             idx = repo.index.targets_view(
                 targets,
                 with_deps=with_deps,
                 recursive=recursive,
                 max_size=max_size,
                 types=types,
             )
             indexes[idx.data_tree.hash_info.value] = idx.data["repo"]
         except Exception as exc:  # pylint: disable=broad-except
             collection_exc = exc
             logger.exception("failed to collect '%s'", rev or "workspace")
-        finally:
-            if remote:
-                repo.config["core"]["remote"] = saved_remote
 
     if not indexes and collection_exc:
         raise collection_exc
 
     return indexes
 
 
@@ -67,14 +70,15 @@
     all_tags=False,
     recursive=False,
     all_commits=False,
     run_cache=False,
     revs=None,
     max_size=None,
     types=None,
+    config=None,
 ) -> int:
     """Download data items from a cloud and imported repositories
 
     Returns:
         int: number of successfully downloaded files
 
     Raises:
@@ -110,14 +114,15 @@
         with_deps=with_deps,
         all_tags=all_tags,
         recursive=recursive,
         all_commits=all_commits,
         revs=revs,
         max_size=max_size,
         types=types,
+        config=config,
     )
 
     cache_key = ("fetch", tokenize(sorted(indexes.keys())))
 
     with Callback.as_tqdm_callback(
         desc="Collecting",
         unit="entry",
```

### Comparing `dvc-3.7.0/dvc/repo/gc.py` & `dvc-3.8.0/dvc/repo/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/get.py` & `dvc-3.8.0/dvc/repo/get.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,14 @@
             "the given path is a DVC file, you must specify a data file or a directory"
         )
 
 
 def get(url, path, out=None, rev=None, jobs=None, force=False, config=None):
     from dvc.config import Config
     from dvc.dvcfile import is_valid_filename
-    from dvc.fs.callbacks import Callback
     from dvc.repo import Repo
 
     out = resolve_output(path, out, force=force)
 
     if is_valid_filename(out):
         raise GetDVCFileError
 
@@ -36,27 +35,23 @@
     with Repo.open(
         url=url,
         rev=rev,
         subrepos=True,
         uninitialized=True,
         config=config,
     ) as repo:
+        from dvc.fs import download
         from dvc.fs.data import DataFileSystem
 
         fs: Union[DataFileSystem, "DVCFileSystem"]
         if os.path.isabs(path):
             fs = DataFileSystem(index=repo.index.data["local"])
             fs_path = fs.from_os_path(path)
         else:
             fs = repo.dvcfs
             fs_path = fs.from_os_path(path)
-
-        with Callback.as_tqdm_callback(
-            desc=f"Downloading {fs.path.name(path)}",
-            unit="files",
-        ) as cb:
-            fs.get(
-                fs_path,
-                os.path.abspath(out),
-                batch_size=jobs,
-                callback=cb,
-            )
+        download(
+            fs,
+            fs_path,
+            os.path.abspath(out),
+            jobs=jobs,
+        )
```

### Comparing `dvc-3.7.0/dvc/repo/get_url.py` & `dvc-3.8.0/dvc/repo/get_url.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     out = resolve_output(url, out, force=force)
     out = os.path.abspath(out)
     (out,) = output.loads_from(None, [out], use_cache=False)
 
     src_fs, src_path = parse_external_url(url, config)
     if not src_fs.exists(src_path):
         raise URLMissingError(url)
-    download(src_fs, src_path, out, jobs=jobs)
+    download(src_fs, src_path, out.fs_path, jobs=jobs)
```

### Comparing `dvc-3.7.0/dvc/repo/graph.py` & `dvc-3.8.0/dvc/repo/graph.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/imp_url.py` & `dvc-3.8.0/dvc/repo/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/imports.py` & `dvc-3.8.0/dvc/repo/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/index.py` & `dvc-3.8.0/dvc/repo/index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/init.py` & `dvc-3.8.0/dvc/repo/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/install.py` & `dvc-3.8.0/dvc/repo/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/ls.py` & `dvc-3.8.0/dvc/repo/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/ls_url.py` & `dvc-3.8.0/dvc/repo/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/metrics/diff.py` & `dvc-3.8.0/dvc/repo/metrics/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/metrics/show.py` & `dvc-3.8.0/dvc/repo/metrics/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/move.py` & `dvc-3.8.0/dvc/repo/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/open_repo.py` & `dvc-3.8.0/dvc/repo/open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/params/diff.py` & `dvc-3.8.0/dvc/repo/params/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/params/show.py` & `dvc-3.8.0/dvc/repo/params/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/plots/__init__.py` & `dvc-3.8.0/dvc/repo/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/plots/diff.py` & `dvc-3.8.0/dvc/repo/plots/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/pull.py` & `dvc-3.8.0/dvc/repo/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/push.py` & `dvc-3.8.0/dvc/repo/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/remove.py` & `dvc-3.8.0/dvc/repo/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/reproduce.py` & `dvc-3.8.0/dvc/repo/reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/run.py` & `dvc-3.8.0/dvc/repo/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/scm_context.py` & `dvc-3.8.0/dvc/repo/scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/stage.py` & `dvc-3.8.0/dvc/repo/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/status.py` & `dvc-3.8.0/dvc/repo/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/trie.py` & `dvc-3.8.0/dvc/repo/trie.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/update.py` & `dvc-3.8.0/dvc/repo/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/repo/worktree.py` & `dvc-3.8.0/dvc/repo/worktree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/rwlock.py` & `dvc-3.8.0/dvc/rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/schema.py` & `dvc-3.8.0/dvc/schema.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/scm.py` & `dvc-3.8.0/dvc/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/__init__.py` & `dvc-3.8.0/dvc/stage/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/cache.py` & `dvc-3.8.0/dvc/stage/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/decorators.py` & `dvc-3.8.0/dvc/stage/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/exceptions.py` & `dvc-3.8.0/dvc/stage/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/imports.py` & `dvc-3.8.0/dvc/stage/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/loader.py` & `dvc-3.8.0/dvc/stage/loader.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/run.py` & `dvc-3.8.0/dvc/stage/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/serialize.py` & `dvc-3.8.0/dvc/stage/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/stage/utils.py` & `dvc-3.8.0/dvc/stage/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/README.rst` & `dvc-3.8.0/dvc/testing/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/api_tests.py` & `dvc-3.8.0/dvc/testing/api_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_checkout.py` & `dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_data_status.py` & `dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/benchmarks/cli/commands/test_plots.py` & `dvc-3.8.0/dvc/testing/benchmarks/cli/commands/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py` & `dvc-3.8.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/benchmarks/fixtures.py` & `dvc-3.8.0/dvc/testing/benchmarks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/benchmarks/plugin.py` & `dvc-3.8.0/dvc/testing/benchmarks/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/cloud.py` & `dvc-3.8.0/dvc/testing/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/fixtures.py` & `dvc-3.8.0/dvc/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/path_info.py` & `dvc-3.8.0/dvc/testing/path_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/plugin.py` & `dvc-3.8.0/dvc/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/remote_tests.py` & `dvc-3.8.0/dvc/testing/remote_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/tmp_dir.py` & `dvc-3.8.0/dvc/testing/tmp_dir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/testing/workspace_tests.py` & `dvc-3.8.0/dvc/testing/workspace_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/ui/__init__.py` & `dvc-3.8.0/dvc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/ui/_rich_progress.py` & `dvc-3.8.0/dvc/ui/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/ui/pager.py` & `dvc-3.8.0/dvc/ui/pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/ui/table.py` & `dvc-3.8.0/dvc/ui/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/updater.py` & `dvc-3.8.0/dvc/updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/__init__.py` & `dvc-3.8.0/dvc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/cli_parse.py` & `dvc-3.8.0/dvc/utils/cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/collections.py` & `dvc-3.8.0/dvc/utils/collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/diff.py` & `dvc-3.8.0/dvc/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/fs.py` & `dvc-3.8.0/dvc/utils/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/humanize.py` & `dvc-3.8.0/dvc/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/hydra.py` & `dvc-3.8.0/dvc/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/serialize/__init__.py` & `dvc-3.8.0/dvc/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/serialize/_common.py` & `dvc-3.8.0/dvc/utils/serialize/_common.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/serialize/_json.py` & `dvc-3.8.0/dvc/utils/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/serialize/_py.py` & `dvc-3.8.0/dvc/utils/serialize/_py.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/serialize/_toml.py` & `dvc-3.8.0/dvc/utils/serialize/_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/serialize/_yaml.py` & `dvc-3.8.0/dvc/utils/serialize/_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/strictyaml.py` & `dvc-3.8.0/dvc/utils/strictyaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/studio.py` & `dvc-3.8.0/dvc/utils/studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/table.py` & `dvc-3.8.0/dvc/utils/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc/utils/threadpool.py` & `dvc-3.8.0/dvc/utils/threadpool.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc.egg-info/PKG-INFO` & `dvc-3.8.0/dvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.7.0
+Version: 3.8.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.7.0/dvc.egg-info/SOURCES.txt` & `dvc-3.8.0/dvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/dvc.egg-info/requires.txt` & `dvc-3.8.0/dvc.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/pyproject.toml` & `dvc-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/conftest.py` & `dvc-3.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/dir_helpers.py` & `dvc-3.8.0/tests/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/api/test_data.py` & `dvc-3.8.0/tests/func/api/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/api/test_experiments.py` & `dvc-3.8.0/tests/func/api/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/api/test_scm.py` & `dvc-3.8.0/tests/func/api/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/api/test_show.py` & `dvc-3.8.0/tests/func/api/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/artifacts/test_artifacts.py` & `dvc-3.8.0/tests/func/artifacts/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/data/db/test_index.py` & `dvc-3.8.0/tests/func/data/db/test_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/conftest.py` & `dvc-3.8.0/tests/func/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/executor/test_ssh.py` & `dvc-3.8.0/tests/func/experiments/executor/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_apply.py` & `dvc-3.8.0/tests/func/experiments/test_apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_diff.py` & `dvc-3.8.0/tests/func/experiments/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_experiments.py` & `dvc-3.8.0/tests/func/experiments/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_queue.py` & `dvc-3.8.0/tests/func/experiments/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_remote.py` & `dvc-3.8.0/tests/func/experiments/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_remove.py` & `dvc-3.8.0/tests/func/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_save.py` & `dvc-3.8.0/tests/func/experiments/test_save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_set_params.py` & `dvc-3.8.0/tests/func/experiments/test_set_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_show.py` & `dvc-3.8.0/tests/func/experiments/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_stash_exp.py` & `dvc-3.8.0/tests/func/experiments/test_stash_exp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/experiments/test_utils.py` & `dvc-3.8.0/tests/func/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/machine/conftest.py` & `dvc-3.8.0/tests/func/machine/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/machine/test_machine_config.py` & `dvc-3.8.0/tests/func/machine/test_machine_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/machine/test_machine_status.py` & `dvc-3.8.0/tests/func/machine/test_machine_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/metrics/test_diff.py` & `dvc-3.8.0/tests/func/metrics/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/metrics/test_show.py` & `dvc-3.8.0/tests/func/metrics/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/params/test_diff.py` & `dvc-3.8.0/tests/func/params/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/params/test_show.py` & `dvc-3.8.0/tests/func/params/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/parsing/__init__.py` & `dvc-3.8.0/tests/func/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/parsing/test_errors.py` & `dvc-3.8.0/tests/func/parsing/test_errors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/parsing/test_foreach.py` & `dvc-3.8.0/tests/func/parsing/test_foreach.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/parsing/test_interpolated_entry.py` & `dvc-3.8.0/tests/func/parsing/test_interpolated_entry.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/parsing/test_resolver.py` & `dvc-3.8.0/tests/func/parsing/test_resolver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/plots/test_diff.py` & `dvc-3.8.0/tests/func/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/plots/test_modify.py` & `dvc-3.8.0/tests/func/plots/test_modify.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/plots/test_show.py` & `dvc-3.8.0/tests/func/plots/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/repro/test_repro.py` & `dvc-3.8.0/tests/func/repro/test_repro.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pytest
 from funcy import lsplit
 
 from dvc.cli import main
 from dvc.dvcfile import LOCK_FILE, PROJECT_FILE
 from dvc.exceptions import CyclicGraphError, ReproductionError
-from dvc.fs import LocalFileSystem, system
+from dvc.fs import system
 from dvc.output import Output
 from dvc.stage import PipelineStage, Stage
 from dvc.stage.cache import RunCacheNotSupported
 from dvc.stage.exceptions import StageFileDoesNotExistError, StageNotFound
 from dvc.utils.fs import remove
 from dvc.utils.serialize import modify_yaml
 from dvc_data.hashfile.hash import file_md5
@@ -620,20 +620,22 @@
         ret = main(["repro", "--force", stage.addressing])
         assert ret == 0
 
         saved_stage = dvc.stage.get_target(stage.addressing)
         assert stage.outs[0].hash_info != saved_stage.outs[0].hash_info
 
     def test_force_import(self, mocker, tmp_dir, dvc):
+        from dvc.dependency import base
+
         tmp_dir.dvc_gen("foo", "foo")
 
         ret = main(["import-url", "foo", "bar"])
         assert ret == 0
 
-        spy_get = mocker.spy(LocalFileSystem, "get")
+        spy_get = mocker.spy(base, "fs_download")
         spy_checkout = mocker.spy(Output, "checkout")
 
         assert main(["unfreeze", "bar.dvc"]) == 0
         ret = main(["repro", "--force", "bar.dvc"])
         assert ret == 0
         assert spy_get.call_count == 1
         assert spy_checkout.call_count == 0
```

### Comparing `dvc-3.7.0/tests/func/repro/test_repro_allow_missing.py` & `dvc-3.8.0/tests/func/repro/test_repro_allow_missing.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/repro/test_repro_pull.py` & `dvc-3.8.0/tests/func/repro/test_repro_pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_add.py` & `dvc-3.8.0/tests/func/test_add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_analytics.py` & `dvc-3.8.0/tests/func/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_check_ignore.py` & `dvc-3.8.0/tests/func/test_check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_checkout.py` & `dvc-3.8.0/tests/func/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_cli.py` & `dvc-3.8.0/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_commit.py` & `dvc-3.8.0/tests/func/test_commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_config.py` & `dvc-3.8.0/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_data_cloud.py` & `dvc-3.8.0/tests/func/test_data_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,16 @@
     dvc.pull()
     # NOTE: 2 are for index.data_tree building
     assert hash_spy.call_count == 3
 
     # Removing cache will invalidate existing state entries
     dvc.cache.local.clear()
 
-    dvc.config["remote"]["upstream"]["verify"] = True
+    with dvc.config.edit() as conf:
+        conf["remote"]["upstream"]["verify"] = True
 
     dvc.pull()
     assert hash_spy.call_count == 10
 
 
 @flaky(max_runs=3, min_passes=1)
 @pytest.mark.parametrize(
```

### Comparing `dvc-3.7.0/tests/func/test_data_status.py` & `dvc-3.8.0/tests/func/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_diff.py` & `dvc-3.8.0/tests/func/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_dvcfile.py` & `dvc-3.8.0/tests/func/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_external_repo.py` & `dvc-3.8.0/tests/func/test_external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_fs.py` & `dvc-3.8.0/tests/func/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_gc.py` & `dvc-3.8.0/tests/func/test_gc.py`

 * *Files 16% similar despite different names*

```diff
@@ -192,19 +192,15 @@
 
 
 def test_gc_cloud_positive(tmp_dir, dvc, tmp_path_factory, local_remote):
     for flag in ["-cw", "-ca", "-cT", "-caT", "-cwT"]:
         assert main(["gc", "-vf", flag]) == 0
 
 
-def test_gc_cloud_remove_order(tmp_dir, scm, dvc, tmp_path_factory, mocker):
-    storage = os.fspath(tmp_path_factory.mktemp("test_remote_base"))
-    dvc.config["remote"]["local_remote"] = {"url": storage}
-    dvc.config["core"]["remote"] = "local_remote"
-
+def test_gc_cloud_remove_order(tmp_dir, scm, dvc, mocker, local_remote):
     (standalone, dir1, dir2) = tmp_dir.dvc_gen(
         {
             "file1": "standalone",
             "dir1": {"file2": "file2"},
             "dir2": {"file3": "file3", "file4": "file4"},
         }
     )
@@ -317,19 +313,15 @@
     assert _count_files(dvc.cache.local.path) == 2
     assert dvc.cache.local.exists("9ae73c65f418e6f79ceb4f0e4a4b98d5")
     assert dvc.cache.local.exists(
         "3bcf3b1be3e794a97a5a6b93a005784c"
     )  # "modified, again"
 
 
-def test_gc_not_in_remote(tmp_dir, scm, dvc, tmp_path_factory, mocker):
-    storage = os.fspath(tmp_path_factory.mktemp("test_remote_base"))
-    dvc.config["remote"]["local_remote"] = {"url": storage}
-    dvc.config["core"]["remote"] = "local_remote"
-
+def test_gc_not_in_remote(tmp_dir, scm, dvc, mocker, local_remote):
     (standalone, dir1, dir2) = tmp_dir.dvc_gen(
         {
             "file1": "standalone",
             "dir1": {"file2": "file2"},
             "dir2": {"file3": "file3", "file4": "file4"},
         }
     )
@@ -354,20 +346,17 @@
     # Order is not guaranteed here.
     assert (
         f"{standalone_hash[2:]}" in arg_list[2][0][1][0]
         or f"{standalone_hash[2:]}" in arg_list[2][0][1][1]
     )
 
 
-def test_gc_not_in_remote_remote_arg(tmp_dir, scm, dvc, tmp_path_factory, mocker):
-    storage = os.fspath(tmp_path_factory.mktemp("test_remote_base"))
-    dvc.config["remote"]["local_remote"] = {"url": storage}
-    dvc.config["core"]["remote"] = "local_remote"
-    other_storage = os.fspath(tmp_path_factory.mktemp("test_remote_other"))
-    dvc.config["remote"]["other_remote"] = {"url": other_storage}
+def test_gc_not_in_remote_remote_arg(tmp_dir, scm, dvc, mocker, make_remote):
+    make_remote("local_remote", typ="local")
+    make_remote("other_remote", typ="local", default=False)
 
     tmp_dir.dvc_gen(
         {
             "file1": "standalone",
             "dir1": {"file2": "file2"},
             "dir2": {"file3": "file3", "file4": "file4"},
         }
@@ -381,23 +370,17 @@
     assert not mocked_remove.mock_calls
 
     dvc.gc(workspace=True, not_in_remote=True, remote="other_remote")
 
     assert len(mocked_remove.mock_calls) == 3
 
 
-def test_gc_not_in_remote_with_remote_field(
-    tmp_dir, scm, dvc, tmp_path_factory, mocker
-):
-    storage = os.fspath(tmp_path_factory.mktemp("test_remote_base"))
-    dvc.config["remote"]["local_remote"] = {"url": storage}
-    dvc.config["core"]["remote"] = "local_remote"
-
-    other_storage = os.fspath(tmp_path_factory.mktemp("test_remote_other"))
-    dvc.config["remote"]["other_remote"] = {"url": other_storage}
+def test_gc_not_in_remote_with_remote_field(tmp_dir, scm, dvc, mocker, make_remote):
+    make_remote("local_remote", typ="local")
+    make_remote("other_remote", typ="local", default=False)
 
     text = textwrap.dedent(
         """\
         outs:
         - path: foo
           remote: other_remote
           hash: md5
@@ -416,20 +399,17 @@
     with pytest.raises(
         InvalidArgumentError,
         match="`--not-in-remote` and `--cloud` are mutually exclusive",
     ):
         dvc.gc(workspace=True, not_in_remote=True, cloud=True)
 
 
-def test_gc_cloud_remote_field(tmp_dir, scm, dvc, tmp_path_factory, mocker):
-    storage = os.fspath(tmp_path_factory.mktemp("test_remote_base"))
-    dvc.config["remote"]["local_remote"] = {"url": storage}
-    dvc.config["core"]["remote"] = "local_remote"
-    other_storage = os.fspath(tmp_path_factory.mktemp("test_remote_other"))
-    dvc.config["remote"]["other_remote"] = {"url": other_storage}
+def test_gc_cloud_remote_field(tmp_dir, scm, dvc, mocker, make_remote):
+    make_remote("local_remote", typ="local")
+    make_remote("other_remote", typ="local", default=False)
 
     text = textwrap.dedent(
         """\
         outs:
         - path: foo
           remote: other_remote
           hash: md5
```

### Comparing `dvc-3.7.0/tests/func/test_get.py` & `dvc-3.8.0/tests/func/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_get_url.py` & `dvc-3.8.0/tests/func/test_get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_ignore.py` & `dvc-3.8.0/tests/func/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_import.py` & `dvc-3.8.0/tests/func/test_import.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_import_url.py` & `dvc-3.8.0/tests/func/test_import_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_init.py` & `dvc-3.8.0/tests/func/test_init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_install.py` & `dvc-3.8.0/tests/func/test_install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_lock.py` & `dvc-3.8.0/tests/func/test_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_lockfile.py` & `dvc-3.8.0/tests/func/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_ls.py` & `dvc-3.8.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_merge_driver.py` & `dvc-3.8.0/tests/func/test_merge_driver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_move.py` & `dvc-3.8.0/tests/func/test_move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_odb.py` & `dvc-3.8.0/tests/func/test_odb.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_remote.py` & `dvc-3.8.0/tests/func/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_remove.py` & `dvc-3.8.0/tests/func/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_repo.py` & `dvc-3.8.0/tests/func/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_repo_index.py` & `dvc-3.8.0/tests/func/test_repo_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_run.py` & `dvc-3.8.0/tests/func/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_run_cache.py` & `dvc-3.8.0/tests/func/test_run_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_scm.py` & `dvc-3.8.0/tests/func/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_scm_context.py` & `dvc-3.8.0/tests/func/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_stage.py` & `dvc-3.8.0/tests/func/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_stage_load.py` & `dvc-3.8.0/tests/func/test_stage_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_state.py` & `dvc-3.8.0/tests/func/test_state.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_status.py` & `dvc-3.8.0/tests/func/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_unprotect.py` & `dvc-3.8.0/tests/func/test_unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_update.py` & `dvc-3.8.0/tests/func/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_used_objs.py` & `dvc-3.8.0/tests/func/test_used_objs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_utils.py` & `dvc-3.8.0/tests/func/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_version.py` & `dvc-3.8.0/tests/func/test_version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/test_virtual_directory.py` & `dvc-3.8.0/tests/func/test_virtual_directory.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/utils/test_hydra.py` & `dvc-3.8.0/tests/func/utils/test_hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/func/utils/test_strict_yaml.py` & `dvc-3.8.0/tests/func/utils/test_strict_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/integration/plots/conftest.py` & `dvc-3.8.0/tests/integration/plots/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/integration/plots/test_plots.py` & `dvc-3.8.0/tests/integration/plots/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/integration/plots/test_repo_plots_api.py` & `dvc-3.8.0/tests/integration/plots/test_repo_plots_api.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/integration/test_studio_live_experiments.py` & `dvc-3.8.0/tests/integration/test_studio_live_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/remotes/git_server.py` & `dvc-3.8.0/tests/remotes/git_server.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/remotes/user.key` & `dvc-3.8.0/tests/remotes/user.key`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/remotes_env.sample` & `dvc-3.8.0/tests/remotes_env.sample`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/scripts.py` & `dvc-3.8.0/tests/scripts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/cli/test_main.py` & `dvc-3.8.0/tests/unit/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/ls/test_ls.py` & `dvc-3.8.0/tests/unit/command/ls/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/ls/test_ls_colors.py` & `dvc-3.8.0/tests/unit/command/ls/test_ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_add.py` & `dvc-3.8.0/tests/unit/command/test_add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_cache.py` & `dvc-3.8.0/tests/unit/command/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_checkout.py` & `dvc-3.8.0/tests/unit/command/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_compat_flag.py` & `dvc-3.8.0/tests/unit/command/test_compat_flag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_config.py` & `dvc-3.8.0/tests/unit/command/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_dag.py` & `dvc-3.8.0/tests/unit/command/test_dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_data_status.py` & `dvc-3.8.0/tests/unit/command/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_data_sync.py` & `dvc-3.8.0/tests/unit/command/test_data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_diff.py` & `dvc-3.8.0/tests/unit/command/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_experiments.py` & `dvc-3.8.0/tests/unit/command/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_gc.py` & `dvc-3.8.0/tests/unit/command/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_get.py` & `dvc-3.8.0/tests/unit/command/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_git_hook.py` & `dvc-3.8.0/tests/unit/command/test_git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_imp.py` & `dvc-3.8.0/tests/unit/command/test_imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_imp_url.py` & `dvc-3.8.0/tests/unit/command/test_imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_ls_url.py` & `dvc-3.8.0/tests/unit/command/test_ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_machine.py` & `dvc-3.8.0/tests/unit/command/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_metrics.py` & `dvc-3.8.0/tests/unit/command/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_params.py` & `dvc-3.8.0/tests/unit/command/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_plots.py` & `dvc-3.8.0/tests/unit/command/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_queue.py` & `dvc-3.8.0/tests/unit/command/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_repro.py` & `dvc-3.8.0/tests/unit/command/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_stage.py` & `dvc-3.8.0/tests/unit/command/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_status.py` & `dvc-3.8.0/tests/unit/command/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/command/test_update.py` & `dvc-3.8.0/tests/unit/command/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/data/db/test_local.py` & `dvc-3.8.0/tests/unit/data/db/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/dependency/test_params.py` & `dvc-3.8.0/tests/unit/dependency/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/fs/test_azure.py` & `dvc-3.8.0/tests/unit/fs/test_azure.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/fs/test_data.py` & `dvc-3.8.0/tests/unit/fs/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/fs/test_dvc.py` & `dvc-3.8.0/tests/unit/fs/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/fs/test_dvc_info.py` & `dvc-3.8.0/tests/unit/fs/test_dvc_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/fs/test_fs.py` & `dvc-3.8.0/tests/unit/fs/test_fs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from dataclasses import dataclass
-
 import pytest
 from dvc_http import HTTPFileSystem, HTTPSFileSystem
 from dvc_s3 import S3FileSystem
 from dvc_ssh import SSHFileSystem
 
 from dvc.config import RemoteNotFoundError
 from dvc.fs import LocalFileSystem, get_cloud_fs, get_fs_cls, get_fs_config
@@ -59,18 +57,12 @@
     assert result == {
         "password": "123",
         "user": "user",
         "url": "http://example.com/r1/r2/foo",
     }
 
 
-@dataclass
-class FakeRepo:
-    config: dict
-
-
 def test_get_cloud_fs():
-    repo = FakeRepo({})
-    cls, config, path = get_cloud_fs(repo, url="ssh://example.com:/dir/path")
+    cls, config, path = get_cloud_fs({}, url="ssh://example.com:/dir/path")
     assert cls is SSHFileSystem
     assert config == {"host": "example.com", "verify": False}
     assert path == "/dir/path"
```

### Comparing `dvc-3.7.0/tests/unit/fs/test_path.py` & `dvc-3.8.0/tests/unit/fs/test_path.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/fs/test_s3.py` & `dvc-3.8.0/tests/unit/fs/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/fs/test_tree.py` & `dvc-3.8.0/tests/unit/fs/test_tree.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     tmp_dir.add_remote(name="first", url="remote://base/first", default=False)
     tmp_dir.add_remote(name="second", url="remote://first/second", default=False)
 
     base = "bucket/path"
     first = f"{base}/first"
     second = f"{first}/second"
 
-    _, _, path = get_cloud_fs(dvc, name="base")
+    _, _, path = get_cloud_fs(dvc.config, name="base")
     assert path == base
-    _, _, path = get_cloud_fs(dvc, name="first")
+    _, _, path = get_cloud_fs(dvc.config, name="first")
     assert path == first
-    _, _, path = get_cloud_fs(dvc, name="second")
+    _, _, path = get_cloud_fs(dvc.config, name="second")
     assert path == second
 
 
 def test_get_cloud_fs_validate(tmp_dir, dvc):
     tmp_dir.add_remote(name="base", url="ssh://example.com/path", default=False)
     tmp_dir.add_remote(
         name="first",
@@ -30,13 +30,13 @@
     )
     tmp_dir.add_remote(
         name="second",
         config={"url": "remote://first/second", "oss_key_id": "mykey"},
         default=False,
     )
 
-    assert get_cloud_fs(dvc, name="base")[1]["host"] == "example.com"
-    assert get_cloud_fs(dvc, name="first")[1]["host"] == "example.com"
-    assert get_cloud_fs(dvc, name="first")[1]["type"] == ["symlink"]
+    assert get_cloud_fs(dvc.config, name="base")[1]["host"] == "example.com"
+    assert get_cloud_fs(dvc.config, name="first")[1]["host"] == "example.com"
+    assert get_cloud_fs(dvc.config, name="first")[1]["type"] == ["symlink"]
 
     with pytest.raises(ConfigError):
-        get_cloud_fs(dvc, name="second")
+        get_cloud_fs(dvc.config, name="second")
```

### Comparing `dvc-3.7.0/tests/unit/machine/test_machine.py` & `dvc-3.8.0/tests/unit/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/output/test_load.py` & `dvc-3.8.0/tests/unit/output/test_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/output/test_local.py` & `dvc-3.8.0/tests/unit/output/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/output/test_output.py` & `dvc-3.8.0/tests/unit/output/test_output.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/remote/test_oss.py` & `dvc-3.8.0/tests/unit/remote/test_oss.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/remote/test_remote.py` & `dvc-3.8.0/tests/unit/remote/test_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,43 +8,43 @@
 def test_remote_with_hash_jobs(dvc):
     dvc.config["remote"]["with_hash_jobs"] = {
         "url": "s3://bucket/name",
         "checksum_jobs": 100,
     }
     dvc.config["core"]["checksum_jobs"] = 200
 
-    cls, config, _ = get_cloud_fs(dvc, name="with_hash_jobs")
+    cls, config, _ = get_cloud_fs(dvc.config, name="with_hash_jobs")
     fs = cls(**config)
     assert fs.hash_jobs == 100
 
 
 def test_remote_with_jobs(dvc):
     dvc.config["remote"]["with_jobs"] = {
         "url": "s3://bucket/name",
         "jobs": 100,
     }
 
-    cls, config, _ = get_cloud_fs(dvc, name="with_jobs")
+    cls, config, _ = get_cloud_fs(dvc.config, name="with_jobs")
     fs = cls(**config)
     assert fs.jobs == 100
 
 
 def test_remote_without_hash_jobs(dvc):
     dvc.config["remote"]["without_hash_jobs"] = {"url": "s3://bucket/name"}
     dvc.config["core"]["checksum_jobs"] = 200
 
-    cls, config, _ = get_cloud_fs(dvc, name="without_hash_jobs")
+    cls, config, _ = get_cloud_fs(dvc.config, name="without_hash_jobs")
     fs = cls(**config)
     assert fs.hash_jobs == 200
 
 
 def test_remote_without_hash_jobs_default(dvc):
     dvc.config["remote"]["without_hash_jobs"] = {"url": "s3://bucket/name"}
 
-    cls, config, _ = get_cloud_fs(dvc, name="without_hash_jobs")
+    cls, config, _ = get_cloud_fs(dvc.config, name="without_hash_jobs")
     fs = cls(**config)
     assert fs.hash_jobs == fs.HASH_JOBS
 
 
 @pytest.mark.parametrize("fs_cls", [GSFileSystem, S3FileSystem])
 def test_makedirs_not_create_for_top_level_path(fs_cls, dvc, mocker):
     url = f"{fs_cls.protocol}://bucket/"
```

### Comparing `dvc-3.7.0/tests/unit/remote/test_webdav.py` & `dvc-3.8.0/tests/unit/remote/test_webdav.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,18 +141,18 @@
     ],
 )
 def test_remote_with_jobs(dvc, base_url, fs_cls):
     scheme = "http" + ("s" if fs_cls is WebDAVSFileSystem else "")
     remote_config = {"url": base_url}
 
     dvc.config["remote"]["dav"] = remote_config
-    cls, config, _ = get_cloud_fs(dvc, name="dav")
+    cls, config, _ = get_cloud_fs(dvc.config, name="dav")
     assert config["user"] == user
     assert f"{scheme}://{user}@example.com" in config["host"]
     assert cls is fs_cls
 
     # config from remote takes priority
     remote_config.update({"user": "admin"})
-    cls, config, _ = get_cloud_fs(dvc, name="dav")
+    cls, config, _ = get_cloud_fs(dvc.config, name="dav")
     assert config["user"] == "admin"
     assert f"{scheme}://{user}@example.com" in config["host"]
     assert cls is fs_cls
```

### Comparing `dvc-3.7.0/tests/unit/remote/test_webhdfs.py` & `dvc-3.8.0/tests/unit/remote/test_webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/render/test_convert.py` & `dvc-3.8.0/tests/unit/render/test_convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/render/test_image_converter.py` & `dvc-3.8.0/tests/unit/render/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/render/test_match.py` & `dvc-3.8.0/tests/unit/render/test_match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/render/test_vega_converter.py` & `dvc-3.8.0/tests/unit/render/test_vega_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/experiments/conftest.py` & `dvc-3.8.0/tests/unit/repo/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/experiments/queue/test_celery.py` & `dvc-3.8.0/tests/unit/repo/experiments/queue/test_celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/experiments/queue/test_remove.py` & `dvc-3.8.0/tests/unit/repo/experiments/queue/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/experiments/test_collect.py` & `dvc-3.8.0/tests/unit/repo/experiments/test_collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/experiments/test_executor_status.py` & `dvc-3.8.0/tests/unit/repo/experiments/test_executor_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/experiments/test_remove.py` & `dvc-3.8.0/tests/unit/repo/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/experiments/test_utils.py` & `dvc-3.8.0/tests/unit/repo/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/plots/test_diff.py` & `dvc-3.8.0/tests/unit/repo/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/test_graph.py` & `dvc-3.8.0/tests/unit/repo/test_graph.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/test_open_repo.py` & `dvc-3.8.0/tests/unit/repo/test_open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/test_repo.py` & `dvc-3.8.0/tests/unit/repo/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/test_reproduce.py` & `dvc-3.8.0/tests/unit/repo/test_reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/repo/test_scm_context.py` & `dvc-3.8.0/tests/unit/repo/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/scm/test_scm.py` & `dvc-3.8.0/tests/unit/scm/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/stage/test_cache.py` & `dvc-3.8.0/tests/unit/stage/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/stage/test_loader_pipeline_file.py` & `dvc-3.8.0/tests/unit/stage/test_loader_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/stage/test_run.py` & `dvc-3.8.0/tests/unit/stage/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/stage/test_serialize_pipeline_file.py` & `dvc-3.8.0/tests/unit/stage/test_serialize_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/stage/test_serialize_pipeline_lock.py` & `dvc-3.8.0/tests/unit/stage/test_serialize_pipeline_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/stage/test_stage.py` & `dvc-3.8.0/tests/unit/stage/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/stage/test_utils.py` & `dvc-3.8.0/tests/unit/stage/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_analytics.py` & `dvc-3.8.0/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_collect.py` & `dvc-3.8.0/tests/unit/test_collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_compare.py` & `dvc-3.8.0/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_config.py` & `dvc-3.8.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_context.py` & `dvc-3.8.0/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_daemon.py` & `dvc-3.8.0/tests/unit/test_daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_dvcfile.py` & `dvc-3.8.0/tests/unit/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_ignore.py` & `dvc-3.8.0/tests/unit/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_imports.py` & `dvc-3.8.0/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_info.py` & `dvc-3.8.0/tests/unit/test_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_interpolate.py` & `dvc-3.8.0/tests/unit/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_lockfile.py` & `dvc-3.8.0/tests/unit/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_logger.py` & `dvc-3.8.0/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_metrics.py` & `dvc-3.8.0/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_params.py` & `dvc-3.8.0/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_pathspec_math.py` & `dvc-3.8.0/tests/unit/test_pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_progress.py` & `dvc-3.8.0/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_rwlock.py` & `dvc-3.8.0/tests/unit/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_tabular_data.py` & `dvc-3.8.0/tests/unit/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/test_updater.py` & `dvc-3.8.0/tests/unit/test_updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/ui/test_console.py` & `dvc-3.8.0/tests/unit/ui/test_console.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/ui/test_pager.py` & `dvc-3.8.0/tests/unit/ui/test_pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/ui/test_table.py` & `dvc-3.8.0/tests/unit/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/serialize/test_python.py` & `dvc-3.8.0/tests/unit/utils/serialize/test_python.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/serialize/test_toml.py` & `dvc-3.8.0/tests/unit/utils/serialize/test_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/serialize/test_yaml.py` & `dvc-3.8.0/tests/unit/utils/serialize/test_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/test_cli_parse.py` & `dvc-3.8.0/tests/unit/utils/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/test_collections.py` & `dvc-3.8.0/tests/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/test_executors.py` & `dvc-3.8.0/tests/unit/utils/test_executors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/test_fs.py` & `dvc-3.8.0/tests/unit/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/test_humanize.py` & `dvc-3.8.0/tests/unit/utils/test_humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/test_studio.py` & `dvc-3.8.0/tests/unit/utils/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/unit/utils/test_utils.py` & `dvc-3.8.0/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/utils/__init__.py` & `dvc-3.8.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.7.0/tests/utils/asserts.py` & `dvc-3.8.0/tests/utils/asserts.py`

 * *Files identical despite different names*

