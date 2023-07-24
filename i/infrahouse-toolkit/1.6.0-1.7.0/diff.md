# Comparing `tmp/infrahouse-toolkit-1.6.0.tar.gz` & `tmp/infrahouse-toolkit-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahouse-toolkit-1.6.0.tar", last modified: Mon Jul 24 05:04:42 2023, max compression
+gzip compressed data, was "infrahouse-toolkit-1.7.0.tar", last modified: Mon Jul 24 22:49:32 2023, max compression
```

## Comparing `infrahouse-toolkit-1.6.0.tar` & `infrahouse-toolkit-1.7.0.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.300160 infrahouse-toolkit-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-24 05:04:42.300160 infrahouse-toolkit-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.268159 infrahouse-toolkit-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.tests.status.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.272159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.276159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.276159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.280159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.280159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.280159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.280159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.280159 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.296160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.296160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.296160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.296160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/s3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.296160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.300160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/githubpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.300160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.300160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/github_pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.300160 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:42.276159 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-24 05:04:42.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-24 05:04:42.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:04:42.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 05:04:42.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:04:32.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 05:04:42.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 05:04:42.000000 infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 05:04:42.300160 infrahouse-toolkit-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 05:03:53.000000 infrahouse-toolkit-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.248200 infrahouse-toolkit-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.248200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.252200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.256200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.256200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.260200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.260200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/s3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.260200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.264200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/githubpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.264200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.264200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:49:32.248200 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:49:22.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 22:49:32.000000 infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 22:49:32.268200 infrahouse-toolkit-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 22:48:52.000000 infrahouse-toolkit-1.7.0/setup.py
```

### Comparing `infrahouse-toolkit-1.6.0/CONTRIBUTING.rst` & `infrahouse-toolkit-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/LICENSE` & `infrahouse-toolkit-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/PKG-INFO` & `infrahouse-toolkit-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.6.0
+Version: 1.7.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.6.0/README.rst` & `infrahouse-toolkit-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/Makefile` & `infrahouse-toolkit-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/conf.py` & `infrahouse-toolkit-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.cli.tests.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.cli.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.backends.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.backends.tests.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.tests.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/infrahouse_toolkit.terraform.tests.status.rst` & `infrahouse-toolkit-1.7.0/docs/infrahouse_toolkit.terraform.tests.status.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/installation.rst` & `infrahouse-toolkit-1.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/docs/usage.rst` & `infrahouse-toolkit-1.7.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,39 +3,45 @@
 
     AWS helper functions.
 """
 
 import boto3
 from botocore.exceptions import ClientError
 
+from infrahouse_toolkit import LOG
+
 
 def assume_role(role_arn) -> dict:
     """
     Assume a given role and return a dictionary with credentials.
 
     :param role_arn: Role to be assumed.
     :type role_arn: str
     :return: A dictionary with three keys: AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY, and
     """
+    value_map = {
+        "AWS_ACCESS_KEY_ID": "AccessKeyId",
+        "AWS_SECRET_ACCESS_KEY": "SecretAccessKey",
+        "AWS_SESSION_TOKEN": "SessionToken",
+        # These are old s3.fs options
+        # Soon they will be deprecated
+        # https://github.com/s3fs-fuse/s3fs-fuse/pull/1729
+        "AWSACCESSKEYID": "AccessKeyId",
+        "AWSSECRETACCESSKEY": "SecretAccessKey",
+        "AWSSESSIONTOKEN": "SessionToken",
+    }
     try:
+        LOG.debug("Assuming role %s", role_arn)
         client = boto3.client("sts")
         response = client.assume_role(RoleArn=role_arn, RoleSessionName="ih-s3-reprepro-s3fs")
-        return {
-            "AWS_ACCESS_KEY_ID": response["Credentials"]["AccessKeyId"],
-            "AWS_SECRET_ACCESS_KEY": response["Credentials"]["SecretAccessKey"],
-            "AWS_SESSION_TOKEN": response["Credentials"]["SessionToken"],
-            # These are old s3.fs options
-            # Soon they will be deprecated
-            # https://github.com/s3fs-fuse/s3fs-fuse/pull/1729
-            "AWSACCESSKEYID": response["Credentials"]["AccessKeyId"],
-            "AWSSECRETACCESSKEY": response["Credentials"]["SecretAccessKey"],
-            "AWSSESSIONTOKEN": response["Credentials"]["SessionToken"],
-        }
+        LOG.debug("Got credentials %r", response["Credentials"])
+        return {var: response["Credentials"].get(key) for var, key in value_map.items()}
     except ClientError as err:
-        print(err)
+        LOG.error(err)
+        LOG.debug("To revert environment:\n%s", "\n".join([f"unset {key}" for key in value_map]))
         raise
 
 
 def get_client(service_name, role_arn=None, session_name=__name__):
     """
     Get an AWS service client assuming a role if specified.
 
@@ -52,10 +58,13 @@
         sts = boto3.client("sts")
         aws_iam_role = sts.assume_role(RoleArn=role_arn, RoleSessionName=session_name)
         session = boto3.Session(
             aws_access_key_id=aws_iam_role["Credentials"]["AccessKeyId"],
             aws_secret_access_key=aws_iam_role["Credentials"]["SecretAccessKey"],
             aws_session_token=aws_iam_role["Credentials"]["SessionToken"],
         )
+        sts = session.client("sts")
+        response = sts.get_caller_identity()
+        LOG.debug("Assumed role: %s", response)
         return session.client(service_name)
 
     return boto3.client(service_name)
```

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 """
 
 from contextlib import contextmanager
 from os import path as osp
 from subprocess import Popen
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 
-from infrahouse_toolkit import DEFAULT_ENCODING, DEFAULT_OPEN_ENCODING
+from botocore.exceptions import ClientError
+
+from infrahouse_toolkit import DEFAULT_ENCODING, DEFAULT_OPEN_ENCODING, LOG
 from infrahouse_toolkit.cli.ih_s3_reprepro.aws import get_client
 
 
 @contextmanager
 def gpg_home() -> str:
     """
     :return: GPG home directory
     """
     with TemporaryDirectory() as path:
+        LOG.debug("GPG home is %s", path)
         yield path
 
 
 @contextmanager
 def gpg(secret_key=None, role_arn=None, secret_passphrase=None) -> str:
     """
     Prepare GPG keyring and yield path to it.
@@ -45,33 +48,43 @@
     :type role_arn: str
     :param secret_passphrase: AWS secret id (name or ARN) with a passphrase for the GPG private key.
     :type secret_passphrase: str
     :return: Path to GPG homedir.
     :rtype: str
     """
     if secret_key:
-        secrets_manager = get_client("secretsmanager", role_arn=role_arn)
-        key = secrets_manager.get_secret_value(SecretId=secret_key)["SecretString"]
+        LOG.debug("Reading GPG key from %s", secret_key)
+        try:
+            secrets_manager = get_client("secretsmanager", role_arn=role_arn)
+            key = secrets_manager.get_secret_value(SecretId=secret_key)["SecretString"]
+        except ClientError as err:
+            LOG.error(err)
+            if err.response["Error"]["Code"] == "ResourceNotFoundException":
+                LOG.error("Make sure that you set a secret value to the key %s:", secret_key)
+                LOG.error("ih-s3-reprepro ... set-secret-value %s /path/to/file/with/%s-value", secret_key, secret_key)
+            raise
 
         with gpg_home() as homedir, NamedTemporaryFile() as gpg_key_desc, NamedTemporaryFile() as gpg_passphrase_desc:
             gpg_key_desc.write(key.encode(DEFAULT_ENCODING))
             gpg_key_desc.flush()
 
             cmd = ["gpg", "--homedir", homedir]
 
             if secret_passphrase:
+                LOG.debug("Reading GPG key passphrase from %s", secret_passphrase)
                 passphrase = secrets_manager.get_secret_value(SecretId=secret_passphrase)["SecretString"]
                 gpg_passphrase_desc.write(passphrase.encode(DEFAULT_ENCODING))
                 gpg_passphrase_desc.flush()
                 write_gpg_cong(
                     osp.join(homedir, "gpg.conf"),
                     {"batch": None, "passphrase-file": gpg_passphrase_desc.name, "pinentry-mode": "loopback"},
                 )
 
             cmd.extend(["--import", gpg_key_desc.name])
+            LOG.debug("Executing: %s", " ".join(cmd))
             proc = Popen(cmd)
             proc.communicate()
             yield homedir
     else:
         yield osp.expanduser("~/.gnupg")
 
 
@@ -80,13 +93,14 @@
     Prepare GPG config file.
 
     :param path: Path name to the GPG config file.
     :type path: str
     :param options: A dictionary with options. For one word options the key value is None.
     :type options: dict
     """
+    LOG.debug("Saving GPG config in %s", path)
     with open(path, "w", encoding=DEFAULT_OPEN_ENCODING) as gpg_conf_desc:
         for key, value in options.items():
             gpg_conf_desc.write(f"{key}")
             if value:
                 gpg_conf_desc.write(f" {value}")
             gpg_conf_desc.write("\n")
```

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """
 .. topic:: ``utils.py``
 
     Various helper functions.
 """
-
+import json
 import sys
 from contextlib import contextmanager
 from os import getgid, getuid
+from os import path as osp
 from subprocess import CalledProcessError, Popen, check_call
 from tempfile import TemporaryDirectory
+from time import sleep, time
+
+import boto3
 
-from infrahouse_toolkit import DEFAULT_OPEN_ENCODING
+from infrahouse_toolkit import DEFAULT_OPEN_ENCODING, LOG
 from infrahouse_toolkit.cli.ih_s3_reprepro.aws import assume_role
 from infrahouse_toolkit.cli.ih_s3_reprepro.gpg import gpg
 
 DEPENDENCIES = ["reprepro", "gpg", "s3fs"]
 
 
 def check_dependencies(binaries: list):
@@ -24,18 +28,19 @@
 
     :param binaries: Dependency commands. List of strings.
     :type binaries: list
     """
     for dep in binaries:
         try:
             with open("/dev/null", "w", encoding=DEFAULT_OPEN_ENCODING) as devnull:
+                LOG.debug("Checking if %s is installed.", dep)
                 check_call([dep, "--help"], stdout=devnull, stderr=devnull)
         except FileNotFoundError:
-            print(f"Looks like {dep} is not installed")
-            print(f"Try installing it by \n\n\tapt-get install {dep}\n")
+            LOG.error("Looks like %s is not installed", dep)
+            LOG.info("Try installing it by \n\n\tapt-get install %s\n", dep)
             sys.exit(1)
 
 
 def mount_s3(bucket: str, path: str, role_arn: str = None):
     """
     Mount an S3 bucket at a path.
 
@@ -45,72 +50,100 @@
     :type path: str
     :param role_arn: Assume role if specified.
     """
     env = {}
     cmd = ["s3fs", bucket, path, "-o", f"uid={getuid()}", "-o", f"gid={getgid()}"]
     if role_arn:
         env = assume_role(role_arn)
-    check_call(cmd, env=env)
+        sts = boto3.client(
+            "sts",
+            aws_access_key_id=env["AWS_ACCESS_KEY_ID"],
+            aws_secret_access_key=env["AWS_SECRET_ACCESS_KEY"],
+            aws_session_token=env["AWS_SESSION_TOKEN"],
+        )
+        response = sts.get_caller_identity()
+        LOG.debug("Assumed role: %s", response)
+
+    LOG.debug("To reproduce environment: \n%s", "\n".join([f'export {key}="{value}"' for key, value in env.items()]))
+    LOG.debug("Command to debug: mkdir -p %s; %s -o dbglevel=info -f -o curldbg", path, " ".join(cmd))
+    execute(cmd, env=env)
 
 
 def umount_s3(path: str):
     """
     Unmount an S3 bucket at a path.
 
     :param path: Local filesystem path name where the S3 bucket is mounted at.
     :type path: str
     """
     try:
         check_call(["umount", path])
-    except CalledProcessError:
+    except CalledProcessError as err:
+        LOG.error(err)
         sys.exit(1)
 
 
 @contextmanager
-def local_s3(bucket, role_arn=None) -> str:
+def local_s3(bucket, role_arn=None, retry_timeout=60) -> str:
     """
     Mount an S3 bucket locally and return a mount point.
 
     :param bucket: AWS S3 bucket name.
     :type bucket: str
     :param role_arn: Assume role if specified.
     :type role_arn: str
+    :param retry_timeout: How many second to keep trying to mount the bucket.
+    :type retry_timeout: int
     :return: Local filesystem path where the S3 bucket is mounted at.
     """
     with TemporaryDirectory() as mnt_dir:
         try:
-            mount_s3(bucket, mnt_dir, role_arn=role_arn)
+            now = time()
+            timeout = now + retry_timeout
+            while True:
+                mount_s3(bucket, mnt_dir, role_arn=role_arn)
+                if osp.exists(osp.join(mnt_dir, "conf/distributions")):
+                    break
+                LOG.warning("Waiting until s3://%s is mounted at %s", bucket, mnt_dir)
+                sleep(1)
+                if time() > timeout:
+                    raise RuntimeError(f"s3://{bucket} is not mounted after {retry_timeout} seconds")
             yield mnt_dir
 
         except Exception as err:
-            print(type(err), err)
+            LOG.exception(err)
             raise
 
         finally:
             umount_s3(mnt_dir)
 
 
-def execute(cmd: list):
+def execute(cmd: list, env: dict = None):
     """
     Execute a command and exit with 1 if the command raises CalledProcessError.
 
     :param cmd: A command to execute. It's passed to check_call() and therefore must be a list.
     :type cmd: list
+    :param env: Pass a dictionary with environment
+    :type env: dict
     """
     try:
-        with Popen(cmd) as proc:
+        LOG.debug("Executing %s", " ".join(cmd))
+        LOG.debug("Environment: %s", json.dumps(env, indent=4) if env else "None")
+        with Popen(cmd, env=env) as proc:
             try:
                 proc.communicate()
             except KeyboardInterrupt:
-                print("Exiting on <ctrl>+c")
+                LOG.info("Exiting on <ctrl>+c")
                 proc.terminate()
-                print(f"Process {cmd[0]} is terminated. Waiting for it to exit.")
+                LOG.info("Process %s is terminated. Waiting for it to exit.", cmd[0])
                 proc.wait(60)
 
-    except CalledProcessError:
+    except CalledProcessError as err:
+        LOG.exception(err)
         sys.exit(1)
 
 
 @contextmanager
 def repo_env(bucket, role_arn, gpg_key_secret_id, gpg_passphrase_secret_id):
     """
     Prepare locally a repo and GPG so "reprepro" can manage it.
```

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/lib.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/lib.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/cli/tests/conftest.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/logging.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/__init__.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/s3backend.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/s3backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/backends/tfbackend.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/backends/tfbackend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/githubpr.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/githubpr.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/status.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/status.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_eq.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_eq.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/PKG-INFO` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.6.0
+Version: 1.7.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.6.0/infrahouse_toolkit.egg-info/SOURCES.txt` & `infrahouse-toolkit-1.7.0/infrahouse_toolkit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -54,17 +54,19 @@
 infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
 infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
 infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
 infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
 infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
 infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
 infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
+infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
 infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
 infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
 infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
+infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
 infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
 infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
 infrahouse_toolkit/cli/tests/__init__.py
 infrahouse_toolkit/cli/tests/conftest.py
 infrahouse_toolkit/cli/tests/test_get_bucket.py
 infrahouse_toolkit/terraform/__init__.py
 infrahouse_toolkit/terraform/exceptions.py
```

### Comparing `infrahouse-toolkit-1.6.0/setup.py` & `infrahouse-toolkit-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     include_package_data=True,
     keywords="infrahouse-toolkit",
     name="infrahouse-toolkit",
     packages=find_packages(include=["infrahouse_toolkit", "infrahouse_toolkit.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/infrahouse/infrahouse-toolkit",
-    version="1.6.0",
+    version="1.7.0",
     zip_safe=False,
 )
```

