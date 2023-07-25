# Comparing `tmp/sagemaker-ssh-helper-1.9.1.tar.gz` & `tmp/sagemaker-ssh-helper-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-ssh-helper-1.9.1.tar", last modified: Fri Jan 20 16:15:55 2023, max compression
+gzip compressed data, was "sagemaker-ssh-helper-2.0.0.tar", last modified: Tue Jul 25 06:54:45 2023, max compression
```

## Comparing `sagemaker-ssh-helper-1.9.1.tar` & `sagemaker-ssh-helper-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,78 @@
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-01-20 16:15:55.586350 sagemaker-ssh-helper-1.9.1/
--rw-r--r--   0 ivankh     (504) staff       (20)      925 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/LICENSE
--rw-r--r--   0 ivankh     (504) staff       (20)     1270 2023-01-20 16:15:55.586144 sagemaker-ssh-helper-1.9.1/PKG-INFO
--rw-r--r--   0 ivankh     (504) staff       (20)    33322 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/README.md
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-01-20 16:15:55.584808 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/
--rw-r--r--   0 ivankh     (504) staff       (20)      684 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/__init__.py
--rw-r--r--   0 ivankh     (504) staff       (20)     4749 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py
--rw-r--r--   0 ivankh     (504) staff       (20)      435 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/env.py
--rw-r--r--   0 ivankh     (504) staff       (20)     5500 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/log.py
--rw-r--r--   0 ivankh     (504) staff       (20)     4143 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/proxy.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2409 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-connect-ssh-proxy
--rw-r--r--   0 ivankh     (504) staff       (20)     2370 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-helper-functions
--rw-r--r--   0 ivankh     (504) staff       (20)     1482 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-init-ssm
--rw-r--r--   0 ivankh     (504) staff       (20)      129 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-install-force
--rw-r--r--   0 ivankh     (504) staff       (20)     1297 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-ide
--rw-r--r--   0 ivankh     (504) staff       (20)      881 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-inference
--rw-r--r--   0 ivankh     (504) staff       (20)      879 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-processing
--rw-r--r--   0 ivankh     (504) staff       (20)      875 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-training
--rw-r--r--   0 ivankh     (504) staff       (20)      879 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-transform
--rwxr-xr-x   0 ivankh     (504) staff       (20)      701 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-start-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)      301 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-save-env
--rw-r--r--   0 ivankh     (504) staff       (20)     1137 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-setup-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)     5612 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-ssh-ide
--rw-r--r--   0 ivankh     (504) staff       (20)     1372 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-start-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)      672 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-wait
--rw-r--r--   0 ivankh     (504) staff       (20)    14088 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/wrapper.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-01-20 16:15:55.585869 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/
--rw-r--r--   0 ivankh     (504) staff       (20)     1270 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/PKG-INFO
--rw-r--r--   0 ivankh     (504) staff       (20)     1030 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/SOURCES.txt
--rw-r--r--   0 ivankh     (504) staff       (20)        1 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/dependency_links.txt
--rw-r--r--   0 ivankh     (504) staff       (20)      274 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/requires.txt
--rw-r--r--   0 ivankh     (504) staff       (20)       21 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/top_level.txt
--rw-r--r--   0 ivankh     (504) staff       (20)       38 2023-01-20 16:15:55.586412 sagemaker-ssh-helper-1.9.1/setup.cfg
--rw-r--r--   0 ivankh     (504) staff       (20)     2916 2023-01-20 16:15:34.000000 sagemaker-ssh-helper-1.9.1/setup.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.782582 sagemaker-ssh-helper-2.0.0/
+-rw-r--r--   0 ivankh     (504) staff       (20)      925 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/LICENSE
+-rw-r--r--   0 ivankh     (504) staff       (20)     1493 2023-07-25 06:54:45.782389 sagemaker-ssh-helper-2.0.0/PKG-INFO
+-rw-r--r--   0 ivankh     (504) staff       (20)    41547 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/README.md
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.770284 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/
+-rw-r--r--   0 ivankh     (504) staff       (20)     2715 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/__init__.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     1038 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/aws.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.772324 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/
+-rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/__init__.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      219 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/advanced_tier_app.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.773608 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm/
+-rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm/__init__.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      284 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm/advanced_tier_lambda.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     9092 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     9166 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack_tests.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     1481 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm/ssm_advanced_tier_stack.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      677 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm/trust_relationship_lambda.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      185 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/iam_ssm_app.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.774596 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/low_gpu/
+-rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/low_gpu/__init__.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     3188 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     2551 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda_stack.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      207 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/low_gpu_lambda_app.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.774849 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/tests/
+-rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/tests/__init__.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.775055 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/tests/unit/
+-rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/tests/unit/__init__.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      207 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/cdk/tests_app.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     2292 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     2242 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/detached_sagemaker.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      761 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/env.py
+-rw-r--r--   0 ivankh     (504) staff       (20)    12110 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/ide.py
+-rw-r--r--   0 ivankh     (504) staff       (20)    11149 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/log.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     7083 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/manager.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     6816 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/proxy.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     4328 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-connect-ssh-proxy
+-rw-r--r--   0 ivankh     (504) staff       (20)     5373 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-helper-functions
+-rw-r--r--   0 ivankh     (504) staff       (20)     2456 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-init-ssm
+-rw-r--r--   0 ivankh     (504) staff       (20)      451 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-configure
+-rw-r--r--   0 ivankh     (504) staff       (20)     3061 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-ide
+-rw-r--r--   0 ivankh     (504) staff       (20)      930 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-inference
+-rw-r--r--   0 ivankh     (504) staff       (20)      841 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-notebook
+-rw-r--r--   0 ivankh     (504) staff       (20)      945 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-processing
+-rw-r--r--   0 ivankh     (504) staff       (20)      955 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-training
+-rw-r--r--   0 ivankh     (504) staff       (20)      945 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-transform
+-rwxr-xr-x   0 ivankh     (504) staff       (20)      996 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-start-ssh
+-rw-r--r--   0 ivankh     (504) staff       (20)      966 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-save-env
+-rw-r--r--   0 ivankh     (504) staff       (20)     4608 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-setup-ssh
+-rw-r--r--   0 ivankh     (504) staff       (20)     9167 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-ssh-ide
+-rw-r--r--   0 ivankh     (504) staff       (20)     1494 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-wait
+-rw-r--r--   0 ivankh     (504) staff       (20)    23937 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/wrapper.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.771387 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper.egg-info/
+-rw-r--r--   0 ivankh     (504) staff       (20)     1493 2023-07-25 06:54:45.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper.egg-info/PKG-INFO
+-rw-r--r--   0 ivankh     (504) staff       (20)     2401 2023-07-25 06:54:45.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)        1 2023-07-25 06:54:45.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)      475 2023-07-25 06:54:45.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper.egg-info/requires.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)       21 2023-07-25 06:54:45.000000 sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper.egg-info/top_level.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)       38 2023-07-25 06:54:45.782635 sagemaker-ssh-helper-2.0.0/setup.cfg
+-rw-r--r--   0 ivankh     (504) staff       (20)     3477 2023-07-25 06:45:10.000000 sagemaker-ssh-helper-2.0.0/setup.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-07-25 06:54:45.781787 sagemaker-ssh-helper-2.0.0/tests/
+-rw-r--r--   0 ivankh     (504) staff       (20)     2132 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_attach.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     4565 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_batch_inference.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     8134 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_clean_core.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      727 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_deregister_instances.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     4021 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_distributed.py
+-rw-r--r--   0 ivankh     (504) staff       (20)    18171 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_end_to_end.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     2376 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_environment.py
+-rw-r--r--   0 ivankh     (504) staff       (20)    28388 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_frameworks.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     9706 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_functions.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     3630 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_hpo.py
+-rw-r--r--   0 ivankh     (504) staff       (20)    13623 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_ide.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     2620 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_inference_registry.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     1732 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_local.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     4926 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_manual.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     5256 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_remote_debug_training.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     6636 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_ssm_manager.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     1091 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_util.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      992 2023-07-25 06:41:39.000000 sagemaker-ssh-helper-2.0.0/tests/test_validation.py
```

### Comparing `sagemaker-ssh-helper-1.9.1/LICENSE` & `sagemaker-ssh-helper-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.1/PKG-INFO` & `sagemaker-ssh-helper-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: sagemaker-ssh-helper
-Version: 1.9.1
-Summary: A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH
+Version: 2.0.0
+Summary: A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH (Secure Shell)
 Home-page: https://github.com/aws-samples/sagemaker-ssh-helper
 Author: Amazon Web Services
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: cdk
 Provides-Extra: test
-Provides-Extra: test-macos
+Provides-Extra: dev
+Provides-Extra: dev-macos
 License-File: LICENSE
 
-SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, remote debugging, and advanced troubleshooting.
+SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, remote debugging, and advanced troubleshooting, also known as "SSH into SageMaker".
 
-For the full description see [README.md](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/README.md).
+For the documentation, see the repo [https://github.com/aws-samples/sagemaker-ssh-helper/](https://github.com/aws-samples/sagemaker-ssh-helper/).
```

### Comparing `sagemaker-ssh-helper-1.9.1/README.md` & `sagemaker-ssh-helper-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 # SageMaker SSH Helper
 
 [![Latest Version](https://img.shields.io/pypi/v/sagemaker-ssh-helper.svg)](https://pypi.python.org/pypi/sagemaker-ssh-helper)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/sagemaker-ssh-helper.svg)](https://pypi.python.org/pypi/sagemaker-ssh-helper)
 [![License](https://img.shields.io/github/license/aws-samples/sagemaker-ssh-helper.svg)](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/LICENSE)
 
-SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, 
+SageMaker SSH Helper is an "army-knife" library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, 
 realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, 
 remote debugging, and advanced troubleshooting.
 
-The two most common scenarios for the library, also known as "SSH into SageMaker", are:
-1. Open a terminal session into a container running in SageMaker to diagnose a stuck training job, use CLI commands 
+Three most common asks that motivated to create the library, sometimes referred as "SSH into SageMaker", are:
+1. A terminal session into a container running in SageMaker to diagnose a stuck training job, use CLI commands 
 like nvidia-smi, or iteratively fix and re-execute your training script within seconds. 
-2. Remote debug a code running in SageMaker from your local favorite IDE like 
+2. Remote debugging of a code running in SageMaker from your local favorite IDE like 
 PyCharm Professional Edition or Visual Studio Code.
+3. Port forwarding to access diagnostic tools running inside SageMaker, e.g., Dask dashboard, TensorBoard or Spark Web UI.
 
-Other scenarios include but not limited to connecting to a remote Jupyter Notebook in SageMaker Studio from your IDE, connect with your browser to a TensorBoard process running in the cloud, or start a VNC session to SageMaker Studio to run GUI apps.  
-
-Also see our [Frequently Asked Questions](FAQ.md), especially if you're using Windows on your local machine.
+Other asks include but not limited to connecting to a remote Jupyter Notebook in SageMaker Studio from your IDE, or start a VNC session to SageMaker Studio to run GUI apps.  
 
 ## How it works
-SageMaker SSH helper uses AWS Systems Manager (SSM) Session Manager, to register the SageMaker container in SSM, followed 
-by creating an SSM session between your client machine and the SageMaker container. Then you can SSH into SageMaker by creating an SSH connection 
-on top of the SSM session, that allows opening a Linux shell, and/or configuring bidirectional SSH port forwarding to 
-enable applications like remote development/debugging/desktop, and others.
+SageMaker SSH helper uses AWS Systems Manager (SSM) Session Manager, to register the SageMaker container in SSM, followed by creating an SSM session between your client machine and the SageMaker container. Then you can "SSH into SageMaker" by creating an SSH (Secure Shell) connection on top of the SSM session, that allows opening a Linux shell and configuring bidirectional SSH port forwarding to run applications like remote development, debugging, desktop GUI, and others.
+
+![Screenshot](images/high-level-architecture.png)
 
-![Screenshot](images/layers.png)
+Once you become familiar with the library, check the [Flow Diagrams](Flow_Diagrams.md) of the common use cases. 
 
-See detailed architecture diagrams of the complete flow of participating components 
-in [Training Diagram](Flows.md), and [IDE integration with SageMaker Studio diagram](Flows_IDE.md).
+Also make sure you looked at our [Frequently Asked Questions](FAQ.md).
 
 ## Getting started
 
-To get started, your AWS system administrator must set up needed IAM and SSM configuration in your AWS account as shown 
+To get started, your AWS system administrator must configure IAM and SSM in your AWS account as shown 
 in [Setting up your AWS account with IAM and SSM configuration](IAM_SSM_Setup.md).
 
 > **Note**: This solution is a sample AWS content. You should not use this content in your production accounts, in a production 
 > environment or on production or other critical data. If you plan to use the solution in production, please, carefully review it with your security team. 
 > You are responsible for testing, securing, and optimizing the sample content 
 > as appropriate for production grade use based on your specific business requirements, including any quality control 
 practices and standards.
 
 
 ## Use Cases
 SageMaker SSH Helper supports a variety of use cases:
-- [Connecting to SageMaker training jobs with SSM](#training) - open a shell to the training job to examine its file systems,
-monitor resources, produce thread-dumps for stuck jobs, and interactively run your train script.
+- [Connecting to SageMaker training jobs with SSM](#training) - open a shell to a single- or multi-node training job to examine its file systems,
+monitor resources, produce thread-dumps for stuck jobs, and interactively run your train script
 - [Connecting to SageMaker inference endpoints with SSM](#inference)
 - [Connecting to SageMaker batch transform jobs](#batch-transform)
 - [Connecting to SageMaker processing jobs](#processing)  
-- [Remote debugging with PyCharm Debug Server over SSH](#pycharm-debug-server)  
-- [Remote code execution with PyCharm / VSCode over SSH](#remote-interpreter)
-- [Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode](#studio)  
+- [Forwarding TCP ports over SSH tunnel](#port-forwarding) - to access remote apps like Dask or Streamlit
+- [Remote debugging with PyCharm Debug Server over SSH](#pycharm-debug-server) - let SageMaker run your code that connects to PyCharm, to start line-by-line debugging with [PyDev.Debugger](https://pypi.org/project/pydevd-pycharm/), a.k.a. pydevd
+- [Remote code execution with PyCharm / VSCode over SSH](#remote-interpreter) - let PyCharm run or debug your code line-by-line inside SageMaker container with SSH interpreter
+- [Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode](#studio) - iterate fast on a single node at early stages of development without submitting SageMaker jobs
+- [Web VNC](#web-vnc) - run any IDE or tool in a browser though [AWS Jupyter Proxy](https://github.com/aws/aws-jupyter-proxy) extension
 
 If you want to add a new use case or a feature, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## <a name="training"></a>Connecting to SageMaker training jobs with SSM
 
 [![Download Demo (.mov)](https://user-images.githubusercontent.com/87804596/205893540-d7a08259-94b3-48f2-b96e-93798b98a06c.png)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Shell-To-Training-Jobs.mov)
 [Download Demo (.mov)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Shell-To-Training-Jobs.mov)
@@ -66,43 +65,51 @@
 
 ```shell
 pip install sagemaker-ssh-helper
 ```
 
 ### Step 2: Modify your start training job code
 1. Add import for SSHEstimatorWrapper
-2. Add a `dependencies` parameter to the Estimator object.
+2. Add a `dependencies` parameter to the Estimator object. Alternatively, add `sagemaker_ssh_helper` into `requirements.txt`.
 3. Add an `SSHEstimatorWrapper.create(estimator,...)` call before calling `fit()` and add SageMaker SSH Helper 
 as `dependencies`.
 4. Add a call to `ssh_wrapper.get_instance_ids()` to get the SSM instance(s) id. We'll use this as the target 
 to connect to later on.   
 
 For example:
 
 ```python
+import logging
 from sagemaker.pytorch import PyTorch
 from sagemaker_ssh_helper.wrapper import SSHEstimatorWrapper  # <--NEW--
 
 role = ...
 
-estimator = PyTorch(entry_point='train.py',
-                    source_dir='source_dir/training/',
-                    dependencies=[SSHEstimatorWrapper.dependency_dir()],  # <--NEW--
-                    role=role,
-                    framework_version='1.9.1',
-                    py_version='py38',
-                    instance_count=1,
-                    instance_type='ml.m5.xlarge')
+estimator = PyTorch(
+    entry_point='train.py',
+    source_dir='source_dir/training/',
+    dependencies=[SSHEstimatorWrapper.dependency_dir()],  # <--NEW 
+    # (alternatively, add sagemaker_ssh_helper into requirements.txt 
+    # inside source dir) --
+    role=role,
+    framework_version='1.9.1',
+    py_version='py38',
+    instance_count=1,
+    instance_type='ml.m5.xlarge'
+)
 
 ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=600)  # <--NEW--
 
 estimator.fit(wait=False)
 
+logging.info(f"To connect over SSH run: sm-local-ssh-training connect {ssh_wrapper.training_job_name()}")
+
 instance_ids = ssh_wrapper.get_instance_ids()  # <--NEW--
-print(f'To connect over SSM run: aws ssm start-session --target {instance_ids[0]}')  # <--NEW--
+
+logging.info(f"To connect over SSM run: aws ssm start-session --target {instance_ids[0]}")
 ```
 
 *Note:* `connection_wait_time_seconds` is the amount of time the SSH helper will wait inside SageMaker before it continues normal execution. It's useful for training jobs, when you want to connect before training starts.
 If you don't want to wait, set it to 0.
 
 *Note:* If you use distributed training (i.e., `instance_count > 1`), SSH Helper
 will start by default only on the first 2 nodes (e.g., on `algo-1` and `algo-2`).
@@ -131,50 +138,55 @@
 to start successfully. Then you'll need to have the ID of the managed instance. The instance id is prefixed by `mi-` 
 and will appear in the job's CloudWatch log like this:
 
 ```text
 Successfully registered the instance with AWS SSM using Managed instance-id: mi-1234567890abcdef0
 ``` 
 
-To fetch the instance IDs from the logs in an automated way, call the Python method of `ssh_wrapper`, 
+To fetch the instance IDs in an automated way, call the Python method `ssh_wrapper.get_instance_ids()`, 
 as mentioned in the previous step:
 
 ```python
 estimator = ...
 ssh_wrapper = ...
 estimator.fit(wait=False)
 instance_ids = ssh_wrapper.get_instance_ids()
 ```
 
-This method accepts the optional parameter `retry` with the number of retry attempts (default is 60). 
-It will retry to get instance IDs until they appear in the CloudWatch logs or number of attempts reached.
-The pause between attempts is fixed to 10 seconds, hence by default it will wait not more than 10 minutes.
+The method `get_instance_ids()` accepts the optional parameter `timeout_in_sec` (default is 600, i.e., 10 minutes). 
+If timeout is not 0, it will retry attempts to get instance IDs every 10 seconds.
 
 With the instance id at hand, you will be able to connect to the training container using the command line or the AWS web console:  
 
 A. Connecting using command line:  
 
-1. On the local machine, make sure that the latest AWS CLI **v2** is installed (v1 won't work), as described in 
-[the documentation for AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).  
-Verify that running `aws --version` prints `aws-cli/2.x.x ...`  
-   
-2. Install AWS Session Manager CLI plugin as described in [the SSM documentation](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html).
+1. On the local machine, make sure that you installed the latest [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and the [AWS Session Manager CLI plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html). Run the following command to perform the installation:
+
+```shell
+sm-local-configure
+```
+
+*Note:* If you start your training job from SageMaker Studio notebook, and execute the installation command from the image terminal, make sure that Python environment is activated, e.g., with `conda activate base`.
 
-3. Run this command (replace the target value with the instance id for your SageMaker job). Example:
+2. Run this command (replace the target value with the instance id for your SageMaker job). Example:
 ```shell
 aws ssm start-session --target mi-1234567890abcdef0
 ```
 
 B. Connecting using the AWS Web Console:  
 
   1. In AWS Web Console, navigate to Systems Manager > Fleet Manager.     
   2. Select the node, then Node actions > Start terminal session.
 
 Once connected to the container, you would want to switch to the root user with `sudo su -` command.
 
+C. Connecting with SSH and port forwarding:
+
+This method uses `sm-local-ssh-training connect` command and described in more details in the section [Forwarding TCP ports over SSH tunnel](README.md#port-forwarding).
+
 #### <a name="cli-commands"></a>Tip: Useful CLI commands
 
 Here are some useful commands to run in a terminal session:  
 - `ps xfaww` - Show running tree of processes
 - `ps xfawwe` - Show running tree of processes with environment variables 
 - `ls -l /opt/ml/input/data` - Show input channels
 - `ls -l /opt/ml/code` - Show your training code
@@ -209,41 +221,49 @@
 ## <a name="inference"></a>Connecting to SageMaker inference endpoints with SSM
 
 Adding SageMaker SSH Helper to inference endpoint is similar to training with the following differences.
 
 1. Wrap your model into `SSHModelWrapper` before calling `deploy()` and add SSH Helper to `dependencies`:
 
 ```python
+from sagemaker import Predictor
 from sagemaker_ssh_helper.wrapper import SSHModelWrapper  # <--NEW--
 
 estimator = ...
 ...
 endpoint_name = ... 
 
-model = estimator.create_model(entry_point='inference.py',
-                               source_dir='source_dir/inference/',
-                               dependencies=[SSHModelWrapper.dependency_dir()])  # <--NEW--
+model = estimator.create_model(
+    entry_point='inference_ssh.py',
+    source_dir='source_dir/inference/',
+    dependencies=[SSHModelWrapper.dependency_dir()]  # <--NEW 
+    # (alternatively, add sagemaker_ssh_helper into requirements.txt 
+    # inside source dir) --
+)
 
 ssh_wrapper = SSHModelWrapper.create(model, connection_wait_time_seconds=0)  # <--NEW--
 
-predictor = model.deploy(initial_instance_count=1,
-                         instance_type='ml.m5.xlarge',
-                         endpoint_name=endpoint_name)
+predictor: Predictor = model.deploy(
+    initial_instance_count=1,
+    instance_type='ml.m5.xlarge',
+    endpoint_name=endpoint_name,
+    wait=True
+)
 
 predicted_value = predictor.predict(data=...)
 ```
 
 *Note:* For the inference endpoint, which is always up and running, there's not too much value 
 in setting `connection_wait_time_seconds`, so it's usually set to `0`.
 
 Similar to training jobs, you can fetch the instance ids for connecting to the endpoint with SSM with 
 `ssh_wrapper.get_instance_ids()`.
 
 
-2. Add the following lines at the top of your `inference.py` script:
+2. Add the following lines at the top of your `inference_ssh.py` script:
 
 ```python
 import os
 import sys
 sys.path.append(os.path.join(os.path.dirname(__file__), "lib"))
 
 import sagemaker_ssh_helper
@@ -286,15 +306,15 @@
 
 mdm.add_model(model_data_source=model.repacked_model_data, model_data_path=model_name)
 
 predicted_value = predictor.predict(data=..., target_model=model_name)
 ```
 
 **Important:** Make sure that you're passing to `add_model()` the model ready for deployment with dependencies located at `model.repacked_model_data`,
-not the `estimator.model_data` that points to the trained model artifact.
+not the `estimator.model_data` that points to the trained model artifact. To obtain model suitable for inference, you might want to deploy first your model to a temporary single-node endpoint, so that SageMaker Python SDK takes care of repacking the model.
 
 Also note that SageMaker SSH Helper will be lazy loaded together with your model upon the first prediction request.
 So you should try to connect to the multi-model endpoint only after calling `predict()`.
 
 The `inference.py` script is the same as for regular endpoints.
 
 If you are using PyTorch containers, make sure you select the latest versions, 
@@ -417,200 +437,275 @@
 import sys
 sys.path.append("/opt/ml/processing/input/")
 
 import sagemaker_ssh_helper
 sagemaker_ssh_helper.setup_and_start_ssh()
 ```
 
+## <a name="port-forwarding"></a>Forwarding TCP ports over SSH tunnel
+
+Previous sections focused on connecting to non-interactive SageMaker containers with SSM.
+
+Next sections rely on the Session Manager capability to create an SSH tunnel over SSM connection. SageMaker SSH Helper in turn runs SSH session over SSH tunnel and forwards the ports, including the SSH server port 22 itself.
+
+The helper script behind this logic is `sm-local-start-ssh`:
+
+```shell
+sm-local-start-ssh "$INSTANCE_ID" \
+  -R localhost:12345:localhost:12345 \
+  -L localhost:8787:localhost:8787 \
+  -L localhost:11022:localhost:22
+```
+
+You can pass `-L` parameters for forwarding remote container port to local machine (e.g., `8787` for [Dask dashboard](https://docs.dask.org/en/stable/dashboard.html) or `8501` for [Streamlit apps](https://docs.streamlit.io/library/get-started)) or `-R` for forwarding local port to remote container. Read more about these options in the [SSH manual](https://man.openbsd.org/ssh).
+
+This low-level script takes the managed instance ID as a parameter. Next sections describe how to use the higher-level APIs that take the SageMaker resource name as a parameter and resolve it into the instance ID automatically (a.k.a. `sm-local-ssh-*` scripts):
+
+* `sm-local-ssh-training`
+* `sm-local-ssh-processing`
+* `sm-local-ssh-inference`
+* `sm-local-ssh-transform`
+* `sm-local-ssh-ide`
+
 ## <a name="pycharm-debug-server"></a>Remote debugging with PyCharm Debug Server over SSH
 
 This procedure uses PyCharm's Professional feature: [Remote debugging with the Python remote debug server configuration](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-debug-config)
 
-1. On the local machine, make sure that the latest AWS CLI **v2** is installed (v1 won't work), as described in 
-[the documentation for AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).  
-Verify that running `aws --version` prints `aws-cli/2.x.x ...`  
-   
-2. Install AWS Session Manager CLI plugin as described in [the SSM documentation](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html).
+1. On the local machine, make sure that you installed the latest [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and the [AWS Session Manager CLI plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html). Run the following command to perform the installation:
 
-3. In PyCharm, go to the Run/Debug Configurations (Run -> Edit Configurations...), add a new Python Debug Server.
+```shell
+sm-local-configure
+```
+
+2. In PyCharm, go to the Run/Debug Configurations (Run -> Edit Configurations...), add a new Python Debug Server.
 Choose the fixed port, e. g. `12345`.
 
-4. Take the correct version of `pydevd-pycharm` package from the configuration window 
+3. Take the correct version of `pydevd-pycharm` package from the configuration window 
 and install it either through `requirements.txt` or by calling `pip` from your source code.
 
-5. Add commands to connect to the Debug Server to your code:
+4. Add commands to connect to the Debug Server to your code **after** the `setup_and_start_ssh()` (e.g., into [a training script](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/tests/source_dir/training_debug/train_debug.py) that you submit as an entry point for a training job):
 ```python
 import pydevd_pycharm
 pydevd_pycharm.settrace('localhost', port=12345, stdoutToServer=True, stderrToServer=True, suspend=True)
 ```
 *Tip*: Check the argument's description in [the library source code](https://github.com/JetBrains/intellij-community/blob/dee787ef05d1187a71b7667652f6b25f3f573a1b/python/helpers/pydev/pydevd.py#L1663).
 
-6. Set extra breakpoints in your code with PyCharm, if needed
-7. Start the Debug Server in PyCharm
-8. Submit your code to SageMaker with SSH Helper as described in previous sections.
+5. Set extra breakpoints in your code with PyCharm, if needed
+6. Start the Debug Server in PyCharm
+7. Submit your code to SageMaker with SSH Helper as described in previous sections.
 Make sure you allow enough time for manually setting up the connection
-(do not set `connection_wait_time_seconds` to 0, recommended minimum value is 600, i.e. 10 minutes).
+(do not set `connection_wait_time_seconds` to `0`, recommended minimum value is `600`, i.e. 10 minutes).
 Don't worry to set it to higher values, e.g. to 30 min, because you will be able to terminate the waiting loop 
 once you connect.
 
-9. Start the port forwarding script once SSH helper connects to SSM and starts waiting inside the training job:
+8. Start the port forwarding script once SSH helper connects to SSM and starts waiting inside the training job:
 ```shell
 sm-local-ssh-training connect <<training_job_name>>
 ```
 It will reverse-forward the remote debugger port `12345` to your local machine's Debug Server port.
 The local port `11022` will be connected to the remote SSH server port, 
 to allow you easily connect with SSH from command line.  
 
 > *Note:* Before running this command make sure that AWS CLI is configured to access the account with `aws s3 ls` and your default region is set with `aws configure` command. Your Python's `<path-to-venv>/bin/` directory should be in the `$PATH`, otherwise you will get a *"command not found"* error.
 
 *Tip:* If you want to connect processing, batch transform jor or to an inference endpoint with SSH, use
 `sm-local-ssh-processing`, `sm-local-ssh-transform` or `sm-local-ssh-inference` scripts respectively.
 
-While this script is running, you may connect with SSH to the specified local port:
+Feel free to use the scripts as templates. Clone and customize them, if you want to change the ports.
 
-```shell
-ssh -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost
+9. Add the following configuration to `~/.ssh/config`:
+
+```text
+Host sagemaker-training
+  HostName localhost
+  IdentityFile ~/.ssh/sagemaker-ssh-gw
+  Port 11022
+  User root
 ```
 
-Feel free to use the scripts as templates. Clone and customize them, if you want to change the ports.
+*Note:* The SSH key specified as `IdentityFile` is automatically generated on your local machine every time when you run `sm-local-ssh-training` command from the step 8.
+
+While the `sm-local-ssh-training` script is running, you *may* connect with SSH to the specified local port (but it's not needed for PyCharm Debugger to work):
+
+```shell
+ssh sagemaker-training
+```
 
 *Tip:* If you log in to the node with SSH and don't see a `sm-wait` process, the training script has already started 
 and failed to connect to the PyCharm Debug Server, so you need to increase the `connection_wait_time_seconds`, 
 otherwise the debugger will miss your breakpoints.
 
 *Tip:* If you don't want `ssh` command to complain about remote host keys, when you switch to a different node,
 consider adding this two options to the command: `-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null`.
 
 10. Stop the waiting loop – connect to the instance and terminate the loop.
 
-As already mentioned in the step 8, make sure you've put enough timeout to allow the port forwarding script set up a tunnel 
+As already mentioned, make sure you've put enough timeout to allow the port forwarding script set up a tunnel 
 before execution of your script continues.
 
 You can use the following CLI command from your local machine to stop the waiting loop (the `sm-wait` remote process):
 ```shell
 sm-local-ssh-training stop-waiting
 ```
 
-Alternatively, if logged to the remote container already, run the `pkill` command from its shell (under `root`):
+Alternatively, if logged to the remote container already, run the `sm-wait stop` command from its shell (under `root`):
 ```text
-pkill sm-wait
+sm-wait stop
 ```
 
-11. After you stop the waiting loop, your code will continue running and will connect to your PyCharm Debug server.
+11. After you stop the waiting loop, your code will continue running and will connect to your PyCharm Debug Server.
+
+If everything is set up correctly, and you followed all the steps, PyCharm will stop at your breakpoint, highlight the line and wait for your input. Debug Server window will say “connected”. You can now press, for example, F8 to "Step Over" the code line or F7 to "Step Into" the code line.
 
 ## <a name="remote-interpreter"></a>Remote code execution with PyCharm / VSCode over SSH
 
-Follow the following steps from the section [Remote debugging with PyCharm Debug Server](#pycharm-debug-server):
-1, 2 and 8, 9, 10.
+Follow the steps from the section [Remote debugging with PyCharm Debug Server](#pycharm-debug-server), but skip the steps 2, 3, 4 and 11 that configure Remote Debug Server.
 
-Before terminating the waiting loop (step 10), make sure you configured and connected to SSH host and port 
-`localhost:11022` from your IDE as the remote Python interpreter. 
-Provide `~/.ssh/sagemaker-ssh-gw` as the private key.
+Instead, you need to configure the remote Python interpreter. Use `sagemaker-training` as the host name in an IDE dialog. 
 
  * [Instructions for PyCharm](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-interpreter)
+
+In PyCharm, use `11022` as the port and `root` as the user.
+
+![](images/pycharm_training.png)
+
  * [Instructions for VSCode](https://code.visualstudio.com/docs/remote/ssh)
 
-Note, that after you finished the waiting loop, your training script will run only once, and you will be able 
-to execute additional code only while your script is running.
-Once the script finishes, you will need to submit another training job and repeat the procedure again.
+![](images/vscode_training.png)
+
+Note, that if you stop the waiting loop, SageMaker will run your training script only once, and you will be able to execute additional code from local machine from PyCharm only while your script is running. Once the script finishes, you will need to submit another training job and repeat the procedure again.
 
 But there's a useful trick: submit a dummy script `train_placeholder.py` with the infinite loop, and while this loop will be running, you can 
 run your real training script again and again with the remote interpreter.
-Setting `max_run` parameter of the estimator is highly recommended in this case.
+Setting `max_run` parameter of the estimator is highly recommended in this case. 
 
 The dummy script may look like this:
 
 ```python
 import time
+from datetime import timedelta
 
-import sagemaker_ssh_helper
-sagemaker_ssh_helper.setup_and_start_ssh()
+from sagemaker_ssh_helper import setup_and_start_ssh, is_last_session_timeout
+
+setup_and_start_ssh()
 
-while True:
+while not is_last_session_timeout(timedelta(minutes=30)):
     time.sleep(10)
 ```
 
-Make also sure that you're aware of [SageMaker Managed Warm Pools](https://docs.amazonaws.cn/en_us/sagemaker/latest/dg/train-warm-pools.html) 
-feature, which is also helpful in such a scenario.
+The method `is_last_session_timeout()` will help to prevent unused resources and the job will end if there's no SSM or SSH sessions for the specified period of time. It will count active SSM sessions, and time out when there are no sessions left. 
+
+*Note:* Keep in mind that SSM sessions will [terminate automatically due to user inactivity](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-preferences-timeout.html), but SSH sessions will keep running until either a user terminates them manually or network timeout occurs (e.g., the user closes the laptop lid or disconnects from Wi-Fi). If the user leaves the local machine unattended and connected to Internet, SSM sessions started by `aws ssm start-session` command will time out, but SSH-over-SSM sessions started with `sm-local-ssh-training connect` will stay open.
+
+Consider sending e-mail notifications for users of the long-running jobs, so the users don't forget to shut down unused resources. See [the related question in FAQ](FAQ.md#i-want-to-send-users-the-sms-or-email-notification-when-the-placeholder-training-job-has-issues-with-low-gpu-utilization-how-to-do-that) for more details.
+
+Make also sure that you're aware of [SageMaker Managed Warm Pools](https://docs.aws.amazon.com/sagemaker/latest/dg/train-warm-pools.html) 
+feature, which is also helpful in the scenario when you need to rerun your code multiple times.
+
+*Pro Tip:* Note that you can debug your code line by line in this scenario, too! See [the tutorial in PyCharm documentation](https://www.jetbrains.com/help/pycharm/debugging-your-first-python-application.html#debug). Some users might prefer this option instead of using Debug Server as a simpler alternative.
+
+It is also interesting to compare this section instructions with the AWS blog post [Run your TensorFlow job on Amazon SageMaker with a PyCharm IDE](https://aws.amazon.com/blogs/machine-learning/run-your-tensorflow-job-on-amazon-sagemaker-with-a-pycharm-ide/). In contrast to using SageMaker SSH Helper, the blog instructions do not demonstrate the remote debugging capabilities, but suggest to use the [SageMaker local mode](https://github.com/aws-samples/amazon-sagemaker-local-mode) instead. As with Managed Warm Pools, SageMaker local mode helps to test your code faster, but it consumes local resources and still doesn't provide the line by line debugging capability.
 
 ## <a name="studio"></a>Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode
 
 [![Download Demo (.mov)](https://user-images.githubusercontent.com/87804596/205895890-e5e87f8b-1ca6-4ce6-bac1-5cb6e6f61dde.png)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
 [Download Demo (.mov)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
 
-Follow the next steps for your local IDE integration with SageMaker Studio:
+Follow the next steps for your local IDE integration with SageMaker Studio.
 
-1. Copy [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) into SageMaker Studio and run it.
+1. On the local machine, install the library: 
 
-*Tip:* Alternatively, attach to a domain the KernelGateway lifecycle config script [kernel-lc-config.sh](kernel-lc-config.sh) 
+```
+pip install sagemaker-ssh-helper
+```
+
+2. Copy [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) into SageMaker Studio and run it. 
+
+*Tip:* Alternatively, instead of using `SageMaker_SSH_IDE.ipynb`, attach to a domain the KernelGateway lifecycle config script [kernel-lc-config.sh](kernel-lc-config.sh) 
 (you may need to ask your administrator to do this).
 Once configured, from the Launcher choose the environment, puck up the lifecycle script and choose 
 'Open image terminal' (so, you don't even need to create a notebook).
 
-2. On the local machine, make sure that the latest AWS CLI **v2** is installed (v1 won't work), as described in 
-[the documentation for AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).  
-Verify that running `aws --version` prints `aws-cli/2.x.x ...`  
-   
-3. Install AWS Session Manager CLI plugin as described in [the SSM documentation](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html).
+> Note that the `main` branch of this repo can contain changes that are not compatible with the version of `sagemaker-ssh-helper` that you installed from pip. To ensure the stable performance, check the version with `pip freeze | grep sagemaker-ssh-helper` and take the notebook and the lifecycle script from [the corresponding tag](https://github.com/aws-samples/sagemaker-ssh-helper/tags).  
 
-4. Install the library: `pip install sagemaker-ssh-helper` .
+3. Make sure that you installed the latest [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and the [AWS Session Manager CLI plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html). Run the following command to perform the installation:
+
+```shell
+sm-local-configure
+```
 
-5. Start SSH tunnel and port forwarding from a terminal session as follows:
+4. Start SSH tunnel and port forwarding from a terminal session as follows:
 
 ```shell
-sm-local-ssh-ide <<kernel_gateway_app_name>>
+sm-local-ssh-ide connect <<kernel_gateway_app_name>>
 ```
 
 The parameter <<kernel_gateway_app_name>> is either taken from SageMaker Studio when you run notebook [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb), 
 or from the image terminal as a `hostname` output, or you can find it in the list of running apps in AWS Console under Amazon SageMaker -> Control Panel -> User Details.
-It looks like this: `datascience-1-0-ml-g4dn-xlarge-1234567890abcdef0`.
+It looks like this: `sagemaker-data-science-ml-m5-large-1234567890abcdef0`.
 
 The local port `10022` will be connected to the remote SSH server port, to let you connect with SSH from IDE.  
 In addition, the local port `8889` will be connected to remote Jupyter notebook port, the port `5901` to the remote VNC server 
 and optionally the remote port `443` will be connected to your local PyCharm license server address.
 
 > *Note:* Before running this command make sure that AWS CLI is configured to access the account with `aws s3 ls` and your default region is set with `aws configure` command. Your Python's `<path-to-venv>/bin/` directory should be in the `$PATH`, otherwise you will get a *"command not found"* error.
 
 Feel free to use the script as a template. Clone and customize it, if you want to change the ports and hosts.
 
-6. Connect local PyCharm or VSCode with remote Python interpreter by using `root@localhost:10022` as SSH parameters.
-Also provide `~/.ssh/sagemaker-ssh-gw` as the private key.
 
-> *Note:* The SSH key is automatically generated on your local machine every time 
-> when you run `sm-local-ssh-ide` command from step 5.
+5. Add the following configuration to `~/.ssh/config`:
+
+```text
+Host sagemaker-studio
+  HostName localhost
+  IdentityFile ~/.ssh/sagemaker-ssh-gw
+  Port 10022
+  User root
+```
+
+*Note:* The SSH key specified as `IdentityFile` is automatically generated on your local machine every time when you run `sm-local-ssh-ide` command from the step 4.
+
+Before moving to the next step, you can optionally check from your local machine that connection is working by running the SSH command in command line:
+
+```shell
+ssh sagemaker-studio
+```
+
+
+6. Connect local PyCharm or VSCode with remote Python interpreter by using `sagemaker-studio` as the remote SSH host.
 
  * [Instructions for SSH in PyCharm](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-interpreter)
+
+In PyCharm, use `11022` as the port and `root` as the user.
+
+![](images/pycharm_studio.png)
+
  * [Instructions for SSH in VSCode](https://code.visualstudio.com/docs/remote/ssh)
 
-*Tip (PyCharm):* When you configure Python interpreter in PyCharm, it's recommended to configure the path mapping (*"Sync folders"* deployment option) for you project to point into `/root/project_name` instead of default `/tmp/pycharm_project_123`. This is how you will be able to see your project in SageMaker Studio and PyCharm will automatically sync your local dir to the remote dir. 
+![](images/vscode_studio.png)
+
+*Tip (PyCharm):* When you configure Python interpreter in PyCharm, it's recommended to configure [the path mapping](https://www.jetbrains.com/help/pycharm/deployment-mappings-tab.htm) (*"Sync folders"* deployment option) for you project to point into `/root/project_name` instead of default `/tmp/pycharm_project_123`. This is how you will be able to see your project in SageMaker Studio and PyCharm will automatically sync your local dir to the remote dir. 
 
 *Tip (PyCharm):* Also instead of creating a new venv, point the Python interpreter to the existing location. 
 You can find this location by running a cell with `import sys; sys.executable` command in a SageMaker Studio notebook. You will get something like `/opt/conda/bin/python`.
 
 Now with PyCharm or VSCode you can run and debug the code remotely inside the kernel gateway app.
 
-You can also check from your local machine that connection is working by running the SSH command in command line:
-
-```shell
-ssh -i ~/.ssh/sagemaker-ssh-gw -p 10022 root@localhost
-```
-
-If you don't want this `ssh` command to complain about remote host keys, when you switch to a different node,
-consider adding this two options to the command: `-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null`.
+You can also configure a remote Jupyter Server as 
+http://127.0.0.1:8889/?token=<<your_token>>.
 
-You may now configure a remote Jupyter Server as 
-http://127.0.0.1:8889/?token=<<your_token>>. You will find the full URL with remote token in 
+You will find the full URL with remote token in 
 the [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) notebook in the output after running the cell
-with `sm-ssh-ide start` command. 
+with `sm-ssh-ide start` command. If you use lifecycle configuration, run `tail /tmp/jupyter-notebook.log` from the image terminal to find the Jupyter Server URL.
 
  * [Instructions for remote Jupyter notebooks in PyCharm](https://www.jetbrains.com/help/pycharm/configuring-jupyter-notebook.html#configure-server)
  * [Instructions for remote Jupyter notebooks in VSCode](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_connect-to-a-remote-jupyter-server) (don't forget to switch kernel to remote after configuring the remote server).
 
 You can also start the VNC session to [vnc://localhost:5901](vnc://localhost:5901) (e.g. on macOS with Screen Sharing app)
-and run IDE or any other GUI app on the remote desktop instead of your local machine.
+and run IDE or any other GUI app on the remote desktop instead of your local machine. For example, you can run `jupyter qtconsole --existing` command to connect to already running SageMaker Studio kernel with the [Jupyter QT app](https://qtconsole.readthedocs.io/en/stable/index.html), instead of using the notebook web UI.
 
 7. If you want to switch to another [kernel](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-change-image.html) 
 or [instance](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-switch-instance-type.html), feel free to do so from SageMaker Studio UI and re-run
 [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb).
 
 Keep in mind that in this case the previous kernel will stop and SSM agent will stop, too.
 To allow multiple kernel and instances to be up and running with SageMaker SSH Helper and SSM agent,
@@ -620,68 +715,60 @@
 
 If you're using lifecycle configuration script, just start another image terminal with different environment settings 
 from Launcher.
 
 8. Don't forget to [shut down](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-shut-down.html)
 SageMaker Studio resources, if you don't need them anymore, e.g., launched notebooks, terminals, apps and instances.
 
-#### Troubleshooting IDE integration
+See the [troubleshooting section of the FAQ](FAQ.md#troubleshooting), if something doesn't work as you expect.
 
-* Check that the instance ID your local machine tries to connect to and instance ID 
-that `init-ssm` command produced in the notebook are the same.
+## <a name="web-vnc"></a>Web VNC
 
-If you initialized SSM multiple times in your kernel app, you can see this error message 
-shortly after the re-initialization:
+At times, you cannot install all the software on your local machine, also because this is the software to process the data, and you cannot copy massive amount of the data to your local machine. 
 
-```text
-An error occurred (TargetNotConnected) when calling the StartSession operation: mi-1234567890abcdef0 is not connected.
-```
+By combining the [noVNC](https://novnc.com/) tool with [AWS Jupyter Proxy](https://github.com/aws/aws-jupyter-proxy) extension you can run virtually any IDE like PyCharm, VSCode, PyDev, or any tool like Blender (to work with 3D data), OpenShot (to work with audio-video data), etc., from a SageMaker Studio web interface.
 
-or this one:
+It's also helpful in situations when you cannot run SSH client on your local machine to forward ports for web tools, like Dask dashboard. In this case, you run a tool in the remote browser running through the web VNC (browser-in-a-browser), like on the below screenshot. You might notice that PyCharm and VSCode are also running in the background:
+![WebWNC Screenshot](images/webVNC.png)
 
-```text
-An error occurred (InvalidInstanceId) when calling the SendCommand operation: Instances [[mi-1234567890abcdef0]] not in a valid state for account 555555555555
-```
+To achieve this result, your Administrator should configure your SageMaker IAM role with both `SSHSageMakerServerPolicy` and `SSHSageMakerClientPolicy`. Configuration of IAM credentials for the local machine is not required in this case. See [IAM_SSM_Setup.md](IAM_SSM_Setup.md) for more details.
+
+Then follow these steps:
+
+1. On the SageMaker Studio System terminal run the commands from [server-lc-config.sh](server-lc-config.sh).
 
-The reason for this error is that CloudWatch logs arrive with some delay, and previous instance ID is fetched 
-instead of a new one. Wait for 30-60 seconds to allow logs to come through and try again.
+Alternatively, ask the Administrator to [attach the lifecycle config](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-lcc-create.html) to the SageMaker Studio domain or to your profile as the `JupyterServer` config.
 
-* Check that `sshd` process is started in SageMaker Studio notebook by running a command in the image terminal:
+2. Follow the step 1 for [the IDE configuration procedure](#studio), i.e., run the IDE notebook or lifecycle config inside the kernel gateway of your choice. 
+
+Instead of your local user ID put the SageMaker Studio user ID (you can get it by running `aws sts get-caller-identity` from a SageMaker Studio terminal).
+
+3. On the System terminal, run:
 
 ```shell
-ps xfa | grep sshd
+sm-local-ssh-ide connect <<kernel_gateway_app_name>>
 ```
 
-If it's not started, there might be some errors in the output of the notebook, and you might get this error on 
-the local machine:
+Add additional params to the command, e.g., `-L localhost:8787:localhost:8787` to forward the Dask dashboard that is running inside the kernel gateway.
 
-```text
-Connection closed by UNKNOWN port 65535
-```
+4. Navigate to `https://d-egm0dexample.studio.eu-west-1.sagemaker.aws/jupyter/default/proxy/6080/vnc.html?host=d-egm0dexample.studio.eu-west-1.sagemaker.aws&port=443&path=jupyter/default/proxy/6080/websockify`
 
-Check carefully the notebook output in SageMaker Studio and try to stop and start SSM & services again.
+Replace both occurrences of `d-egm0dexample` with your SageMaker Studio domain ID, and `eu-west-1` with your AWS Region.
 
-* Also check SSM agent logs inside SageMaker Studio. From the image terminal run:
-```text
-tail /var/log/amazon/ssm/*.log && date
-```
+You will see the noVNC welcome screen.
 
-* Sometimes you can see this error message on your local machine when trying to connect with SSM, even 
-if you correctly completed all configuration steps, including the step to enable advanced tier:
+5. Press "Connect" and enter your password (default is `123456`).
 
-```text
-An error occurred (BadRequest) when calling the StartSession operation: Enable advanced-instances tier to use Session Manager with your on-premises instances
-```
+Congratulations! You now have successfully logged into the remote desktop environment running inside a SageMaker Studio kernel gateway.
 
-In this case check that AWS Region in your AWS console is the same as on your local machine.
-To do this, run the following command locally:
+*Tip:* If you have issues with copy-pasting through system clipboard, use the temp file, e.g. `clip.txt`, and open it in VNC session and SageMaker Studio file browser at the same time.
 
-```text
-aws configure list | grep region
+*Pro Tip:* To set the resolution that matches your browser window size, make a page screenshot (in Firefox - right-click on an empty area -> Take Screenshot -> Save visible), then inspect the resolution of the image, e.g. 1920x970. Then add and switch resolution inside the VNC session:
+```shell
+$ cvt 1920 970 60
+# 1920x970 59.93 Hz (CVT) hsync: 60.35 kHz; pclk: 154.50 MHz
+Modeline "1920x970_60.00"  154.50  1920 2040 2240 2560  970 973 983 1007 -hsync +vsync
+$ xrandr --newmode "1920x970_60.00"  154.50  1920 2040 2240 2560  970 973 983 1007 -hsync +vsync
+$ xrandr --addmode VNC-0 1920x970_60.00
+$ xrandr -s 1920x970_60.00
 ```
 
-It will provide you the locally configured region and will show where this setting is coming from, e.g., env variables 
-or AWS config file:
-
-```text
-    region                eu-west-1      config-file    ~/.aws/config
-```
```

### Comparing `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-inference` & `sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-transform`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 #!/bin/bash
 
 # Commands:
-# connect <endpoint_name>
+# connect <transform_job_name> [<extra_ssh_args>]
 # stop-waiting
 # run-command <command> <args...>
 
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
-  ENDPOINT_NAME=$2
+  JOB_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
-import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
+import sagemaker; from sagemaker_ssh_helper.manager import SSMManager;
 import logging; logging.basicConfig(level=logging.INFO);
-print(SSHLog().get_endpoint_ssm_instance_ids("$ENDPOINT_NAME", retry=30)[0])
+print(SSMManager().get_transformer_instance_ids("$JOB_NAME", timeout_in_sec=300)[0])
 EOF
   )
 
+  shift
+  shift
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
-      -L localhost:11022:localhost:22
+      -L localhost:16022:localhost:22 \
+      $*
 
 elif [[ "$COMMAND" == "stop-waiting" ]]; then
 
-  $0 run-command pkill sm-wait
+  $0 run-command sm-wait stop
 
 elif [[ "$COMMAND" == "run-command" ]]; then
 
   shift
   ARGS=$*
 
   # shellcheck disable=SC2086
-  ssh -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
+  ssh -4 -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
     -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
     $ARGS
 
 else
     echo "Unknown command: $COMMAND"
 fi
```

### Comparing `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-processing` & `sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-inference`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 #!/bin/bash
 
 # Commands:
-# connect <processing_job_name>
+# connect <endpoint_name> [<extra_ssh_args>]
 # stop-waiting
 # run-command <command> <args...>
 
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
-  JOB_NAME=$2
+  ENDPOINT_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
 import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
 import logging; logging.basicConfig(level=logging.INFO);
-print(SSHLog().get_processing_ssm_instance_ids("$JOB_NAME", retry=30)[0])
+print(SSHLog().get_endpoint_ssm_instance_ids("$ENDPOINT_NAME", retry=30)[0])
 EOF
   )
 
+  shift
+  shift
+
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
-      -L localhost:11022:localhost:22
+      -L localhost:12022:localhost:22 \
+      $*
 
 elif [[ "$COMMAND" == "stop-waiting" ]]; then
 
-  $0 run-command pkill sm-wait
+  $0 run-command sm-wait stop
 
 elif [[ "$COMMAND" == "run-command" ]]; then
 
   shift
   ARGS=$*
 
   # shellcheck disable=SC2086
-  ssh -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
+  ssh -4 -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
     -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
     $ARGS
 
 else
     echo "Unknown command: $COMMAND"
 fi
```

### Comparing `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-training` & `sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-processing`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 #!/bin/bash
 
 # Commands:
-# connect <training_job_name>
+# connect <processing_job_name> [<extra_ssh_args>]
 # stop-waiting
 # run-command <command> <args...>
 
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
   JOB_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
-import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
+import sagemaker; from sagemaker_ssh_helper.manager import SSMManager;
 import logging; logging.basicConfig(level=logging.INFO);
-print(SSHLog().get_training_ssm_instance_ids("$JOB_NAME", retry=30)[0])
+print(SSMManager().get_processing_instance_ids("$JOB_NAME", timeout_in_sec=300)[0])
 EOF
   )
 
+  shift
+  shift
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
-      -L localhost:11022:localhost:22
+      -L localhost:14022:localhost:22 \
+      $*
 
 elif [[ "$COMMAND" == "stop-waiting" ]]; then
 
-  $0 run-command pkill sm-wait
+  $0 run-command sm-wait stop
 
 elif [[ "$COMMAND" == "run-command" ]]; then
 
   shift
   ARGS=$*
 
   # shellcheck disable=SC2086
-  ssh -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
+  ssh -4 -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
     -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
     $ARGS
 
 else
     echo "Unknown command: $COMMAND"
 fi
```

### Comparing `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-transform` & `sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-ssh-training`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 #!/bin/bash
 
 # Commands:
-# connect <transform_job_name>
+# connect <training_job_name> [<extra_ssh_args>]
 # stop-waiting
 # run-command <command> <args...>
 
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
   JOB_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
-import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
+import sagemaker; from sagemaker_ssh_helper.wrapper import SSHEstimatorWrapper;
 import logging; logging.basicConfig(level=logging.INFO);
-print(SSHLog().get_transformer_ssm_instance_ids("$JOB_NAME", retry=30)[0])
+print(SSHEstimatorWrapper.attach("$JOB_NAME").get_instance_ids(timeout_in_sec=300)[0])
 EOF
   )
 
+  shift
+  shift
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
-      -L localhost:11022:localhost:22
+      -L localhost:11022:localhost:22 \
+      $*
 
 elif [[ "$COMMAND" == "stop-waiting" ]]; then
 
-  $0 run-command pkill sm-wait
+  $0 run-command sm-wait stop
 
 elif [[ "$COMMAND" == "run-command" ]]; then
 
   shift
   ARGS=$*
 
   # shellcheck disable=SC2086
-  ssh -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
+  ssh -4 -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost \
     -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
     $ARGS
 
 else
     echo "Unknown command: $COMMAND"
 fi
```

### Comparing `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-start-ssh` & `sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper/sm-local-start-ssh`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 #!/bin/bash
 
+# Syntax:
+# sm-local-start-ssh <instance_id> <extra_ssh_args>
+
 INSTANCE_ID=$1
 shift
 
+INSTANCE_ID=$(echo "$INSTANCE_ID" | tr '\n' ' ' | grep -o 'mi-.*$' | awk -F' ' '{print $1}')
+
 if [ -z "${INSTANCE_ID}" ]; then
-  echo "INSTANCE_ID not provided"
+  echo "INSTANCE_ID is not provided or incorrect (should be in the form mi-1234567890abcdef0)"
   exit 1
-else
-  echo "INSTANCE_ID -> ${INSTANCE_ID}"
 fi
 
 # Useful for port forwarding and debugging, eg. passing -vvv option
 EXTRA_SSH_ARGS=$*
 
+read -r -d '' program << EOF
+import logging
+import sagemaker
+logging.getLogger('sagemaker.config').setLevel(logging.WARNING)
+print(sagemaker.Session().default_bucket())
+EOF
+
 if [ -z "${SSH_AUTHORIZED_KEYS_PATH}" ]; then
-  bucket=$(python -c 'import sagemaker; print(sagemaker.Session().default_bucket())')
+  bucket=$(python -c "$program")
   SSH_AUTHORIZED_KEYS_PATH="s3://$bucket/ssh-authorized-keys/"
 fi
 
 echo "SSH authorized keys path -> ${SSH_AUTHORIZED_KEYS_PATH}"
 
 # shellcheck disable=SC2086  # extra args have to be unquoted to be parsed from the inner script
 sm-connect-ssh-proxy "${INSTANCE_ID}" \
```

### Comparing `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/PKG-INFO` & `sagemaker-ssh-helper-2.0.0/sagemaker_ssh_helper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: sagemaker-ssh-helper
-Version: 1.9.1
-Summary: A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH
+Version: 2.0.0
+Summary: A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH (Secure Shell)
 Home-page: https://github.com/aws-samples/sagemaker-ssh-helper
 Author: Amazon Web Services
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: cdk
 Provides-Extra: test
-Provides-Extra: test-macos
+Provides-Extra: dev
+Provides-Extra: dev-macos
 License-File: LICENSE
 
-SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, remote debugging, and advanced troubleshooting.
+SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, remote debugging, and advanced troubleshooting, also known as "SSH into SageMaker".
 
-For the full description see [README.md](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/README.md).
+For the documentation, see the repo [https://github.com/aws-samples/sagemaker-ssh-helper/](https://github.com/aws-samples/sagemaker-ssh-helper/).
```

### Comparing `sagemaker-ssh-helper-1.9.1/setup.py` & `sagemaker-ssh-helper-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,94 @@
 import setuptools
 
 required_packages = [
-    "sagemaker>=2.125.0"
+    "sagemaker>=2.145.0",
+    "psutil",
 ]
 
 extras = {
+    "cdk": [
+        "aws-cdk-lib==2.64.0",
+        "constructs>=10.0.0,<11.0.0",
+    ],
     "test": [
-        "black",
         "coverage",
         "flake8",
         "mock",
         "pydocstyle",
         "pytest",
         "pytest-cov",
+        "pytest-html",
+        "pytest-profiling",
+        "bandit",
+        "aws-cdk-lib==2.64.0",
+        "constructs>=10.0.0,<11.0.0",
+        "sagemaker-studio-image-build",
+        "sagemaker-training",
+        "selenium"
+    ],
+    "dev": [
         "sagemaker-pytorch-training",
         "sagemaker-pytorch-inference",
         "torch-model-archiver",
         "tox",
         "wheel",
         "build",
         "twine",
-        "pydevd-pycharm~=213.6777.50",
+        "pydevd-pycharm~=222.4459.20",
         "scikit-learn"
     ],
-    "test-macos": [
+    "dev-macos": [
         "tensorflow-macos==2.9.2",
         "numpy==1.22.4"
     ]
 }
 setuptools.setup(
     name='sagemaker-ssh-helper',
-    version='1.9.1',
+    version='2.0.0',
     author="Amazon Web Services",
-    description="A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH",
+    description="A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH (Secure Shell)",
     long_description="SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's "
                      "training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook "
-                     "containers for fast interactive experimentation, remote debugging, and advanced troubleshooting."
+                     "containers for fast interactive experimentation, remote debugging, and advanced troubleshooting, "
+                     "also known as \"SSH into SageMaker\"."
                      "\n\n"
-                     "For the full description see [README.md]"
-                     "(https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/README.md).",
+                     "For the documentation, see the repo [https://github.com/aws-samples/sagemaker-ssh-helper/]"
+                     "(https://github.com/aws-samples/sagemaker-ssh-helper/).",
     long_description_content_type='text/markdown',
     url='https://github.com/aws-samples/sagemaker-ssh-helper',
     packages=setuptools.find_packages(),
     include_package_data=True,
     scripts=['sagemaker_ssh_helper/sm-helper-functions',
              'sagemaker_ssh_helper/sm-connect-ssh-proxy',
              'sagemaker_ssh_helper/sm-wait',
              'sagemaker_ssh_helper/sm-local-start-ssh',
-             'sagemaker_ssh_helper/sm-local-install-force',
              'sagemaker_ssh_helper/sm-local-ssh-ide',
+             'sagemaker_ssh_helper/sm-local-ssh-notebook',
              'sagemaker_ssh_helper/sm-local-ssh-training',
              'sagemaker_ssh_helper/sm-local-ssh-transform',
              'sagemaker_ssh_helper/sm-local-ssh-inference',
              'sagemaker_ssh_helper/sm-local-ssh-processing',
-             'sagemaker_ssh_helper/sm-start-ssh',
+             'sagemaker_ssh_helper/sm-local-configure',
              'sagemaker_ssh_helper/sm-ssh-ide',
              'sagemaker_ssh_helper/sm-save-env',
              'sagemaker_ssh_helper/sm-init-ssm',
-             'sagemaker_ssh_helper/sm-setup-ssh'],
+             'sagemaker_ssh_helper/sm-setup-ssh',
+             ],
     python_requires=">=3.7",
     install_requires=required_packages,
     extras_require=extras,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT No Attribution License (MIT-0)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ]
 )
```

