# Comparing `tmp/lmql-0.0.6.6.tar.gz` & `tmp/lmql-0.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.6.6.tar", last modified: Tue Jul 25 10:40:20 2023, max compression
+gzip compressed data, was "lmql-0.7b1.tar", last modified: Tue Jul 25 15:21:24 2023, max compression
```

## Comparing `lmql-0.0.6.6.tar` & `lmql-0.7b1.tar`

### file list

```diff
@@ -1,316 +1,350 @@
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.646276 lmql-0.0.6.6/.github/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/.github/workflows/
--rw-r--r--   0 docker    (1000) docker    (1000)     2590 2023-07-14 15:52:52.000000 lmql-0.0.6.6/.github/workflows/lmql-ci.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     1543 2023-07-14 11:33:53.000000 lmql-0.0.6.6/.github/workflows/lmql-tests.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     2285 2023-07-20 09:50:34.000000 lmql-0.0.6.6/.github/workflows/lmql-web.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     2743 2023-07-14 11:31:18.000000 lmql-0.0.6.6/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.6/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)      140 2023-07-14 11:31:18.000000 lmql-0.0.6.6/MANIFEST.in
--rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-25 10:40:20.730274 lmql-0.0.6.6/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)     9448 2023-07-14 15:36:31.000000 lmql-0.0.6.6/README.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/
--rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/Makefile
--rw-r--r--   0 docker    (1000) docker    (1000)      444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/RELEASE.md
--rw-r--r--   0 docker    (1000) docker    (1000)      799 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/make.bat
--rw-r--r--   0 docker    (1000) docker    (1000)       81 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/requirements.txt
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_ext/
--rw-r--r--   0 docker    (1000) docker    (1000)     5728 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/_ext/lmql_snippets.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.646276 lmql-0.0.6.6/docs/source/_static/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_static/css/
--rw-r--r--   0 docker    (1000) docker    (1000)     6010 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/_static/css/lmql-docs.css
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_static/images/
--rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/_static/images/lmql.svg
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_static/js/
--rw-r--r--   0 docker    (1000) docker    (1000)     2087 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/_static/js/lmql-playground.js
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_templates/
--rw-r--r--   0 docker    (1000) docker    (1000)      292 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/_templates/layout.html
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.658276 lmql-0.0.6.6/docs/source/blog/
--rw-r--r--   0 docker    (1000) docker    (1000)     4591 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.1.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2068 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.3.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3221 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.4.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5872 2023-07-20 09:50:34.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)     8976 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1167 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/conf.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1293 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/dev-setup.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2333 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/docker-setup.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.658276 lmql-0.0.6.6/docs/source/images/
--rw-r--r--   0 docker    (1000) docker    (1000)   125712 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/images/inference.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     2823 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/index.rst
--rw-r--r--   0 docker    (1000) docker    (1000)     2563 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/installation.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.658276 lmql-0.0.6.6/docs/source/language/
--rw-r--r--   0 docker    (1000) docker    (1000)     2313 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/azure.md
--rw-r--r--   0 docker    (1000) docker    (1000)     7435 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/constraints.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5365 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/decoders.md
--rw-r--r--   0 docker    (1000) docker    (1000)     7850 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/functions.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3967 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/hf.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2027 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/llama.cpp.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2896 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/models.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5710 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/openai.md
--rw-r--r--   0 docker    (1000) docker    (1000)     8292 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/overview.md
--rw-r--r--   0 docker    (1000) docker    (1000)     6032 2023-07-20 09:50:34.000000 lmql-0.0.6.6/docs/source/language/scripted_prompts.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)    28444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/logo.png
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.662275 lmql-0.0.6.6/docs/source/pending/
--rw-r--r--   0 docker    (1000) docker    (1000)     3550 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/pending/release-next.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.666275 lmql-0.0.6.6/docs/source/python/
--rw-r--r--   0 docker    (1000) docker    (1000)       11 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)     4924 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/comparison.md
--rw-r--r--   0 docker    (1000) docker    (1000)    11193 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/langchain.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     1157 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/lc.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6681 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/llama_index.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)    75148 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/lmql.txt
--rw-r--r--   0 docker    (1000) docker    (1000)     7458 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/output.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     9592 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/pandas.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)    13317 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/python.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     4806 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/quickstart.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.666275 lmql-0.0.6.6/docs/source/releases/
--rw-r--r--   0 docker    (1000) docker    (1000)     2263 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/releases/misc-snippets.md
--rw-r--r--   0 docker    (1000) docker    (1000)      321 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/releases/release-0.0.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)      257 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/todo.md
--rw-r--r--   0 docker    (1000) docker    (1000)      137 2023-07-14 11:31:18.000000 lmql-0.0.6.6/pyproject.toml
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.670275 lmql-0.0.6.6/scripts/
--rw-r--r--   0 docker    (1000) docker    (1000)      577 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/Dockerfile
--rw-r--r--   0 docker    (1000) docker    (1000)      295 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/activate-dev.sh
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.670275 lmql-0.0.6.6/scripts/conda/
--rw-r--r--   0 docker    (1000) docker    (1000)      198 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/conda/requirements-no-gpu.yml
--rw-r--r--   0 docker    (1000) docker    (1000)      332 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/conda/requirements.yml
--rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/pypi-release.sh
--rw-r--r--   0 docker    (1000) docker    (1000)     3897 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/serve-all.py
--rw-r--r--   0 docker    (1000) docker    (1000)      854 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/wheel.sh
--rw-r--r--   0 docker    (1000) docker    (1000)      868 2023-07-25 10:40:20.730274 lmql-0.0.6.6/setup.cfg
--rw-r--r--   0 docker    (1000) docker    (1000)       37 2023-07-14 11:31:18.000000 lmql-0.0.6.6/setup.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.670275 lmql-0.0.6.6/src/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.674275 lmql-0.0.6.6/src/lmql/
--rw-r--r--   0 docker    (1000) docker    (1000)     7767 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.674275 lmql-0.0.6.6/src/lmql/algorithms/
--rw-r--r--   0 docker    (1000) docker    (1000)       45 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/algorithms/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2696 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/algorithms/cache.py
--rw-r--r--   0 docker    (1000) docker    (1000)      926 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/algorithms/functools.py
--rwxr-xr-x   0 docker    (1000) docker    (1000)     8313 2023-07-14 11:38:09.000000 lmql-0.0.6.6/src/lmql/cli.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1578 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/demo.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1531 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/http.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.678275 lmql-0.0.6.6/src/lmql/language/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/language/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    29360 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/language/compiler.py
--rw-r--r--   0 docker    (1000) docker    (1000)    11042 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/language/fragment_parser.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4545 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/language/qstrings.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1804 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/language/validator.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.678275 lmql-0.0.6.6/src/lmql/models/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.682275 lmql-0.0.6.6/src/lmql/models/lmtp/
--rw-r--r--   0 docker    (1000) docker    (1000)     6156 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/README.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.682275 lmql-0.0.6.6/src/lmql/models/lmtp/backends/
--rw-r--r--   0 docker    (1000) docker    (1000)      493 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)      694 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/__main__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4362 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/llama_cpp_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/lmtp_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2002 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/random_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4327 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/transformers_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)       42 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/errors.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4669 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_async.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5645 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_client.py
--rw-r--r--   0 docker    (1000) docker    (1000)    20135 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_dcmodel.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2283 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_inference_server.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5606 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_multiprocessing.py
--rw-r--r--   0 docker    (1000) docker    (1000)      298 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
--rw-r--r--   0 docker    (1000) docker    (1000)    15201 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_scheduler.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6381 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_serve.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3562 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_threading.py
--rw-r--r--   0 docker    (1000) docker    (1000)      634 2023-07-14 15:36:31.000000 lmql-0.0.6.6/src/lmql/models/lmtp/utils.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3396 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/model.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.682275 lmql-0.0.6.6/src/lmql/ops/
--rw-r--r--   0 docker    (1000) docker    (1000)       93 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ops/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     7542 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ops/follow_map.py
--rw-r--r--   0 docker    (1000) docker    (1000)    42177 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/ops/ops.py
--rw-r--r--   0 docker    (1000) docker    (1000)    21170 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ops/token_set.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.686275 lmql-0.0.6.6/src/lmql/output/
--rw-r--r--   0 docker    (1000) docker    (1000)       57 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2334 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/http.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1889 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/sse.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2282 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/ws.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/bopenai/
--rw-r--r--   0 docker    (1000) docker    (1000)     2236 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/bopenai/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    29628 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/bopenai/batched_openai.py
--rw-r--r--   0 docker    (1000) docker    (1000)    21823 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/bopenai/openai_api.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2096 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/caching.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/dclib/
--rw-r--r--   0 docker    (1000) docker    (1000)      494 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    18839 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_array.py
--rw-r--r--   0 docker    (1000) docker    (1000)    26354 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_cache.py
--rw-r--r--   0 docker    (1000) docker    (1000)      592 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_global.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4970 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     8589 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-r--r--   0 docker    (1000) docker    (1000)    32348 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_seq.py
--rw-r--r--   0 docker    (1000) docker    (1000)    22035 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/decoders.py
--rw-r--r--   0 docker    (1000) docker    (1000)    39830 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/interpreter.py
--rw-r--r--   0 docker    (1000) docker    (1000)      250 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/interrupt.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1231 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/langchain.py
--rw-r--r--   0 docker    (1000) docker    (1000)    10237 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/lmql_runtime.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1940 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/loop.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1245 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/maiohttp.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1726 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/masks.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3145 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/model_registry.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5943 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/multi_head_interpretation.py
--rw-r--r--   0 docker    (1000) docker    (1000)    44838 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/openai_integration.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2179 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/openai_secret.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4042 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/output_writer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/postprocessing/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/postprocessing/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3543 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-r--r--   0 docker    (1000) docker    (1000)      152 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/postprocessing/group_by.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2209 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/program_state.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1317 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/stats.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2220 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/token_distribution.py
--rw-r--r--   0 docker    (1000) docker    (1000)    11565 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/tokenizers/
--rw-r--r--   0 docker    (1000) docker    (1000)     4509 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizers/hf_tokenizer.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3427 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3207 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.694275 lmql-0.0.6.6/src/lmql/tests/
--rw-r--r--   0 docker    (1000) docker    (1000)      319 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)      907 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/tests/all.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5914 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/tests/expr_test_utils.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1314 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/fin_and.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/tests/outdated/
--rw-r--r--   0 docker    (1000) docker    (1000)     1611 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/mask_product_test.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2789 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/monotonicity.py
--rw-r--r--   0 docker    (1000) docker    (1000)      546 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/one_of_tests.py
--rw-r--r--   0 docker    (1000) docker    (1000)      758 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/sentences_op.py
--rw-r--r--   0 docker    (1000) docker    (1000)      984 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/starts_with_op_test.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1236 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/stops_at.py
--rw-r--r--   0 docker    (1000) docker    (1000)      537 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/str_in_str_tests.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4738 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/test_multi_head.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3036 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/token_set_test.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/tests/queryargs/
--rw-r--r--   0 docker    (1000) docker    (1000)     4489 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_args.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2072 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_query_str.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1095 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_run.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1066 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_sync.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1092 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_var_errors.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/tests/system/
--rw-r--r--   0 docker    (1000) docker    (1000)     3402 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/system/basic_use_cases.py
--rw-r--r--   0 docker    (1000) docker    (1000)      842 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/tail_token_set.py
--rw-r--r--   0 docker    (1000) docker    (1000)      788 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_back2back_caching.py
--rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_beam_in.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2775 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_eq.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1756 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_escaping.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2370 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/tests/test_f.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1033 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/tests/test_local_model_python.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_minimal_syntax.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1139 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_multibyte_characters.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1171 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_multibyte_local_models.py
--rw-r--r--   0 docker    (1000) docker    (1000)      457 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_orop.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2931 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_qstrings.py
--rw-r--r--   0 docker    (1000) docker    (1000)      479 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_query_args.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2639 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_sample_queries.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1703 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_scoping.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3647 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_stopping.py
--rw-r--r--   0 docker    (1000) docker    (1000)      707 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/tiktoken_tsets.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/ui/
--rw-r--r--   0 docker    (1000) docker    (1000)       27 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/ui/live/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6747 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/live.js
--rw-r--r--   0 docker    (1000) docker    (1000)     3475 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/live.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3885 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/livelib.py
--rw-r--r--   0 docker    (1000) docker    (1000)      349 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/package.json
--rw-r--r--   0 docker    (1000) docker    (1000)    33701 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/yarn.lock
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.702275 lmql-0.0.6.6/src/lmql/ui/playground/
--rw-r--r--   0 docker    (1000) docker    (1000)       31 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/.dockerignore
--rw-r--r--   0 docker    (1000) docker    (1000)       34 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/.env
--rw-r--r--   0 docker    (1000) docker    (1000)      310 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)      354 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/Dockerfile
--rw-r--r--   0 docker    (1000) docker    (1000)     3359 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1327 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/package.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.702275 lmql-0.0.6.6/src/lmql/ui/playground/public/
--rw-r--r--   0 docker    (1000) docker    (1000)       90 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/_headers
--rw-r--r--   0 docker    (1000) docker    (1000)     3870 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/favicon.ico
--rw-r--r--   0 docker    (1000) docker    (1000)     1678 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/index.html
--rw-r--r--   0 docker    (1000) docker    (1000)     2817 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)      306 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/manifest.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.718274 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/
--rw-r--r--   0 docker    (1000) docker    (1000)  1227728 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/calc.json
--rw-r--r--   0 docker    (1000) docker    (1000)   295285 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/chat.json
--rw-r--r--   0 docker    (1000) docker    (1000)   160131 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/cot.json
--rw-r--r--   0 docker    (1000) docker    (1000)    81768 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-r--r--   0 docker    (1000) docker    (1000)    22895 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/hello.json
--rw-r--r--   0 docker    (1000) docker    (1000)    89531 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/joke.json
--rw-r--r--   0 docker    (1000) docker    (1000)   265372 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/json-template.json
--rw-r--r--   0 docker    (1000) docker    (1000)  1710847 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/kv.json
--rw-r--r--   0 docker    (1000) docker    (1000)    52748 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/list.json
--rw-r--r--   0 docker    (1000) docker    (1000)   628184 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/meta.json
--rw-r--r--   0 docker    (1000) docker    (1000)   264768 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/translation.json
--rw-r--r--   0 docker    (1000) docker    (1000)   215050 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-r--r--   0 docker    (1000) docker    (1000)       67 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/robots.txt
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.718274 lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/
--rw-r--r--   0 docker    (1000) docker    (1000)   381736 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-r--r--   0 docker    (1000) docker    (1000)   184008 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-r--r--   0 docker    (1000) docker    (1000)       62 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/ref.py
--rw-r--r--   0 docker    (1000) docker    (1000)       80 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/run-in-docker.sh
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.726274 lmql-0.0.6.6/src/lmql/ui/playground/src/
--rw-r--r--   0 docker    (1000) docker    (1000)    75521 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/App.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      246 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/App.test.js
--rw-r--r--   0 docker    (1000) docker    (1000)    29983 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      807 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/Configuration.js
--rw-r--r--   0 docker    (1000) docker    (1000)     1174 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/DataListView.js
--rw-r--r--   0 docker    (1000) docker    (1000)    21617 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/DecoderGraph.js
--rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/DecodingTree.js
--rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/Embed.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)     9601 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/Explore.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      675 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/SharedState.js
--rw-r--r--   0 docker    (1000) docker    (1000)     4819 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/State.js
--rw-r--r--   0 docker    (1000) docker    (1000)     5871 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)     9360 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/browser_process.js
--rw-r--r--   0 docker    (1000) docker    (1000)     1163 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/build_info.js
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.726274 lmql-0.0.6.6/src/lmql/ui/playground/src/editor/
--rw-r--r--   0 docker    (1000) docker    (1000)     8696 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-r--r--   0 docker    (1000) docker    (1000)     4758 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/editor/theme.json
--rw-r--r--   0 docker    (1000) docker    (1000)      889 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/explore.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     1345 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/graph-layout.css
--rw-r--r--   0 docker    (1000) docker    (1000)     1698 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/index.css
--rw-r--r--   0 docker    (1000) docker    (1000)      489 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/index.js
--rw-r--r--   0 docker    (1000) docker    (1000)     2632 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/logo.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     8766 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/queries.js
--rw-r--r--   0 docker    (1000) docker    (1000)     5990 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/remote_process.js
--rw-r--r--   0 docker    (1000) docker    (1000)      362 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/reportWebVitals.js
--rw-r--r--   0 docker    (1000) docker    (1000)     9520 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/screenshot.css
--rw-r--r--   0 docker    (1000) docker    (1000)      241 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/setupTests.js
--rw-r--r--   0 docker    (1000) docker    (1000)     3466 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/spinner.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     3200 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/tagged-model-result.js
--rw-r--r--   0 docker    (1000) docker    (1000)   449905 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/yarn.lock
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/ui/vscode/
--rw-r--r--   0 docker    (1000) docker    (1000)       76 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.gitattributes
--rw-r--r--   0 docker    (1000) docker    (1000)       19 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.gitignore
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/ui/vscode/.vscode/
--rw-r--r--   0 docker    (1000) docker    (1000)      540 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.vscode/launch.json
--rw-r--r--   0 docker    (1000) docker    (1000)       66 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.vscodeignore
--rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)      959 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/language-configuration.json
--rw-r--r--   0 docker    (1000) docker    (1000)    11532 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/lmql-vscode.png
--rw-r--r--   0 docker    (1000) docker    (1000)     1214 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/package.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/
--rw-r--r--   0 docker    (1000) docker    (1000)      518 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-r--r--   0 docker    (1000) docker    (1000)      642 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-r--r--   0 docker    (1000) docker    (1000)      853 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/utils/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2402 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/docstring_parser.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4933 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/graph.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2715 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/nputil.py
--rw-r--r--   0 docker    (1000) docker    (1000)      114 2023-07-25 10:40:12.000000 lmql-0.0.6.6/src/lmql/version.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.674275 lmql-0.0.6.6/src/lmql.egg-info/
--rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)     9166 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/SOURCES.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/dependency_links.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       39 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/entry_points.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       95 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/requires.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        5 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/top_level.txt
--rw-r--r--   0 docker    (1000) docker    (1000)   115785 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)       86 2023-07-14 11:31:18.000000 lmql-0.0.6.6/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.237754 lmql-0.7b1/.github/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.241754 lmql-0.7b1/.github/workflows/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2590 2023-07-14 15:52:52.000000 lmql-0.7b1/.github/workflows/lmql-ci.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     1543 2023-07-14 11:33:53.000000 lmql-0.7b1/.github/workflows/lmql-tests.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2372 2023-07-25 13:45:45.000000 lmql-0.7b1/.github/workflows/lmql-web.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2743 2023-07-14 11:31:18.000000 lmql-0.7b1/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.7b1/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      140 2023-07-14 11:31:18.000000 lmql-0.7b1/MANIFEST.in
+-rw-r--r--   0 docker    (1000) docker    (1000)     9896 2023-07-25 15:21:24.281753 lmql-0.7b1/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)     9448 2023-07-14 15:36:31.000000 lmql-0.7b1/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.241754 lmql-0.7b1/docs/
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/Makefile
+-rw-r--r--   0 docker    (1000) docker    (1000)      444 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/RELEASE.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      799 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/make.bat
+-rw-r--r--   0 docker    (1000) docker    (1000)       81 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/requirements.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_ext/
+-rw-r--r--   0 docker    (1000) docker    (1000)     5728 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/_ext/lmql_snippets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.237754 lmql-0.7b1/docs/source/_static/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_static/css/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6010 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/_static/css/lmql-docs.css
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_static/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/_static/images/lmql.svg
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_static/js/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2087 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/_static/js/lmql-playground.js
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_templates/
+-rw-r--r--   0 docker    (1000) docker    (1000)      292 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/_templates/layout.html
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/blog/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4591 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.1.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2068 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.3.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3221 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.4.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5872 2023-07-20 09:50:34.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1445 2023-07-25 13:45:45.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.6.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8976 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1167 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/conf.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1293 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/dev-setup.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2333 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/docker-setup.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)   125712 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/images/inference.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     2823 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/index.rst
+-rw-r--r--   0 docker    (1000) docker    (1000)     2563 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/installation.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2313 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/azure.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     7435 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/constraints.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5365 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/decoders.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     7850 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/functions.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3967 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/hf.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2027 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/llama.cpp.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2896 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/models.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5710 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/openai.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8292 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/overview.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     6032 2023-07-20 09:50:34.000000 lmql-0.7b1/docs/source/language/scripted_prompts.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)    28444 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/logo.png
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/pending/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3550 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/pending/release-next.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/docs/source/python/
+-rw-r--r--   0 docker    (1000) docker    (1000)       11 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)     4924 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/comparison.md
+-rw-r--r--   0 docker    (1000) docker    (1000)    11193 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/langchain.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     1157 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/lc.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6681 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/llama_index.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    75148 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/lmql.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)     7458 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/output.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     9592 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/pandas.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    13317 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/python.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     4806 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/quickstart.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/docs/source/releases/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2263 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/releases/misc-snippets.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      321 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/releases/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      257 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/todo.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      137 2023-07-14 11:31:18.000000 lmql-0.7b1/pyproject.toml
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/scripts/
+-rw-r--r--   0 docker    (1000) docker    (1000)      577 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)      295 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/activate-dev.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-25 13:45:45.000000 lmql-0.7b1/scripts/changelog.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/scripts/conda/
+-rw-r--r--   0 docker    (1000) docker    (1000)      198 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/conda/requirements-no-gpu.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      332 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/conda/requirements.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/pypi-release.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)     3897 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/serve-all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      854 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/wheel.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)      866 2023-07-25 15:21:24.281753 lmql-0.7b1/setup.cfg
+-rw-r--r--   0 docker    (1000) docker    (1000)       37 2023-07-14 11:31:18.000000 lmql-0.7b1/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/lmql/
+-rw-r--r--   0 docker    (1000) docker    (1000)        6 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)     8078 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/lmql/algorithms/
+-rw-r--r--   0 docker    (1000) docker    (1000)       45 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/algorithms/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2763 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/algorithms/cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      942 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/algorithms/functools.py
+-rwxr-xr-x   0 docker    (1000) docker    (1000)     8644 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/cli.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1577 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/demo.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1531 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/http.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/language/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    32080 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/language/compiler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11442 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/language/fragment_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4700 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/language/qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1804 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/language/validator.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/lib/
+-rw-r--r--   0 docker    (1000) docker    (1000)      143 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    12764 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/lib/actions.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    61974 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/algebra222.csv
+-rw-r--r--   0 docker    (1000) docker    (1000)     5225 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/data.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/lib/prompts/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1682 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_code copy.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1625 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_code.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1450 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_use.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1694 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_use_kevin.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5900 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/wiki_prompt.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     7473 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/types.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      942 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/value.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/models/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/models/lmtp/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6156 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/models/lmtp/backends/
+-rw-r--r--   0 docker    (1000) docker    (1000)      493 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      694 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/__main__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4362 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/llama_cpp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/lmtp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2002 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/random_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4327 2023-07-20 09:50:34.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/transformers_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       42 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/errors.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4669 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_async.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5645 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_client.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    20210 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_dcmodel.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2283 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_inference_server.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5606 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_multiprocessing.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      298 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    15201 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_scheduler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6381 2023-07-20 09:50:34.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_serve.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3562 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_threading.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      634 2023-07-14 15:36:31.000000 lmql-0.7b1/src/lmql/models/lmtp/utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3396 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/model.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/ops/
+-rw-r--r--   0 docker    (1000) docker    (1000)       93 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ops/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1656 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/booleans.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8088 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/follow_map.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4377 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/inline_call.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8362 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/node.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    37311 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/ops.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8370 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/regex.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21352 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/token_set.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/output/
+-rw-r--r--   0 docker    (1000) docker    (1000)       57 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2334 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/http.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1889 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/sse.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2282 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/ws.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/runtime/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/runtime/bopenai/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2236 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/bopenai/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    29922 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/bopenai/batched_openai.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21823 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/runtime/bopenai/openai_api.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2096 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/caching.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/runtime/dclib/
+-rw-r--r--   0 docker    (1000) docker    (1000)      494 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    18839 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_array.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    26386 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      592 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_global.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4970 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     9585 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    33321 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_seq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    22268 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/decoders.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    52685 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/runtime/interpreter.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      250 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/interrupt.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1231 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/langchain.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11319 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/lmql_runtime.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1940 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/loop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1245 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/maiohttp.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1726 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/masks.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3145 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/runtime/model_registry.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5965 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/multi_head_interpretation.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    45053 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/openai_integration.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2179 2023-07-20 09:50:34.000000 lmql-0.7b1/src/lmql/runtime/openai_secret.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4038 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/output_writer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/runtime/postprocessing/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/postprocessing/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3543 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      152 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/postprocessing/group_by.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2298 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/program_state.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1317 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/stats.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2220 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/token_distribution.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    12577 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/runtime/tokenizers/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4509 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/tokenizers/hf_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3427 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3207 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/tests/
+-rw-r--r--   0 docker    (1000) docker    (1000)      319 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1018 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/tests/all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5916 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/tests/expr_test_utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1314 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/fin_and.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/tests/outdated/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1611 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/mask_product_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2789 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/monotonicity.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      546 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/one_of_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      758 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/sentences_op.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      984 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1236 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/stops_at.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      537 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4738 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/test_multi_head.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3036 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/token_set_test.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/tests/queryargs/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4489 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2072 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_args_query_str.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1095 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_args_run.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1066 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_sync.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1092 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_var_errors.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/tests/system/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3402 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/system/basic_use_cases.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      842 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/tail_token_set.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      788 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_back2back_caching.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_beam_in.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2775 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_eq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1756 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_escaping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2370 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/tests/test_f.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1033 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/tests/test_local_model_python.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_minimal_syntax.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1139 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_multibyte_characters.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1171 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_multibyte_local_models.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      457 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_orop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2931 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      479 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_query_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2639 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_sample_queries.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1703 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_scoping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3647 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_stopping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      707 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/tiktoken_tsets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/
+-rw-r--r--   0 docker    (1000) docker    (1000)       27 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/chat/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6267 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/__main__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/chat/assets/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1665 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/code.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     7015 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/index.css
+-rw-r--r--   0 docker    (1000) docker    (1000)     8687 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/index.html
+-rw-r--r--   0 docker    (1000) docker    (1000)     8689 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/lmql-monaco.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)      551 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/send.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     7853 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/studio.css
+-rw-r--r--   0 docker    (1000) docker    (1000)    13744 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/studio.html
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/live/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6747 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/live.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3475 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/live.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3885 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/livelib.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      349 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/package.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    33701 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.269753 lmql-0.7b1/src/lmql/ui/playground/
+-rw-r--r--   0 docker    (1000) docker    (1000)       31 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/.dockerignore
+-rw-r--r--   0 docker    (1000) docker    (1000)       34 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/.env
+-rw-r--r--   0 docker    (1000) docker    (1000)      310 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)      354 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)     3359 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1327 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.269753 lmql-0.7b1/src/lmql/ui/playground/public/
+-rw-r--r--   0 docker    (1000) docker    (1000)       90 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/_headers
+-rw-r--r--   0 docker    (1000) docker    (1000)     3870 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/favicon.ico
+-rw-r--r--   0 docker    (1000) docker    (1000)     1678 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/index.html
+-rw-r--r--   0 docker    (1000) docker    (1000)     2817 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)      306 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/manifest.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.273753 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/
+-rw-r--r--   0 docker    (1000) docker    (1000)  1227728 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   295285 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   160131 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    13974 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/date-regex.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    81768 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    22895 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    89531 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   484450 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/json-robust.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   265372 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/json-template.json
+-rw-r--r--   0 docker    (1000) docker    (1000)  1710847 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    52748 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/list.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   628184 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   264768 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   215050 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       67 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/robots.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.273753 lmql-0.7b1/src/lmql/ui/playground/public/snippets/
+-rw-r--r--   0 docker    (1000) docker    (1000)   381736 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   184008 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       62 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/ref.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       80 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/run-in-docker.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.277753 lmql-0.7b1/src/lmql/ui/playground/src/
+-rw-r--r--   0 docker    (1000) docker    (1000)    76544 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/App.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      246 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/App.test.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    29983 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      961 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/Configuration.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1174 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/DataListView.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    21726 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/DecodingTree.js
+-rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/Embed.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)    12240 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/ui/playground/src/Explore.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      675 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/SharedState.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4819 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/State.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5871 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)     9360 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/browser_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1163 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/build_info.js
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.277753 lmql-0.7b1/src/lmql/ui/playground/src/editor/
+-rw-r--r--   0 docker    (1000) docker    (1000)     9032 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4758 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/editor/theme.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      889 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/explore.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     1345 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/graph-layout.css
+-rw-r--r--   0 docker    (1000) docker    (1000)     1698 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/index.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      489 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/index.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     2632 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/logo.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)    12203 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/ui/playground/src/queries.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5990 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/remote_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      362 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     9520 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/screenshot.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      241 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/setupTests.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3466 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/spinner.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     3200 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-r--r--   0 docker    (1000) docker    (1000)   449905 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/ui/vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)       76 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.gitattributes
+-rw-r--r--   0 docker    (1000) docker    (1000)       19 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.gitignore
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/ui/vscode/.vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)      540 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.vscode/launch.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       66 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.vscodeignore
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      959 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/language-configuration.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    11532 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/lmql-vscode.png
+-rw-r--r--   0 docker    (1000) docker    (1000)     1214 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/
+-rw-r--r--   0 docker    (1000) docker    (1000)      518 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      642 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      853 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/utils/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2402 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/docstring_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4933 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/graph.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2715 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/nputil.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      112 2023-07-25 15:21:16.000000 lmql-0.7b1/src/lmql/version.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/lmql.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)     9896 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)    10123 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       39 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/entry_points.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       95 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        5 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)   115785 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)       86 2023-07-14 11:31:18.000000 lmql-0.7b1/yarn.lock
```

### Comparing `lmql-0.0.6.6/.github/workflows/lmql-ci.yml` & `lmql-0.7b1/.github/workflows/lmql-ci.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/.github/workflows/lmql-tests.yml` & `lmql-0.7b1/.github/workflows/lmql-tests.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/.github/workflows/lmql-web.yml` & `lmql-0.7b1/.github/workflows/lmql-web.yml`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,17 @@
       ', github.ref)
     steps:
     - uses: actions/checkout@master
     - uses: actions/download-artifact@master
       with:
         name: lmql-web-payload
         path: web-deploy
-    - run: cp web-deploy/index-next.html web-deploy/index.html
+    - run: cp -r web-deploy/playground/* web-deploy/
     - name: Deploy to web branch
       uses: JamesIves/github-pages-deploy-action@v4
       with:
+        repository-name: lmql-lang/lmql-next
+        ssh-key: ${{ secrets.LMQL_LANG_NEXT_PUSH_KEY }} 
         folder: web-deploy
-        branch: web-next
+        branch: web
```

### Comparing `lmql-0.0.6.6/.gitignore` & `lmql-0.7b1/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/LICENSE` & `lmql-0.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/PKG-INFO` & `lmql-0.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.6
+Version: 0.7b1
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.6 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.7b1 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6.6/README.md` & `lmql-0.7b1/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/Makefile` & `lmql-0.7b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/make.bat` & `lmql-0.7b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/_ext/lmql_snippets.py` & `lmql-0.7b1/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/_static/css/lmql-docs.css` & `lmql-0.7b1/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/_static/images/lmql.svg` & `lmql-0.7b1/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/_static/js/lmql-playground.js` & `lmql-0.7b1/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/blog/release-0.0.5.md` & `lmql-0.7b1/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/blog/release-0.0.6.1.md` & `lmql-0.7b1/docs/source/blog/release-0.0.6.1.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/blog/release-0.0.6.3.md` & `lmql-0.7b1/docs/source/blog/release-0.0.6.3.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/blog/release-0.0.6.4.md` & `lmql-0.7b1/docs/source/blog/release-0.0.6.4.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/blog/release-0.0.6.5.md` & `lmql-0.7b1/docs/source/blog/release-0.0.6.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/blog/release-0.0.6.md` & `lmql-0.7b1/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/conf.py` & `lmql-0.7b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/dev-setup.md` & `lmql-0.7b1/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/docker-setup.md` & `lmql-0.7b1/docs/source/docker-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/images/inference.svg` & `lmql-0.7b1/docs/source/images/inference.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/index.rst` & `lmql-0.7b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/installation.md` & `lmql-0.7b1/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/azure.md` & `lmql-0.7b1/docs/source/language/azure.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/constraints.md` & `lmql-0.7b1/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/decoders.md` & `lmql-0.7b1/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/functions.md` & `lmql-0.7b1/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/hf.md` & `lmql-0.7b1/docs/source/language/hf.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/llama.cpp.md` & `lmql-0.7b1/docs/source/language/llama.cpp.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/models.md` & `lmql-0.7b1/docs/source/language/models.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/openai.md` & `lmql-0.7b1/docs/source/language/openai.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/overview.md` & `lmql-0.7b1/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/language/scripted_prompts.md` & `lmql-0.7b1/docs/source/language/scripted_prompts.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/lmql.svg` & `lmql-0.7b1/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/logo.png` & `lmql-0.7b1/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/pending/release-next.md` & `lmql-0.7b1/docs/source/pending/release-next.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/comparison.md` & `lmql-0.7b1/docs/source/python/comparison.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/langchain.ipynb` & `lmql-0.7b1/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/lc.py` & `lmql-0.7b1/docs/source/python/lc.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/llama_index.ipynb` & `lmql-0.7b1/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/lmql.txt` & `lmql-0.7b1/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/output.ipynb` & `lmql-0.7b1/docs/source/python/output.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/pandas.ipynb` & `lmql-0.7b1/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/python/python.ipynb` & `lmql-0.7b1/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/quickstart.md` & `lmql-0.7b1/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/docs/source/releases/misc-snippets.md` & `lmql-0.7b1/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/scripts/Dockerfile` & `lmql-0.7b1/scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/scripts/pypi-release.sh` & `lmql-0.7b1/scripts/pypi-release.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/scripts/serve-all.py` & `lmql-0.7b1/scripts/serve-all.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/scripts/wheel.sh` & `lmql-0.7b1/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/setup.cfg` & `lmql-0.7b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.6.6
+version = 0.7b1
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.6.6/src/lmql/__init__.py` & `lmql-0.7b1/src/lmql/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # re-export lmql runtime functions
 from lmql.runtime.lmql_runtime import (FunctionContext, LMQLInputVariableScope,
                                        LMQLQueryFunction, compiled_query, tag,
                                        EmptyVariableScope)
 from lmql.runtime.model_registry import LMQLModelRegistry
 from lmql.runtime.output_writer import headless, printing, silent, stream
 from lmql.runtime.interpreter import LMQLResult
+
 from lmql.models.model import model
 from lmql.runtime.loop import main
 
 from typing import Optional
 
 model_registry = LMQLModelRegistry
 
@@ -193,21 +194,32 @@
 
     def lmql_query_wrapper(*args, **kwargs):
         return module.query(*args, **kwargs)
 
     # copy some attributes of model.query to the wrapper function
     for attr in ["aschain", "lmql_code", "is_async", "output_variables"]:
         setattr(lmql_query_wrapper, attr, getattr(module.query, attr))
+    setattr(lmql_query_wrapper, "__lmql_query_function__", module.query)
 
     return lmql_query_wrapper
 
 async def static_prompt(query_fct, *args, **kwargs):
     """
     Returns the static prompt prefix that is generated by the given query function up until the first variable.
     """
     res = await query_fct(*args, **kwargs, return_prompt_string=True)
     return res[0]
 
+def main(query_fct, *args, **kwargs):
+    """
+    Runs the provided query function in the main thread
+    and returns the result.
+
+    This call is blocking.
+    """
+    import asyncio
+    return asyncio.run(query_fct(*args, **kwargs))
+
 def serve(*args, **kwargs):
     assert not "LMQL_BROWSER" in os.environ, "lmql.serve is not available in the browser distribution of LMQL."
     from lmql.models.lmtp.lmtp_serve import serve
     return serve(*args, **kwargs)
```

### Comparing `lmql-0.0.6.6/src/lmql/algorithms/cache.py` & `lmql-0.7b1/src/lmql/algorithms/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pickle
 import os
 import inspect
 
 from lmql.runtime.lmql_runtime import LMQLQueryFunction
+import lmql
 from lmql import LMQLResult, F
 
 # cache query results by query code and arguments
 global cache_file
 cache_file = None
 global cache
 cache = None
@@ -42,58 +43,62 @@
 def persist_cache():
     global cache
     global cache_file
     if cache is not None and cache_file is not None:
         with open(cache_file, "wb") as f:
             pickle.dump(cache, f)
 
+
 async def apply(q, *args, **kwargs):
     global cache
 
     if type(q) is str:
         where = kwargs.pop("where", None)
         q = F(q, constraints=where, is_async=True)
 
+    lmql_code = q.lmql_code
+
     # handle non-LMQL queries
     if type(q) is not LMQLQueryFunction:
         if inspect.iscoroutinefunction(q):
             return await q(*args)
         return q(*args)
 
     global stats
     stats["total"] += 1
 
     # get source code for q.__fct__
     try:
         # convert dict to list
         key_args = [tuple(sorted(list(a.items()))) if type(a) is dict else a for a in args]
         key_args = [tuple(a) if type(a) is list else a for a in key_args]
-        key = (q.lmql_code, *key_args).__hash__()
-        key = (q.lmql_code, *key_args)
+        key = (lmql_code, *key_args).__hash__()
+        key = (lmql_code, *key_args)
     except:
         print("warning: cannot hash LMQL query arguments {}. Change the argument types to be hashable.".format(args))
-        key = str(q.lmql_code) + str(args)
+        key = str(lmql_code) + str(args)
     
     if cache is not None and key in cache.keys():
         stats["cached"] += 1
         return cache[key]
     else:
+        kwargs = {}
         try:
             result = await q(*args, **kwargs)
             if len(result) == 1:
                 result = result[0]
             if type(result) is LMQLResult:
                 if "RESULT" in result.variables.keys():
                     result = result.variables["RESULT"].strip()
 
             if cache is not None:
                 cache[key] = result
                 persist_cache()
         except Exception as e:
-            print("Failed for args: {}".format(args), flush=True)
+            print("Failed for args: {} {}".format(args, kwargs), flush=True)
             raise e
 
         return result
 
 def get_stats():
     global stats
     return "lmql.algorithms Stats: Total queries: {}, Cached queries: {}".format(stats["total"], stats["cached"])
```

### Comparing `lmql-0.0.6.6/src/lmql/algorithms/functools.py` & `lmql-0.7b1/src/lmql/algorithms/functools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import sys
 from .cache import apply
 
-async def map(q, items, chunksize=None, progress=False, **kwargs):
+async def map(q, items, chunksize=None, progress=False, parameter=None, **kwargs):
     chunks = []
     if chunksize is None:
         chunksize = len(items)
     for i in range(0, len(items), chunksize):
         chunks.append(items[i:i+chunksize])
     
     total_results = []
```

### Comparing `lmql-0.0.6.6/src/lmql/cli.py` & `lmql-0.7b1/src/lmql/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,24 @@
 project_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 def cmd_serve_model():
     """emoji:🏄 Serve a 🤗 Transformers model via the LMQL inference API"""
     os.chdir(project_root)
     os.system("python -m lmql.models.lmtp.lmtp_serve " + " ".join(sys.argv[2:]))
 
+def cmd_chat():
+    """emoji:💬 Serve a given query file as an interactive LMQL chatbot"""
+    if len(sys.argv) == 2:
+        print("Usage: 💬 lmql chat <file>")
+        return
+    file = sys.argv[2]
+    absolute_path = os.path.abspath(file)
+    os.chdir(project_root)
+    os.system("python -m lmql.ui.chat " + absolute_path)
+
 def cmd_run():
     """
     emoji:🏃 run a LMQL script (e.g. "lmql run latest/hello.lmql")
     """
     import asyncio
     import time
```

### Comparing `lmql-0.0.6.6/src/lmql/demo.py` & `lmql-0.7b1/src/lmql/demo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 A: Let's think step by step.
 Jerry will spend 8 games x 2 hours per game = << 8*2 = 16 >>16 hours watching one daughter play her games.
 He will spend 16 x 2 = << 16*2 = 32 >>32 hours watching both daughters play their games.
 He will spend 8 games x 4 hours of practice = << 8*4 = 32 >>32 hours watching one daughter practice.
 He will spend 32 x 2 = << 32*2 = 64 >>64 hours watching both daughters practice.
 He will spend a total of 32 hours watching games + 64 hours watching practice = << 32+64 = 96 >>96 hours.
 So the answer is 96
-"""
+"""
```

### Comparing `lmql-0.0.6.6/src/lmql/http.py` & `lmql-0.7b1/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/language/compiler.py` & `lmql-0.7b1/src/lmql/language/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from _ast import And, AsyncFunctionDef, BinOp, ClassDef, Compare, FunctionDef, Import, ImportFrom, Return
 import ast
-import sys
-from typing import Any
-import astunparse
-import os
 import importlib
+import os
 import re
-
+import sys
+from _ast import (And, AsyncFunctionDef, Await, BinOp, Call, ClassDef, Compare, ExceptHandler,
+                  FunctionDef, If, Import, ImportFrom, Return)
 from io import StringIO
-from lmql.ops.ops import lmql_operation_registry
+from typing import Any
+
+import astunparse
 
-from lmql.language.qstrings import qstring_to_stmts, TemplateVariable, FExpression, DistributionVariable, TagExpression, stmts_to_qstring
-from lmql.language.validator import LMQLValidator, LMQLValidationError
-from lmql.language.fragment_parser import LMQLDecoderConfiguration, LMQLQuery, LanguageFragmentParser, FragmentParserError
-from lmql.runtime.model_registry import model_name_aliases
 import lmql.runtime.lmql_runtime as lmql_runtime
+from lmql.language.fragment_parser import (FragmentParserError,
+                                           LanguageFragmentParser,
+                                           LMQLDecoderConfiguration, LMQLQuery)
+from lmql.language.qstrings import (DistributionVariable, FExpression,
+                                    TagExpression, TemplateVariable,
+                                    qstring_to_stmts, stmts_to_qstring)
+from lmql.language.validator import LMQLValidationError, LMQLValidator
+from lmql.ops.ops import lmql_operation_registry
 from lmql.runtime.dclib import get_all_decoders
+from lmql.runtime.model_registry import model_name_aliases
 
 OPS_NAMESPACE = "lmql.ops"
+LIB_NAMESPACE = "lmql.lib"
 
 class FreeVarCollector(ast.NodeVisitor):
     def __init__(self, free_vars, exclude_criteria=None):
         self.free_vars = free_vars
         
         self.exclude = exclude_criteria or []
 
@@ -92,14 +98,15 @@
         if query.prologue is None: return
         
         DefinedVarsCollector(self.prologue_vars, self.defined_constraints).visit(ast.parse(query.prologue))
 
     def scope(self, query: LMQLQuery):
         self.distribution_vars = set([query.distribution.variable_name]) if query.distribution is not None else set()    
         self.defined_vars = set()
+        self.template_vars = set()
         self.prologue_vars = set()
 
         # collect set of global query template variables
         self.free_vars = set()
         self.written_vars = set()
 
         # collect defined vars in prologue
@@ -129,26 +136,29 @@
             self.scope_Constant(expr.value)
         else:
             super().generic_visit(expr)
 
     def visit_BoolOp(self, node: ast.BoolOp) -> Any:
         if is_query_string_with_constraints(node):
             self.scope_Constant(node.values[0])
+        else:
+            super().generic_visit(node)
 
     def scope_Constant(self, node):
         if type(node.value) is not str: return super().visit_Constant(node)
         qstring = node.value
 
         stmts = qstring_to_stmts(qstring, mode="all")
 
         # capture set of defined vars
         declared_template_vars = [v.name for v in stmts if type(v) is TemplateVariable]
         for v in declared_template_vars: 
             self.defined_vars.add(v)
             self.written_vars.add(v)
+            self.template_vars.add(v)
             if v in self.free_vars: self.free_vars.remove(v)
 
         used_fstring_expr = [s.expr for s in stmts if type(s) is FExpression]
         for v in used_fstring_expr:
             try:
                 parsed = ast.parse(v, mode="eval")
                 self.visit(parsed)
@@ -202,14 +212,18 @@
         if type(node.ctx) is ast.Load:
             if self.exclude_identifier(name):
                 return
             self.free_vars.add(name)
         
         return True
     
+    def visit_ExceptHandler(self, node: ExceptHandler) -> Any:
+        self.written_vars.add(node.name)
+        self.generic_visit(node)
+    
     def visit_FunctionDef(self, node: FunctionDef) -> Any:
         self.defined_vars.add(node.name)
     
     def visit_AsyncFunctionDef(self, node: AsyncFunctionDef) -> Any:
         self.defined_vars.add(node.name)
 
     def visit_ClassDef(self, node: ClassDef) -> Any:
@@ -235,32 +249,64 @@
 
 def is_query_string_with_constraints(node: ast.BoolOp):
     if len(node.values) < 1:
         return False
     left_most_operand = node.values[0]
     return type(left_most_operand) is ast.Constant and type(left_most_operand.value) is str and isinstance(node.op, ast.And)
 
-class QueryStringTransformation(ast.NodeTransformer):
+class FunctionCallTransformation(ast.NodeTransformer):
+    """
+    Translates function calls into lmql.call calls (to enable automatic await and unpacking 
+    when calling subqueries).
+    """
+    def visit_Await(self, node: Await) -> Any:
+        super().generic_visit(node)
+
+        if type(node.value) is ast.Await:
+            return node.value
+        return node.value
+
+    def is_excluded_from_call_transformation(self, node):
+        if not type(node) is ast.Name: return False
+        if ast.unparse(node).startswith("lmql.runtime_support.call"): return True
+        return node.id in ["print", "eval", "locals", "globals"]
+
+    def visit_Call(self, node: Call) -> Any:
+        f = self.visit(node.func)
+        args = [self.visit(a) for a in node.args]
+        keywords = [self.visit(k) for k in node.keywords]
+
+        if self.is_excluded_from_call_transformation(node.func):
+            node.func = f
+            node.args = args
+            node.keywords = keywords
+            return node
+
+        wrapped = Call(ast.parse("lmql.runtime_support.call"), [f, *args], keywords)
+        wrapped = ast.Await(wrapped)
+
+        return wrapped
+class PromptClauseTransformation(FunctionCallTransformation):
     """
     Transformes string expressions on statement level to model queries.
     """
     
     def __init__(self, query):
         self.query = query
     
     def transform(self):
         self.query.prompt = [self.visit(p) for p in self.query.prompt]
 
     def visit_Expr(self, expr):
         if type(expr.value) is ast.Constant:
             expr.value = self.transform_Constant(expr.value)
+            return expr
         else:
-            self.generic_visit(expr)
-        return expr
-    
+            return self.generic_visit(expr)
+
     # translate id access to context
     def visit_Name(self, node: ast.Name):
         name = str(node.id)
         
         if type(node.ctx) is ast.Load:
             if name == "context":
                 return ast.parse("(" + yield_call("get_context", ()) + ")").body[0].value
@@ -272,22 +318,24 @@
             if len(node.values[1:]) > 1:
                 constraints_expression = ast.BoolOp(op=node.op, values=node.values[1:])
             if len(node.values[1:]) == 1:
                 constraints_expression = node.values[1]
             elif len(node.values[1:]) == 0:
                 constraints_expression = None
             return self.transform_Constant(left_most_operand, constraints = constraints_expression)
-        return node
+        return self.generic_visit(node)
 
     def transform_Constant(self, constant, constraints=None):
         if type(constant.value) is not str: return constant
         
         qstring = constant.value
-        qstring = qstring.encode("unicode_escape").decode("utf-8").encode('unicode_escape').decode('utf-8')
-        
+        if len(qstring) == 0: return constant
+        if qstring.strip().startswith("lmql"): return constant
+
+        qstring = qstring.encode("unicode_escape").decode("utf-8").encode('unicode_escape').decode('utf-8')        
         compiled_qstring = ""
 
         declared_template_vars = set()
 
         for stmt in qstring_to_stmts(qstring, mode="square-only"):
             if type(stmt) is str:
                 compiled_qstring += stmt
@@ -298,14 +346,18 @@
                 compiled_qstring += str(stmt)
 
         # keep track of last stmt in this qstring
         last_stmt = stmt
 
         if len(compiled_qstring) == 0:
             return constant
+        
+        qstring_as_fstring: ast.JoinedStr = ast.parse(f'f"""{compiled_qstring}"""').body[0].value
+        function_call_transformer = FunctionCallTransformation()
+        qstring_as_fstring.values = [function_call_transformer.visit(v) for v in qstring_as_fstring.values]
 
         if constraints is not None:
             constraint_transformation = InlineConstraintsTransformation(constraints, scope=self.query.scope)
             code_str, result_reference = constraint_transformation.transform()
             result_code = code_str + "\n"
 
             # result_code = f'yield context.query(f"""{compiled_qstring}""")'
@@ -392,49 +444,44 @@
         bn = get_builtin_name(node, plain_python)
         if bn is not None: return bn
         # check if variable is distribution variable
         if node.id in self.scope.distribution_vars:
             raise LMQLValidationError("Distribution variable {} cannot be used in where clause.".format(node.id))
 
         # check for template variables
-        if node.id in self.scope.defined_vars and not keep_variables:
+        if node.id in self.scope.template_vars and not keep_variables:
             return f"lmql.runtime_support.Var('{node.id}')"
         else:
-            return f"lmql.runtime_support.Var('{node.id}', python_variable=True)"
+            return f"lmql.runtime_support.Var('{node.id}', python_variable=True, python_value={node.id})"
 
         return bn or node.id
 
     def transform_node(self, expr, snf):
         if type(expr) is ast.BoolOp:
             if type(expr.op) is ast.And or type(expr.op) is ast.Or:
                 ops = expr.values
                 tops = [self.transform_node(op, snf) for op in ops]
                 tops_list = ",\n  ".join([t.strip() or "None" for t in tops])
                 
                 Op = f"{OPS_NAMESPACE}.AndOp" if type(expr.op) is ast.And else f"{OPS_NAMESPACE}.OrOp"
                 return snf.add(f"{Op}([\n  {tops_list}\n])")
-        # elif type(expr) is ast.Call:
-        #     tfunc = self.transform_node(expr.func, snf)
-        #     targs = [self.transform_node(a, snf) for a in expr.args]
-        #     targs_list = ", ".join(targs)
-        #     return f"{tfunc}({targs_list})"
         elif type(expr) is ast.Name:
             return self.transform_name(expr)
         elif type(expr) is ast.UnaryOp:
             op = expr.op
             
             Ops = {
                 ast.Not: f"{OPS_NAMESPACE}.NotOp"
             }
 
             for OpT, impl in Ops.items():
                 if type(op) is OpT:
                     operand = self.transform_node(expr.operand, snf).strip()
                     return snf.add(f"{impl}([{operand}])")
-            
+
             assert False, "unary operator {} not supported.".format(type(expr.op))
         elif type(expr) is ast.Compare:
             op = expr.ops[0]
             assert len(expr.ops) == 1, "compiler currently does not support comparison with more than one operator"
             
             Ops = {
                 ast.Eq: f"{OPS_NAMESPACE}.EqOp",
@@ -445,44 +492,51 @@
 
             for OpT, impl in Ops.items():
                 if type(op) is OpT: 
                     ops = [self.transform_node(c, snf) for c in [expr.left] + expr.comparators]
                     ops_list = ", ".join(ops).strip()
                     return snf.add(f"{impl}([{ops_list}])")
             
-            # if is_type_constraint(expr):
-            #     type_name = expr.comparators[0].id
-            #     var_name = expr.left.args[0].id
-            #     return snf.add(f"{OPS_NAMESPACE}.TypeConstraint([{type_name}, {OPS_NAMESPACE}.Var('{var_name}')])")
+            if is_type_constraint(expr):
+                type_name = expr.comparators[0].id
+                var_name = expr.left.args[0].id
+                return snf.add(f"{OPS_NAMESPACE}.CallOp([{LIB_NAMESPACE}.types.is_type, [{OPS_NAMESPACE}.Var('{var_name}'), {type_name}]], locals(), globals())")
+                # return snf.add(f"{LIB_NAMESPACE}.is_type([{type_name}, {OPS_NAMESPACE}.Var('{var_name}')])")
             
             assert False, "operator {} is not supported.".format(astunparse.unparse(expr))
         elif type(expr) is ast.Constant:
             return self.default_transform_node(expr, snf).strip()
         elif type(expr) is ast.ListComp:
             return self.default_transform_node(expr, snf).strip()
         elif type(expr) is ast.Call:
             constraint_ref = get_builtin_name(expr.func) or get_inner_constraint_ref(expr.func, self.scope)
             if constraint_ref is not None:
                 args = [self.transform_node(a, snf) for a in expr.args]
                 args_list = ", ".join(args)
                 return f"{constraint_ref}([{args_list}])"
             if is_allowed_builtin_python_call(expr.func):
                 return self.default_transform_node(expr, snf).strip()
+            
+            assert type(expr.func) is ast.Name, "In LMQL constraint expressions, only function calls to direct function references are allowed: {}".format(astunparse.unparse(expr))
+            tfunc = ast.unparse(expr.func)
+            targs = [self.transform_node(a, snf) for a in expr.args]
+            targs_list = ", ".join(targs)
+            return f"{OPS_NAMESPACE}.CallOp([{tfunc}, [{targs_list}]], locals(), globals())"
         elif type(expr) is ast.List:
             return self.default_transform_node(expr, snf).strip()
 
         print(f"compiler warning: expressions of type {type(expr)} are not explicitly supported: '{astunparse.unparse(expr).strip()}'")
         return snf.add(self.default_transform_node(expr, snf))
 
     def default_transform_node(self, node, snf):
         # collect the set of captured template variables
         names = set()
         def collect_name(node):
             name = node.id
-            if name in self.scope.defined_vars:
+            if name in self.scope.template_vars:
                 names.add(name)
         NameVisitor(collect_name).visit(node)
         names = sorted(list(names))
 
         # if no template variable names are capture, node represents a constant expression
         if len(names) == 0: return astunparse.unparse(node)
 
@@ -608,15 +662,15 @@
 
 
         return self.query
 
 class CompilerTransformations:
     def __init__(self):
         self.transformations = [
-            QueryStringTransformation,
+            PromptClauseTransformation,
             WhereClauseTransformation,
             DecodeClauseTransformation,
             ReturnStatementTransformer
         ]
     
     def transform(self, query):
         for T in self.transformations:
@@ -631,15 +685,15 @@
         self.prologue = prologue
         
         self.in_memory_contents = ""
         
         self.file = open(self.filename, "w")
 
         self.indent = "  "
-        self.write("import lmql\n")
+        self.write("import lmql\nimport lmql.lib\n")
         self.write(self.prologue)
         
         if decorators is not None:
             if decorators_args is None:
                 decorators_args = [None] * len(decorators)
             for d,args in zip(decorators, decorators_args):
                 self.write(f"@{d}({args})\n")
@@ -726,15 +780,18 @@
         try:
             # parse file
             with open(filepath) as f:
                 contents = f.read()
             lmql_code = preprocess_text(contents)
             buf = StringIO(lmql_code)
             parser = LanguageFragmentParser()
-            q = parser.parse(buf.readline)
+            try:
+                q = parser.parse(buf.readline)
+            except IndentationError as e:
+                raise RuntimeError("parsing error: {}.\nFailed when parsing:\n {}".format(e, lmql_code))
 
             # output file path
             basename = os.path.basename(filepath).split(".lmql")[0]
             output_file = os.path.join(os.path.dirname(filepath), f"{basename}_compiled.py")
 
             # scoping
             scope = PromptScope()
@@ -772,12 +829,15 @@
                 if q.distribution:
                     writer.add("# distribution")
                     # writer.add("context.set_distribution('{}', {})".format(q.distribution.variable_name, astunparse.unparse(q.distribution.values).strip()))
                     writer.add(yield_call("set_distribution", "\"" + q.distribution.variable_name + "\"", astunparse.unparse(q.distribution.values).strip()))
                 
                 writer.add(f"yield ('result', (" + yield_call("get_return_value", ()) + "))")
 
+            if q.decode.has_dump_compiled_code_flag:
+                print(writer.in_memory_contents)
+
             return LMQLModule(output_file, lmql_code=lmql_code, output_variables=[v for v in scope.defined_vars])
         except FragmentParserError as e:
             sys.stderr.write("error: " + str(e) + "\n")
             sys.exit(1)
```

### Comparing `lmql-0.0.6.6/src/lmql/language/fragment_parser.py` & `lmql-0.7b1/src/lmql/language/fragment_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 class FragmentParserError(Exception): pass
 
 @dataclass
 class LMQLDecoderConfiguration:
     method: ast.AST
     decoding_args: List[ast.keyword]
 
+    @property
+    def has_dump_compiled_code_flag(self):
+        for kwa in self.decoding_args:
+            if kwa.arg == "dump_compiled_code":
+                if type(kwa.value) is ast.Constant and kwa.value.value == True:
+                    return True
+        return False
+
 @dataclass
 class LMQLDistributionClause:
     variable_name: str
     values: List[str]
 
 @dataclass
 class LMQLQuery:
@@ -89,14 +97,16 @@
     assert type(s) is list
     return tokenize.untokenize([transform_token(t) for t in s if t.type != tokenize.COMMENT])
 
 def transform_token(t):
     return t
 
 def ast_parse(s, unindent=False, oneline=False, loc=None):
+    # for special symbols
+    if len(s) > 0 and all(type(e) is str for e in s): return ast.parse('"' + " ".join(s) + '"')
     try:
         s = remove_comments(s)
         if unindent: s = remove_indentation(s, oneline=oneline)
         return ast.parse(s)
     except SyntaxError as e:
         msg = ""
```

### Comparing `lmql-0.0.6.6/src/lmql/language/qstrings.py` & `lmql-0.7b1/src/lmql/language/qstrings.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,8 +133,11 @@
         
         for i, s in enumerate(self.stmts):
             if type(s) is TemplateVariable and s.name.startswith("distribution:"):
                 self.stmts[i] = DistributionVariable(s.name[len("distribution:"):])
             elif type(s) is FExpression and s.expr.startswith(":"):
                 self.stmts[i] = TagExpression(s.expr)
 
+        # filter out empty name template variables
+        self.stmts = [s for s in self.stmts if not (type(s) is TemplateVariable and len(s.name) == 0)]
+
         return self.stmts
```

### Comparing `lmql-0.0.6.6/src/lmql/language/validator.py` & `lmql-0.7b1/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/README.md` & `lmql-0.7b1/src/lmql/models/lmtp/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/backends/__main__.py` & `lmql-0.7b1/src/lmql/models/lmtp/backends/__main__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/backends/llama_cpp_model.py` & `lmql-0.7b1/src/lmql/models/lmtp/backends/llama_cpp_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/backends/lmtp_model.py` & `lmql-0.7b1/src/lmql/models/lmtp/backends/lmtp_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/backends/random_model.py` & `lmql-0.7b1/src/lmql/models/lmtp/backends/random_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/backends/transformers_model.py` & `lmql-0.7b1/src/lmql/models/lmtp/backends/transformers_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_async.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_async.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_client.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_dcmodel.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_dcmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,16 @@
             if decoder_step is not None:
                 data["_step"] = decoder_step
             printer.report_model_stats(**data)
 
     async def _score_next_tokens(self, s, next_tokens, noscore=False):
         if noscore:
             return np.zeros(len(next_tokens), dtype=np.float32)
+    
+        await self.ensure_connected()
         
         scores = []
         i = 0
         
         ids = self.tokenizer.convert_bytes_to_ids(s.input_ids)
         next_tokens = self.tokenizer.convert_bytes_to_ids(next_tokens)
 
@@ -326,19 +328,19 @@
         await self.ensure_connected()
         
         assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
 
         def make_detseq(s, token_score, completion):
             # compose deterministic flags
             if type(deterministic) is bool:
-                deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
+                deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])], dtype=np.bool_)
                 next_deterministic = np.array([deterministic] * len(completion[1:]))
             else:
                 assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored, but is {} and {}".format(deterministic, completion)
-                deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])])
+                deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])], dtype=np.bool_)
                 next_deterministic = np.array(deterministic[1:])
 
             return dc.detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
                     next_ids=completion[1:],
                     logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
                     next_logprobs=token_score[1:],
                     deterministic=deterministic_flags,
```

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_inference_server.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_inference_server.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_multiprocessing.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_scheduler.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_scheduler.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_serve.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_serve.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_threading.py` & `lmql-0.7b1/src/lmql/models/lmtp/lmtp_threading.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/lmtp/utils.py` & `lmql-0.7b1/src/lmql/models/lmtp/utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/models/model.py` & `lmql-0.7b1/src/lmql/models/model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ops/follow_map.py` & `lmql-0.7b1/src/lmql/ops/follow_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,32 @@
         result_map.simplify()
 
         return result_map
 
     def map(self, fct):
         mappings = [(pattern, fct(pattern, value)) for pattern, value in self.components]
         return fmap(*mappings)
+    
+    def flat_map(self, fct, simplify=True):
+        mappings = []
+        
+        for pattern, value in self.components:
+            submap = fct(pattern, value)
+            if submap is None:
+                mappings.append((pattern, value))
+            else:
+                submap = submap.intersect(pattern)
+                for subpattern, subvalue in submap.components:
+                    mappings.append((subpattern, subvalue))
+        result = fmap(*mappings)
+        
+        if simplify: result.simplify()
+
+        return result
+
 
 def zip_fmap(*fmaps):
     """
     Simple zip of multiple fmaps (number of components and 
     patterns must match for all fmaps).
     """
```

### Comparing `lmql-0.0.6.6/src/lmql/ops/ops.py` & `lmql-0.7b1/src/lmql/ops/ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from tokenize import Token
 from typing import Iterable, Tuple, List
 from itertools import product
 
 from lmql.ops.token_set import *
 from lmql.ops.follow_map import *
+from lmql.ops.node import *
+
+from lmql.ops.inline_call import InlineCallOp
+from lmql.ops.booleans import *
+from lmql.ops.regex import Regex
 
 lmql_operation_registry = {}
 
 # @LMQLOp('function_name') decorator
 def LMQLOp(name):
     def class_transformer(cls):
         # get full import path of cls
@@ -21,60 +26,14 @@
             for n in name:
                 lmql_operation_registry[n] = cls_name
             return cls
         lmql_operation_registry[name] = cls_name
         return cls
     return class_transformer
 
-class Node:
-    def __init__(self, predecessors):
-        assert type(predecessors) is list, "Predecessors must be a list, not {}".format(type(predecessors))
-        self.predecessors = predecessors
-        self.depends_on_context = False
-    
-    def execute_predecessors(self, trace, context):
-        return [execute_op(p, trace=trace, context=context) for p in self.predecessors]
-
-    def forward(self, *args, **kwargs):
-        raise NotImplementedError(type(self) + " does not implement forward()")
-
-    def follow(self, *args, **kwargs):
-        raise NotImplementedError(type(self) + " does not implement follow()")
-    
-    def final(self, args, **kwargs):
-        if all([a == "fin" for a in args]):
-            return "fin"
-        return "var"
-
-    def __nodelabel__(self):
-        return str(type(self))
-    
-    def postprocess_var(self, var_name):
-        """
-        Returns true if this operations provides postprocessing semantics for complete values for the given variable name.
-        """
-        return False
-
-    def postprocess(self, operands, value):
-        """
-        Returns the postprocessed variant of `value`. Only called if `postprocess_var` returns true for variable name of value.
-        
-        You can return a tuple of postprocessed_rewrite (prompt) and postprocessed_value (variable value), to additionally 
-        provide different postprocessing semantics for the variable value and the rewrite of the prompt.
-        """
-        pass
-
-    def postprocess_order(self, other, **kwargs):
-        """
-        Orders application of postprocessing operations. Returns "before", "after" or 0 if order is not defined.
-        
-        Only invoked for `other` operations, that return true for the same `postprocess_var`.
-        """
-        return 0 # by default, no order is defined (only one postprocessing operation per variable can be applied)
-
 def DynamicTypeDispatch(name, type_map):
     class TypeDispatchingNode(Node):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             
             self.delegate_args = args
             self.delegate_kwargs = kwargs
@@ -131,39 +90,14 @@
         
         def __nodelabel__(self):
             if self.delegate is not None:
                 return self.delegate.__nodelabel__()
             return name
 
     return TypeDispatchingNode
-
-NextToken = "<lmql.next>"
-
-def is_next_token(t): 
-    return t == NextToken
-
-def strip_next_token(x):
-    if type(x) is list:
-        return [i for i in x if not is_next_token(i)]
-    elif type(x) is tuple:
-        return tuple(i for i in x if not is_next_token(i))
-    if type(x) is not str:
-        return x
-    if x.endswith(NextToken):
-        x = x[:-len(NextToken)]
-    return x
-
-class postprocessed_value:
-    def __init__(self, value):
-        self.value = value
-class postprocessed_rewrite:
-    def __init__(self, rewrite):
-        self.rewrite = rewrite
-
-
 @LMQLOp("SENTENCES")
 class Sentences(Node):
     def forward(self, v, **kwargs):
         sentences = tuple(self.split(v, separator=["."]))
         return self.strip(sentences)
     
     def strip(self, sentences):
@@ -237,51 +171,67 @@
     def follow(self, v, **kwargs):
         if v is None: return None
         
         has_next_token = v != strip_next_token(v)
         v = strip_next_token(v)
 
         context = kwargs.get("context", None)
+
         if context.runtime.prefers_compact_mask:
             number_tokens = tset("1","2","3","4","5","6","7","8","9","Ġ2","Ġ3","Ġ4","Ġ5","Ġ0","Ġ6","Ġ7","Ġ8","Ġ9","10","12","50","19","11","20","30","15","14","16","13","25","18","17","24","80","40","22","60","23","29","27","26","28","99","33","70","45","35","64","75","21","38","44","36","32","39","34","37","48","66","55","47","49","65","68","31","67","59","77","58","69","88","46","57","43","42","78","79","90","95","41","56","54","98","76","52","53","51","86","74","89","72","73","96","71","63","62","85","61","97","84","87","94","92","83","93","91","82","81", exact=True, name="number_tokens")
-            number_continuation_tokens = tset("0","1","2","3","4","5","6","7","8","9","00","01","10","12","50","19","11","20","30","15","14","16","13","25","18","17","24","80","40","22","60","23","29","27","26","28","99","33","70","45","35","64","75","21","38","44","36","32","39","34","05","37","48","66","55","47","08","49","09","65","07","02","04","03","68","31","67","59","06","77","58","69","88","46","57","43","42","78","79","90","95","41","56","54","98","76","52","53","51","86","74","89","72","73","96","71","63","62","85","61","97","84","87","94","92","83","93","91","82","81", exact=True, name="number_continuation_tokens")
         else:
             number_tokens = tset("[ 1-9][0-9]*$", regex=True, name="full_number_tokens")
-            number_continuation_tokens = tset("[0-9]+$", regex=True, name="full_number_continuation_tokens")
+            number_cont_tokens = tset("[1-9][0-9]*$", regex=True, name="number_continuation_tokens")
 
         if not has_next_token:
             return fmap(
                 ("eos", len(v.strip()) != 0),
                 ("*", self.forward(v))
             )
 
+        if not all([c.strip() in ",0123456789" for c in v]) and len(v.strip()) > 0:
+            return fmap(
+                ("*", False)
+            )
+
+        if "turbo" in context.runtime.model_identifier or "gpt-4" in context.runtime.model_identifier:
+            if not all([c in "0123456789" for c in v]):
+                return fmap(
+                    ("*", False)
+                )
+            else:
+                return fmap(
+                    ("*", True)
+                )
+
         if len(v) == 0:
             return fmap(
                 (number_tokens, True),
                 ("*", False)
             )
         else:
             if len(v.strip()) == 0:
                 # do not allow empty strings
                 return fmap(
-                    (number_continuation_tokens, True),
+                    (number_cont_tokens, True),
                     ("eos", False),
                     ("*", False)
                 )
 
+            # allow anything (either continue as number or stop by predicting any other 
+            # token, which will be removed by the postprocessing)
             return fmap(
-                (number_continuation_tokens, True),
-                ("eos", True),
-                ("*", False)
+                ("*", True)
             )
         
     def postprocess_var(self, var_name):
         return var_name == self.predecessors[0].name
 
     def postprocess(self, operands, raw):
+        raw = "".join([c for c in raw if c in "0123456789"])
         value = int(raw)
         return postprocessed_rewrite(str(value)), postprocessed_value(value)
 
     def postprocess_order(self, other, **kwargs):
         if isinstance(other, StopAtOp):
             return "after" # apply Int after StopAt
         else:
@@ -385,21 +335,14 @@
                 len_masks.append((tmask, len(v) + l))
 
             return fmap(*len_masks)
 
     def final(self, x, operands=None, result=None, **kwargs):
         return x[0]
 
-class NotOp(Node):
-    def forward(self, op, **kwargs):
-        return not op
-
-    def follow(self, v, **kwargs):
-        return not v
-
 class Lt(Node):
     def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         return args[0] < args[1]
     
     def follow(self, *args, **kwargs):
         if any([a is None for a in args]): return None
@@ -575,66 +518,14 @@
 
         if l == "fin": 
             return "fin"
         if result is not None and (l == "fin" or l == "inc"):
             return "fin"
         else: return "var"
 
-class Var(Node):
-    def __init__(self, name, python_variable=False):
-        super().__init__([])
-        self.name = name
-        self.python_variable = python_variable
-
-        self.depends_on_context = True
-        
-        # indicates whether the downstream node requires text diff information
-        self.diff_aware_read = False
-
-    async def json(self):
-        return self.name
-
-    def forward(self, context, **kwargs):
-        if self.python_variable:
-            return context.python_scope.get(self.name)
-
-        if self.diff_aware_read:
-            return (context.get(self.name, None), context.get_diff(self.name, None))
-        
-        return context.get(self.name, None)
-    
-    def follow(self, context, **kwargs):
-        if self.python_variable:
-            return context.python_scope.get(self.name)
-
-        value = context.get(self.name, None)
-        if value is None: return None
-        
-        # also return the text diff if required
-        if self.diff_aware_read:
-            value = (value, context.get_diff(self.name, None))
-
-        # strip_next_token but also supports tuples
-        def strip_nt(v):
-            if type(v) is tuple: return (strip_next_token(v[0]), v[1])
-            else: return strip_next_token(v)
-
-        return fmap(
-            ("eos", PredeterminedFinal(strip_nt(value), "fin")),
-            ("*", value),
-        )
-
-    def final(self, x, context, operands=None, result=None, **kwargs):
-        if self.python_variable:
-            return "fin"
-        return context.final(self.name)
-
-    def __repr__(self) -> str:
-        return f"<Var {self.name}>"
-
 class RawValueOp(Node):
     def __init__(self, args):
         super().__init__([])
         
         value, final = args
         self.value = value
         self.final_value = final
@@ -760,97 +651,87 @@
             return "var"
 
 InOp = DynamicTypeDispatch("InOp", (
     ((str, str), InOpStrInStr),
     ("*", InOpStrInSet),
 ))
 
-class OrOp(Node):
-    def forward(self, *args, **kwargs):
-        if any([a == True for a in args]):
-            return True
-        elif all([a == False for a in args]):
-            return False
-        else:
-            return None
-
-    def follow(self, *args, **kwargs):
-        return fmap(
-            ("*", self.forward(*args))
-        )
-
-    def final(self, args, operands=None, result=None, **kwargs):
-        if result:
-            if any(a == "fin" and v == True for a,v in zip(args, operands)):
-                return "fin"
-            return "var"
-        else: # not result
-            if any(a == "var" for a in args):
-                return "var"
-            return "fin"
-
-class AndOp(Node):
-    def forward(self, *args, **kwargs):
-        if type(args[0]) is tuple and len(args) == 1:
-            args = args[0]
-
-        if any([a == False for a in args]):
-            return False
-        elif any([a is None for a in args]):
-            return None
-        else:
-            return all([a for a in args])
-
-    def follow(self, *v, **kwargs):
-        return fmap(
-            ("*", self.forward(*v))
-        )
-
-    def final(self, args, operands=None, result=None, **kwargs):
-        if result:
-            if all([a == "fin" for a in args]):
-                return "fin"
-            return "var"
-        else: # not result
-            if any([a == "fin" and v == False for a,v in zip(args, operands)]):
-                return "fin"
-            return "var"
-
 def seq_starts_with(seq1, seq2):
     num_matching = sum([1 if i1 == i2 else 0 for i1,i2 in zip(seq1, seq2)])
     return num_matching == len(seq2)
 
 def remainder(seq: str, phrase: str):
     overlap = 0
     for i in range(len(phrase)):
         if seq[-i:] == phrase[:i]:
             overlap = i
 
     if overlap == 0: return None
     else: return phrase[i:]
 
+@LMQLOp("REGEX")
+class RegexOp(Node):
+    def forward(self, *args, **kwargs):
+        if any([a is None for a in args]): return None
+        x = args[0]
+        ex = args[1]
+        assert isinstance(ex, str)
+        return Regex(ex).fullmatch(x)
+    
+    def follow(self, *args, **kwargs):
+        if any([a is None for a in args]): return None
+        x = args[0]
+        ex = args[1]
+        assert isinstance(ex, str)
+        
+        if x == strip_next_token(x):
+            return fmap(
+                ("*", Regex(ex).fullmatch(x))
+            )
+
+        r = Regex(ex)
+        rd = r.d(strip_next_token(x)) # take derivative
+        print(f"r={r.pattern} x={strip_next_token(x)} --> {rd.pattern if rd is not None else '[no drivative]'}")
+        if rd is None:
+            return False 
+        elif rd.is_empty(): # derivative is empty -> full match; therefore we must end
+            return fmap(
+                ("eos", True)
+            )
+        else: # only permit tokens form the regex derivative
+            return fmap(
+                (tset(rd.pattern, regex=True, prefix=True), True),
+                #('*', False)
+            )
+
+    def final(self, ops_final, result=None, operands=None, **kwargs):
+        if ops_final[0] == "fin": return "fin"
+        else: return "var"
+
 @LMQLOp("STARTS_WITH")
 class StartsWithOp(Node):
     def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         
         x = args[0]
         allowed_phrases = args[1]
+        if isinstance(args[1], str): allowed_phrases = [allowed_phrases]
 
         for phrase in allowed_phrases:
             if x.startswith(phrase):
                 return True
 
         return False
 
     def follow(self, *args, **kwargs):
         if any([a is None for a in args]): return None
 
         x = args[0]
         allowed_phrases = args[1]
+        if isinstance(args[1], str): allowed_phrases = [allowed_phrases]
 
         # if there is any full match, then the result is True
         if any(strip_next_token(x).startswith(phrase) for phrase in allowed_phrases):
             return True
 
         # otherwise check for partial matches with the allowed phrases
         suffixes = list(matching_phrases_suffixes(x, allowed_phrases))
@@ -869,25 +750,23 @@
 
         if op1 == "inc" and op2 == "fin":
             if len(operands[0]) == 0 and not result:
                 return "var"
             return "fin"
         
         return super().final(ops_final, **kwargs)
-
 @LMQLOp(["STOPS_AT", "stops_at"])
 class StopAtOp(Node):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._tokenized_stopping_phrase_cache = {}
 
     def execute_predecessors(self, trace, context):
         var_op: Var = self.predecessors[0]
         assert type(var_op) is Var, "The first argument of STOPS_AT must be a direct reference to a template variable."
-        assert type(self.predecessors[1]) is str, "The second argument of STOPS_AT must be a string literal."
+        assert type(self.predecessors[1]) is str or type(self.predecessors[1]) is Var, "The second argument of STOPS_AT must be a string literal, but is {}.".format(type(self.predecessors[1]))
         var_op.diff_aware_read = True
         return super().execute_predecessors(trace, context)
     
     @property
     def variable(self):
         return self.predecessors[0]
 
@@ -916,15 +795,16 @@
         match_only_with_diff = op2 in op1 and matched_phrase_index >= len(op1) - len(op1_diff)
 
         return match_only_with_diff or op1.endswith(op2)
 
     def stopping_phrase(self, trace):
         if type(self.predecessors[1]) is Node:
             return trace[self.predecessors[1]]
-        return self.predecessors[1]
+        if type(self.predecessors[1]) is str:
+            return self.predecessors[1]
 
     def postprocess_var(self, var_name):
         return var_name == self.predecessors[0].name
 
     def postprocess(self, operands, value):
         if value != operands[0][0]:
             return value
@@ -984,95 +864,121 @@
             return None
 
         if matched_phrase_index != -1:
             value = value[:matched_phrase_index]
 
         return postprocessed_rewrite(value), postprocessed_value(value)
 
-class OpaqueLambdaOp(Node):
+class CallOp(Node):
+    def __new__(cls, predecessors, lcls, glbs):
+        fct, *args = predecessors
+        if hasattr(fct, "__lmql_query_function__"):
+            return InlineCallOp(predecessors, lcls, glbs)
+        
+        return super().__new__(cls)
+
+    def __init__(self, predecessors, lcls, glbs):
+        super().__init__(predecessors)
+        
+        self.fct, *self.args = predecessors
+
     def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         fct, *args = args
         return fct(*args)
     
     def follow(self, *v, **kwargs):
         if any([a is None for a in v]): return None
 
         fct, *args = v
-        return fmap(
-            ("*", fct(*args))
-        )
+        return fmap(("*", fct(*args)))
 
-def create_mask(follow_map, valid, final):
-    if follow_map is None:
-        return "*"
-    
-    allowed_tokens = tset()
-    otherwise_result = None
-
-    for pattern, result in follow_map:
-        if pattern == "*":
-            otherwise_result = result
+@LMQLOp(["ESCAPED", "escaped"])
+class EscapedOp(Node):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-        if result is not None:
-            value, final = result
-        else:
-            value = None
-            final = "var"
+    def execute_predecessors(self, trace, context):
+        var_op: Var = self.predecessors[0]
+        assert type(var_op) is Var, "The first argument of STOPS_AT must be a direct reference to a template variable."
+        return super().execute_predecessors(trace, context)
+    
+    def forward(self, *args, **kwargs):
+        return True
+    
+    def follow(self, *args, **kwargs):
+        return fmap(("*", True))
+    
+    def final(self, ops_final, operands, result, **kwargs):
+        return ops_final[0]
+    
+    @property
+    def variable(self):
+        return self.predecessors[0]
 
-        if value == True or value is None:
-            allowed_tokens = union(allowed_tokens,pattern)
-        elif value == False and final == ("var",):
-            allowed_tokens = union(allowed_tokens, pattern)
-        elif value is None and len(follow_map.components) == 1:
-            allowed_tokens = "*"
-        elif result == (False, ('fin',)):
-            if pattern != "*":
-                allowed_tokens = setminus(allowed_tokens, pattern)
-
-    if allowed_tokens == "∅":
-        return tset("eos")
-
-    if len(allowed_tokens) == 0:
-        if otherwise_result is not None:
-            othw_value, othw_final = otherwise_result
-        else:
-            othw_value, othw_final = None, "var"
-        if not othw_value and othw_final == ("fin",):
-            return tset("eos")
-        else:
-            return "*"
+    def postprocess_var(self, var_name):
+        return var_name == self.predecessors[0].name
 
-    return allowed_tokens
+    def postprocess(self, operands, value):
+        value = value.replace("\n",  "\\n")
+        value = value.replace("\t",  "\\t")
 
-def is_node(op):
-    return issubclass(type(op), Node)
+        return postprocessed_rewrite(value), postprocessed_value(value)
 
-def derive_predecessor_final(op, trace):
-    def get_final(v):
-        # for nodes, get final value from trace
-        if is_node(v): return trace[v][1]
-        # for constants, final value is always "fin"
-        return "fin"
-    return [get_final(p) for p in op.predecessors]
+    def postprocess_order(self, other, **kwargs):
+        if isinstance(other, StopAtOp):
+            return "after"
+        return 0
 
-def derive_final(op, trace, context, result):
-    predecessor_final = derive_predecessor_final(op, trace)
+@LMQLOp(["ERASE"])
+class EraseOp(Node):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-    def get_predecessor_result(v):
-        if is_node(v): return trace[v][0]
-        return v
+    def execute_predecessors(self, trace, context):
+        var_op: Var = self.predecessors[0]
+        assert type(var_op) is Var, "The first argument of STOPS_AT must be a direct reference to a template variable."
+        return super().execute_predecessors(trace, context)
+    
+    def forward(self, *args, **kwargs):
+        return True
     
-    predecessor_values = [get_predecessor_result(p) for p in op.predecessors]
+    def follow(self, *args, **kwargs):
+        return fmap(("*", True))
+    
+    def final(self, ops_final, operands, result, **kwargs):
+        return ops_final[0]
+    
+    @property
+    def variable(self):
+        return self.predecessors[0]
+
+    def postprocess_var(self, var_name):
+        return var_name == self.predecessors[0].name
+
+    def postprocess(self, operands, value):
+        return postprocessed_rewrite(""), postprocessed_value(value)
 
-    context_arg = ()
-    if op.depends_on_context: 
-        context_arg += (context,)
+    def postprocess_order(self, other, **kwargs):
+        if isinstance(other, StopAtOp):
+            return "after"
+        return 0
+class OpaqueLambdaOp(Node):
+    def forward(self, *args, **kwargs):
+        if any([a is None for a in args]): return None
+        fct, *args = args
+        return fct(*args)
     
-    return op.final(predecessor_final, *context_arg, operands=predecessor_values, result=result)
+    def follow(self, *v, **kwargs):
+        if any([a is None for a in v]): return None
+
+        fct, *args = v
+        return fmap(
+            ("*", fct(*args))
+        )
 
 def execute_op_stops_at_only(variable: str, op: Node, trace, result=None, sidecondition=None):
     """
     Evaluates a Node and returns the list of defined StopAtOps for the query.
     """
     is_root_call = result is None and sidecondition is None
     
@@ -1137,15 +1043,21 @@
                 current_op, current_op_inputs = postprocessors[i]
                 relative_order = op.postprocess_order(current_op, operands=inputs, other_inputs=current_op_inputs)
                 if relative_order == "before":
                     break
                 elif relative_order == "after":
                     i += 1
                 else:
-                    assert len(postprocessors) == 0, "The specified set of constraints contains multiple incompatible postprocessing operations for the same variable. The conflicting operations are: {} and {}. Please make sure the used constraints implement postprocess_order for each other, to use them together.".format(current_op, op)
+                    relative_order = current_op.postprocess_order(op, operands=current_op_inputs, other_inputs=inputs)
+                    if relative_order == "before":
+                        i += 1
+                    elif relative_order == "after":
+                        break
+                    else:
+                        assert len(postprocessors) == 0, "The specified set of constraints contains multiple incompatible postprocessing operations for the same variable. The conflicting operations are: {} and {}. Please make sure the used constraints implement postprocess_order for each other, to use them together.".format(current_op, op)
             postprocessors.insert(i, (op, inputs))
 
     # filter out stopping conditions as postprocessors that were not actually triggered (due to unfulfilled sideconditions)
     stopping_conditions: List[StopAtOp] = execute_op_stops_at_only(var_name, root_op, trace)
     postprocessors = [p for p in postprocessors if not isinstance(p[0], StopAtOp) or p[0] in stopping_conditions]
 
     rewritten_value = None
@@ -1169,69 +1081,8 @@
                 rewritten_value = result
     
     if rewritten_prompt is None:
         rewritten_prompt = str(value)
     if rewritten_value is None:
         rewritten_value = value
     
-    return rewritten_value, rewritten_prompt
-
-def execute_op(op: Node, trace=None, context=None, return_final=False, semantics="forward"):
-    # for constant dependencies, just return their value
-    if not is_node(op): 
-        return op
-    
-    # only evaluate each operation once
-    if op in trace.keys(): 
-        return trace[op][0]
-    
-    # compute predecessor values
-    inputs = op.execute_predecessors(trace, context)
-    
-    if op.depends_on_context: 
-        inputs += (context,)
-
-    inputs_final = derive_predecessor_final(op, trace)
-    semantics_fct = op.__getattribute__(semantics)
-    result = semantics_fct(*inputs, final=inputs_final)
-    is_final = derive_final(op, trace, context, result)
-    
-    if trace is not None: 
-        trace[op] = (result, is_final)
-
-    if return_final:
-        return result, is_final
-
-    return result
-
-def digest(expr, context, follow_context, no_follow=False):
-    if expr is None: return True, "fin", {}, {}
-
-    trace = {}
-    follow_trace = {}
-    expr_value, is_final = execute_op(expr, trace=trace, context=context, return_final=True)
-
-    if no_follow:
-        return expr_value, is_final, trace, follow_trace
-
-    for op, value in trace.items():
-        # determine follow map of predecessors
-        if len(op.predecessors) == 0: 
-            # empty argtuple translates to no follow input
-            intm = all_fmap((ArgTuple(), ["fin"])) 
-        else:
-            # use * -> value, for constant value predecessor nodes
-            def follow_map(p):
-                if is_node(p): return follow_trace[p]
-                else: return fmap(("*", (p, ("fin",))))
-            intm = fmap_product(*[follow_map(p) for p in op.predecessors])
-        
-        # apply follow map
-        op_follow_map = follow_apply(intm, op, value, context=follow_context)
-
-        # name = op.__class__.__name__
-        # print(name, value)
-        # print("follow({}) = {}".format(name, op_follow_map))
-
-        follow_trace[op] = op_follow_map
-    
-    return expr_value, is_final, trace, follow_trace
+    return rewritten_value, rewritten_prompt
```

### Comparing `lmql-0.0.6.6/src/lmql/ops/token_set.py` & `lmql-0.7b1/src/lmql/ops/token_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from itertools import product
 
 from lmql.utils import nputil
 import numpy as np
 from lmql.runtime.stats import Stats
 from lmql.runtime.caching import cachefile, cache_file_exists
 from lmql.runtime.tokenizer import get_vocab
+from lmql.ops.regex import Regex
 
 class VocabularyMatcher:
     """
     Generates sub-token level logit masks from provided tokens.
     """
     def __init__(self, tokenizer, model_identifier):
         self.tokenizer = tokenizer
@@ -131,35 +132,38 @@
             def do_make_mask():
                 if tokens is not None:
                     mask = self._make_mask_from_tokens(tokens, prefix, exact=exact)
                 elif charlen is not None:
                     mask = self._make_mask_from_char_length(charlen)
                 else:
                     assert regex is not None, "TokenSetConcrete: either tokens or regex must be set."
-                    assert not prefix, "TokenSetConcrete: prefix is not supported for regex."
-                    mask = self._make_mask_from_regex(regex)
+                    mask = self._make_mask_from_regex(regex, prefix)
 
                 if minus: mask = np.logical_not(mask)
 
                 return mask
             
             return VocabularyMatcher.with_cache(cache_keys, do_make_mask)
 
-    def _make_mask_from_regex(self, regex):
+    def _make_mask_from_regex(self, regex, prefix=False):
         regex = regex.replace(" ", self.space_repr)
         regex = regex.replace("\n", self.nl_repr)
-
         regex = regex.replace(" ", self.tokenizer.tokenize(" ")[0])
 
         mask = np.zeros([self.vocab_size], dtype=np.bool_)
-
-        pattern = re.compile(regex, re.UNICODE)
-        for id, subtoken in self.vocab.items():
-            if pattern.match(subtoken) is not None:
-                mask[id] = True
+        if prefix:
+            r = Regex(regex)
+            for id, subtoken in self.vocab.items():
+                if r.is_prefix(subtoken):
+                    mask[id] = True
+        else:
+            pattern = re.compile(regex, re.UNICODE)
+            for id, subtoken in self.vocab.items():
+                if pattern.match(subtoken) is not None:
+                    mask[id] = True
 
         return mask
 
     @property
     def vocab_size(self):
         return self.tokenizer.vocab_size
 
@@ -529,15 +533,15 @@
     return p1.union(p2)
 
 def tset(*tokens, regex=False, prefix=False, exact=False, charlen=None, name=None):
     if charlen is not None:
         return TokenSet(charlen=charlen, name=name)
     if regex:
         assert len(tokens) == 1, "cannot create a TokenSet from multiple regexes."
-        return TokenSet(regex=tokens[0], name=name)
+        return TokenSet(regex=tokens[0], prefix=prefix, name=name)
     if len(tokens) == 1 and type(tokens[0]) is set:
         return TokenSet(set(list(tokens[0])), minus=False, name=name)
     return TokenSet(set(tokens), minus=False, prefix=prefix, exact=exact, name=name)
 
 def charlen_tsets():
     l1 = tset(charlen=1)
     token_lengths = VocabularyMatcher.instance().token_lengths
```

### Comparing `lmql-0.0.6.6/src/lmql/output/http.py` & `lmql-0.7b1/src/lmql/output/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/output/sse.py` & `lmql-0.7b1/src/lmql/output/sse.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/output/ws.py` & `lmql-0.7b1/src/lmql/output/ws.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.7b1/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.7b1/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,20 @@
         
     def task_type(self, task):
         keys = ["model", "max_tokens", "temperature", "logprobs", "user", "logit_bias", "echo"]
         def get(k): 
             if k == "logit_bias": return "-".join([f"{k}={v}" for k,v in sorted(task.get(k, {}).items())])
             return str(task.get(k, "<none>"))
         identifier = "|".join([f"{k}={get(k)}" for k in keys])
+        # check for str or int prompt
+        if isinstance(task["prompt"], str):
+            identifier += "-str"
+        else:
+            identifier += "-int"
+        
         return identifier
 
     def group(self):
         assert len(self.queued_requests) == 0, f"Batcher.groups() called before self.queued_requests was emptied"
 
         buckets = {}
         
@@ -426,15 +432,15 @@
                 return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
             raise StopAsyncIteration
         check_done_task = asyncio.create_task(self.slice.done.wait(), name="check_done_task")
         self.waiting_tasks.append(check_done_task)
         
         get_next_item_task = asyncio.create_task(self.slice.data_queue.get())
         done, pending = await asyncio.wait([get_next_item_task, check_done_task], 
-            return_when=asyncio.FIRST_COMPLETED, timeout=5.0)
+            return_when=asyncio.FIRST_COMPLETED, timeout=self.slice.kwargs.get("timeout", 15.0))
     
         self.waiting_tasks.remove(check_done_task)
 
         if check_done_task in done:
             # this indicates the end of this response stream
             for t in pending: t.cancel()
             if self.n == 0:
@@ -678,15 +684,16 @@
                 request_ids = kwargs.pop("request_id")
                 retries = self.maximum_retries
                 while True:
                     try:
                         if retries != self.maximum_retries:
                             print("Retrying", retries, "more times")
                             await asyncio.sleep(0.5)
-                        res = await self._create(**kwargs)
+                        task = asyncio.create_task(self._create(**kwargs))
+                        res = await asyncio.wait_for(task, timeout=5.5)
                         break
                     except Exception as e:
                         if type(e) is AssertionError:
                             raise e
                         self.stats.errors += 1
                         retries -= 1            
                         print("OpenAI:", str(e), '"' + str(type(e)) + '"', flush=True)
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.7b1/src/lmql/runtime/bopenai/openai_api.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/caching.py` & `lmql-0.7b1/src/lmql/runtime/caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.7b1/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.7b1/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,19 +453,19 @@
                 ids = continued_seq.input_ids
                 for i, (score, token) in enumerate(zip(token_scores[-len(tok):], tok)):
                     self.set_cache([(self.base_key(ids), str(token))], (np.array(token), np.array(score)))
                     ids = np.append(ids, token)
                 
             # determine detseq deterministic flags
             if type(deterministic) is bool:
-                deterministic_flags = np.concatenate([sq.deterministic, np.array([deterministic])])
+                deterministic_flags = np.concatenate([sq.deterministic, np.array([deterministic])], dtype=np.bool_)
                 next_deterministic = np.array([deterministic] * len(completion[1:]))
             else:
                 assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored, but is {} and {}".format(deterministic, completion)
-                deterministic_flags = np.concatenate([sq.deterministic, np.array(deterministic[:1])])
+                deterministic_flags = np.concatenate([sq.deterministic, np.array(deterministic[:1])], dtype=np.bool_)
                 next_deterministic = np.array(deterministic[1:])
 
             # create actual detseq
             return detseq(ids=np.concatenate([sq.input_ids, completion[:1]], axis=0), 
                     next_ids=completion[1:],
                     logprobs=np.concatenate([sq.logprobs, token_scores[:1]], axis=0),
                     next_logprobs=token_scores[1:],
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.7b1/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.7b1/src/lmql/runtime/dclib/dclib_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.7b1/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,46 @@
         if type(seqs_or_seq) is not list:
             seqs = [seqs_or_seq]
             unwrap = lambda v: v[0] if type(v) is list and len(v) == 1 else v
 
         # do not rewrite deterministic sequences (rewrite mask set to False)
         mask_seq_to_rewrite = np.array([s.needs_rewrite for s in seqs], dtype=np.bool_)
 
-        rewriter = self.model_args["modern_rewriter"]
-        rewritten_ids = await rewriter(seqs, mask_seq_to_rewrite)
+        rewriting_iterations = 0
+        results = [None for _ in seqs]
+        still_need_rewrite = list(zip(range(len(seqs)), seqs, mask_seq_to_rewrite))
+
+        did_rewrite = False
+        
+        while len(still_need_rewrite) > 0:
+            rewriting_iterations += 1
+            
+            indices = [i for i, _, _ in still_need_rewrite]
+            seqs = [s for _, s, _ in still_need_rewrite]
+            mask = [v for _, _, v in still_need_rewrite]
+            
+            rewriter = self.model_args["modern_rewriter"]
+            rewritten_ids = await rewriter(seqs, mask)
+            final_result = rewritten_ids.final
+
+            if rewritten_ids.strip_eos[0] != False:
+                did_rewrite = True
+
+            still_need_rewrite = []
+            iteration_results = await self.apply_rewrite(seqs, rewritten_ids, noscore=noscore, unwrap=unwrap)
+            for i, s, done in zip(indices, iteration_results, final_result):
+                results[i] = s
+                if not done and s.is_done():
+                    still_need_rewrite.append((i, s, mask_seq_to_rewrite[i]))
+        
+        # print("rewrite iterations:", rewriting_iterations)
+
+        return unwrap(results)
     
+    async def apply_rewrite(self, seqs, rewritten_ids, noscore=False, unwrap=lambda v: v):
         # update user data, if rewriter provides it
         for s, user_data in zip(seqs, rewritten_ids.user_data):
             s.user_data = deepmerge(deepcopy(s.user_data), user_data) if user_data is not None else s.user_data
             s.user_data["set_by"] = "rewrite"
 
         all_updated_ids = rewritten_ids.appended_input_ids
         if all_updated_ids is None:
@@ -121,23 +150,20 @@
             # offset updated_ids to the number of tokens that are already present as continued_seq
             appended_ids = updated_ids[offset:]
 
             if len(appended_ids) == 0:
                 return DecoderSequence(continued_seq.input_ids, continued_seq.logprobs, continued_seq.deterministic, stop_phrase=continued_seq.stop_phrase,
                                     predecessor=continued_seq, user_data=user_data, sticky_user_data_keys=continued_seq.sticky_user_data_keys, epsilon_node=True)
 
-            # check if rewriting action provides user data specifically for the rewritten sequence
-            # user_data = rewritten_ids.rewritten_seq_user_data[seqidx] or user_data
-
             # value tokens
             num_value_tokens = value_offset - offset
             deterministic = [True if i + 1 > num_value_tokens else False for i in range(len(appended_ids))]
             continuation = (await self.score([continued_seq], [appended_ids], deterministic=deterministic, stop_phrase=False, needs_rewrite=False, user_data=user_data, noscore=noscore))[0]
             
-            continuation.stop_phrase = s.stop_phrase[:len(continuation.input_ids)]
+            # continuation.stop_phrase = s.stop_phrase[:len(continuation.input_ids) - 1] 
             continuation.needs_rewrite = False
             
             steps = 0
             while type(continuation) is DeterministicDecoderSequence and len(continuation.next_ids) > 0 and steps < num_value_tokens:
                 continuation.user_data = deepcopy(s.predecessor.user_data)
                 # print("continuation.user_data", continuation.user_data, flush=True)
                 continuation = continuation.extend(Continuation(continuation.next_ids[0], continuation.next_logprobs[0], continuation.user_data))
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.7b1/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,19 @@
         else:
             assert predecessor is not None, "Predecessor is None"
             self.prompt_len = self.predecessor.prompt_len
 
         self.epsilon_node = epsilon_node
 
         # if no deterministic is provided assume all tokens to be deterministic
-        if deterministic is None: self.deterministic = np.array([True for _ in range(len(input_ids))])
+        if deterministic is None: self.deterministic = np.array([True for _ in range(len(input_ids))], dtype=np.bool_)
         else: self.deterministic = deterministic
+
+        assert self.deterministic.dtype == np.bool_
+
         assert len(self.deterministic) == len(self.input_ids), "Length of determinism status does not match length of inputs"
 
         # if no stop_phrase is provided assume no tokens to be stop_phrase
         if stop_phrase is None: self.stop_phrase = np.array([False for _ in range(len(input_ids))])
         else: self.stop_phrase = stop_phrase
         assert len(self.stop_phrase) == len(self.input_ids), "Length of stop_phrase status does not match length of inputs for {} and {}".format(self.stop_phrase, self.input_ids)
 
@@ -246,21 +249,46 @@
         if self.epsilon_node: text = [""]
         root = False
         if self.predecessor is None:
             text = await self.detokenized("seqtext")
             # text = str([await get_tokenizer().decode(self.input_ids)])[2:-2],
             root = True
 
+        # handle empty seq
+        if len(self.input_ids) == 0:
+            return {
+                "seq_id": self.id,
+                "text": [""],
+                "seqtext": "",
+                "root": root,
+                "logprob": [],
+                "logprobs": [],
+                "logprobs_det": [],
+                "logprobs_norm": [],
+                "seqlogprob": 0,
+                **({"deterministic": True} if self.epsilon_node else {}),
+                "score_det": 0,
+                "score_nor": 0,
+                "score_tot": 0,
+                "pool": self.pool,
+                "user_data": await self.user_data_json(),
+                "token_id": "",
+                "deterministic_5": [],
+                "stop_phrase_5": [],
+                "prompt_len" : self.prompt_len,
+                "sticky_user_data_keys": list(self.sticky_user_data_keys)
+            }
+
         return {
             "seq_id": self.id,
             # "input_ids": self.input_ids.tolist(),
             "text": [text],
             "seqtext": seqtext,
             "root": root,
-            "logprob": self.logprobs[-1],
+            "logprob": self.logprobs[-1:] if len(self.logprobs) > 0 else [],
             "logprobs": self.logprobs[-5:].tolist(),
             "logprobs_det": self.logprobs[-5:][self.deterministic[-5:]].tolist(),
             "logprobs_norm": self.logprobs[-5:][~self.deterministic[-5:]].tolist(),
             "seqlogprob": self.logprobs.sum(),
             **({"deterministic": True} if self.epsilon_node else {}),
             # "score_det": alpha_length_normalized.score(self.logprobs[self.prompt_len:][self.deterministic[self.prompt_len:]], alpha=self.data("scorer_alpha")),
             # "score_nor": alpha_length_normalized.score(self.logprobs[self.prompt_len:][~self.deterministic[self.prompt_len:]], alpha=self.data("scorer_alpha")),
@@ -331,29 +359,29 @@
         stop_phrase = self.detect_stop_phrase(continuation)
 
         return DecoderSequence(
             input_ids_or_str=np.concatenate([self.input_ids, continuation.token.reshape(1)]), 
             logprobs=np.concatenate([self.logprobs, continuation.logprob.reshape(1)]),
             # deterministic tokens are only extended in DeterministicDecoderSequence.extend.
             # So here, all extended tokens are non-deterministic, i.e. model predictions.
-            deterministic=np.concatenate([self.deterministic, np.array([False])]),
+            deterministic=np.concatenate([self.deterministic, np.array([False])], dtype=np.bool_),
             stop_phrase=stop_phrase,
             predecessor=self,
             user_data=self.extend_user_data(continuation),
             sticky_user_data_keys=self.sticky_user_data_keys,
             internal=internal
         )
 
     def detect_stop_phrase(self, continuation):
         old_stop_phrase = self.stop_phrase
         new_stop_phrase = np.concatenate([old_stop_phrase, np.array([False])])
         
         stop_phrases = self.data("head").stopping_phrases["tokenized"] if self.data("head") is not None else []
 
-        if stop_phrases is None:
+        if stop_phrases is None or len(stop_phrases) == 0:
             return new_stop_phrase
 
         ids = np.concatenate([self.input_ids, continuation.token.reshape(1)])
         for stop in stop_phrases:
             len_stop = len(stop)
             if all(ids[-len_stop:] == stop):
                 new_stop_phrase[-len_stop:] = True
@@ -364,18 +392,19 @@
     def __len__(self):
         return len(self.input_ids)
 
     def __repr__(self) -> str:
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         return f"<seq token_len={len(self.input_ids)} ids=[... {ids}]>"
 
-    async def text(self, offset:int=None, limit:int=None, pretty=True) -> str:
+    async def text(self, offset:int=None, limit:int=None, pretty=False) -> str:
         offset = offset or 0
         limit = limit or len(self.input_ids)
         raw_text = get_tokenizer().decode(self.input_ids[offset:limit])
+        
         if not pretty: 
             return raw_text
         else:
             return str([raw_text])[2:-2]
 
     async def str(self, full=False) -> str:
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
@@ -399,14 +428,15 @@
     def make_successors(self, next_tokens, next_token_scores, logits, user_data=None):
         # remove very low scoring tokens (likely they were masked and therefore score low)
         next_tokens = nputil.ensure_iterable(next_tokens)
         next_token_scores = nputil.ensure_iterable(next_token_scores)
         
         tokens = [t for t, s in zip(next_tokens, next_token_scores) if s > DecoderSequence.truncation_threshold]
         scores = [s for s in next_token_scores if s > DecoderSequence.truncation_threshold]
+
         if len(tokens) == 0:
             print("WARNING: all continuation token fall below truncation threshold. This is likely due to a too small truncation factor. Try increasing it. Continuing with the top 1 token.")
             tokens = [t for t, s in zip(next_tokens, next_token_scores)][:1]
             scores = [s for s in next_token_scores][:1]
         next_tokens = np.stack(tokens, axis=0)
         next_token_scores = np.stack(scores, axis=0)
 
@@ -482,37 +512,33 @@
     # async def text(self, offset: int = None, limit: int = None, pretty=True) -> str:
     #     return "<detseq> " + await super().text(offset, limit, pretty)
 
     def align_user_data(self):
         if self.user_data is None: return
         if not "head" in self.user_data: return
 
-        # lmql-specific user data should be different for deterministic sequences
-        head_variable = resolve_path(self.user_data, "head.variable")
-
-        if head_variable is not None:
-            # if "before(" in head_variable:
-            #     head_variable = head_variable.split(":before(", 1)[0]
-            # if head_variable == "__done__":
-            #     set_path(self.user_data, "head", self.user_data["head"].updated(variable="__done__"))
-            # else:
-            #     if len(self.next_ids) > 0:
-            #         set_path(self.user_data, "head", self.user_data["head"].updated(variable=head_variable + ":before(" + str(len(self.next_ids)) + ")"))
-            #     else:
-            #         set_path(self.user_data, "head", self.user_data["head"].updated(variable=head_variable))
-            # deterministic sequences don't have stopping phrases
-            set_path(self.user_data, "head", self.user_data["head"].updated(stopping_phrases={"tokenized": [], "text": []}))
-        else:
-            set_path(self.user_data, "head", self.user_data["head"].updated(variable="<prompt>"))
+        # lmql-specific user data has to be different for deterministic sequences
         
-        if len(self.next_ids) > 0:
-            set_path(self.user_data, "head", self.user_data["head"].updated(mask="{token_id=" + str(self.next_ids[0]) + "}"))
-        else:
-            set_path(self.user_data, "head", self.user_data["head"].updated(mask="<not available yet>"))
-    
+        # make sure to update all "head" an "head[...]" user data keys (head[...] belong to subinterpreters)
+        head_user_data_keys = [k for k in self.user_data.keys() if k.startswith("head[") or k == "head"]
+        
+        for head_key in head_user_data_keys:
+            head_variable = resolve_path(self.user_data, f"{head_key}.variable")
+            
+            if head_variable is not None:
+                # deterministic sequences don't have stopping phrases
+                set_path(self.user_data, head_key, self.user_data[head_key].updated(stopping_phrases={"tokenized": [], "text": []}))
+            else:
+                set_path(self.user_data, head_key, self.user_data[head_key].updated(variable="<prompt>"))
+            
+            if len(self.next_ids) > 0:
+                set_path(self.user_data, head_key, self.user_data[head_key].updated(mask="{token_id=" + str(self.next_ids[0]) + "}"))
+            else:
+                set_path(self.user_data, head_key, self.user_data[head_key].updated(mask="<not available yet>"))
+
     @property
     def is_query_constrained(self):
         """Deterministic sequences are not query constrained, as long as they are fixed to their predetermined content."""
         return True if len(self.next_ids) == 0 else False
 
     async def json(self):
         seqtext = await self.detokenized("seqtext")
@@ -563,25 +589,24 @@
         if len(self.next_ids) <= 0:
             return super().extend(continuation)
 
         assert continuation.token == self.next_ids[0], "deterministic sequences must be extended by the predetermined next token: provided: " + str(continuation.token) + ", predetermined: " + str(self.next_ids[0])
 
         extended_input_ids = np.concatenate([self.input_ids, continuation.token.reshape(1)])
         extended_logprobs = np.concatenate([self.logprobs, continuation.logprob.reshape(1)])
-        extended_deterministic = np.concatenate([self.deterministic, np.array([True]) if self.next_deterministic is None else self.next_deterministic[0:1]])
+        extended_deterministic = np.concatenate([self.deterministic, np.array([True]) if self.next_deterministic is None else self.next_deterministic[0:1]], dtype=np.bool_)
 
         reduced_next_ids = self.next_ids[1:]
         reduced_next_logprobs = self.next_logprobs[1:] if self.next_logprobs is not None else None
         reduced_deterministic = None if self.next_deterministic is None else self.next_deterministic[1:]
 
         user_data = self.extend_user_data(continuation)
 
         stop_phrase = self.detect_stop_phrase(continuation)
         if self.data("injected_stop_phrase"):
-            print(self)
             assert not extended_deterministic[-1]
 
         return DeterministicDecoderSequence(
             input_ids=extended_input_ids, 
             logprobs=extended_logprobs, 
             deterministic=extended_deterministic,
             stop_phrase=stop_phrase,#np.concatenate([self.stop_phrase, self.data("injected_stop_phrase")]),
@@ -636,14 +661,18 @@
             score = self.next_logprobs[0]
         else:
             score = raw_logits[predetermined_token]
             if score < DecoderSequence.truncation_threshold:
                 print("warning: a deterministic token scored below the truncation threshold ({})".format(DecoderSequence.truncation_threshold))
         
         return Continuation(predetermined_token, score, user_data)
+    
+    def __str__(self) -> str:
+        ids = ", ".join([str(i) for i in self.input_ids[-10:]])
+        return f"<detseq token_len={len(self.input_ids)} ids=[... {ids}] next_ids=[{self.next_ids[:10]}]>"
 
 def is_deterministic(s):
     return issubclass(type(s), DeterministicDecoderSequence)
 
 def next_is_deterministic(s):
     return is_deterministic(s) and len(s.next_ids) > 0
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/dclib/decoders.py` & `lmql-0.7b1/src/lmql/runtime/dclib/decoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,14 +465,15 @@
         i = 0
 
         while not is_seq_beams_search_done(active, variable_done, num_beams=b):
             # inner variable decoding (beam_sample with 2*n beams and branching factor n)
             if sample:
                 active = active.extend(await model.sample(active, temperature=temperature, num_samples=b))
             else:
+                kwargs.pop("temperature", None)
                 active = active.extend(await model.topk_continuations(active, k=b, **kwargs))
             
             active = await model.rewrite(active)
 
             active, variable_done = (active + variable_done).separate_by(is_active_variable)
             active = dc.topk(active, b)
 
@@ -488,14 +489,15 @@
         top_variable_done = dc.seqs()
 
         while not (len(active) == 0 or (len(top_variable_done) == b and dc.max_score(active, scorer=nw_score) < dc.min_score(top_variable_done, scorer=nw_score))):
             # inner variable decoding (beam_sample with 2*n beams and branching factor n)
             if sample:
                 active = active.extend(await model.sample(active, temperature=temperature, num_samples=b))
             else:
+                kwargs.pop("temperature", None)
                 active = active.extend(await model.topk_continuations(active, k=b, **kwargs))
             
             for s in active.flatten().items():
                 # s.data("eos_score", s.score
                 s.data("eos_score", regular_scorer(s.logprobs))
 
             active = await model.rewrite(active)
@@ -599,7 +601,10 @@
     yield done
     
     dc.finish(dc.array_sorted(done.flatten(), key=lambda s: -s.logprobs.sum()))
 
 def is_seq_beams_search_done(active_hypotheses, done_hypotheses, num_beams, scorer=None):
     return len(active_hypotheses) == 0 or (len(done_hypotheses) == num_beams and dc.max_score(active_hypotheses, scorer=scorer) < dc.min_score(done_hypotheses, scorer=scorer))
 
+@dc.decoder
+def incontext(*args, **kwargs):
+    raise NotImplementedError("incontext is not a valid decoder function for standalone use")
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/interpreter.py` & `lmql-0.7b1/src/lmql/runtime/interpreter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,32 @@
-import inspect
 import asyncio
+import inspect
 from collections import namedtuple
-
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, List, Union, NamedTuple, Tuple
+from typing import Any, Dict, Optional, List, Union, NamedTuple, Tuple, Set
 import numpy as np
-from lmql.runtime.multi_head_interpretation import InterpretationHead, InterpreterCall, InterpretationHeadDone
-from lmql.runtime.program_state import ProgramState
+
+import re
+import lmql.ops.ops as ops
 import lmql.runtime.dclib as dc
+from lmql.language.qstrings import (DistributionVariable, TemplateVariable,
+                                    qstring_to_stmts)
+from lmql.ops.follow_map import FollowMap
+from lmql.ops.token_set import VocabularyMatcher, has_tail, tset
+from lmql.ops.follow_map import fmap
+from lmql.runtime.interrupt import interrupt
+from lmql.runtime.model_registry import LMQLModelRegistry
+from lmql.runtime.multi_head_interpretation import (InterpretationHead,
+                                                    InterpretationHeadDone,
+                                                    InterpreterCall)
+from lmql.runtime.program_state import ProgramState
 from lmql.runtime.stats import Stats
 from lmql.runtime.tokenizer import LMQLTokenizer
+
+from lmql.utils.nputil import replace_inf_nan_with_str
 from lmql.runtime.interrupt import interrupt
 from lmql.language.qstrings import qstring_to_stmts, TemplateVariable, DistributionVariable, unescape_qstring
 from lmql.utils.nputil import replace_inf_nan_with_str
 
 from lmql.ops.token_set import VocabularyMatcher, has_tail
 from lmql.runtime.model_registry import LMQLModelRegistry
 from lmql.models.model import model, LMQLModel
@@ -21,28 +34,48 @@
 from lmql.ops.token_set import tset
 import lmql.ops.ops as ops
 
 class _DCLibDebugPrinter: pass
 _DCLibDebugPrinter.printer = None
 
 def set_dclib_debug_printer(printer):
-    _DCLibDebugPrinter.printer = printer
+    if hasattr(printer, "add_decoder_state"):
+        _DCLibDebugPrinter.printer = printer
+
+emoji_mapping = {}
 
 @dataclass
 class RewrittenInputIds:
     appended_input_ids: List[np.ndarray]
     strip_eos: bool = True
     user_data: Optional[Union[List[Dict[str, Any]], Dict[str, Any]]] = None
     value_offset: Optional[int] = None
+    
+    # indicates whether or not this rewrite is a final rewrite (i.e. no further rewrites will be applied if it ends on eos)
+    final: bool = True
 
     rewritten_seq_user_data: Optional[Union[List[Dict[str, Any]], Dict[str, Any]]] = None
 
+    @staticmethod
+    def stack(results):
+        return RewrittenInputIds(
+            appended_input_ids=[r.appended_input_ids if r is not None else None for r in results],
+            strip_eos=[r.strip_eos if r is not None else None for r in results],
+            user_data=[r.user_data if r is not None else None for r in results],
+            value_offset=[r.value_offset if r is not None else None for r in results],
+            rewritten_seq_user_data=[r.rewritten_seq_user_data if r is not None else None for r in results],
+            final=[r.final if r is not None else True for r in results]
+        )
+
 class advance: pass # used as symbol
 
 class PromptState(NamedTuple):
+    interpreter: 'PromptInterpreter'
+    subinterpreters: Set['SubInterpreter']
+
     variable : str
     prompt : str
     
     stmt_buffer : List[Any]
     query_head : Any
     program_state : Any
     
@@ -54,17 +87,18 @@
 
     # only set after processing where clause
     valid: Optional[bool]
     final: Optional[str] 
     mask : Optional[Any]
     stopping_phrases: Optional[Any]
     where: Optional[Any]
+    tail: Optional[str]
 
     def __str__(self):
-        return f"<PromptState '{self.prompt}'>"
+        return f"<PromptState '{self.variable}' '{[self.prompt]}'>"
 
     def updated(self, **updated):
         data_dict = self._asdict()
         data_dict.update(updated)
         return PromptState(**data_dict)
     
     def full_where_condition(self, interpreter):
@@ -72,25 +106,25 @@
             return self.constraints
         elif self.constraints is None:
             return interpreter.where
         else:
             return ops.AndOp([interpreter.where, self.constraints])
 
 class LMQLContext:
-    def __init__(self, interpreter, state):
+    def __init__(self, interpreter, state, prompt):
         self.interpreter = interpreter
         
         if state:
             self.program_state: ProgramState = state.program_state
             self.state = state
             self.prompt = state.prompt
         else:
-            self.program_state = ProgramState()
+            self.program_state = ProgramState(prompt)
             self.state = None
-            self.prompt = "<prompt not available>"
+            self.prompt = prompt
 
         self.program_state.runtime = interpreter
 
     async def json(self):
         return self.program_state
 
     # LMQL runtime API
@@ -160,57 +194,74 @@
 
 class PromptInterpreter:
     """
     The PromptInterpreter is the main entry point for an LMQL query. It handles program execution, 
     token masking and scripted interaction during query execution.
     """
 
-    def __init__(self, force_model=None) -> None:
+    def __init__(self, context=None, force_model=None) -> None:
         # model-specific components
         self.model = force_model
         self.model_identifier = force_model
         self.tokenizer: LMQLTokenizer = None
 
         # decoder configuration
         self.decoder = None
-        self.decoder_kwargs = {}
+        self.decoder_kwargs = None
         self.decoder_step = 0
-        
+
         # extra interpreter flags passed via @lmql.query/@lmql.compiled_query
         self.extra_kwargs = {}
 
         # query program
-        self.fct = None
         self.root_state = None
 
         # constraints
         self.where = None
 
         # distribution variable if any
         self.distribution_variable = None
         self.distribution_values = None
 
         # logging and debugger output
         self.output_writer = None
         self.prefers_compact_mask  = False
+        
+        # caching configuration
         self.caching = True
         self.cache_file = None
         self.show_speculative = False
         
+        # key to use to store program statein decoding tree
+        self.user_data_key = "head"
+
         self.eager_followmap_expansion = True
+        
+        # subinterpreters in case of inline queries
+        self.subinterpreters = {}
+
+        # decoder graph if decoder graph logging is enabled
+        self.decoder_graph = None
+
+        # context to determine model
+        self.context = context
 
     def set_where_clause(self, where):
         self.where = where
 
     def set_extra_args(self, **kwargs):
         if "output_writer" in kwargs:
             self.output_writer = kwargs["output_writer"]
+        # store remaining flags
         self.extra_kwargs.update(kwargs)
 
     def set_decoder(self, method, **kwargs):
+        # remove compiler-level flags
+        if "dump_compiled_code" in kwargs:
+            kwargs.pop("dump_compiled_code")
         self.decoder_kwargs = kwargs
         self.decoder_kwargs["decoder"] = method
 
         if "backend" in kwargs:
             LMQLModelRegistry.backend_configuration = kwargs["backend"]
 
     def set_model(self, model_name):
@@ -259,58 +310,61 @@
 
         self.model = client
 
     async def advance(self, state: PromptState):
         if state.variable is not None:
             return state
         
+        active_decoder_graph = dc.DecoderSequence.graph
+        dc.DecoderSequence.graph = None
+        
         variable = state.variable
         constraints = state.constraints
         
         stmt_buffer = state.stmt_buffer
         constraints_after_last_continue = constraints
         program_variables_after_last_continue = None
         prompt = state.prompt
 
-        distribution_variable = None
-        distribution_values = None
-
         query_head = state.query_head
 
         async def continue_for_more_prompt_stmts():
             nonlocal stmt_buffer, query_head, constraints_after_last_continue, program_variables_after_last_continue
 
             if len(stmt_buffer) != 0: return
             
             if query_head.current_args is None:
                 query_head = query_head.copy()
                 assert query_head.fresh_copy, "query head must be fresh copy to avoid state sharing side effects"
-                query_head.context = LMQLContext(self, state)
+                query_head.context = LMQLContext(self, state, prompt)
                 await query_head.continue_()
 
             qstring = query_head.current_args[0]
             constraints_after_last_continue = query_head.current_args[2] if len(query_head.current_args) > 2 else None
             
             if len(query_head.current_args) > 2:
                 program_variables_after_last_continue = query_head.current_args[1]
             
             stmt_buffer = qstring_to_stmts(qstring) + [advance]
 
             # return context used for last continue_
             return query_head.context
         
+        # disable DecoderSequence.graph for the duration of executing the prompt
+
         try:
             while variable is None and query_head.result is None:
                 if len(stmt_buffer) == 0 and variable is None:
                     await continue_for_more_prompt_stmts()
 
                 s = stmt_buffer[0]
 
                 if type(s) is str:
-                    prompt += unescape_qstring(s)
+                    s = self.process_query_string(s)
+                    prompt += s
                     stmt_buffer = stmt_buffer[1:]
                     constraints = None
                     
                     # keep latest prompt in transient state
                     state = state.updated(prompt=prompt)
                 elif type(s) is TemplateVariable:
                     variable = s.name
@@ -326,107 +380,74 @@
                     # distribution variables are skipped here, as they are handled in a postprocessing step after returning an LMQL result
                     # self.query_head must terminate after this part of the prompt (ensure by validation)
                     stmt_buffer = stmt_buffer[1:]
                     assert len([s for s in stmt_buffer if s is not advance]) == 0, "Distribution variables must be the last statement in a prompt, but is {}".format(stmt_buffer)
                     # this will consume the set_distribution call
                 elif s is advance:
                     query_head: InterpretationHead = query_head.copy()
-                    query_head.context = LMQLContext(self, state)
+                    query_head.context = LMQLContext(self, state, prompt)
                     assert query_head.fresh_copy, "query head must be fresh copy to avoid state sharing side effects"
                     await query_head.advance(None)
                     stmt_buffer = stmt_buffer[1:]
                 else:
                     assert False, "prompt interpreter encountered unsupported prompt stmt of type {}: {}".format(type(s), s)
         except InterpretationHeadDone:
             pass
 
+        # re-enable DecoderSequence.graph
+        dc.DecoderSequence.graph = active_decoder_graph
+        if self.output_writer is not None:
+            self.output_writer.disable = False
+
         program_state = state.program_state.copy()
         program_state.python_scope = program_variables_after_last_continue or program_state.python_scope
 
         # merge named tuple with new stmt_buffer
         return state.updated(
             variable=variable,
             prompt=prompt,
             constraints=constraints,
             stmt_buffer=stmt_buffer,
             query_head=query_head,
             program_state=program_state
         )
 
+    def process_query_string(self, s: str):
+        if not ("turbo" in self.model_identifier or "gpt-4" in self.model_identifier):
+            # replace all r"<lmql:(.*?)\/>" tags with ((\1))
+            s = re.sub(r"<lmql:(.*?)\/>", "", s)
+        s = unescape_qstring(s)
+        return s
+
     def interpreter_state_user_data(self, state: PromptState):
-        return {"head": state}
+        return {self.user_data_key: state}
 
     def interpreter_state_from_user_data(self, seq, noroot=False):
         if noroot:
-            if seq.data("head") is None:
+            if seq.data(self.user_data_key) is None:
                 return None
-        state_dict = seq.data("head")
+        state_dict = seq.data(self.user_data_key)
         if state_dict is None and not noroot:
             return self.root_state
+        assert state_dict.interpreter is self, "error: interpreter state does not belong to this interpreter, {} vs. {} via {}".format(state_dict.interpreter, self, self.user_data_key)
+        
         return state_dict
 
-    async def where_for_sequence(self, s: dc.DecoderSequence, needs_masking, seqidx, **kwargs):
-        mask, logit_mask, state = await self.where_step_for_sequence(s, needs_masking, seqidx, **kwargs)
+    async def where_for_sequence(self, s: dc.DecoderSequence, needs_masking, seqidx, return_follow_map=False, **kwargs):
+        mask, logit_mask, state = await self.where_step_for_sequence(s, needs_masking, seqidx, return_follow_map=return_follow_map, **kwargs)
 
         # check for tail and prescore
-        if hasattr(self.dcmodel, "prescore_tokens"):
+        if hasattr(self.dcmodel, "prescore_tokens") and (not type(s) is dc.DeterministicDecoderSequence or len(s.next_ids) == 0):
             if has_tail(mask):
                 tail_tokenized = self.tokenizer.tokenize(mask.tail, asbytes=True)
                 await self.dcmodel.prescore_tokens(s, tail_tokenized, noscore=kwargs.get("noscore", False))
-        
-        return logit_mask, state
 
-        # eager follow map expansion (w/o) model prediction in between
-
-        # # if we cannot predict the next token deterministically
-        # if mask is None or len(mask) > 1 or not needs_masking:
-        #     # ask the model to predict the next token
-        #     return logit_mask, state
-
-        # # otherwise, we can expand the sequence deterministically, until a probabilistic token mask is encountered
-        # masks = [mask]
-        # logit_masks = [logit_mask]
-        # states = [state]
-
-        # #  checks if current mask can be expanded further
-        # mask_can_be_expanded_further = lambda: mask is not None and len(mask) == 1 and mask.mask.argmax() != self.model.get_tokenizer().eos_token_id
-
-        # unexpanded_offset = len(s.input_ids)
-        # initial_s = s
-
-        # # expand as far as possible
-        # while mask_can_be_expanded_further() and self.eager_followmap_expansion:
-        #     # extend the sequence with the next token
-        #     s = s.extend(dc.Continuation(mask.mask.argmax(), np.array([0]), None), internal=True)
-        #     # do not futher expand sequences at <eos>
-        #     if s.is_done(): break
-
-        #     # rewrite to get next-token user data and set it on the sequence
-        #     rewrite_result: RewrittenInputIds = await self.rewrite_for_sequence(s, True, assert_no_advance=True)
-        #     s.user_data = rewrite_result.user_data
-        #     s.user_data["set_by"] = "rewrite"
-
-        #     # call another step of where_for_sequence
-        #     mask, logit_mask, state = await self.where_step_for_sequence(s, needs_masking, seqidx, **kwargs)
-
-        #     if mask_can_be_expanded_further():
-        #         # save the current mask
-        #         masks.append(mask)
-        #         logit_masks.append(logit_mask)
-        #         states.append(state)
-
-        # # pre-score the expanded sequences
-        # if len(s.input_ids) - unexpanded_offset > 0:
-        #     num_to_score = len(s.input_ids) - unexpanded_offset
-        #     if hasattr(self.dcmodel, "prescore"):
-        #         await self.dcmodel.prescore([initial_s], [s.input_ids[-num_to_score:]], deterministic=[[False] * num_to_score], user_data=[states[-num_to_score:]], noscore=kwargs.get("noscore", False))
-
-        # return logit_masks[0], states[0]
+        return logit_mask, state
 
-    async def where_step_for_sequence(self, s: dc.DecoderSequence, needs_masking, seqidx, **kwargs):
+    async def where_step_for_sequence(self, s: dc.DecoderSequence, needs_masking, seqidx, return_follow_map=False, **kwargs):
         state = self.interpreter_state_from_user_data(s)
         
         if not needs_masking:
             return None, None, self.interpreter_state_user_data(state)
 
         is_done = state.query_head.result is not None
 
@@ -444,28 +465,41 @@
         where = self.where
 
         if is_done:
             mask = tset("eos")
             logit_mask = mask.mask
             stopping_phrases = {"text": [], "tokenized": []}
             follow_trace = None
+            
+            follow_map = fmap(
+                ("eos", (True, "fin")),
+                ("*", (False, "fin"))
+            )
         elif variable is not None:
+            is_before = ":before" in variable
             if ":before" in variable:
                 variable = variable.split(":before",1)[0]
 
             text = await s.text(variable_offset, pretty=False)
             diff_text = text[len(await s.text(variable_offset, limit=-1, pretty=False)):]
 
+            # run applicable inline ops (sub interpreters)
+            subvalid, subfollow, state = await self.subinterpreter_results(s, variable, text, diff_text, state, is_before, **kwargs)
+
             # current context
             program_state: ProgramState = state.program_state.copy()
             program_state.set(variable, text, scores=(), diff=diff_text, montonicity="inc")
+            program_state.subinterpreter_results = subvalid
+            program_state.prompt = state.prompt
 
             # follow context
             follow_program_state: ProgramState = state.program_state.copy()
             follow_program_state.set(variable, text + str(ops.NextToken), scores=(), diff=diff_text, montonicity="inc")
+            follow_program_state.subinterpreter_results = subfollow
+            follow_program_state.prompt = state.prompt
 
             # determine full where condition
             where = state.full_where_condition(self)
 
             # digest token with where expr
             valid, is_final, trace, follow_trace = ops.digest(where,
                 context=program_state,
@@ -485,21 +519,25 @@
             # check stopping conditions
             stopping_conditions: List[ops.StopAtOp] = ops.execute_op_stops_at_only(state.variable, where, trace)
             for sc in stopping_conditions:
                 stop_trace = trace.copy()
                 del stop_trace[sc]
                 # check if stopping phrase applies in this step
                 if ops.execute_op(sc, stop_trace, context=program_state, semantics="stop"):
-                    # print("apply stop", sc, [text], [diff_text])
                     mask = tset("eos")
                     logit_mask = mask.mask
+                    follow_map = fmap(
+                        ("eos", (True, "fin")),
+                        ("*", (False, "fin"))
+                    )
                     trace[sc] = (sc.stopping_phrase(trace), "stopped")
             stopping_phrases = {
                 "text": [sc.stopping_phrase(trace) for sc in stopping_conditions if type(sc) is ops.StopBeforeOp],
-                "tokenized": [self.tokenizer.tokenize(sc.stopping_phrase(trace), asbytes=True) for sc in stopping_conditions if type(sc) is ops.StopBeforeOp]
+                "tokenized": [self.tokenizer.tokenize(sc.stopping_phrase(trace), asbytes=True) 
+                              for sc in stopping_conditions if type(sc) is ops.StopBeforeOp and sc.stopping_phrase(trace) is not None]
             }
 
         else:
             assert False, f"error: where() is called but current variable and current prompt are None and query head has result {state.query_head.result}"
 
         await self.debugger_output(state, s, valid, is_final, mask, stopping_phrases, program_state, trace, text, where)
 
@@ -509,14 +547,23 @@
                         final=is_final,
                         mask=mask,
                         program_state=program_state,
                         stopping_phrases=stopping_phrases,
                         where=await self.where_graph_with_trace(where, trace, follow_trace)
         )
 
+        if has_tail(mask):
+            state = state.updated(tail = mask.tail)
+
+        if return_follow_map:
+            return mask, follow_map, self.interpreter_state_user_data(state)
+
+        # truncate mask to remove LMQL specific token IDs
+        logit_mask = self.tokenizer.truncate_to_model_dim(logit_mask)
+
         # no mask, no logits processing
         if logit_mask is None:
             return None, None, self.interpreter_state_user_data(state)
         
         # translate boolean mask to logit bias mask
         if len(mask) == 1:
             logit_mask = mask.mask.argmax()
@@ -555,41 +602,110 @@
         zipped_task_inputs = zip(seqs, additional_logits_processor_mask, range(len(seqs)))
         token_mask_tasks = [self.where_for_sequence(s, needs_masking, seqidx, **kwargs) for s,needs_masking, seqidx in zipped_task_inputs]
         results = [(mask, user_data) for mask, user_data in await asyncio.gather(*token_mask_tasks)]
         
         return TokenMask([r[0] for r in results], [r[1] for r in results])
 
     async def rewrite_for_sequence(self, seq: dc.DecoderSequence, needs_rewrite, assert_no_advance=False):
-        if not needs_rewrite:
+        if not needs_rewrite and not seq.is_done():
             return None
+    
+        # assert len([h for h in seq.user_data.keys() if "head" in h]) <= 2, "at max two heads are allowed in a sequence user_data"
 
         # obtain interpreter state from predecessor node
         state = self.interpreter_state_from_user_data(seq.predecessor, noroot=True)
-        
         assert state is not None, "prompt interpreter state must be set in predecessor node"
 
+        if state.tail is not None:
+            rewritten_state = state.updated(tail=None)
+            prompt_ids = seq.input_ids.tolist()
+            tail_ids = self.tokenizer.tokenize(state.tail, asbytes=True)
+            tail_ids = tail_ids[:-1]
+            if len(tail_ids) > 1:
+                updated_ids = prompt_ids + tail_ids[1:]
+
+                return RewrittenInputIds(
+                    appended_input_ids=updated_ids,
+                    strip_eos=False,
+                    value_offset=state.variable_offset + len(tail_ids),
+                    user_data=self.interpreter_state_user_data(state),
+                    rewritten_seq_user_data=self.interpreter_state_user_data(rewritten_state)
+                )
+
+        # first check for sub-interpreters
+        subinterpreters: Set[SubInterpreter] = state.subinterpreters.copy()
+        sub_results = []
+        subrewrite_applied = False
+
+        assert len(subinterpreters) <= 1
+
+        user_data = seq.data() or {}
+
+        for si in list(subinterpreters):
+            if si.user_data_key not in seq.predecessor.user_data:
+                subinterpreters.remove(si)
+                continue
+
+            result: RewrittenInputIds = await si.rewrite_for_sequence(seq, needs_rewrite, assert_no_advance=assert_no_advance)
+            # print("sub rewrite result", result)
+            user_data = dc.deepmerge(user_data, result.user_data)
+
+            if result.appended_input_ids is not None or result.strip_eos != False:
+                assert not subrewrite_applied, "subinterpreter must not apply rewrite if another subinterpreter already did"
+
+                # apply rewrite
+                sub_results.append(result)
+
+                # remove subinterpreter if it rewrites to an eos token
+                if result.appended_input_ids is not None and result.appended_input_ids[-1] == self.tokenizer.eos_token_id:
+                    subinterpreters.remove(si)
+                subrewrite_applied = True
+
+        if len(sub_results) > 0:
+            # make sure that changes to 'subinterpreters' are reflected in the state of the parent interpreter 
+            # if a subtinterpreter has been removed
+            state = state.updated(subinterpreters=subinterpreters)
+            sub_results[0].user_data = dc.deepmerge(sub_results[0].user_data, self.interpreter_state_user_data(state))
+            sub_results[0].rewritten_seq_user_data = dc.deepmerge(sub_results[0].rewritten_seq_user_data, self.interpreter_state_user_data(state))
+            
+            assert len(sub_results) == 1, "internal limitation: multiple concurrent subinterpreter rewrites are currently not supported. are you using more than one strategy constraint on the same variable?"
+
+            sub_result = sub_results[0]
+            sub_result.final = False
+            return sub_result
+
         if seq.is_done() and state.variable is not None:
             program_state = state.program_state.copy()
+            program_state.prompt = state.prompt
             variable = state.variable
             
             text = (await seq.text(offset=state.variable_offset, limit=-1, pretty=False))
             text_diff = text[len(await seq.text(state.variable_offset, limit=-2, pretty=False)):]
             
             variable_value = text
             # set raw variable value
             program_state.set(variable, variable_value, scores=(), diff=text_diff, montonicity="fin")
 
-            # get full where condition
             where = state.full_where_condition(self)
 
             # apply postprocessing, if constraints specify it
             # - variable_value is the postprocessed, converted value (does not have to be a string)
             # - postprocessed_prompt is the string in the prompt that corresponds to the variable value
             variable_value, postprocessed_prompt = ops.execute_postprocess(where, variable, variable_value, context=program_state)
-            
+
+            if type(variable_value) is SubInterpreter:
+                si = variable_value
+                result_state = si.interpreter_state_from_user_data(seq)
+                if result_state.query_head.result is not None:
+                    variable_value = result_state.query_head.result
+                    if type(variable_value) is LMQLResult:
+                        postprocessed_prompt = variable_value.prompt
+                    else:
+                        postprocessed_prompt = str(result_state.query_head.result)
+
             # set postprocessed variable value and program value
             program_state.set(variable, postprocessed_prompt, program_value=variable_value, scores=(), diff="", montonicity="fin")
 
             # current variable is done
             variable = None
             prompt = state.prompt
 
@@ -600,28 +716,35 @@
             
             appended_value_prompt = prompt[prompt_length_before:]
 
             #  advance to next variable in prompt program (appends intermediate instructions to prompt)
             assert not assert_no_advance, f"error: prompt interpreter tried to advance query program even though assert_no_advance was set"
 
             state = state.updated(variable=variable, prompt=prompt, program_state=program_state)
+            
             while state.variable is None and state.query_head.result is None:
                 state = await self.advance(state)
             reached_end = state.query_head.result is not None
-            
+
+            if reached_end:
+                # make sure to store latest interpreter state in rewritten sequence when query is finished
+                seq.user_data = self.interpreter_state_user_data(state)
+
             prompt = state.prompt
 
             # determines part of advanced_head.prompt that was appended by variable or program
             appended_program_prompt = prompt[prompt_length_before + len(appended_value_prompt):]
 
             variable_offset = state.variable_offset
 
             if old_prompt != prompt:
                 n_tokens_to_strip = len(seq.input_ids) - variable_offset
                 value_ids, program_ids = await asyncio.gather(*[self.tokenize(appended_value_prompt), self.tokenize(appended_program_prompt)])
+
+                assert len(seq.input_ids) - n_tokens_to_strip == variable_offset, f"error: variable offset is not correct. expected {len(seq.input_ids) - n_tokens_to_strip} but got {state.variable_offset}"
                 
                 # if query is finished, add eos token to appended IDs (indicates to decoder that this sequence/query has finished decoding)
                 if reached_end:
                     program_ids += [self.tokenizer.eos_token_id]
                 
                 # value_offset indicates to the decoder, that the first `value_offset` appended tokens are still the value 
                 # of the variable, not deterministic tokens introduced by the prompt program
@@ -642,55 +765,66 @@
                             j += 1
                         r = self.tokenizer.decode_bytes(combined_new_ids[i:j])
                         res += r
                         i = j
                 combined_new_ids = np.array(res, dtype=np.bytes_)
 
                 variable_offset = len(combined_new_ids)
-                rewritten_state = state.updated(variable_offset=variable_offset, variable="__done__" if state.variable is None else state.variable + ":before")
-                # state = state.updated(variable_offset=variable_offset)
+
+                res = []
+                i = 0
+                while i < len(combined_new_ids):
+                    if type(combined_new_ids[i]) is bytes or type(combined_new_ids[i]) is np.bytes_:
+                        res += [combined_new_ids[i]]
+                        i += 1
+                    else:
+                        j = i+1
+                        while j < len(combined_new_ids) and type(combined_new_ids[j]) is not bytes:
+                            j += 1
+                        r = self.tokenizer.decode_bytes(combined_new_ids[i:j])
+                        res += r
+                        i = j
+                combined_new_ids = np.array(res, dtype=np.bytes_)
+                
+                rewritten_state = state.updated(prompt=prompt, variable_offset=variable_offset, variable="__done__" if state.variable is None else state.variable + ":before")
 
                 # appended input ids are now a full replacement for input ids
                 return RewrittenInputIds(
                     appended_input_ids=combined_new_ids, 
                     strip_eos=-n_tokens_to_strip,
                     value_offset=value_offset,
                     user_data=self.interpreter_state_user_data(state),
-                    rewritten_seq_user_data=self.interpreter_state_user_data(rewritten_state)
+                    rewritten_seq_user_data={
+                        "backlink": seq.id,
+                        **self.interpreter_state_user_data(rewritten_state)
+                    }
                 )
             else:
                 # do nothing rewrite
                 variable_offset = len(seq.input_ids) - 1
                 state = state.updated(variable_offset=variable_offset, variable="__done__" if state.variable is None else state.variable)
                 return RewrittenInputIds(
                     appended_input_ids=None, 
                     strip_eos=not reached_end, 
                     user_data=self.interpreter_state_user_data(state)
                 )
-        user_data = (seq.data() or {}).copy()
-        user_data["head"] = state
+        user_data[self.user_data_key] = state
         return RewrittenInputIds(appended_input_ids=None, strip_eos=False, user_data=user_data)
 
     async def tokenize(self, *args):
         # tokenize should be specific to the current model in use (infer from currently process
         # dc.seq, interpreter should not be tokenizer-specific)
         async def task():
             return self.tokenizer(*args)["input_ids"]
         t = asyncio.create_task(task())
         return (await t)
     
     async def rewrite_processor(self, seqs, mask_seq_to_rewrite):
         results = await asyncio.gather(*[self.rewrite_for_sequence(s, needs_rewrite) for s,needs_rewrite in zip(seqs, mask_seq_to_rewrite)])
-        return RewrittenInputIds(
-            appended_input_ids=[r.appended_input_ids if r is not None else None for r in results],
-            strip_eos=[r.strip_eos if r is not None else None for r in results],
-            user_data=[r.user_data if r is not None else None for r in results],
-            value_offset=[r.value_offset if r is not None else None for r in results],
-            rewritten_seq_user_data=[r.rewritten_seq_user_data if r is not None else None for r in results]
-        )
+        return RewrittenInputIds.stack(results)
     
     async def input(self, *args):
         """Uses the output_writer input() implementation if available."""
         if hasattr(self.output_writer, "input"):
             return await self.output_writer.input(*args)
         else:
             return input(*args)
@@ -699,22 +833,24 @@
         self.fct = fct
 
         # intercept symbol table entry for input
         if "input" in kwargs.keys() and kwargs["input"] == input:
             kwargs["input"] = self.input
 
         # prepare initial program state
-        context = LMQLContext(self, None)
+        context = LMQLContext(self, None, "")
         query_head = InterpretationHead(fct, context, args, kwargs)
-        self.root_state = PromptState(variable=None, prompt="", stmt_buffer=[],
+        self.root_state = PromptState(interpreter=self, subinterpreters={},
+            variable=None, prompt="", stmt_buffer=[],
             query_head=query_head, program_state=context.program_state,
             constraints=None,
             recurring_variable_counter={}, variable_offset=0,
             valid=None, final=None, mask=None, 
-            stopping_phrases=None, where=None)
+            stopping_phrases=None, where=None,
+            tail=None)
         self.root_state = await self.advance(self.root_state)
 
         # prepare dcmodel
         decoder_args = self.decoder_kwargs
         self.model.decoder_args = decoder_args
         self.dcmodel: dc.DcModel = self.model.get_dclib_model()
 
@@ -762,14 +898,15 @@
         elif self.output_writer is not None:
             set_dclib_debug_printer(self.output_writer)
 
         if _DCLibDebugPrinter.printer is not None:
             if hasattr(_DCLibDebugPrinter.printer, "records_graph"):
                 if _DCLibDebugPrinter.printer.records_graph:
                     dc.set_record_graph()
+                    self.decoder_graph = dc.DecoderSequence.graph
 
         # get decoder function
         mode = decoder_args["decoder"].lower()
         # handle dynamically-set decoding (e.g. set via @lmql.query(decoder="beam", n=2))
         if mode == "__dynamic__":
             mode, extra_decoder_args = self.derive_decoder_args(self.extra_kwargs)
             decoder_args = {**decoder_args, **extra_decoder_args}
@@ -809,14 +946,16 @@
 
         assert len(prompt_ids) < decoder_args["max_len"], "The initial prompt already exceeds the provided max_len. Please increase the max_len or reduce the initial prompt (Initial prompt: '{}', max_len: {})".format(len(prompt_ids), decoder_args["max_len"])
 
         # set step budget at least to max_len
         step_budget = decoder_args.get("step_budget", max(1024, decoder_args.get("max_len", 1024)))
         
         async def debug_out(decoder_step):
+            if PromptInterpreter.main != self:
+                return
             if _DCLibDebugPrinter.printer is not None and dc.DecoderSequence.graph is not None:
                 data = await dc.DecoderSequence.graph.json(diff=True)
                 data = replace_inf_nan_with_str(data)
                 _DCLibDebugPrinter.printer.add_decoder_state(data)
             self.dcmodel.report_stats(_DCLibDebugPrinter.printer, decoder_step)
 
         try:
@@ -871,15 +1010,15 @@
                 state = self.interpreter_state_from_user_data(s)
                 if state.query_head.result is not None:
                     results.append(state.query_head.result)
                 else:
                     state = await self.advance(state)
                     assert len(s.input_ids) < decoder_args["max_len"], "The decoder returned a sequence that exceeds the provided max_len (max_len={}, sequence length={}). To increase the max_len, please provide a corresponding max_len argument to the decoder function.".format(decoder_args["max_len"], len(s.input_ids))
 
-                    assert state.query_head.result is not None, "decoder designates sequence {} as finished but the underyling query program has not produced a result. This is likekly a decoder bug. Decoder in use {}".format(await s.str(), decoder_args["decoder"])
+                    assert state.query_head.result is not None, "decoder designates sequence {} as finished but the underyling query program has not produced a result. This is likekly a decoder bug. Decoder in use {}".format(await s.text(), decoder_args["decoder"])
                     results.append(state.query_head.result)
             
             # set decoder step +1, for all stats logging that happens in postprocessing
             self.decoder_step += 1
 
             return results
 
@@ -912,8 +1051,162 @@
         decoder_arg_names = inspect.getfullargspec(decoder_fct).args
         decoder_kwarg_names = inspect.getfullargspec(decoder_fct).kwonlyargs
         for k in decoder_args.keys():
             if k not in decoder_arg_names and k not in decoder_kwarg_names and k not in INTERNAL_ARGS:
                 raise ValueError("Unknown decoder argument: {}".format(k))
 
     def print_stats(self):
-        self.dcmodel.report_stats(self.output_writer, self.decoder_step)
+        self.dcmodel.report_stats(self.output_writer, self.decoder_step)
+
+    def subinterpreter(self, identifier, prompt, fct, captures):
+        key = (identifier, prompt)
+
+        if key in self.subinterpreters.keys():
+            return self.subinterpreters[key]
+        else:
+            subinterpreter = SubInterpreter(fct, self, captures, model=self.model, model_identifier=self.model_identifier)
+            
+            # inherits interpreter attributes from parent
+            subinterpreter.tokenizer = self.tokenizer
+            subinterpreter.dcmodel = self.dcmodel
+            
+            self.subinterpreters[key] = subinterpreter
+            
+            return subinterpreter
+        
+    async def subinterpreter_results(self, s: dc.DecoderSequence, variable, text, diff_text, calling_state, is_before, **kwargs):
+        where = calling_state.full_where_condition(self)
+        inline_calls: List[ops.InlineCallOp] = [ic for ic in ops.InlineCallOp.collect(where) if ic.variable.name == variable]
+        
+        subfollow = {}
+        subvalid = {}
+        subinterpreters = []
+
+        for ic in inline_calls:
+            si = ic.subinterpreter(self, calling_state.prompt)
+            if si is None: continue
+            
+            subinterpreters.append(si)
+            
+            # prepare subinterpreter if this is the first time it is used
+            if si.root_state is None:
+                await si.prepare(calling_state.variable_offset, calling_state.prompt)
+
+            state = si.interpreter_state_from_user_data(s)
+            # ids so far in subtinterpreter sequence space
+            subinterpreter_prompt = calling_state.prompt + text
+            # check if we need to first add the initial_subprompt_ids
+            if len(si.root_state.prompt) > len(subinterpreter_prompt):
+                remaining_suffix = si.root_state.prompt[len(subinterpreter_prompt):]
+                # mask deterministically to produce si.root_state.prompt
+                mask = ops.tset(remaining_suffix, prefix=True) # gives us first token of si.root_state.prompt + tail with remaining tokens
+
+                s.user_data = dc.deepmerge(s.user_data, si.interpreter_state_user_data(state))
+                s.user_data["set_by"] = "sub-where"
+
+                subvalid[si] = state.valid
+                subfollow[si] = ops.fmap(
+                    (mask, ops.PredeterminedFinal(True, "var")),
+                    ("*", ops.PredeterminedFinal(False, "fin"))
+                )
+            else:
+                if len(si.root_state.prompt) == len(subinterpreter_prompt):
+                    # set actual variable offset and store state back into current sequence
+                    updated_offset_state = state.updated(variable_offset=len(s.input_ids))
+                    s.user_data = dc.deepmerge(s.user_data, si.interpreter_state_user_data(updated_offset_state))
+
+                follow_map, updated_user_data = await si.where_for_sequence(s, True, 0, return_follow_map=True, **kwargs)
+                
+                if updated_user_data is not None:
+                    s.user_data = dc.deepmerge(s.user_data, updated_user_data)
+                    s.user_data["set_by"] = "sub-where"
+                
+                valid = si.interpreter_state_from_user_data(s).valid
+                
+                subvalid[si] = valid
+
+                # nothing to process if follow_map is None
+                if follow_map is None:
+                    subfollow[si] = None
+                    continue
+
+                # make sure final information is also propagated to the parent interpreter
+                fixed_final_value_components = []
+                for m, c in follow_map.components:
+                    v, f = c
+                    if type(f) is tuple:
+                        f = f[0]
+                    fixed_final_value_components.append((m, ops.PredeterminedFinal(v, f)))
+
+                subfollow[si] = ops.fmap(*fixed_final_value_components)
+
+        calling_state = calling_state.updated(subinterpreters=subinterpreters)
+        
+        return subvalid, subfollow, calling_state
+
+class UserDataLayer:
+    def __init__(self, sqs: List[dc.DecoderSequence], mappings):
+        self.sqs: dc.DecoderSequence = sqs
+        self.mappings = mappings
+        self.prev_mappings = {}
+    
+    # enter and exit
+    def __enter__(self):
+        # for s in self.sqs:
+        #     self.prev_mappings[s.id] = s.user_data
+        #     s.user_data = self.mappings.get(s.id)
+        pass
+
+    def __exit__(self, type, value, traceback):
+        # for s in self.sqs:
+        #     self.mappings[s.id] = s.user_data
+        #     s.user_data = self.prev_mappings.get(s.id)
+        pass
+
+PromptInterpreter.main = None
+
+class SubInterpreter(PromptInterpreter):
+    def __init__(self, fct, parent_interpreter: PromptInterpreter, captures: Dict[str, Any], model: str = None, model_identifier: str = None):
+        super().__init__(context=parent_interpreter)
+        self.query_fct = fct
+        self.fct = fct.fct
+        self.captures = captures
+
+        # maps seq_id to this subinterpreters user_data layer
+        self.user_data_mappings = {}
+
+        self.user_data_key = "head[sub-" + str(id(self)) + "]"
+
+        self.initial_subprompt_ids = None
+        
+        self.model = model
+        self.model_identifier = model_identifier
+
+    def set_model(self, model):
+        # ignore set_model for subinterpreters
+        pass
+
+    def user_data_layer(self, *sqs):
+        return UserDataLayer(sqs, self.user_data_mappings)
+
+    async def prepare(self, parent_offset: int, prompt: str):
+        # prepare initial program state
+        context = LMQLContext(self, None, "")
+
+        query_head = InterpretationHead(self.fct, context, args=[], kwargs=self.captures)
+        self.root_state = PromptState(interpreter=self, subinterpreters=set(),
+            variable=None, prompt=prompt, stmt_buffer=[],
+            query_head=query_head, program_state=context.program_state,
+            constraints=None,
+            recurring_variable_counter={}, variable_offset=parent_offset,
+            valid=None, final=None, mask=None, 
+            stopping_phrases=None, where=None,
+            tail=None)
+        self.root_state = await self.advance(self.root_state)
+
+        self.initial_subprompt_ids = await self.tokenize(self.root_state.prompt)
+        self.n = len(self.initial_subprompt_ids)
+
+        self.root_state = self.root_state.updated(variable_offset=self.n)
+
+    def run(self, prompt, **kwargs):
+        raise NotImplementedError("A SubInterpreter cannot be run directly. Please use the parent interpreter instead.")
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/langchain.py` & `lmql-0.7b1/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/lmql_runtime.py` & `lmql-0.7b1/src/lmql/runtime/lmql_runtime.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,53 +39,59 @@
     def resolve(self, name, errors=None):
         if name in __builtins__.keys():
             return __builtins__[name]
         else:
             if errors == "ignore":
                 return None
             else:
-                raise TypeError("Failed to resolve value of variable '" + name + "' in LMQL query")
+                raise TypeError("Failed to resolve value of variable '" + name + "' in @lmql.query function.")
 
 @dataclass
 class FunctionContext:
     argnames: inspect.Signature
     args_of_query: List[str]
     scope: LMQLInputVariableScope
 
 
 class LMQLQueryFunction:
     fct: Any
     output_variables: List[str]
     postprocessors: List[Any]
     scope: Any
 
+    name: str = None
+
     output_writer: Optional[Any] = None
     args: Optional[List[str]] = None
     model: Optional[Any] = None
     function_context: Optional[FunctionContext] = None
     
     # extra arguments to consider as query context (e.g. passed to the @lmql.query(<args>) decorator)
     extra_args: Dict = None
 
     lmql_code: str = None
 
+    __lmql_query_function__ = True
     is_async: bool = True
     
     def __init__(self, fct, output_variables, postprocessors, scope, *args, **kwargs):
         self.fct = fct
         self.output_variables = output_variables
         self.postprocessors = postprocessors
         self.scope = scope
         
         self.output_writer = None
         self.args = [a for a in inspect.getfullargspec(fct).args if a != "context"]
         self.model = None
         # only set if the query is defined inline of a Python file
         self.function_context = None
 
+    def __hash__(self):
+        return hash(self.fct)
+
     @property
     def input_keys(self) -> List[str]:
         return self.args
     
     def __getattribute__(self, __name: str) -> Any:
         return super().__getattribute__(__name)
 
@@ -133,15 +139,15 @@
         # initialize with default values
         for name, param in signature.parameters.items():
             if param.default is not inspect.Parameter.empty and name in args_of_query:
                 compiled_query_args[name] = param.default
 
         # bind args and kwargs to signature
         try:
-            signature = signature.bind(*args, **query_kwargs)
+            signature: inspect.BoundArguments = signature.bind(*args, **query_kwargs)
         except TypeError as e:
             if "too many positional arguments" in str(e):
                 # this is different from Python behavior, but we allow it for lmql.F and lmql.run
                 pos_as_kw = self.try_bind_positional_to_kwargs(signature, *args, **kwargs)
                 if pos_as_kw is not None:
                     signature = pos_as_kw
                 else:
@@ -149,14 +155,16 @@
             else:    
                 if len(e.args) == 1 and e.args[0].startswith("missing "):
                     e.args = (f"Call to @lmql.query function is " + e.args[0] + "." + f" Expecting {signature}, but got positional args {args} and {kwargs}.",)
                 elif len(e.args) == 1:
                     e.args = (e.args[0] + "." + f" Expecting {signature}, but got positional args {args} and {kwargs}.",)
                 raise e
         
+        signature.apply_defaults()
+
         # special case, if signature is empty (no input variables provided)
         if len(signature.arguments) == 0:
             # bind kwargs dynamically in compiled_query_args
             for k,v in kwargs.items():
                 if k in args_of_query:
                     # compiled_query_args[k] = v
                     compiled_query_args[k] = v
@@ -168,23 +176,23 @@
         for name, value in signature.arguments.items():
             if name in args_of_query:
                 compiled_query_args[name] = value
                 captured_variables.remove(name)
 
         failed_to_resolve = []
 
-
         # resolve remaining unset args from scope
         for v in captured_variables:
             if not v in compiled_query_args:
                 try:
                     compiled_query_args[v] = scope.resolve(v, errors="raise")
                 except TypeError:
                     failed_to_resolve.append(v)
 
+        # disable this check for now, as dynamic variable resolution cannot always be checked at compile time (e.g. import * from module)
         if len(failed_to_resolve) == 1:
             raise TypeError("Failed to resolve variable '" + failed_to_resolve[0] + "' in LMQL query.")
         elif len(failed_to_resolve) > 0:
             raise TypeError("Failed to resolve variables in LMQL query: " + ", ".join(f"'{v}'" for v in sorted(failed_to_resolve)))
 
         return compiled_query_args, runtime_args
 
@@ -205,16 +213,23 @@
         runtime_args  = {**(self.extra_args or {}), **runtime_args}
         interpreter.set_extra_args(**runtime_args)
 
         # rename 'self'
         if "self" in query_kwargs:
             query_kwargs["__self__"] = query_kwargs.pop("self")
 
-        # execute main prompt
-        results = await interpreter.run(self.fct, **query_kwargs)
+        # keep track of the main interpreter (only produces debug output for this one)
+        try:
+            if PromptInterpreter.main is None:
+                PromptInterpreter.main = interpreter
+            # execute main prompt
+            results = await interpreter.run(self.fct, **query_kwargs)
+        finally:
+            if PromptInterpreter.main == interpreter:
+                PromptInterpreter.main = None
 
         # applies distribution postprocessor if required
         results = await (ConditionalDistributionPostprocessor(interpreter).process(results))
 
         # apply remaining postprocessors
         if self.postprocessors is not None:
             for postprocessor in self.postprocessors:
@@ -266,8 +281,20 @@
 
     def func_transformer(fct):
         return LMQLQueryFunction(fct, 
                                  output_variables=output_variables, 
                                  postprocessors=postprocessors, 
                                  scope=LMQLInputVariableScope(fct, calling_frame))
     return func_transformer
-    
+    
+
+async def call(fct, *args, **kwargs):
+    if type(fct) is LMQLQueryFunction or (hasattr(fct, "__lmql_query_function__") and fct.__lmql_query_function__.is_async):
+        result = await fct(*args, **kwargs)
+        if len(result) == 1: 
+            return result[0]
+        else: 
+            return result
+    if inspect.iscoroutinefunction(fct):
+        return await fct(*args, **kwargs)
+    else:
+        return fct(*args, **kwargs)
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/loop.py` & `lmql-0.7b1/src/lmql/runtime/loop.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/maiohttp.py` & `lmql-0.7b1/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/masks.py` & `lmql-0.7b1/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/model_registry.py` & `lmql-0.7b1/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.7b1/src/lmql/runtime/multi_head_interpretation.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,8 +144,8 @@
         self.fresh_copy = False
         return self._iterator_fct
     
     def __repr__(self):
         return str(self)
     
     def __str__(self):
-        return f"<InterpretationHead {self.fct.__name__}, {self.args}, {self.kwargs}>"
+        return f"<InterpretationHead {self.fct.__name__}, {self.args}, {self.kwargs}, result={self.result}>"
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/openai_integration.py` & `lmql-0.7b1/src/lmql/runtime/openai_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,26 +148,26 @@
 
             # check for <eos> case
             if masks.mask_is_allowed(mask, self.eos_token_id):
                 return CompletionCall("fixed", token, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
             else:
                 # otherwise we can treat this as a score call
                 return CompletionCall("fixed", token, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
-        elif num_allowed < self.tokenizer.vocab_size:
-            if self.tokenizer.vocab_size - num_allowed > num_allowed:
+        elif num_allowed < self.tokenizer.model_vocab_size:
+            if self.tokenizer.model_vocab_size - num_allowed > num_allowed:
                 # if we have to mask more than half of the tokens, we should just invert the masking
                 invert = True
         else: # num_allowed == mask.shape[-1] (full vocabulary)
             return CompletionCall("*", None, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
 
         # num_allowed < mask.shape[-1] and num_allowed > 1 (needs mask)
         return CompletionCall("complete", mask, s.input_ids, kwargs, invert=invert, stopping_phrases=stopping_phrases)
 
     async def api_score(self, input_ids, offset):
-        if input_ids[0] == self.tokenizer.bos_token_id:
+        if len(input_ids) > 0 and input_ids[0] == self.tokenizer.bos_token_id:
             input_ids = input_ids[1:]
 
         prompt_str = self.tokenizer.convert_bytes_to_string(input_ids)
 
         # rstripped_eos = False
         # if prompt_str.endswith("<|endoftext|>"):
         #     rstripped_eos = True
@@ -229,19 +229,19 @@
         if user_data is None:
             user_data = {}
         user_data["openai-continuations"] = None
         
         def make_detseq(s, token_score, completion):
             # compose deterministic flags
             if type(deterministic) is bool:
-                deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
+                deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])], dtype=np.bool_)
                 next_deterministic = np.array([deterministic] * len(completion[1:]))
             else:
                 assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored, but is {} and {}".format(deterministic, completion)
-                deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])])
+                deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])], dtype=np.bool_)
                 next_deterministic = np.array(deterministic[1:])
 
             return detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
                     next_ids=completion[1:],
                     logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
                     next_logprobs=token_score[1:],
                     deterministic=deterministic_flags,
@@ -271,15 +271,15 @@
 
         batch_size = 1
         input_ids = completion_call.input_ids.reshape(-1)
         prompt_str = self.tokenizer.convert_bytes_to_string(input_ids)
         tokenized_input_ids = await self.tokenize(prompt_str)
 
         # do not include bos token in prompt for request
-        if input_ids[0] == self.tokenizer.bos_token_id:
+        if len(input_ids) > 0 and input_ids[0] == self.tokenizer.bos_token_id:
             input_ids = input_ids[1:]
 
         temperature = completion_call.kwargs.get("temperature", 0.0)
         logprobs = completion_call.kwargs.get("logprobs", 5)
         noscore = completion_call.kwargs.get("noscore", False)
 
         kwargs = {
@@ -471,14 +471,16 @@
                         user_data = {
                             "openai-continuations": {
                                 continuation.continuation_type: continuation
                             }
                         }
                         # print("token stream gives", result_id, tokens, scores, edge_type, flush=True)
 
+                        scores = [0.0 if str(s) == "[]" else s for s in scores]
+
                         yield (s, tokens, scores, edge_type, user_data)
                     except IndexError:
                         break
                 # print("fully expanded speculativate continuation:", [await self.detokenize(tokens)], flush=True)
                 # if len(tokens) > 1:
                 #     await self.cache(s, tokens, scores, edge_type)
             except Exception as e:
@@ -505,14 +507,15 @@
                 data["_step"] = decoder_step
             printer.report_model_stats(**data)
 
     async def sample(self, sequences, num_samples=1, **kwargs):
         """
         Returns a pool with `n` sampled successor nodes per node in the pool.
         """
+
         kwargs = {**self.model_args, **kwargs}
 
         async def op_sample(seqs):
             completions: List[CompletionResult] = await self.completion_buffer(seqs, logprobs=num_samples, **kwargs)
             
             next_token_ids = []
             next_token_scores = []
@@ -527,22 +530,23 @@
                 continuation = CompletionResult(completion.buffer[1:], completion.continuation_type, completion.logit_mask_or_fixed_id)
                 continuation_buffers.append(continuation)
 
                 # detect fixed results (i.e. deterministic tokens)
                 if "fixed" in complete_data.keys():
                     next_token = [complete_data["logprobs"]["tokens"]]
                     next_token_score = complete_data["logprobs"]["token_logprobs"]
+                    if str(next_token_score) == "[]": next_token_score = np.array([0.0])
                     next_token_ids.append(np.array([next_token]))
                     next_token_scores.append(np.array([next_token_score], dtype=np.float32))
-                    
+
                     full_logits = TokenDistribution()
                     full_logits[next_token] = next_token_score
-                    # else: 
-                    #  next_token is a special token, which is not in the vocab
+
                     logits.append(full_logits)
+
                     continue
 
                 # get sampled token and score
                 next_token = complete_data["logprobs"]["tokens"]
                 next_token_score = complete_data["logprobs"]["token_logprobs"]
                 
                 probs = sorted(list(complete_data["logprobs"]["top_logprobs"].items()))
@@ -627,15 +631,15 @@
         assert k <= 5, "The OpenAI API only supports topk probabilities with k <= 5"
         assert k >= 1, "topk_continuations() requires k >= 1"
         
         assert not "turbo" in self.model_identifier, f"Chat API models do not support topk_continuations which is required for the requested decoding algorithm, use 'sample' or 'argmax' instead."
 
         kwargs = {**self.model_args, **kwargs}
         kwargs.update({"temperature": 0.0})
-        
+
         async def op_topk(seqs):
             completions: List[CompletionResult] = await self.completion_buffer(seqs, logprobs=k, **kwargs)
             
             next_token_ids = []
             next_token_scores = []
             logits = []
             continuation_buffers: List[CompletionResult] = []
@@ -646,14 +650,15 @@
                 continuation = CompletionResult(completion.buffer[1:], completion.continuation_type, completion.logit_mask_or_fixed_id)
                 continuation_buffers.append(continuation)
 
                 # detect fixed results (i.e. deterministic tokens)
                 if "fixed" in complete_data.keys():
                     next_token = [complete_data["logprobs"]["tokens"]]
                     next_token_score = complete_data["logprobs"]["token_logprobs"]
+                    if str(next_token_score) == "[]": next_token_score = np.array([0.0])
                     next_token_ids.append(np.array([next_token]))
                     next_token_scores.append(np.array([next_token_score], dtype=np.float32))
                     
                     distribution = TokenDistribution()
                     distribution[next_token] = next_token_score
                     logits.append(distribution)
                     continue
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/openai_secret.py` & `lmql-0.7b1/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/output_writer.py` & `lmql-0.7b1/src/lmql/runtime/output_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 Currently active token mask.
             num_tokens (int): 
                 Number of tokens in the current 'prompt'.
             program_variables (ProgramState): 
                 The current program state (lmql.runtime.program_state). E.g. program_variables.variable_values is a mapping of variable names to their current values.
         """
         pass
-    
+
     def add_compiler_output(self, code): 
         pass
 
 class PrintingOutputWriter:
     def __init__(self, clear=False):
         self.clear = clear
         self.print_output = True
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.7b1/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/program_state.py` & `lmql-0.7b1/src/lmql/runtime/program_state.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 class ProgramState:
     """
     Program state tracked by the interpreter during program execution.
     """
-    def __init__(self, runtime=None):
+    def __init__(self, prompt, runtime=None):
         self.variable_values = {}
         # postprocessed, converted variable values if not just str (e.g. objects, int)
         self.variable_program_values = {}
         self.variable_diffs = {}
         self.variable_scores = {}
         self.variable_monotonicity = {}
 
         # python scope of local variables (also user-defined ones)
         self.python_scope = {}
 
         self.runtime = runtime
+        self.subinterpreter_results = {}
+        self.prompt = prompt
 
     async def json(self):
         def json_value(k):
             fin = self.variable_monotonicity.get(k, "var")
             # do not include diff and score for now
             return fin + "(\"" + str(self.variable_values[k]) + "\")"
         return {k: json_value(k) for k in self.variable_values.keys()}
@@ -44,15 +46,15 @@
     def get_diff(self, name, default=None):
         return self.variable_diffs.get(name, default)
 
     def final(self, name):
         return self.variable_monotonicity.get(name, "var")
 
     def copy(self):
-        s = ProgramState()
+        s = ProgramState(self.prompt)
         s.variable_values = self.variable_values.copy()
         s.variable_program_values = self.variable_program_values.copy()
         s.variable_monotonicity = self.variable_monotonicity.copy()
         s.variable_diffs = self.variable_diffs.copy()
         s.variable_scores = self.variable_scores.copy()
         s.runtime = self.runtime
         s.python_scope = self.python_scope
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/stats.py` & `lmql-0.7b1/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/token_distribution.py` & `lmql-0.7b1/src/lmql/runtime/token_distribution.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/tokenizer.py` & `lmql-0.7b1/src/lmql/runtime/tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,62 +9,78 @@
 import numpy as np
 from typing import Optional
 
 from lmql.runtime.caching import cache_file_exists, cachefile
 
 from lmql.runtime.tokenizers.pure_python_tokenizer import PythonBackedTokenizer
 from lmql.runtime.tokenizers.tiktoken_tokenizer import TiktokenTokenizer
-from threading import Thread
 
 global special_token_mappings
 special_token_mappings = {}
 global reverse_special_token_mappings
 reverse_special_token_mappings = {}
 
 class LMQLTokenizer:
     INVALID_CHARACTER = "\uFFFD"
 
     def __init__(self, model_identifier, tokenizer_impl=None, loader=None):
         self._tokenizer_impl = None
         self.loader_thread = None
 
+        self.model_identifier = model_identifier
+
+        self._vocab = None
+        self.vocab_range = None
+
         if loader is not None:
+            from threading import Thread
             def load():
                 t = loader()
                 self._tokenizer_impl = t
                 self.loader_thread = None
+                
+                self._vocab = get_vocab(self.tokenizer_impl)
+                self.vocab_range = max(max(self._vocab.values()) + 1, self.tokenizer_impl.vocab_size)
             self.loader_thread = Thread(target=load)
             self.loader_thread.start()
         else:
             self._tokenizer_impl = tokenizer_impl
-
-        self.model_identifier = model_identifier
-        self.detokenizer_cache = {}
-
-        self._vocab = get_vocab(self.tokenizer_impl)
-        self.vocab_range = max(max(self._vocab.values()) + 1, self.tokenizer_impl.vocab_size)
+            self._vocab = get_vocab(self.tokenizer_impl)
+            self.vocab_range = max(max(self._vocab.values()) + 1, self.tokenizer_impl.vocab_size)
 
         if "FORCE_TIKTOKEN" in os.environ:
             assert type(self.tokenizer_impl) is TiktokenTokenizer
 
     @property
+    def model_vocab_size(self):
+        """
+        The model vocab size is the size of the vocabulary that a model uses
+        as the dimensionality of its output distribution. This is different from
+        the vocab_size of the tokenizer, which is the size of the vocabulary
+        + some reserved LMQL-specific tokens.
+        """
+        return self.vocab_range
+    
+    @property
     def tokenizer_impl(self):
         if self._tokenizer_impl is None:
             self.loader_thread.join()
         return self._tokenizer_impl
     
     @property
     def name(self):
         return self.tokenizer_impl.name
 
     @property
     def vocab_size(self):
-        # in LMQL vocab_size is the vocab_range (the highest vocabulary ID + 1)
-        # this allows us to use a dense one hot array where no IDs are skipped
-        return self.vocab_range
+        """
+        The vocab_size is the vocab_range (the highest vocabulary ID + 1)
+        this allows us to use a dense one hot array where no IDs are skipped.
+        """
+        return self.vocab_range + 100 # 100 reserved tokens for LMQL tags
 
     @property
     def bos_token_id(self) -> Optional[int]:
         return self.tokenizer_impl.bos_token_id
     
     @property
     def eos_token_id(self):
@@ -162,28 +178,37 @@
             input_ids.append(chunk_input_ids)
         
         if unpack:
             return {"input_ids": input_ids[0]}
         else:
             return {"input_ids": input_ids}
     
+    def is_special_id(self, id: str):
+        return id >= self.model_vocab_size
+
+    def truncate_to_model_dim(self, mask):
+        if mask is None:
+            return mask
+        return mask[:self.model_vocab_size]
+
     def special_token_id(self, identifier):
         global special_token_mappings
         global reverse_special_token_mappings
         
         if identifier not in special_token_mappings:
             if len(special_token_mappings) == 0:
-                # offset vocabulary IDs by at least the next decimal power of 10
-                offset = 10 ** (len(str(self.vocab_range)))
+                # offset vocabulary IDs by at least 1 to avoid collisions with the tokenizer's vocabulary
+                offset = self.vocab_range + 1
                 special_token_mappings[identifier] = offset
                 reverse_special_token_mappings[offset] = identifier
             else:
                 next_id = max(special_token_mappings.values()) + 1
                 special_token_mappings[identifier] = next_id
                 reverse_special_token_mappings[next_id] = identifier
+                assert next_id < self.vocab_size, "LMQL special tokens exhausted (only 100 allowed by default)"
         return special_token_mappings[identifier]
     
     def chunk_out_by_special_ids(self, input_ids, tokenize=True):
         global reverse_special_token_mappings
         c = []
         for i in input_ids:
             if i in reverse_special_token_mappings.keys():
```

### Comparing `lmql-0.0.6.6/src/lmql/runtime/tokenizers/hf_tokenizer.py` & `lmql-0.7b1/src/lmql/runtime/tokenizers/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/tokenizers/pure_python_tokenizer.py` & `lmql-0.7b1/src/lmql/runtime/tokenizers/pure_python_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py` & `lmql-0.7b1/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/all.py` & `lmql-0.7b1/src/lmql/tests/all.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 import sys
 import subprocess
+import lmql
 
 THIS_DIR = os.path.dirname(__file__)
 files = sorted(os.listdir(THIS_DIR))
 TEST_TIMEOUT = float(os.environ.get("TEST_TIMEOUT", 3*60.0))
 
 errors = 0 
 files = [f for f in files if f.startswith("test_")]
 
+print(f"Testing LMQL distribution {lmql.__version__} at {lmql.__file__} with {len(files)} tests")
+
 for i,f in enumerate(files):
     try:
         print(">", f"[{i+1}/{len(files)}]", f)
 
         cmd = "python " + os.path.join(THIS_DIR, f)
         timeout = TEST_TIMEOUT
         result = subprocess.call(cmd, shell=True, timeout=timeout)
```

### Comparing `lmql-0.0.6.6/src/lmql/tests/expr_test_utils.py` & `lmql-0.7b1/src/lmql/tests/expr_test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def digest(self, seq, variable_name="SEQ", return_follow_map=False, debug=False):
         sequence = seq
         if type(sequence) is str:
             sequence = sequence.split(" ")
         full_text = ""
 
-        program_variables = ProgramState()
+        program_variables = ProgramState("")
         
         digested = []
         results = []
 
         for tok in sequence:
             added = (" " if len(full_text) > 0 else "") + tok
             full_text += added
```

### Comparing `lmql-0.0.6.6/src/lmql/tests/fin_and.py` & `lmql-0.7b1/src/lmql/tests/fin_and.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.7b1/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.7b1/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.7b1/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.7b1/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.7b1/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/stops_at.py` & `lmql-0.7b1/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.7b1/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.7b1/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.7b1/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/queryargs/test_args.py` & `lmql-0.7b1/src/lmql/tests/queryargs/test_args.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_query_str.py` & `lmql-0.7b1/src/lmql/tests/queryargs/test_args_query_str.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_run.py` & `lmql-0.7b1/src/lmql/tests/queryargs/test_args_run.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/queryargs/test_sync.py` & `lmql-0.7b1/src/lmql/tests/queryargs/test_sync.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/queryargs/test_var_errors.py` & `lmql-0.7b1/src/lmql/tests/queryargs/test_var_errors.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.7b1/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/tail_token_set.py` & `lmql-0.7b1/src/lmql/tests/tail_token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_back2back_caching.py` & `lmql-0.7b1/src/lmql/tests/test_back2back_caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_eq.py` & `lmql-0.7b1/src/lmql/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_escaping.py` & `lmql-0.7b1/src/lmql/tests/test_escaping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_f.py` & `lmql-0.7b1/src/lmql/tests/test_f.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_local_model_python.py` & `lmql-0.7b1/src/lmql/tests/test_local_model_python.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_minimal_syntax.py` & `lmql-0.7b1/src/lmql/tests/test_minimal_syntax.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_multibyte_characters.py` & `lmql-0.7b1/src/lmql/tests/test_multibyte_characters.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_multibyte_local_models.py` & `lmql-0.7b1/src/lmql/tests/test_multibyte_local_models.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_qstrings.py` & `lmql-0.7b1/src/lmql/tests/test_qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_sample_queries.py` & `lmql-0.7b1/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_scoping.py` & `lmql-0.7b1/src/lmql/tests/test_scoping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/test_stopping.py` & `lmql-0.7b1/src/lmql/tests/test_stopping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/tests/tiktoken_tsets.py` & `lmql-0.7b1/src/lmql/tests/tiktoken_tsets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/live/live.js` & `lmql-0.7b1/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/live/live.py` & `lmql-0.7b1/src/lmql/ui/live/live.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/live/livelib.py` & `lmql-0.7b1/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/live/yarn.lock` & `lmql-0.7b1/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/README.md` & `lmql-0.7b1/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/package.json` & `lmql-0.7b1/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.7b1/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/index.html` & `lmql-0.7b1/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.7b1/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/json-template.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/json-template.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.7b1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.7b1/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/App.jsx` & `lmql-0.7b1/src/lmql/ui/playground/src/App.jsx`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,25 @@
     width: 12pt;
     height: 12pt;
     position: relative;
     margin-right: 9pt;
     margin-left: 5pt;
     top: 2pt;
   }
+
+  span.badge {
+    background-color: #383666;
+    font-size: 8pt;
+    padding: 2pt;
+    border-radius: 2pt;
+    color: white;
+    margin-left: 5pt;
+    position: relative;
+    top: -1pt;
+  }
 `;
 
 const Sidebar = styled.div.attrs(props => ({ className: "sidebar" }))`
   width: 35pt;
   border-radius: 5pt;
   border-top-left-radius: 0pt;
   border-bottom-left-radius: 0pt;
@@ -795,15 +806,15 @@
       border-radius: 0;
       font-size: 0.8em;
       /* special case for with-sidebar */
       &.with-sidebar {
         width: calc(100% - 15pt - 27.5pt);
       }
     }
-
+  }
 `
 
 const IconButton = styled.button`
   background-color: transparent;
   border: none;
   outline: none;
   cursor: pointer;
@@ -870,14 +881,15 @@
     <span className="spacer wide"> </span>
     {p.children}
   </ToolbarIconButton>
 }
 
 function OutputPanelContent(props) {
   const [output, setOutput] = useState("Client ready.\n");
+  const [alwaysShow, setAlwaysShow] = useState(false);
 
   const onConsoleOut = data => {
     let newOutput = ""
     if (typeof data === 'string') {
       newOutput = data
     } else {
       newOutput = JSON.stringify(data, null, 2);
@@ -902,45 +914,29 @@
 
   props = Object.assign({}, props)
   props.style = Object.assign({
     fontSize: "8pt",
   }, props.style)
 
   return <>
-    <OutputText style={props.style} readOnly={true} value={output}></OutputText>
+    {props.className == "simple" &&
+    <ToggleButton checked={alwaysShow} onClick={() => setAlwaysShow(s => !s)} style={{ float: "right", color: "white" }}>...</ToggleButton>}
+    <OutputText style={props.style} className={props.className + (alwaysShow ? " always" : "")} readOnly={true} value={output}></OutputText>
   </>
 }
 
 const ModelResultText = styled.div`
   flex: 1; 
   display: flex;
   flex-direction: column;
   line-height: 1.6em;
   white-space: pre-wrap;
   overflow-y: auto;
   font-size: 10pt;
 
-  &.chat-mode {
-    padding-bottom: 50pt;
-  }
-
-  &.chat-mode .system-message {
-    text-align: center;
-    display: block;
-    font-size: 8pt;
-    background-color: transparent !important;
-    color: #adadad;
-    margin-top: 10pt;
-  }
-
-  .system-message {
-    display: none;
-  }
-
-
   &::-webkit-scrollbar {
     width: 0px;
   }
 
   h3 {
     margin: 0;
     padding: 0;
@@ -963,31 +959,49 @@
     padding-bottom: 20pt;
   }
 
   div .prompt {
     opacity: 0.95;
   }
   
+  &.chat-mode {
+    padding-bottom: 50pt;
+  }
+
+  &.chat-mode .system-message {
+    display: block;
+    font-size: 8pt;
+  }
+
+  .system-message {
+    display: none;
+    text-align: center;
+  }
+
   div .tag {
     display: block;
     text-align: center;
     font-size: 8pt;
     color: #5c5c5c;
-    padding: 0;
-    margin: 0;
     display: none;
   }
 
   &.chat-mode .variable.eos {
     display: inline;
-    margin: 0pt;
-    position: relative;
-    left: calc(50% - 15pt);
-    top: 10pt;
     opacity: 0.5;
+    text-align: center;
+  }
+
+  div .tag-system:after {
+    content: "System";
+    position: absolute;
+    right: 5pt;
+    top: 0pt;
+    font-size: 8pt;
+    text-transform: uppercase;
   }
 
   div .tag-system {
     display: block;
     text-align: center;
     background-color: #ffffff13;
     border-radius: 2pt;
@@ -1121,14 +1135,15 @@
 `
 
 const TypingIndicator = styled.span`
   display: inline-block;
   width: 8pt;
   height: 12pt;
   position: relative;
+  border-radius: 2pt;
   top: 3.5pt;
   left: 2pt;
   background-color: #d7d5d5;
   animation: typing 1s infinite;
 
   @keyframes typing {
     0% { opacity: 0.2; }
@@ -1391,15 +1406,15 @@
       // determine base variable name
       let baseVariableName = segment.variable
       if (segment.variable.endsWith("]")) {
         baseVariableName = segment.variable.substr(0, segment.variable.indexOf("["))
       }
 
       if (segment.variable == "__prompt__") {
-        if (segment.content == "\\n" || segment.content.trim() == "") {
+        if (segment.content.trim() == "") {
           continue;
         }
         result.push({
           variableClassName: "prompt tag-" + segment.tag,
           variable: segment.variable,
           content: segment.content
         })
@@ -1550,14 +1565,27 @@
 }
 
 const OutputText = styled.textarea`
   font-size: 9pt;
   font-family: monospace;
   background-color: #222;
   padding: 0;
+
+  &.simple {
+    flex: 0;
+    border-top: 1px solid #444;
+    padding-top: 10pt;
+    display: none !important;
+  }
+
+  &.simple.always {
+    flex: 0.4;
+    height: 40pt;
+    display: flex !important;
+  }
 `
 const CompiledCodeEditorContainer = styled.div`
   flex: 1;
   display: flex;
   flex-direction: column;
 `
 
@@ -1784,15 +1812,15 @@
 
 function InspectorPanelContent(props) {
   let nodeInfo = unpack(props.nodeInfo, "user_data")
   nodeInfo = unpack(nodeInfo, "head")
 
   const valid = ["valid", <ValidText final={resolve(nodeInfo, "final")} valid={resolve(nodeInfo, "valid")} onOpenValidationGraph={props.onOpenValidationGraph}/>]
 
-  const DECODER_KEYS = ["logprob", "seqlogprob", "pool"]
+  const DECODER_KEYS = ["logprob", "seqlogprob", "pool", "prompt"]
   const INTERPRETER_KEYS = ["variable", valid, "mask", "head_index"]
   const PROGRAM_VARIABLES = resolve(nodeInfo, "program_state") ? Object.keys(resolve(nodeInfo, "program_state"))
     .map(key => [key, resolve(nodeInfo, "program_state." + key)]) : []
 
   const KEYS_TO_FILTER = ["user_data", "parent", "layouted", "label", "id", "full_text", "program_state", "program_variables", "valid", "final", "text", "trace", "root", "seqtext", "where"]
 
   const decoderKeys = DECODER_KEYS.filter(key => typeof resolve(nodeInfo, key) !== "undefined")
@@ -2046,24 +2074,28 @@
           {props.simpleMode &&
             <CheckableToolbarIconButton checked={trackMostLikly} onClick={() => setTrackMostLikly(!trackMostLikly)}>
               Show Latest
             </CheckableToolbarIconButton>
           }
         </>}
       </h2>
-      <OutputPanelContent style={{ display: sidepanel === 'output' ? 'block' : 'none' }} clearTrigger={clearTrigger} />
       <CompiledCodePanelContent style={{ display: sidepanel === 'code' ? 'block' : 'none' }} />
       <ModelResultContent style={{ display: sidepanel === 'model' ? 'flex' : 'none' }}
         selectedNodes={props.selectedNodes}
         perVariableColor={perVariableColor}
         mostLikelyNode={props.mostLikelyNode}
         trackMostLikly={trackMostLikly || !props.simpleMode}
         onTrackLatest={() => setTrackMostLikly(true)}
         processStatus={props.processStatus}
       />
+      <OutputPanelContent 
+        className={!props.simpleMode && sidepanel != 'output' ? "simple" : ""} 
+        style={{ display: ((!props.simpleMode) || sidepanel === 'output') ? 'block' : 'none' }} 
+        clearTrigger={clearTrigger} 
+      />
       {/* <StatisticsPanelContent style={{display: sidepanel === 'stats' ? 'flex' : 'none'}}/> */}
 
       <Sidebar>
         {displayState.mode == "embed" && displayState.embedFile && <IconButton onClick={() => window.open(window.location.href.split('?')[0] + "?snippet=" + displayState.embedFile, "_blank")}>
           <BsBoxArrowUpRight size={16} />
         </IconButton>}
         <IconButton onClick={() => setSidepanelTo('model')} className={sidepanel === 'model' ? 'active' : ''}>
@@ -2805,16 +2837,21 @@
 
     return (
       <ContentContainer className={this.state.graphLayout ? 'graph-layout' : ''}>
         {displayState.mode != "embed" && <Toolbar>
           <Title>
             <img src="/lmql.svg" alt="LMQL Logo"/>  
             LMQL Playground
+            {configuration.NEXT_MODE && <span className="badge">PREVIEW</span>}
           </Title>
-          {configuration.DEMO_MODE && <FancyButton className="in-toolbar" onClick={() => ExploreState.setVisibility(true)}><ExploreIc/> Explore LMQL</FancyButton>}
+          {configuration.DEMO_MODE && <FancyButton className="in-toolbar" onClick={() => ExploreState.setVisibility(true)}>
+            <ExploreIc/> 
+            {!configuration.NEXT_MODE && <>Explore LMQL</>}
+            {configuration.NEXT_MODE && <>Explore New Features</>}
+          </FancyButton>}
           {window.location.hostname.includes("lmql.ai") && <a href={"https://docs.lmql.ai/en/latest/quickstart.html"} target="_blank" rel="noreferrer" className="hidden-on-small">
           Install LMQL Locally </a>}
           <Spacer />
           {/* show tooltip with build time */}
           {/* trigger button */}
           {/* <ToggleButton onClick={() => this.setGraphLayout(!this.state.graphLayout)} toggled={this.state.graphLayout}>
             <BsLayoutWtf size={14} />
```

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.7b1/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.7b1/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.7b1/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -186,14 +186,17 @@
 
     cy.elements().depthFirstSearch({
         roots: rootNodes,
         visit: (node, edge, previous, i, depth) => {
             if (node.hasClass("compound")) return;
             if (node.data("_noUserData")) return;
 
+            // console.log("data", node.data())
+            depth = parseInt(node.data("seq_id").substr(2))
+
             if (depth >= mostLikelyDepth) {
                 if (depth > mostLikelyDepth) {
                     mostLikelyMostRecentNode = null
                 }
                 mostLikelyDepth = depth
                 if (mostLikelyMostRecentNode) {
                     if (mostLikelyMostRecentNode.data("seqlogprob") < node.data("seqlogprob")) {
```

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.7b1/src/lmql/ui/playground/src/Explore.jsx`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import React, { useEffect, useState } from "react";
 import styled from "styled-components";
 import {queries} from "./queries";
 import { displayState, persistedState, trackingState } from "./State";
+import {configuration} from "./Configuration"
 
 export const PromptPopup = styled.div`
   position: absolute;
   top: 0;
   left: 0;
   width: 100vw;
   height: 100vh;
   background-color: #000000c2;
   z-index: 999;
   display: flex;
   flex-direction: column;
+  overflow: hidden;
 
   animation: fade-in 0.2s;
 
   @keyframes fade-in {
     0% {
       opacity: 0;
     }
@@ -34,21 +36,23 @@
     z-index: -1;
   }
 `
 
 export const Dialog = styled.div`
   background-color: #ffffff;
   border-radius: 4pt;
+  overflow: hidden;
   padding: 10pt;
   margin: auto;
-  max-width: 500pt;
+  max-width: 1100pt;
   max-height: 500pt;
-  overflow: auto;
   color: black;
 
+  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica;
+
   input {
     border: none;
     background-color: #dfdfdf;
     border-radius: 4pt;
     font-size: 14pt;
     outline: none;
     padding: 5pt;
@@ -76,64 +80,111 @@
     position: relative;
     top: 8pt;
     left: 2pt;
   }
 `
 
 const ExploreDialog = styled(Dialog)`
-  width: 550pt;
-  height: 550pt;
+  width: 800pt;
+  height: 700pt;
   max-height: 100vh;
   max-width: 100vh;
   overflow-y: auto;
+
+  /* invisible scroll bar */
+  ::-webkit-scrollbar {
+    width: 0px;
+    background: transparent;
+  }
+
   position: relative;
-  padding: 20pt;
+  padding: 0pt;
+  
 
   @media (max-width: 550pt) {
     width: calc(100vw - 20pt);
     height: calc(100vh - 20pt);
     max-height: 100vh;
-    max-width: 100vh;
+    max-width: 100vw;
     overflow-y: auto;
     position: relative;
     padding: 10pt;
     padding-bottom: 80pt;
+    padding-left: 0;
+    margin: 0;
+    border-radius: 0;
+
+    div.tile {
+      display: block !important;
+      width: 100% !important;
+      border: 1pt solid transparent;
+
+      &:hover {
+        transform: none !important;
+        border: 1pt solid #ababab;
+      }
+    }
   }
 
   /* very light white to grey grdient */
   background: linear-gradient(180deg, #ffffff 0%, #e4e2e2 100%);
 
   >div {
+    padding: 5pt 20pt;
+    position: relative;
+  }
+
+  >div .sidenote a {
+    padding-left: 2pt;
+  }
+
+  >div .sidenote {
+    position: absolute;
+    top: 15pt;
+    right: 15pt;
+    font-size: 8pt;
+  }
+
+  div.highlight {
+    background-color: #dedef8;
+  }
+
+  >div>div {
     display: flex;
     flex-direction: row;
     flex-wrap: wrap;
   }
 
   p {
     text-align: justify;
   }
 
+  h1 {
+    margin: 0;
+    padding: 20pt;
+  }
+
   h1 img {
     width: 20pt;
     height: 20pt;
     margin-right: 8pt;
     position: relative;
     top: 2pt;
   }
 
   h2 {
     font-size: 12pt;
-    color: #373737;
   }
 
   h3 {
     font-size: 12pt;
     color: #373737;
     margin: 0;
     z-index: 999;
+    font-weight: 500;
   }
 
   .close {
     position: absolute;
     top: 10pt;
     right: 10pt;
     width: 30pt;
@@ -144,47 +195,48 @@
     cursor: pointer;
   }
 `
 
 const Tile = styled.div.attrs({
   className: "tile"
 })`
-  background-color: #1e1e1e;
+  background-color: #f5f5f5;
   border-radius: 4pt;
   padding: 10pt;
   margin: 10pt;
   margin-left: 0pt;
   margin-top: 0pt;
   cursor: pointer;
   transition: 0.1s;
   height: 80pt;
   width: 100pt;
-  border: 2pt solid white;
+  border: 0.5pt solid #ababab;
   opacity: 0.9;
   position: relative;
   display: flex;
   flex-direction: column;
+  
   align-items: flex-start;
-  justify-content: flex-end;
+  justify-content: flex-start;
 
   :hover {
     transform: scale(1.05);
     opacity: 1.0;
   }
 
   h3 {
-    color: #e9e8e8;
+    color: #212121;
   }
 
   code {
     opacity: 0.3;
   }
 
   p {
-    color: white;
+    color: #010101;
     font-size: 10pt;
     font-style: italic;
     z-index: 999;
     text-align: left;
   }
 
   .badge {
@@ -219,15 +271,15 @@
   transform: scale(0.8);
   transform-origin: top left;
   max-height: 50pt;
   position: absolute;
   top: 0;
   left: 0;
   width: 100%;
-  color: white;
+  color: #323232;
 
   .keyword {
     color: #ff79c6;
     font-weight: bold;
   }
 
   code {
@@ -251,15 +303,15 @@
   :after {
     content: "";
     position: absolute;
     bottom: -2px;
     left: 0;
     right: 0;
     height: 20pt;
-    background: linear-gradient(180deg, transparent 0%, #1e1e1e 100%);
+    /* background: linear-gradient(180deg, transparent 0%, #f5f5f561 100%); */
   }
 `
 
 const TypingContainer = styled.span`
   .cursor {
     animation: blink 2s linear infinite;
     transform: scale(2.2);
@@ -285,16 +337,16 @@
     100% {
       opacity: 0;
     }
   }
 `
 
 
-function TypedText() {
-  const text = "Welcome To LMQL";
+function TypedText(props) {
+  const text = props.text;
   const speed = 50;
   let [index, setIndex] = useState(window.textWasTyped ? text.length : 0);
   let [isTyping, setIsTyping] = useState(!window.textWasTyped);
 
   useEffect(() => {
     if (!isTyping) return;
     
@@ -328,27 +380,33 @@
   })
   return <CodeContainer>
     <code>{result}</code>
   </CodeContainer>
 }
 
 const Description = styled.p`
-  font-size: 12pt;
+  font-size: 14pt;
   color: #696969;
+  padding: 0pt 20pt;
 `
 
 const CiteBox = styled.code`
   display: block;
-  background-color: #dfdede;
+  background-color: #dbdbdb;
   padding: 4pt;
   border-radius: 4pt;
 `
 
 let didLoadAnchor = false;
 
+const PreviewQueries = {
+  queries: [],
+  listeners: []
+}
+
 export function Explore() {
     const [visible, setVisible] = useState(ExploreState.visible);
 
     const onClickTile = (q) => {
       ExploreState.setVisibility(false);
       if (q.state) {
         fetch(q.state).then((r) => r.text()).then((r) => {
@@ -358,15 +416,34 @@
         }).catch((e) => {
           console.error(e)
           alert("Error loading example.")
         });
       } else {
         persistedState.setItem("lmql-editor-contents", q.code)
       }
-  }
+    }
+
+    let [exploreQueries, setExploreQueries] = useState(configuration.NEXT_MODE ? PreviewQueries.queries : queries);
+
+    useEffect(() => {
+      if (configuration.NEXT_MODE) {
+        let url = "https://raw.githubusercontent.com/lmql-lang/awesome-lmql/main/next/showcase-playground.js";
+        url += "?nocache=" + Math.random();
+        fetch(url).then((r) => r.text()).then((r) => {
+          // eslint-disable-next-line no-eval
+          let queries = eval(r).queries;
+          PreviewQueries.queries = queries;
+          PreviewQueries.listeners.forEach((l) => l());
+          console.log("Loaded list of Preview release queries.", queries)
+        }).catch((e) => {
+          console.error(e)
+          console.error("Error loading list of Preview release queries.")
+        });
+      }
+    }, [])
 
     useEffect(() => {
         // register listeners
         ExploreState.listeners.push(setVisible);
 
         // check if first visit
         const editorContents = window.localStorage.getItem("lmql-editor-contents");
@@ -386,43 +463,70 @@
         }
 
         return () => {
             ExploreState.listeners = ExploreState.listeners.filter((l) => l !== setVisible);
         }
     }, []);
 
+    useEffect(() => {
+      if (configuration.NEXT_MODE) {
+        const listener = () => {
+          setExploreQueries(PreviewQueries.queries);
+        }
+        PreviewQueries.listeners.push(listener);
+        return () => {
+          PreviewQueries.listeners = PreviewQueries.listeners.filter((l) => l !== listener);
+        }
+      }
+    }, [])
+
+
     if (!visible) return null;
 
+    let description = <>
+    This playground allows you to explore LMQL's capabilities. To get started, choose one of the example queries below.
+    </>
+
+    if (configuration.NEXT_MODE) {
+      description = <>This is the preview channel of LMQL. It contains the latest features, but may be unstable. If you are looking for the stable version, please visit <a href="https://lmql.ai/playground">the stable Playground IDE</a>.</>
+    }
+
     return <PromptPopup>
         <div className="click-handler" onClick={() => ExploreState.setVisibility(false)}/>
         <ExploreDialog>
           <h1 key="welcome">
             <img src="/lmql.svg" alt="LMQL Logo"/>  
             <TypedText text="Welcome To LMQL" speed={20}/>
           </h1>
-          <Description>
-            LMQL is a query language for large language models. This playground allows you to explore LMQL's capabilities. To get started, choose one of the example queries below, demonstrating <i>constrained model use</i>, <i>control-flow guided generation</i>, and tool-augmented LLMs.
-          </Description>
+          <Description>{description}</Description>
           <span className="close" onClick={() => ExploreState.setVisibility(false)}>
             &times;
           </span>
-          {queries.map(c => 
-            <>
+          {exploreQueries.map(c => 
+            <div className={c.highlight ? "highlight" : ""} key={c.category + "-container"}>
             <h2 key={c.category}>{c.category}</h2>
+            {c.highlight && <span class="sidenote">
+              <a href="https://github.com/eth-sri/lmql/issues" target="_blank" rel="noreferrer"> Report Issues</a>
+            </span>}
             <div key={c.category + "-div"}>
             {c.queries.map((q,i) => <Tile key={c.category + "-" + i} onClick={() => onClickTile(q)}>
               {/* {q.state && <div className="badge">PRECOMPUTED</div>} */}
               <BasicHighlighted code={q.code}/>
               <h3>{q.name}</h3>
               <p>{q.description}</p>
             </Tile>)}
             </div>
-            </>
+            </div>
           )}
+          {!configuration.NEXT_MODE && <>
+          <div>
           <h2 key="read-paper">Read the Paper</h2>
           <CiteBox key="cite">
           Beurer-Kellner, Luca, Marc Fischer, and Martin Vechev. "Prompting Is Programming: A Query Language For Large Language Models." 
           <a target="_blank" rel="noreferrer" href="https://arxiv.org/pdf/2212.06094">arXiv preprint arXiv:2212.06094</a> (2022).
           </CiteBox>
+          <br/>
+          </div>
+          </>}
         </ExploreDialog>
     </PromptPopup>
 }
```

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.7b1/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/State.js` & `lmql-0.7b1/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.7b1/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.7b1/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/build_info.js` & `lmql-0.7b1/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.7b1/src/lmql/ui/chat/assets/lmql-monaco.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 // Adapted from https://raw.githubusercontent.com/microsoft/monaco-editor/main/src/basic-languages/python/python.ts.
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Microsoft Corporation. All rights reserved.
  *  Licensed under the MIT License. See License.txt in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
-export function registerLmqlLanguage(monaco) {
+function registerLmqlLanguage(monaco) {
     const conf = {
         comments: {
             lineComment: '#',
             blockComment: ["'''", "'''"]
         },
         brackets: [
             ['{', '}'],
```

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.7b1/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/explore.svg` & `lmql-0.7b1/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.7b1/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/index.css` & `lmql-0.7b1/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/logo.svg` & `lmql-0.7b1/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/queries.js` & `lmql-0.7b1/src/lmql/ui/playground/src/queries.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -43,16 +43,16 @@
         "- [THING] \\n"
 from
     'openai/text-ada-001'
 where
     THING in set(["Volleyball", "Sunscreen", "Bathing Suite"])`,
                 state: 'precomputed/list.json'
             }, {
-                name: "📝 Generate JSON",
-                description: "Template-Based Generation",
+                name: "📝 Templates",
+                description: "Template-Based Generation for JSON data",
                 code: `argmax 
     """
     Write a summary of Bruno Mars, the singer:
     {{
       "name": "[STRING_VALUE]",
       "age": [INT_VALUE],
       "top_songs": [[
@@ -66,14 +66,140 @@
 where
     STOPS_BEFORE(STRING_VALUE, '"') and INT(INT_VALUE) and len(TOKENS(INT_VALUE)) < 2
          
          `,
                 state: 'precomputed/json-template.json'
             }]
         }, {
+            category: "Features In Preview",
+            highlight: true,
+            queries: [{
+                // hello world
+                name: "👨‍👩‍👧 Types / JSON",
+                description: "Generate schema-safe, typed data.",
+                code: `import lmql
+from dataclasses import dataclass
+
+@dataclass
+class Employer:
+    employer_name: str
+    location: str
+
+@dataclass
+class Person:
+    name: str
+    age: int
+    employer: Employer
+    job: str
+
+argmax
+    "Alice is a 21 years old and works as an engineer at LMQL Inc in Zurich, Switzerland.\\n"
+    "Structured: [PERSON_DATA]\\n"
+    "Their name is {PERSON_DATA.name} and she works in {PERSON_DATA.employer.location}."
+from 
+    "openai/text-davinci-003" 
+where 
+    type(PERSON_DATA) is Person
+          
+`,
+                state: 'precomputed/json-robust.json'
+            }, {
+                name: "🛠️ Multi-Tool Use",
+                description: "Simply expose Python functions as LLM tools.",
+                code: `from lmql.lib.actions import inline_use, calc, wiki
+
+argmax
+    "Q: What is the population of the US and Germany combined?\\n"
+    "A: Let's think step by step\\n"
+    "[REASONING]\\n"
+    "Therefore the answer is[ANSWER]"
+from 
+    'openai/text-davinci-003'
+where
+    inline_use(REASONING, [wiki, calc]) and INT(ANSWER)
+          `,
+                state: ''
+            }, {
+                name: "🔤 Regex Constraints",
+                description: "Specify constraints using regex.",
+                code: `"It's the last day of June so today is [RESPONSE]" where REGEX(RESPONSE, r"[0-9]{2}/[0-9]{2}")`,
+                state: 'precomputed/date-regex.json'
+            }, {
+                // hello world
+                name: "❤️ Sentiment Constraints",
+                description: "Affect sentiment with in-context prompting.",
+                code: `@lmql.query(cache="mood.tokens", model="chatgpt")
+async def mood_description(m: str):
+    '''lmql
+    print("Generating mood for", m)
+    """Provide a one sentence instruction that prompts a model to write text that 
+    is written in a {m} tone, addressing some previously provided question.\\n"""
+    "[SUMMARY]\\n"
+    return SUMMARY.strip();
+    '''
+
+@lmql.query
+async def mood(m: str):
+    '''lmql
+    """
+    Instruction: {await mood_description(m)}
+    Answer: [RESPONSE]
+    """ where stops_at(RESPONSE, ".") and stops_at(RESPONSE, "\\n")
+
+    return RESPONSE.strip(); 
+    '''
+
+# main query
+argmax
+    for q in ["Hi", "Who are you", "How is your day going?"]:
+        "Q: {q}\\n"
+        "A: [RESPONSE]\\n"
+from 
+    "chatgpt" 
+where 
+    mood(RESPONSE, "loving like a partner")
+          
+`,
+                state: ''
+            }, {
+                // hello world
+                name: "📝 Write A Poem",
+                description: "Insert dynamic instructions with incontext.",
+                code: `@lmql.query
+async def rhyme():
+    '''
+    """
+    Above is the beginning of the poem. Generate the next verse that rhymes with the last line and has the same number of syllables.
+    [VERSE]
+    """ where stops_before(VERSE, "\\n")
+    return VERSE
+    '''
+
+@lmql.query
+async def first_verse():
+    '''
+    """
+    Generate a verse that would be perfect for the start of a beautiful rhyme. 
+    [VERSE]
+    """ where stops_before(VERSE, "\\n")
+    return VERSE
+    '''
+
+argmax
+    "[FIRST_VERSE]\\n"
+    for i in range(5):
+        "[VERSE]\\n"
+from 
+    "chatgpt" 
+where 
+    rhyme(VERSE) and first_verse(FIRST_VERSE)
+`,
+                state: ''
+            }]
+        }, {
             category: "LLM Reasoning",
             queries: [{
                 name: "🧠 Chain-Of-Thought",
                 description: "CoT with robust result extraction.",
                 code: `# zero-shot cot based on https://arxiv.org/pdf/2205.11916.pdf
 argmax
     """Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?
```

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.7b1/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.7b1/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.7b1/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.7b1/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/playground/yarn.lock` & `lmql-0.7b1/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.7b1/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/LICENSE` & `lmql-0.7b1/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.7b1/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.7b1/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/package.json` & `lmql-0.7b1/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.7b1/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/utils/docstring_parser.py` & `lmql-0.7b1/src/lmql/utils/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/utils/graph.py` & `lmql-0.7b1/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql/utils/nputil.py` & `lmql-0.7b1/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.6/src/lmql.egg-info/PKG-INFO` & `lmql-0.7b1/src/lmql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.6
+Version: 0.7b1
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.6 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.7b1 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6.6/src/lmql.egg-info/SOURCES.txt` & `lmql-0.7b1/src/lmql.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 docs/source/_static/js/lmql-playground.js
 docs/source/_templates/layout.html
 docs/source/blog/release-0.0.5.md
 docs/source/blog/release-0.0.6.1.md
 docs/source/blog/release-0.0.6.3.md
 docs/source/blog/release-0.0.6.4.md
 docs/source/blog/release-0.0.6.5.md
+docs/source/blog/release-0.0.6.6.md
 docs/source/blog/release-0.0.6.md
 docs/source/images/inference.svg
 docs/source/language/azure.md
 docs/source/language/constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
 docs/source/language/hf.md
@@ -54,20 +55,22 @@
 docs/source/python/output.ipynb
 docs/source/python/pandas.ipynb
 docs/source/python/python.ipynb
 docs/source/releases/misc-snippets.md
 docs/source/releases/release-0.0.5.md
 scripts/Dockerfile
 scripts/activate-dev.sh
+scripts/changelog.sh
 scripts/pypi-release.sh
 scripts/serve-all.py
 scripts/wheel.sh
 scripts/conda/requirements-no-gpu.yml
 scripts/conda/requirements.yml
 src/lmql.svg
+src/lmql/.gitignore
 src/lmql/__init__.py
 src/lmql/cli.py
 src/lmql/demo.py
 src/lmql/http.py
 src/lmql/version.py
 src/lmql.egg-info/PKG-INFO
 src/lmql.egg-info/SOURCES.txt
@@ -79,14 +82,25 @@
 src/lmql/algorithms/cache.py
 src/lmql/algorithms/functools.py
 src/lmql/language/__init__.py
 src/lmql/language/compiler.py
 src/lmql/language/fragment_parser.py
 src/lmql/language/qstrings.py
 src/lmql/language/validator.py
+src/lmql/lib/__init__.py
+src/lmql/lib/actions.py
+src/lmql/lib/algebra222.csv
+src/lmql/lib/data.py
+src/lmql/lib/types.py
+src/lmql/lib/value.py
+src/lmql/lib/prompts/inline_code copy.py
+src/lmql/lib/prompts/inline_code.py
+src/lmql/lib/prompts/inline_use.py
+src/lmql/lib/prompts/inline_use_kevin.py
+src/lmql/lib/prompts/wiki_prompt.py
 src/lmql/models/__init__.py
 src/lmql/models/model.py
 src/lmql/models/lmtp/README.md
 src/lmql/models/lmtp/errors.py
 src/lmql/models/lmtp/lmtp_async.py
 src/lmql/models/lmtp/lmtp_client.py
 src/lmql/models/lmtp/lmtp_dcmodel.py
@@ -100,16 +114,20 @@
 src/lmql/models/lmtp/backends/__init__.py
 src/lmql/models/lmtp/backends/__main__.py
 src/lmql/models/lmtp/backends/llama_cpp_model.py
 src/lmql/models/lmtp/backends/lmtp_model.py
 src/lmql/models/lmtp/backends/random_model.py
 src/lmql/models/lmtp/backends/transformers_model.py
 src/lmql/ops/__init__.py
+src/lmql/ops/booleans.py
 src/lmql/ops/follow_map.py
+src/lmql/ops/inline_call.py
+src/lmql/ops/node.py
 src/lmql/ops/ops.py
+src/lmql/ops/regex.py
 src/lmql/ops/token_set.py
 src/lmql/output/__init__.py
 src/lmql/output/http.py
 src/lmql/output/sse.py
 src/lmql/output/ws.py
 src/lmql/runtime/__init__.py
 src/lmql/runtime/caching.py
@@ -180,14 +198,24 @@
 src/lmql/tests/queryargs/test_args_query_str.py
 src/lmql/tests/queryargs/test_args_run.py
 src/lmql/tests/queryargs/test_sync.py
 src/lmql/tests/queryargs/test_var_errors.py
 src/lmql/tests/system/basic_use_cases.py
 src/lmql/ui/.gitignore
 src/lmql/ui/__init__.py
+src/lmql/ui/chat/__init__.py
+src/lmql/ui/chat/__main__.py
+src/lmql/ui/chat/assets/code.svg
+src/lmql/ui/chat/assets/index.css
+src/lmql/ui/chat/assets/index.html
+src/lmql/ui/chat/assets/lmql-monaco.js
+src/lmql/ui/chat/assets/lmql.svg
+src/lmql/ui/chat/assets/send.svg
+src/lmql/ui/chat/assets/studio.css
+src/lmql/ui/chat/assets/studio.html
 src/lmql/ui/live/__init__.py
 src/lmql/ui/live/live.js
 src/lmql/ui/live/live.py
 src/lmql/ui/live/livelib.py
 src/lmql/ui/live/package.json
 src/lmql/ui/live/yarn.lock
 src/lmql/ui/playground/.dockerignore
@@ -204,17 +232,19 @@
 src/lmql/ui/playground/public/index.html
 src/lmql/ui/playground/public/lmql.svg
 src/lmql/ui/playground/public/manifest.json
 src/lmql/ui/playground/public/robots.txt
 src/lmql/ui/playground/public/precomputed/calc.json
 src/lmql/ui/playground/public/precomputed/chat.json
 src/lmql/ui/playground/public/precomputed/cot.json
+src/lmql/ui/playground/public/precomputed/date-regex.json
 src/lmql/ui/playground/public/precomputed/distribution.json
 src/lmql/ui/playground/public/precomputed/hello.json
 src/lmql/ui/playground/public/precomputed/joke.json
+src/lmql/ui/playground/public/precomputed/json-robust.json
 src/lmql/ui/playground/public/precomputed/json-template.json
 src/lmql/ui/playground/public/precomputed/kv.json
 src/lmql/ui/playground/public/precomputed/list.json
 src/lmql/ui/playground/public/precomputed/meta.json
 src/lmql/ui/playground/public/precomputed/translation.json
 src/lmql/ui/playground/public/precomputed/wiki.json
 src/lmql/ui/playground/public/snippets/dynamic-cfg.json
```

### Comparing `lmql-0.0.6.6/src/lmql.svg` & `lmql-0.7b1/src/lmql.svg`

 * *Files identical despite different names*

