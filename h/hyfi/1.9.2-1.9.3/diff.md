# Comparing `tmp/hyfi-1.9.2.tar.gz` & `tmp/hyfi-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.9.2.tar", max compression
+gzip compressed data, was "hyfi-1.9.3.tar", max compression
```

## Comparing `hyfi-1.9.2.tar` & `hyfi-1.9.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1071 2023-07-24 19:08:25.043397 hyfi-1.9.2/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-24 19:08:25.043397 hyfi-1.9.2/README.md
--rw-r--r--   0        0        0     4852 2023-07-24 19:09:01.939751 hyfi-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     4346 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/__click__.py
--rw-r--r--   0        0        0     1538 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-24 19:09:01.839750 hyfi-1.9.2/src/hyfi/_version.py
--rw-r--r--   0        0        0     1497 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-24 19:08:25.047397 hyfi-1.9.2/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24454 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      193 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0     1053 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      955 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      876 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      159 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
--rw-r--r--   0        0        0      213 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/dataset_sample.yaml
--rw-r--r--   0        0        0      113 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
--rw-r--r--   0        0        0       69 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      738 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      338 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     6219 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10023 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/core/config.py
--rw-r--r--   0        0        0     5675 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/core/hydra/__init__.py
--rw-r--r--   0        0        0     3344 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/core/hydra/main.py
--rw-r--r--   0        0        0     5744 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/core/hydra/utils.py
--rw-r--r--   0        0        0     5911 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-24 19:08:25.051397 hyfi-1.9.2/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    20170 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4327 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1323 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/pipe/datasets.py
--rw-r--r--   0        0        0     1455 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8383 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5822 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     7916 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1184 2023-07-24 19:08:25.055398 hyfi-1.9.2/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 23:53:12.333019 hyfi-1.9.3/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-24 23:53:12.333019 hyfi-1.9.3/README.md
+-rw-r--r--   0        0        0     4852 2023-07-24 23:53:39.065429 hyfi-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4334 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/__click__.py
+-rw-r--r--   0        0        0     1649 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 23:53:38.985427 hyfi-1.9.3/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1497 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24454 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0     1053 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      955 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      876 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      159 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
+-rw-r--r--   0        0        0      213 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/dataset_sample.yaml
+-rw-r--r--   0        0        0      113 2023-07-24 23:53:12.337019 hyfi-1.9.3/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
+-rw-r--r--   0        0        0       69 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      738 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      338 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     7421 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10023 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     4950 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/core/hydra/__init__.py
+-rw-r--r--   0        0        0     3344 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/core/hydra/main.py
+-rw-r--r--   0        0        0     5744 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/core/hydra/utils.py
+-rw-r--r--   0        0        0     5911 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    20188 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4327 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/pipe/datasets.py
+-rw-r--r--   0        0        0     1455 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8383 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5822 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     7916 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1184 2023-07-24 23:53:12.341019 hyfi-1.9.3/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.9.3/PKG-INFO
```

### Comparing `hyfi-1.9.2/LICENSE` & `hyfi-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/README.md` & `hyfi-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/pyproject.toml` & `hyfi-1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.9.2"
+version = "1.9.3"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.9.2/src/hyfi/__cli__.py` & `hyfi-1.9.3/src/hyfi/__cli__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,22 @@
         sys.argv.append(f"--config-dir={search_path}")
     if not config_path:
         config_path = __global_hyfi__.config_module_path
     if not config_name:
         config_name = __global_hyfi__.config_name
     if not plugins:
         plugins = __global_hyfi__.plugins
-    if __global_hyfi__.__package_name__ != __hyfi_package_name__:
+    if __global_hyfi__.package_name != __hyfi_package_name__:
         overrides = overrides or []
-        override = f"about={__global_hyfi__.__package_name__}"
+        override = f"about={__global_hyfi__.package_name}"
         if override not in overrides:
             overrides.append(override)
             logger.debug(
                 "Overriding `about` config group with `%s`",
-                __global_hyfi__.__package_name__,
+                __global_hyfi__.package_name,
             )
     hyfi_hydra_main(
         config_path=config_path,
         config_name=config_name,
         version_base=__hydra_version_base__,
         overrides=overrides,
         plugins=plugins,
```

### Comparing `hyfi-1.9.2/src/hyfi/__click__.py` & `hyfi-1.9.3/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/__init__.py` & `hyfi-1.9.3/src/hyfi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
     All names of configuration folders and their counterparts folders for pydantic models
     are singular, e.g. `conf` instead of `configs`.
     All matching pydantic models are named `Config`, e.g. `BatchConfig` instead of `BatchConfigs`.
 
     Other module folders are plural, e.g. `utils` instead of `util`.
 """
+from typing import List, Optional
+
 from hyfi.__cli__ import hydra_main, hyfi_main
 from hyfi.core import __global_hyfi__ as global_hyfi
 from hyfi.core import __hydra_version_base__
 from hyfi.core.config import __global_config__ as global_config
 from hyfi.main import HyFI
 from hyfi.main import HyFI as H
 from hyfi.main import HyFI as HI
@@ -27,26 +29,27 @@
     "LOGGING",
     "__hydra_version_base__",
     "initialize_global_hyfi",
 ]
 
 
 def initialize_global_hyfi(
-    package_name: str,
+    package_path: str,
     version: str,
+    plugins: Optional[List[str]] = None,
 ) -> None:
     """
     Initializes the global HyFI instance.
 
     This function should be called before any other HyFI function.
 
     A plugin is a python module which contains a configuration module.
 
     Be careful!
     It does not check if the plugin is importable.
 
     Args:
-        package_name: Name of the package. e.g. `hyfi`
+        package_path: Path to the package root folder. e.g. `./src/hyfi`
         version: Version of the package. e.g. `0.1.0`
         plugins: A list of plugins to load. e.g. `["hyfi.conf"]`
     """
-    global_hyfi.initialize(package_name=package_name, version=version)
+    global_hyfi.initialize(package_path=package_path, version=version, plugins=plugins)
```

### Comparing `hyfi-1.9.2/src/hyfi/about/__init__.py` & `hyfi-1.9.3/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/batch/__init__.py` & `hyfi-1.9.3/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/__init__.py` & `hyfi-1.9.3/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.9.3/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/cache_file.py` & `hyfi-1.9.3/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/common.py` & `hyfi-1.9.3/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/file_lock.py` & `hyfi-1.9.3/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/meta.py` & `hyfi-1.9.3/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/progress.py` & `hyfi-1.9.3/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.9.3/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.9.3/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.9.3/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.9.3/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.9.3/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/testing.py` & `hyfi-1.9.3/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/cached_path/util.py` & `hyfi-1.9.3/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/composer/__init__.py` & `hyfi-1.9.3/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/composer/base.py` & `hyfi-1.9.3/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/composer/pydantic.py` & `hyfi-1.9.3/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.9.3/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.9.3/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.9.3/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.9.3/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.9.3/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.9.3/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.9.3/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/copier/__init__.py` & `hyfi-1.9.3/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/core/__init__.py` & `hyfi-1.9.3/src/hyfi/core/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
     HyFI Core Module
 """
-import importlib
 import os
 from pathlib import Path
-from typing import Any, List, Optional
+from typing import List, Optional, Tuple
 
 from pydantic import BaseModel
 
 from hyfi.utils.logging import LOGGING
-from hyfi.utils.packages import PKGs
 
 logger = LOGGING.getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
 __hydra_default_config_group_value__ = "__init__"
 __hyfi_name__: str = "HyFI"
-__hyfi_config_path__ = "conf"
+__hyfi_config_dirname__ = "conf"
 __hyfi_config_name__ = "config"
-__hyfi_package_name__: str = "hyfi"
+__hyfi_user_config_path__ = "config"
 __hyfi_package_path__: str = Path(__file__).parent.parent.as_posix()
-__hyfi_config_module_path__ = f"{__hyfi_package_name__}.{__hyfi_config_path__}"
+__hyfi_package_name__: str = os.path.basename(__hyfi_package_path__)
+__hyfi_config_module_path__ = f"{__hyfi_package_name__}.{__hyfi_config_dirname__}"
 
 _batcher_instance_ = None
 
 
 def __hyfi_version__() -> str:
     """
     Returns the version of HyFI.
@@ -39,52 +38,57 @@
 
 class GlobalHyFIConfig(BaseModel):
     """Global configuration for HyFI
 
     Attributes:
     __package_name__ (str): The name of the package.
     __package_path__ (str): The path to the package root folder.
+    __version__ (str): The version number of the package.
+    __plugins__ (List[Any]): A list of plugins to load.
     __config_name__ (str): The name of the configuration module.
-    __config_path__ (str): The path to the configuration module.
+    __config_dirname__ (str): The name of the configuration directory.
     __user_config_path__ (str): The path to the user configuration directory.
-    __plugins__ (List[Any]): A list of plugins to load.
-    __version__ (str): The version number of the package.
     """
 
     __package_name__: str = __hyfi_package_name__
     __package_path__: str = __hyfi_package_path__
-    __config_name__: str = __hyfi_config_name__
-    __config_path__: str = __hyfi_config_path__
-    __user_config_path__: str = "config"
-    __plugins__: Optional[List[str]] = None
     __version__: str = __hyfi_version__()
+    __plugins__: Optional[List[str]] = None
+
+    __config_name__: str = __hyfi_config_name__
+    __config_dirname__: str = __hyfi_config_dirname__
+    __user_config_path__: str = __hyfi_user_config_path__
+
+    _packages_: List[Tuple[str, str]] = [(__hyfi_package_path__, __hyfi_version__())]
 
     def initialize(
         self,
-        package_name: str = __hyfi_name__,
+        package_path: str = __hyfi_name__,
         version: str = __hyfi_version__(),
         plugins: Optional[List[str]] = None,
     ) -> None:
         """
         Initializes the global HyFI instance.
 
         This function should be called before any other HyFI function.
 
         A plugin is a python module which contains a configuration module.
 
         Be careful!
         It does not check if the plugin is importable.
 
         Args:
-            package_name: Name of the package. e.g. `hyfi`
+            package_path: Path to the package root folder. e.g. `./src/hyfi`
             version: Version of the package. e.g. `0.1.0`
             plugins: A list of plugins to load. e.g. `["hyfi.conf"]`
         """
-        self.__package_name__ = package_name
+        self.__package_path__ = package_path
         self.__version__ = version
+        if package_path not in self._packages_:
+            self._packages_.append((package_path, version))
         if plugins:
             self.__plugins__ = self.get_plugins(plugins)
 
     @property
     def plugins(self) -> Optional[List[str]]:
         """Returns the list of plugins to load."""
         return self.__plugins__
@@ -98,28 +102,55 @@
 
         Args:
             plugins: List[str]: A list of plugins to load.
         """
         _plugins = []
         for plugin in plugins:
             plugin = plugin.split(".")[0]
-            config_module = f"{plugin}.{self.__config_path__}"
-            # if PKGs.is_importable(config_module):
+            config_module = f"{plugin}.{self.__config_dirname__}"
             _plugins.append(config_module)
         return _plugins
 
     @property
+    def package_name(self) -> str:
+        """Returns the name of the package."""
+        self.__package_name__ = os.path.basename(self.__package_path__)
+        return self.__package_name__
+
+    @property
+    def package_path(self) -> str:
+        """Returns the path to the package root folder.
+
+        If there are multiple packages, the second package is returned.
+        If there is only one package, the first package is returned. (default: hyfi)
+        """
+        if len(self._packages_) > 1:
+            self.__package_path__ = self._packages_[1][0]
+        else:
+            self.__package_path__ = self._packages_[0][0]
+        return self.__package_path__
+
+    @property
     def version(self) -> str:
         """Returns the version number of the package."""
+        if len(self._packages_) > 1:
+            self.__version__ = self._packages_[1][1]
+        else:
+            self.__version__ = self._packages_[0][1]
         return self.__version__
 
     @property
+    def config_dirname(self) -> str:
+        """Returns the name of the configuration directory."""
+        return self.__config_dirname__
+
+    @property
     def config_module(self) -> str:
         """Returns the name of the configuration module."""
-        return f"{self.__package_name__}.{self.__config_path__}"
+        return f"{self.package_name}.{self.config_dirname}"
 
     @property
     def config_module_path(self) -> str:
         """Returns the path to the configuration module."""
         return f"pkg://{self.config_module}"
 
     @property
@@ -196,19 +227,19 @@
     """
     Returns the package name of the App
 
     Returns:
         string containing the package name of the App
     """
 
-    return __global_hyfi__.__package_name__
+    return __global_hyfi__.package_name
 
 
 def __package_path__() -> str:
     """
     Returns the path to the App root folder
 
     Returns:
         string containing the path to the App root folder
     """
 
-    return __global_hyfi__.__package_path__
+    return __global_hyfi__.package_path
```

### Comparing `hyfi-1.9.2/src/hyfi/core/config.py` & `hyfi-1.9.3/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/core/hydra/__init__.py` & `hyfi-1.9.3/src/hyfi/core/hydra/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from hydra._internal.config_search_path_impl import ConfigSearchPathImpl
 from hydra._internal.hydra import Hydra
 from hydra.core.config_search_path import ConfigSearchPath
 from hydra.core.global_hydra import GlobalHydra
 from hydra.core.singleton import Singleton
 from hydra.errors import HydraException
 
-from hyfi.core import __hyfi_config_module_path__, __hyfi_config_path__
+from hyfi.core import __hyfi_config_module_path__
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.packages import PKGs
 
 logger = LOGGING.getLogger(__name__)
 
 
 def get_gh_backup() -> Any:
@@ -28,27 +28,14 @@
 def restore_gh_from_backup(_gh_backup: Any) -> Any:
     if _gh_backup is None:
         del Singleton._instances[GlobalHydra]
     else:
         Singleton._instances[GlobalHydra] = _gh_backup
 
 
-def get_caller_config_module_path(
-    config_path: Optional[str] = __hyfi_config_path__,
-) -> str:
-    """Returns the path to the caller module's config folder"""
-    caller_module_name = PKGs.get_caller_module_name()
-    config_module = caller_module_name.split(".")[0]
-    config_module_path = f"{config_module}.{config_path}"
-    if config_module_path == __hyfi_config_module_path__:
-        return config_module_path
-    # check if the config module is importable
-    return config_module_path if PKGs.is_importable(config_module_path) else ""
-
-
 _UNSPECIFIED_: Any = object()
 
 
 class initialize_config:
     """
     Initializes Hydra and add the config_module to the config search path.
     The config module must be importable (an __init__.py must exist at its top level)
@@ -137,17 +124,14 @@
             if config_module.startswith("pkg://")
             else f"pkg://{config_module}"
             if "." in config_module
             else ""
         )
         append_search_path("main", path, search_path)
 
-    # if caller_config_module := get_caller_config_module_path():
-    #     append_search_path("caller", f"pkg://{caller_config_module}", search_path)
-
     if search_path_dir is not None and os.path.isdir(search_path_dir):
         append_search_path("user", f"file://{search_path_dir}", search_path)
 
     search_path_plugins = Plugins.instance().discover(SearchPathPlugin)
     for spp in search_path_plugins:
         plugin = spp()
         assert isinstance(plugin, SearchPathPlugin)
```

### Comparing `hyfi-1.9.2/src/hyfi/core/hydra/main.py` & `hyfi-1.9.3/src/hyfi/core/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/core/hydra/utils.py` & `hyfi-1.9.3/src/hyfi/core/hydra/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/dotenv/__init__.py` & `hyfi-1.9.3/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/graphics/__init__.py` & `hyfi-1.9.3/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/graphics/collage.py` & `hyfi-1.9.3/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/graphics/motion.py` & `hyfi-1.9.3/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/graphics/utils.py` & `hyfi-1.9.3/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/joblib/__init__.py` & `hyfi-1.9.3/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/joblib/batch/apply.py` & `hyfi-1.9.3/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.9.3/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.9.3/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/main/__init__.py` & `hyfi-1.9.3/src/hyfi/main/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,35 +99,35 @@
     __app_version__ = __app_version__()
 
     def __init__(self) -> None:
         raise NotImplementedError("Use one of the static construction functions")
 
     @staticmethod
     def initialize_global_hyfi(
-        package_name: str,
+        package_path: str,
         version: str,
         plugins: Optional[List[str]] = None,
     ) -> None:
         """
         Initializes the global HyFI instance.
 
         This function should be called before any other HyFI function.
 
         A plugin is a python module which contains a configuration module.
 
         Be careful!
         It does not check if the plugin is importable.
 
         Args:
-            package_name: Name of the package. e.g. `hyfi`
+            package_path: Path to the package root folder. e.g. `./src/hyfi`
             version: Version of the package. e.g. `0.1.0`
             plugins: A list of plugins to load. e.g. `["hyfi.conf"]`
         """
         __global_hyfi__.initialize(
-            package_name=package_name, version=version, plugins=plugins
+            package_path=package_path, version=version, plugins=plugins
         )
 
     @staticmethod
     def about(**args) -> None:
         """Print the about information"""
         __global_config__.print_about(**args)
```

### Comparing `hyfi-1.9.2/src/hyfi/path/__init__.py` & `hyfi-1.9.3/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/path/base.py` & `hyfi-1.9.3/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/path/batch.py` & `hyfi-1.9.3/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/path/dirnames.py` & `hyfi-1.9.3/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/path/task.py` & `hyfi-1.9.3/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/pipe/__init__.py` & `hyfi-1.9.3/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/pipe/datasets.py` & `hyfi-1.9.3/src/hyfi/pipe/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/pipe/test.py` & `hyfi-1.9.3/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/pipeline/__init__.py` & `hyfi-1.9.3/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/pipeline/configs.py` & `hyfi-1.9.3/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/project/__init__.py` & `hyfi-1.9.3/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/task/__init__.py` & `hyfi-1.9.3/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/task/batch.py` & `hyfi-1.9.3/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/conf.py` & `hyfi-1.9.3/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/contexts.py` & `hyfi-1.9.3/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/datasets.py` & `hyfi-1.9.3/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/envs.py` & `hyfi-1.9.3/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/funcs.py` & `hyfi-1.9.3/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/gpumon.py` & `hyfi-1.9.3/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/iolibs.py` & `hyfi-1.9.3/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/logging.py` & `hyfi-1.9.3/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/notebooks.py` & `hyfi-1.9.3/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/utils/packages.py` & `hyfi-1.9.3/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/src/hyfi/workflow/__init__.py` & `hyfi-1.9.3/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.2/PKG-INFO` & `hyfi-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.9.2
+Version: 1.9.3
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

