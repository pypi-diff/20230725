# Comparing `tmp/infrahouse-toolkit-1.7.0.tar.gz` & `tmp/infrahouse-toolkit-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahouse-toolkit-1.7.0.tar", last modified: Mon Jul 24 22:49:32 2023, max compression
+gzip compressed data, was "infrahouse-toolkit-1.7.1.tar", last modified: Tue Jul 25 03:38:48 2023, max compression
```

## Comparing `infrahouse-toolkit-1.7.0.tar` & `infrahouse-toolkit-1.7.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.248200 infrahouse-toolkit-1.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.status.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.248200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.256200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.256200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.260200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.260200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/s3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.260200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.264200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/githubpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.264200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.264200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.248200 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:49:22.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.backends.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.tests.status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_publish/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.139604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.139604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/tests/test_get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.139604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/s3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/s3backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/githubpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/github_pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.143604 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/test_parse_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/test_parse_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:38:48.135604 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-25 03:38:48.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-25 03:38:48.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:38:48.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-25 03:38:48.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:38:38.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 03:38:48.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 03:38:48.000000 infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-25 03:38:48.147604 infrahouse-toolkit-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-25 03:38:01.000000 infrahouse-toolkit-1.7.1/setup.py
```

### Comparing `infrahouse-toolkit-1.7.0/CONTRIBUTING.rst` & `infrahouse-toolkit-1.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/LICENSE` & `infrahouse-toolkit-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/PKG-INFO` & `infrahouse-toolkit-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.7.0
+Version: 1.7.1
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.7.0/README.rst` & `infrahouse-toolkit-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/Makefile` & `infrahouse-toolkit-1.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/conf.py` & `infrahouse-toolkit-1.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.tests.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.cli.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.backends.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.backends.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.tests.github_pr.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.status.rst` & `infrahouse-toolkit-1.7.1/docs/infrahouse_toolkit.terraform.tests.status.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/installation.rst` & `infrahouse-toolkit-1.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/docs/usage.rst` & `infrahouse-toolkit-1.7.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,14 +44,50 @@
     required=True,
 )
 @click.option("--role-arn", help="Assume this role for all AWS operations.")
 @click.option("--gpg-key-secret-id", help="AWS secrets manager secret name that stores a GPG private key.")
 @click.option(
     "--gpg-passphrase-secret-id", help="AWS secrets manager secret name that stores a passphrase to the GPG key."
 )
+@click.option(
+    "--aws-region",
+    help="AWS region name. By default, let boto3 detect it.",
+    default=None,
+    type=click.Choice(
+        [
+            "us-east-2",
+            "us-east-1",
+            "us-west-1",
+            "us-west-2",
+            "af-south-1",
+            "ap-east-1",
+            "ap-south-2",
+            "ap-southeast-3",
+            "ap-southeast-4",
+            "ap-south-1",
+            "ap-northeast-3",
+            "ap-northeast-2",
+            "ap-southeast-1",
+            "ap-southeast-2",
+            "ap-northeast-1",
+            "ca-central-1",
+            "eu-central-1",
+            "eu-west-1",
+            "eu-west-2",
+            "eu-south-1",
+            "eu-west-3",
+            "eu-south-2",
+            "eu-north-1",
+            "eu-central-2",
+            "me-south-1",
+            "me-central-1",
+            "sa-east-1",
+        ]
+    ),
+)
 @click.pass_context
 def ih_s3_reprepro(*args, **kwargs):  # pylint: disable=unused-argument
     """
     Tool to manage deb packages to a Debian repository hosted in an S3 bucket.
     """
     setup_logging(LOG, debug=kwargs["debug"])
     check_dependencies(DEPENDENCIES)
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,91 @@
 """
 .. topic:: ``aws.py``
 
     AWS helper functions.
 """
 
 import boto3
+import requests
 from botocore.exceptions import ClientError
 
 from infrahouse_toolkit import LOG
 
+VALUE_MAP = {
+    "AWS_ACCESS_KEY_ID": "AccessKeyId",
+    "AWS_SECRET_ACCESS_KEY": "SecretAccessKey",
+    "AWS_SESSION_TOKEN": "SessionToken",
+    # These are old s3.fs options
+    # Soon they will be deprecated
+    # https://github.com/s3fs-fuse/s3fs-fuse/pull/1729
+    "AWSACCESSKEYID": "AccessKeyId",
+    "AWSSECRETACCESSKEY": "SecretAccessKey",
+    "AWSSESSIONTOKEN": "SessionToken",
+}
 
-def assume_role(role_arn) -> dict:
+
+def assume_role(role_arn, region=None) -> dict:
     """
     Assume a given role and return a dictionary with credentials.
 
     :param role_arn: Role to be assumed.
     :type role_arn: str
+    :param region: AWS region name.
+    :type region: str
     :return: A dictionary with three keys: AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY, and
     """
-    value_map = {
-        "AWS_ACCESS_KEY_ID": "AccessKeyId",
-        "AWS_SECRET_ACCESS_KEY": "SecretAccessKey",
-        "AWS_SESSION_TOKEN": "SessionToken",
-        # These are old s3.fs options
-        # Soon they will be deprecated
-        # https://github.com/s3fs-fuse/s3fs-fuse/pull/1729
-        "AWSACCESSKEYID": "AccessKeyId",
-        "AWSSECRETACCESSKEY": "SecretAccessKey",
-        "AWSSESSIONTOKEN": "SessionToken",
-    }
     try:
         LOG.debug("Assuming role %s", role_arn)
-        client = boto3.client("sts")
+        client = boto3.client("sts", region_name=region)
         response = client.assume_role(RoleArn=role_arn, RoleSessionName="ih-s3-reprepro-s3fs")
         LOG.debug("Got credentials %r", response["Credentials"])
-        return {var: response["Credentials"].get(key) for var, key in value_map.items()}
+        return {var: response["Credentials"].get(key) for var, key in VALUE_MAP.items()}
     except ClientError as err:
         LOG.error(err)
-        LOG.debug("To revert environment:\n%s", "\n".join([f"unset {key}" for key in value_map]))
+        LOG.debug("To revert environment:\n%s", "\n".join([f"unset {key}" for key in VALUE_MAP]))
         raise
 
 
-def get_client(service_name, role_arn=None, session_name=__name__):
+def get_client(service_name, role_arn=None, region=None, session_name=__name__):
     """
     Get an AWS service client assuming a role if specified.
 
     :param service_name: AWS service. ec2, sts, etc.
     :type service_name: str
     :param role_arn: Role ARN if it needs to be assumed.
     :type role_arn: str
     :param session_name: A human-readable string that tells something about this session.
         Exact value isn't important.
     :type session_name: str
+    :param region: AWS region name.
+    :type region: str
     :return: AWS boto3 client.
     """
     if role_arn:
-        sts = boto3.client("sts")
+        sts = boto3.client("sts", region_name=region)
         aws_iam_role = sts.assume_role(RoleArn=role_arn, RoleSessionName=session_name)
         session = boto3.Session(
             aws_access_key_id=aws_iam_role["Credentials"]["AccessKeyId"],
             aws_secret_access_key=aws_iam_role["Credentials"]["SecretAccessKey"],
             aws_session_token=aws_iam_role["Credentials"]["SessionToken"],
+            region_name=region,
         )
-        sts = session.client("sts")
+        sts = session.client("sts", region_name=region)
         response = sts.get_caller_identity()
         LOG.debug("Assumed role: %s", response)
-        return session.client(service_name)
+        return session.client(service_name, region_name=region)
+
+    return boto3.client(service_name, region_name=region)
+
+
+def get_credentials_from_profile() -> dict:
+    """
+    Another way to get AWS credentials is from EC2 instance metadata.
+
+    :return: A dictionary with AWS_* variables.
+    """
+    url = "http://169.254.169.254/latest/meta-data/iam/security-credentials/"
+    profile_name = requests.get(url, timeout=10).text
+    profile_data = requests.get(f"{url}/{profile_name}", timeout=10).json()
+    profile_data["SessionToken"] = profile_data["Token"]
 
-    return boto3.client(service_name)
+    return {var: profile_data.get(key) for var, key in VALUE_MAP.items()}
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @click.command(name="check")
 @click.argument("codenames", nargs=-1)
 @click.pass_context
 def cmd_check(ctx: Context, codenames):
     """Check for all needed files to be registered properly."""
     bucket = ctx.parent.params["bucket"]
     role_arn = ctx.parent.params["role_arn"]
-    with local_s3(bucket, role_arn) as path:
+    with local_s3(bucket, role_arn, region=ctx.parent.params["aws_region"]) as path:
         cmd = [
             "reprepro",
             "-V",
             "-b",
             path,
             "check",
         ]
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 
 @click.command(name="deleteunreferenced")
 @click.pass_context
 def cmd_deleteunreferenced(ctx: Context):
     """Remove all known files (and forget them) in the pool not marked to be needed by anything."""
     bucket = ctx.parent.params["bucket"]
     role_arn = ctx.parent.params["role_arn"]
-    with local_s3(bucket, role_arn) as path:
+    with local_s3(bucket, role_arn, region=ctx.parent.params["aws_region"]) as path:
         cmd = ["reprepro", "-V", "-b", path, "deleteunreferenced"]
         execute(cmd)
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 
 @click.command(name="dumpunreferenced")
 @click.pass_context
 def cmd_dumpunreferenced(ctx: Context):
     """Print a list of all filed believed to be in the pool, that are not known to be needed."""
     bucket = ctx.parent.params["bucket"]
     role_arn = ctx.parent.params["role_arn"]
-    with local_s3(bucket, role_arn) as path:
+    with local_s3(bucket, role_arn, region=ctx.parent.params["aws_region"]) as path:
         cmd = ["reprepro", "-V", "-b", path, "dumpunreferenced"]
         execute(cmd)
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 """
 .. topic:: ``ih-s3-reprepro includedeb``
 
     A ``ih-s3-reprepro includedeb`` subcommand.
 
     See ``ih-s3-reprepro includedeb --help`` for more details.
 """
+import sys
 
 import click
+from botocore.exceptions import BotoCoreError, ClientError
 from click import Context
 
+from infrahouse_toolkit import LOG
 from infrahouse_toolkit.cli.ih_s3_reprepro.utils import execute, repo_env
 
 
 @click.command(name="includedeb")
 @click.argument("codename")
 @click.argument("deb_file")
 @click.pass_context
 def cmd_includedeb(ctx: Context, codename, deb_file):
     """
     Include the given binary package.
 
     Include the given binary Debian package (.deb) in the specified distribution,
     applying override information and guessing all values not given and guessable.
     """
-    with repo_env(
-        ctx.parent.params["bucket"],
-        ctx.parent.params["role_arn"],
-        ctx.parent.params["gpg_key_secret_id"],
-        ctx.parent.params["gpg_passphrase_secret_id"],
-    ) as (path, gpg_home):
-        execute(["reprepro", "-V", "-b", path, "--gnupghome", gpg_home, "includedeb", codename, deb_file])
+    try:
+        with repo_env(
+            ctx.parent.params["bucket"],
+            ctx.parent.params["role_arn"],
+            ctx.parent.params["gpg_key_secret_id"],
+            ctx.parent.params["gpg_passphrase_secret_id"],
+            region=ctx.parent.params["aws_region"],
+        ) as (path, gpg_home):
+            execute(["reprepro", "-V", "-b", path, "--gnupghome", gpg_home, "includedeb", codename, deb_file])
+
+    except (ClientError, BotoCoreError) as err:
+        LOG.error(err)
+        sys.exit(1)
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,12 +16,11 @@
 @click.argument("distribution")
 @click.argument("package_name", nargs=-1)
 @click.pass_context
 def cmd_list(ctx: Context, distribution: str, package_name: str):
     """List all packages by the given name occurring in the given distribution."""
     bucket = ctx.parent.params["bucket"]
     role_arn = ctx.parent.params["role_arn"]
-    with local_s3(bucket, role_arn) as path:
-        # input("press enter")
+    with local_s3(bucket, role_arn, region=ctx.parent.params["aws_region"]) as path:
         cmd = ["reprepro", "-V", "-b", path, "list", distribution]
         cmd.extend(package_name)
         execute(cmd)
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 """
 .. topic:: ``ih-s3-reprepro remove``
 
     A ``ih-s3-reprepro remove`` subcommand.
 
     See ``ih-s3-reprepro remove --help`` for more details.
 """
+import sys
 
 import click
+from botocore.exceptions import BotoCoreError, ClientError
 from click import Context
 
+from infrahouse_toolkit import LOG
 from infrahouse_toolkit.cli.ih_s3_reprepro.utils import execute, repo_env
 
 
 @click.command(name="remove")
 @click.argument("codename")
 @click.argument("package_name")
 @click.pass_context
 def cmd_remove(ctx: Context, codename, package_name):
     """Delete  all packages in the specified distribution, that have package name listed as argument."""
-    with repo_env(
-        ctx.parent.params["bucket"],
-        ctx.parent.params["role_arn"],
-        ctx.parent.params["gpg_key_secret_id"],
-        ctx.parent.params["gpg_passphrase_secret_id"],
-    ) as (path, gpg_home):
-        execute(["reprepro", "-V", "-b", path, "--gnupghome", gpg_home, "remove", codename, package_name])
+    try:
+        with repo_env(
+            ctx.parent.params["bucket"],
+            ctx.parent.params["role_arn"],
+            ctx.parent.params["gpg_key_secret_id"],
+            ctx.parent.params["gpg_passphrase_secret_id"],
+            region=ctx.parent.params["aws_region"],
+        ) as (path, gpg_home):
+            execute(["reprepro", "-V", "-b", path, "--gnupghome", gpg_home, "remove", codename, package_name])
+
+    except (ClientError, BotoCoreError) as err:
+        LOG.error(err)
+        sys.exit(1)
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 .. topic:: ``ih-s3-reprepro set-secret-value``
 
     A ``ih-s3-reprepro set-secret-value`` subcommand.
 
     See ``ih-s3-reprepro set-secret-value --help`` for more details.
 """
+import sys
 
 import click
+from botocore.exceptions import BotoCoreError, ClientError
 from click import Context
 
 from infrahouse_toolkit import DEFAULT_OPEN_ENCODING, LOG
 from infrahouse_toolkit.cli.ih_s3_reprepro.aws import get_client
 
 
 @click.command(name="set-secret-value")
@@ -25,17 +27,22 @@
 
     \b
     ih-s3-reprepro ... set-secret-value mysecret /path/to/file_with_value
 
     if the path is omitted, a user will be prompt for the value.
     """
     role_arn = ctx.parent.params["role_arn"]
-    client = get_client("secretsmanager", role_arn=role_arn)
-    if path:
-        with open(path[0], encoding=DEFAULT_OPEN_ENCODING) as secret_value_desc:
-            value = secret_value_desc.read()
-    else:
-        value = click.prompt("Enter a secret value and press ENTER", hide_input=True)
-
-    LOG.debug("Secret value: %s", value)
-    client.put_secret_value(SecretId=secret_id, SecretString=value)
-    LOG.info("Value of %s is successfully set.", secret_id)
+    try:
+        client = get_client("secretsmanager", role_arn=role_arn, region=ctx.parent.params["aws_region"])
+        if path:
+            with open(path[0], encoding=DEFAULT_OPEN_ENCODING) as secret_value_desc:
+                value = secret_value_desc.read()
+        else:
+            value = click.prompt("Enter a secret value and press ENTER", hide_input=True)
+
+        LOG.debug("Secret value: %s", value)
+        client.put_secret_value(SecretId=secret_id, SecretString=value)
+        LOG.info("Value of %s is successfully set.", secret_id)
+
+    except (ClientError, BotoCoreError) as err:
+        LOG.error(err)
+        sys.exit(1)
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
     with TemporaryDirectory() as path:
         LOG.debug("GPG home is %s", path)
         yield path
 
 
 @contextmanager
-def gpg(secret_key=None, role_arn=None, secret_passphrase=None) -> str:
+def gpg(secret_key=None, role_arn=None, secret_passphrase=None, region: str = None) -> str:
     """
     Prepare GPG keyring and yield path to it.
     If no function arguments are specified, it will return the default path ~/.gnupg.
 
     If secret_key is specified, the function will pull the GPG key from this secret.
     Optionally, it will assume a role, if given.
 
@@ -44,21 +44,23 @@
 
     :param secret_key: AWS secret id (name or ARN) with a GPG private key.
     :type secret_key: str
     :param role_arn: If specified, assume this role in AWS client.
     :type role_arn: str
     :param secret_passphrase: AWS secret id (name or ARN) with a passphrase for the GPG private key.
     :type secret_passphrase: str
+    :param region: AWS region name.
+    :type region: str
     :return: Path to GPG homedir.
     :rtype: str
     """
     if secret_key:
         LOG.debug("Reading GPG key from %s", secret_key)
         try:
-            secrets_manager = get_client("secretsmanager", role_arn=role_arn)
+            secrets_manager = get_client("secretsmanager", role_arn=role_arn, region=region)
             key = secrets_manager.get_secret_value(SecretId=secret_key)["SecretString"]
         except ClientError as err:
             LOG.error(err)
             if err.response["Error"]["Code"] == "ResourceNotFoundException":
                 LOG.error("Make sure that you set a secret value to the key %s:", secret_key)
                 LOG.error("ih-s3-reprepro ... set-secret-value %s /path/to/file/with/%s-value", secret_key, secret_key)
             raise
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 from subprocess import CalledProcessError, Popen, check_call
 from tempfile import TemporaryDirectory
 from time import sleep, time
 
 import boto3
 
 from infrahouse_toolkit import DEFAULT_OPEN_ENCODING, LOG
-from infrahouse_toolkit.cli.ih_s3_reprepro.aws import assume_role
+from infrahouse_toolkit.cli.ih_s3_reprepro.aws import (
+    assume_role,
+    get_credentials_from_profile,
+)
 from infrahouse_toolkit.cli.ih_s3_reprepro.gpg import gpg
 
 DEPENDENCIES = ["reprepro", "gpg", "s3fs"]
 
 
 def check_dependencies(binaries: list):
     """
@@ -36,36 +39,41 @@
                 check_call([dep, "--help"], stdout=devnull, stderr=devnull)
         except FileNotFoundError:
             LOG.error("Looks like %s is not installed", dep)
             LOG.info("Try installing it by \n\n\tapt-get install %s\n", dep)
             sys.exit(1)
 
 
-def mount_s3(bucket: str, path: str, role_arn: str = None):
+def mount_s3(bucket: str, path: str, role_arn: str = None, region: str = None):
     """
     Mount an S3 bucket at a path.
 
     :param bucket: AWS S3 bucket name.
     :type bucket: str
     :param path: Local filesystem path name.
     :type path: str
     :param role_arn: Assume role if specified.
+    :param region: AWS region name.
+    :type region: str
     """
     env = {}
     cmd = ["s3fs", bucket, path, "-o", f"uid={getuid()}", "-o", f"gid={getgid()}"]
     if role_arn:
         env = assume_role(role_arn)
         sts = boto3.client(
             "sts",
             aws_access_key_id=env["AWS_ACCESS_KEY_ID"],
             aws_secret_access_key=env["AWS_SECRET_ACCESS_KEY"],
             aws_session_token=env["AWS_SESSION_TOKEN"],
+            region_name=region,
         )
         response = sts.get_caller_identity()
         LOG.debug("Assumed role: %s", response)
+    else:
+        env = get_credentials_from_profile()
 
     LOG.debug("To reproduce environment: \n%s", "\n".join([f'export {key}="{value}"' for key, value in env.items()]))
     LOG.debug("Command to debug: mkdir -p %s; %s -o dbglevel=info -f -o curldbg", path, " ".join(cmd))
     execute(cmd, env=env)
 
 
 def umount_s3(path: str):
@@ -79,44 +87,42 @@
         check_call(["umount", path])
     except CalledProcessError as err:
         LOG.error(err)
         sys.exit(1)
 
 
 @contextmanager
-def local_s3(bucket, role_arn=None, retry_timeout=60) -> str:
+def local_s3(bucket, role_arn=None, retry_timeout=60, region=None) -> str:
     """
     Mount an S3 bucket locally and return a mount point.
 
     :param bucket: AWS S3 bucket name.
     :type bucket: str
     :param role_arn: Assume role if specified.
     :type role_arn: str
     :param retry_timeout: How many second to keep trying to mount the bucket.
     :type retry_timeout: int
+    :param region: AWS region name.
+    :type region: str
     :return: Local filesystem path where the S3 bucket is mounted at.
     """
     with TemporaryDirectory() as mnt_dir:
         try:
             now = time()
             timeout = now + retry_timeout
             while True:
-                mount_s3(bucket, mnt_dir, role_arn=role_arn)
+                mount_s3(bucket, mnt_dir, role_arn=role_arn, region=region)
                 if osp.exists(osp.join(mnt_dir, "conf/distributions")):
                     break
                 LOG.warning("Waiting until s3://%s is mounted at %s", bucket, mnt_dir)
                 sleep(1)
                 if time() > timeout:
                     raise RuntimeError(f"s3://{bucket} is not mounted after {retry_timeout} seconds")
             yield mnt_dir
 
-        except Exception as err:
-            LOG.exception(err)
-            raise
-
         finally:
             umount_s3(mnt_dir)
 
 
 def execute(cmd: list, env: dict = None):
     """
     Execute a command and exit with 1 if the command raises CalledProcessError.
@@ -140,29 +146,31 @@
 
     except CalledProcessError as err:
         LOG.exception(err)
         sys.exit(1)
 
 
 @contextmanager
-def repo_env(bucket, role_arn, gpg_key_secret_id, gpg_passphrase_secret_id):
+def repo_env(bucket, role_arn, gpg_key_secret_id, gpg_passphrase_secret_id, region=None):
     """
     Prepare locally a repo and GPG so "reprepro" can manage it.
 
     :param bucket: AWS S3 bucket with the repo. The repo must be in the root.
     :type bucket: str
     :param role_arn: Optional role ARN. If specified, AWS client will assume it.
     :type role_arn: str
     :param gpg_key_secret_id: AWS secretsmanager secret (name or ARN) that stores the private GPG key,
         needed by ``reprepro`` to sign the repo.
     :type gpg_key_secret_id: str
     :param gpg_passphrase_secret_id: AWS secretsmanager secret (name or ARN) that stores a passphrase for
         the private GPG key. Note, it's not the passphrase itself, it's a secret that stores it.
     :type gpg_passphrase_secret_id: str
+    :param region: AWS region name.
+    :type region: str
     :return: A tuple with two strings: Local filesystem directory with a mounted S3 bucket
         and GPG home directory.
     """
-    with local_s3(bucket, role_arn) as path:
+    with local_s3(bucket, role_arn, region=region) as path:
         with gpg(
-            secret_key=gpg_key_secret_id, role_arn=role_arn, secret_passphrase=gpg_passphrase_secret_id
+            secret_key=gpg_key_secret_id, role_arn=role_arn, secret_passphrase=gpg_passphrase_secret_id, region=region
         ) as gpg_home:
             yield path, gpg_home
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/lib.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/lib.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/conftest.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/logging.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/__init__.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/s3backend.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/s3backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tfbackend.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/backends/tfbackend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/githubpr.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/githubpr.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/status.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/status.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_eq.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_eq.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_metadata.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/test_parse_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit/terraform/tests/test_parse_plan.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/PKG-INFO` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.7.0
+Version: 1.7.1
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/SOURCES.txt` & `infrahouse-toolkit-1.7.1/infrahouse_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.7.0/setup.py` & `infrahouse-toolkit-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     include_package_data=True,
     keywords="infrahouse-toolkit",
     name="infrahouse-toolkit",
     packages=find_packages(include=["infrahouse_toolkit", "infrahouse_toolkit.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/infrahouse/infrahouse-toolkit",
-    version="1.7.0",
+    version="1.7.1",
     zip_safe=False,
 )
```

