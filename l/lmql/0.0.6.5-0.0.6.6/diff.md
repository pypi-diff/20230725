# Comparing `tmp/lmql-0.0.6.5.tar.gz` & `tmp/lmql-0.0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.6.5.tar", last modified: Fri Jul 14 15:57:02 2023, max compression
+gzip compressed data, was "lmql-0.0.6.6.tar", last modified: Tue Jul 25 10:40:20 2023, max compression
```

## Comparing `lmql-0.0.6.5.tar` & `lmql-0.0.6.6.tar`

### file list

```diff
@@ -1,315 +1,316 @@
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.080351 lmql-0.0.6.5/.github/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/.github/workflows/
--rw-r--r--   0 docker    (1000) docker    (1000)     2590 2023-07-14 15:52:52.000000 lmql-0.0.6.5/.github/workflows/lmql-ci.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     1543 2023-07-14 11:33:53.000000 lmql-0.0.6.5/.github/workflows/lmql-tests.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     2285 2023-07-14 11:31:18.000000 lmql-0.0.6.5/.github/workflows/lmql-web.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     2743 2023-07-14 11:31:18.000000 lmql-0.0.6.5/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.5/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)      140 2023-07-14 11:31:18.000000 lmql-0.0.6.5/MANIFEST.in
--rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-14 15:57:02.120350 lmql-0.0.6.5/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)     9448 2023-07-14 15:36:31.000000 lmql-0.0.6.5/README.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/
--rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/Makefile
--rw-r--r--   0 docker    (1000) docker    (1000)      444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/RELEASE.md
--rw-r--r--   0 docker    (1000) docker    (1000)      799 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/make.bat
--rw-r--r--   0 docker    (1000) docker    (1000)       81 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/requirements.txt
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_ext/
--rw-r--r--   0 docker    (1000) docker    (1000)     5728 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/_ext/lmql_snippets.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.080351 lmql-0.0.6.5/docs/source/_static/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_static/css/
--rw-r--r--   0 docker    (1000) docker    (1000)     6010 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/_static/css/lmql-docs.css
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_static/images/
--rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/_static/images/lmql.svg
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_static/js/
--rw-r--r--   0 docker    (1000) docker    (1000)     2087 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/_static/js/lmql-playground.js
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_templates/
--rw-r--r--   0 docker    (1000) docker    (1000)      292 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/_templates/layout.html
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/blog/
--rw-r--r--   0 docker    (1000) docker    (1000)     4591 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.1.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2068 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.3.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3221 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.4.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5349 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)     8976 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1167 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/conf.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1293 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/dev-setup.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2333 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/docker-setup.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/images/
--rw-r--r--   0 docker    (1000) docker    (1000)   125712 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/images/inference.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     2823 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/index.rst
--rw-r--r--   0 docker    (1000) docker    (1000)     2563 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/installation.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/language/
--rw-r--r--   0 docker    (1000) docker    (1000)     2313 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/azure.md
--rw-r--r--   0 docker    (1000) docker    (1000)     7435 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/constraints.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5365 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/decoders.md
--rw-r--r--   0 docker    (1000) docker    (1000)     7850 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/functions.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3967 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/hf.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2027 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/llama.cpp.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2896 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/models.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5710 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/openai.md
--rw-r--r--   0 docker    (1000) docker    (1000)     8292 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/overview.md
--rw-r--r--   0 docker    (1000) docker    (1000)     6032 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/scripted_prompts.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)    28444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/logo.png
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/pending/
--rw-r--r--   0 docker    (1000) docker    (1000)     3550 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/pending/release-next.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/python/
--rw-r--r--   0 docker    (1000) docker    (1000)       11 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)     4924 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/comparison.md
--rw-r--r--   0 docker    (1000) docker    (1000)    11193 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/langchain.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     1157 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/lc.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6681 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/llama_index.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)    75148 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/lmql.txt
--rw-r--r--   0 docker    (1000) docker    (1000)     7458 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/output.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     9592 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/pandas.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)    13317 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/python.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     4806 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/quickstart.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/releases/
--rw-r--r--   0 docker    (1000) docker    (1000)     2263 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/releases/misc-snippets.md
--rw-r--r--   0 docker    (1000) docker    (1000)      321 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/releases/release-0.0.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)      257 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/todo.md
--rw-r--r--   0 docker    (1000) docker    (1000)      137 2023-07-14 11:31:18.000000 lmql-0.0.6.5/pyproject.toml
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/scripts/
--rw-r--r--   0 docker    (1000) docker    (1000)      577 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/Dockerfile
--rw-r--r--   0 docker    (1000) docker    (1000)      295 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/activate-dev.sh
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/scripts/conda/
--rw-r--r--   0 docker    (1000) docker    (1000)      198 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/conda/requirements-no-gpu.yml
--rw-r--r--   0 docker    (1000) docker    (1000)      332 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/conda/requirements.yml
--rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/pypi-release.sh
--rw-r--r--   0 docker    (1000) docker    (1000)     3897 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/serve-all.py
--rw-r--r--   0 docker    (1000) docker    (1000)      854 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/wheel.sh
--rw-r--r--   0 docker    (1000) docker    (1000)      868 2023-07-14 15:57:02.120350 lmql-0.0.6.5/setup.cfg
--rw-r--r--   0 docker    (1000) docker    (1000)       37 2023-07-14 11:31:18.000000 lmql-0.0.6.5/setup.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/src/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/src/lmql/
--rw-r--r--   0 docker    (1000) docker    (1000)     7767 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/algorithms/
--rw-r--r--   0 docker    (1000) docker    (1000)       45 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/algorithms/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2556 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/algorithms/cache.py
--rw-r--r--   0 docker    (1000) docker    (1000)      916 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/algorithms/functools.py
--rwxr-xr-x   0 docker    (1000) docker    (1000)     8313 2023-07-14 11:38:09.000000 lmql-0.0.6.5/src/lmql/cli.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1578 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/demo.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1531 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/http.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/language/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    27521 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/compiler.py
--rw-r--r--   0 docker    (1000) docker    (1000)    11042 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/fragment_parser.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4545 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/qstrings.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1804 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/validator.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/models/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/models/lmtp/
--rw-r--r--   0 docker    (1000) docker    (1000)     6156 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/README.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/models/lmtp/backends/
--rw-r--r--   0 docker    (1000) docker    (1000)      493 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)      694 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/__main__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4159 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/llama_cpp_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/lmtp_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2002 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/random_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3906 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/transformers_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)       42 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/errors.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4669 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_async.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5645 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_client.py
--rw-r--r--   0 docker    (1000) docker    (1000)    20101 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_dcmodel.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2283 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_inference_server.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5606 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_multiprocessing.py
--rw-r--r--   0 docker    (1000) docker    (1000)      298 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
--rw-r--r--   0 docker    (1000) docker    (1000)    15157 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_scheduler.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5685 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_serve.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3562 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_threading.py
--rw-r--r--   0 docker    (1000) docker    (1000)      634 2023-07-14 15:36:31.000000 lmql-0.0.6.5/src/lmql/models/lmtp/utils.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3396 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/model.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/ops/
--rw-r--r--   0 docker    (1000) docker    (1000)       93 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     7542 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/follow_map.py
--rw-r--r--   0 docker    (1000) docker    (1000)    41979 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/ops.py
--rw-r--r--   0 docker    (1000) docker    (1000)    21170 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/token_set.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/output/
--rw-r--r--   0 docker    (1000) docker    (1000)       57 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2334 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/http.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1889 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/sse.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2282 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/ws.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/bopenai/
--rw-r--r--   0 docker    (1000) docker    (1000)     2236 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/bopenai/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    29480 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/bopenai/batched_openai.py
--rw-r--r--   0 docker    (1000) docker    (1000)    21828 2023-07-14 15:36:31.000000 lmql-0.0.6.5/src/lmql/runtime/bopenai/openai_api.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2096 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/caching.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/dclib/
--rw-r--r--   0 docker    (1000) docker    (1000)      494 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    18839 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_array.py
--rw-r--r--   0 docker    (1000) docker    (1000)    26354 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_cache.py
--rw-r--r--   0 docker    (1000) docker    (1000)      592 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_global.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4970 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     8589 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-r--r--   0 docker    (1000) docker    (1000)    32348 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_seq.py
--rw-r--r--   0 docker    (1000) docker    (1000)    22035 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/decoders.py
--rw-r--r--   0 docker    (1000) docker    (1000)    39770 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/interpreter.py
--rw-r--r--   0 docker    (1000) docker    (1000)      250 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/interrupt.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1231 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/langchain.py
--rw-r--r--   0 docker    (1000) docker    (1000)     8977 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/lmql_runtime.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1940 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/loop.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1245 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/maiohttp.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1726 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/masks.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3139 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/model_registry.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5943 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/multi_head_interpretation.py
--rw-r--r--   0 docker    (1000) docker    (1000)    44972 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/openai_integration.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1971 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/openai_secret.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4042 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/output_writer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/postprocessing/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/postprocessing/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3543 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-r--r--   0 docker    (1000) docker    (1000)      152 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/postprocessing/group_by.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2209 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/program_state.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1317 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/stats.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2220 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/token_distribution.py
--rw-r--r--   0 docker    (1000) docker    (1000)    11565 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/tokenizers/
--rw-r--r--   0 docker    (1000) docker    (1000)     4509 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizers/hf_tokenizer.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3427 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3207 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/
--rw-r--r--   0 docker    (1000) docker    (1000)      319 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)      907 2023-07-14 11:44:57.000000 lmql-0.0.6.5/src/lmql/tests/all.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5914 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/expr_test_utils.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1314 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/fin_and.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/outdated/
--rw-r--r--   0 docker    (1000) docker    (1000)     1611 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/mask_product_test.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2789 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/monotonicity.py
--rw-r--r--   0 docker    (1000) docker    (1000)      546 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/one_of_tests.py
--rw-r--r--   0 docker    (1000) docker    (1000)      758 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/sentences_op.py
--rw-r--r--   0 docker    (1000) docker    (1000)      984 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/starts_with_op_test.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1236 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/stops_at.py
--rw-r--r--   0 docker    (1000) docker    (1000)      537 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/str_in_str_tests.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4738 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/test_multi_head.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3036 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/token_set_test.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/queryargs/
--rw-r--r--   0 docker    (1000) docker    (1000)     4489 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_args.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2072 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_query_str.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1095 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_run.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1066 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_sync.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1092 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_var_errors.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/system/
--rw-r--r--   0 docker    (1000) docker    (1000)     3402 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/system/basic_use_cases.py
--rw-r--r--   0 docker    (1000) docker    (1000)      842 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/tail_token_set.py
--rw-r--r--   0 docker    (1000) docker    (1000)      788 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_back2back_caching.py
--rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_beam_in.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2775 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_eq.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1756 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_escaping.py
--rw-r--r--   0 docker    (1000) docker    (1000)      877 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_local_model_python.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_minimal_syntax.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1139 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_multibyte_characters.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1171 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_multibyte_local_models.py
--rw-r--r--   0 docker    (1000) docker    (1000)      457 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_orop.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2931 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_qstrings.py
--rw-r--r--   0 docker    (1000) docker    (1000)      479 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_query_args.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2639 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_sample_queries.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1703 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_scoping.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3647 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_stopping.py
--rw-r--r--   0 docker    (1000) docker    (1000)      707 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/tiktoken_tsets.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/ui/
--rw-r--r--   0 docker    (1000) docker    (1000)       27 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.108351 lmql-0.0.6.5/src/lmql/ui/live/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6747 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/live.js
--rw-r--r--   0 docker    (1000) docker    (1000)     3475 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/live.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3885 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/livelib.py
--rw-r--r--   0 docker    (1000) docker    (1000)      349 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/package.json
--rw-r--r--   0 docker    (1000) docker    (1000)    33701 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/yarn.lock
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.108351 lmql-0.0.6.5/src/lmql/ui/playground/
--rw-r--r--   0 docker    (1000) docker    (1000)       31 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/.dockerignore
--rw-r--r--   0 docker    (1000) docker    (1000)       34 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/.env
--rw-r--r--   0 docker    (1000) docker    (1000)      310 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)      354 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/Dockerfile
--rw-r--r--   0 docker    (1000) docker    (1000)     3359 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1327 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/package.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.108351 lmql-0.0.6.5/src/lmql/ui/playground/public/
--rw-r--r--   0 docker    (1000) docker    (1000)       90 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/_headers
--rw-r--r--   0 docker    (1000) docker    (1000)     3870 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/favicon.ico
--rw-r--r--   0 docker    (1000) docker    (1000)     1678 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/index.html
--rw-r--r--   0 docker    (1000) docker    (1000)     2817 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)      306 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/manifest.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.112351 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/
--rw-r--r--   0 docker    (1000) docker    (1000)  1227728 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/calc.json
--rw-r--r--   0 docker    (1000) docker    (1000)   295285 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/chat.json
--rw-r--r--   0 docker    (1000) docker    (1000)   160131 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/cot.json
--rw-r--r--   0 docker    (1000) docker    (1000)    81768 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-r--r--   0 docker    (1000) docker    (1000)    22895 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/hello.json
--rw-r--r--   0 docker    (1000) docker    (1000)    89531 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/joke.json
--rw-r--r--   0 docker    (1000) docker    (1000)   265372 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/json-template.json
--rw-r--r--   0 docker    (1000) docker    (1000)  1710847 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/kv.json
--rw-r--r--   0 docker    (1000) docker    (1000)    52748 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/list.json
--rw-r--r--   0 docker    (1000) docker    (1000)   628184 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/meta.json
--rw-r--r--   0 docker    (1000) docker    (1000)   264768 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/translation.json
--rw-r--r--   0 docker    (1000) docker    (1000)   215050 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-r--r--   0 docker    (1000) docker    (1000)       67 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/robots.txt
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.116351 lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/
--rw-r--r--   0 docker    (1000) docker    (1000)   381736 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-r--r--   0 docker    (1000) docker    (1000)   184008 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-r--r--   0 docker    (1000) docker    (1000)       62 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/ref.py
--rw-r--r--   0 docker    (1000) docker    (1000)       80 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/run-in-docker.sh
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.116351 lmql-0.0.6.5/src/lmql/ui/playground/src/
--rw-r--r--   0 docker    (1000) docker    (1000)    75521 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/App.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      246 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/App.test.js
--rw-r--r--   0 docker    (1000) docker    (1000)    29983 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      807 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/Configuration.js
--rw-r--r--   0 docker    (1000) docker    (1000)     1174 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/DataListView.js
--rw-r--r--   0 docker    (1000) docker    (1000)    21617 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/DecoderGraph.js
--rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/DecodingTree.js
--rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/Embed.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)     9601 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/Explore.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      675 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/SharedState.js
--rw-r--r--   0 docker    (1000) docker    (1000)     4819 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/State.js
--rw-r--r--   0 docker    (1000) docker    (1000)     5871 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)     9360 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/browser_process.js
--rw-r--r--   0 docker    (1000) docker    (1000)     1163 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/build_info.js
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/playground/src/editor/
--rw-r--r--   0 docker    (1000) docker    (1000)     8696 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-r--r--   0 docker    (1000) docker    (1000)     4758 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/editor/theme.json
--rw-r--r--   0 docker    (1000) docker    (1000)      889 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/explore.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     1345 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/graph-layout.css
--rw-r--r--   0 docker    (1000) docker    (1000)     1698 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/index.css
--rw-r--r--   0 docker    (1000) docker    (1000)      489 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/index.js
--rw-r--r--   0 docker    (1000) docker    (1000)     2632 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/logo.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     8766 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/queries.js
--rw-r--r--   0 docker    (1000) docker    (1000)     5990 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/remote_process.js
--rw-r--r--   0 docker    (1000) docker    (1000)      362 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/reportWebVitals.js
--rw-r--r--   0 docker    (1000) docker    (1000)     9520 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/screenshot.css
--rw-r--r--   0 docker    (1000) docker    (1000)      241 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/setupTests.js
--rw-r--r--   0 docker    (1000) docker    (1000)     3466 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/spinner.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     3200 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/tagged-model-result.js
--rw-r--r--   0 docker    (1000) docker    (1000)   449905 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/yarn.lock
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/vscode/
--rw-r--r--   0 docker    (1000) docker    (1000)       76 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.gitattributes
--rw-r--r--   0 docker    (1000) docker    (1000)       19 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.gitignore
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/vscode/.vscode/
--rw-r--r--   0 docker    (1000) docker    (1000)      540 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.vscode/launch.json
--rw-r--r--   0 docker    (1000) docker    (1000)       66 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.vscodeignore
--rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)      959 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/language-configuration.json
--rw-r--r--   0 docker    (1000) docker    (1000)    11532 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/lmql-vscode.png
--rw-r--r--   0 docker    (1000) docker    (1000)     1214 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/package.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/
--rw-r--r--   0 docker    (1000) docker    (1000)      518 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-r--r--   0 docker    (1000) docker    (1000)      642 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-r--r--   0 docker    (1000) docker    (1000)      853 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/utils/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2402 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/docstring_parser.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4933 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/graph.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2715 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/nputil.py
--rw-r--r--   0 docker    (1000) docker    (1000)      114 2023-07-14 15:56:54.000000 lmql-0.0.6.5/src/lmql/version.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/src/lmql.egg-info/
--rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)     9141 2023-07-14 15:57:02.000000 lmql-0.0.6.5/src/lmql.egg-info/SOURCES.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/dependency_links.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       39 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/entry_points.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       95 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/requires.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        5 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/top_level.txt
--rw-r--r--   0 docker    (1000) docker    (1000)   115785 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)       86 2023-07-14 11:31:18.000000 lmql-0.0.6.5/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.646276 lmql-0.0.6.6/.github/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/.github/workflows/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2590 2023-07-14 15:52:52.000000 lmql-0.0.6.6/.github/workflows/lmql-ci.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     1543 2023-07-14 11:33:53.000000 lmql-0.0.6.6/.github/workflows/lmql-tests.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2285 2023-07-20 09:50:34.000000 lmql-0.0.6.6/.github/workflows/lmql-web.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2743 2023-07-14 11:31:18.000000 lmql-0.0.6.6/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.6/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      140 2023-07-14 11:31:18.000000 lmql-0.0.6.6/MANIFEST.in
+-rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-25 10:40:20.730274 lmql-0.0.6.6/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)     9448 2023-07-14 15:36:31.000000 lmql-0.0.6.6/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/Makefile
+-rw-r--r--   0 docker    (1000) docker    (1000)      444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/RELEASE.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      799 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/make.bat
+-rw-r--r--   0 docker    (1000) docker    (1000)       81 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/requirements.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_ext/
+-rw-r--r--   0 docker    (1000) docker    (1000)     5728 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/_ext/lmql_snippets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.646276 lmql-0.0.6.6/docs/source/_static/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_static/css/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6010 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/_static/css/lmql-docs.css
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_static/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/_static/images/lmql.svg
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_static/js/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2087 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/_static/js/lmql-playground.js
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.654276 lmql-0.0.6.6/docs/source/_templates/
+-rw-r--r--   0 docker    (1000) docker    (1000)      292 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/_templates/layout.html
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.658276 lmql-0.0.6.6/docs/source/blog/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4591 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.1.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2068 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.3.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3221 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.4.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5872 2023-07-20 09:50:34.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8976 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/blog/release-0.0.6.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1167 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/conf.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1293 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/dev-setup.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2333 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/docker-setup.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.658276 lmql-0.0.6.6/docs/source/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)   125712 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/images/inference.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     2823 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/index.rst
+-rw-r--r--   0 docker    (1000) docker    (1000)     2563 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/installation.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.658276 lmql-0.0.6.6/docs/source/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2313 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/azure.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     7435 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/constraints.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5365 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/decoders.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     7850 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/functions.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3967 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/hf.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2027 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/llama.cpp.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2896 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/models.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5710 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/language/openai.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8292 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/language/overview.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     6032 2023-07-20 09:50:34.000000 lmql-0.0.6.6/docs/source/language/scripted_prompts.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)    28444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/logo.png
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.662275 lmql-0.0.6.6/docs/source/pending/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3550 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/pending/release-next.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.666275 lmql-0.0.6.6/docs/source/python/
+-rw-r--r--   0 docker    (1000) docker    (1000)       11 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)     4924 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/comparison.md
+-rw-r--r--   0 docker    (1000) docker    (1000)    11193 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/langchain.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     1157 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/lc.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6681 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/llama_index.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    75148 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/lmql.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)     7458 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/output.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     9592 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/pandas.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    13317 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/python/python.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     4806 2023-07-14 15:36:31.000000 lmql-0.0.6.6/docs/source/quickstart.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.666275 lmql-0.0.6.6/docs/source/releases/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2263 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/releases/misc-snippets.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      321 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/source/releases/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      257 2023-07-14 11:31:18.000000 lmql-0.0.6.6/docs/todo.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      137 2023-07-14 11:31:18.000000 lmql-0.0.6.6/pyproject.toml
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.670275 lmql-0.0.6.6/scripts/
+-rw-r--r--   0 docker    (1000) docker    (1000)      577 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)      295 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/activate-dev.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.670275 lmql-0.0.6.6/scripts/conda/
+-rw-r--r--   0 docker    (1000) docker    (1000)      198 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/conda/requirements-no-gpu.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      332 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/conda/requirements.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/pypi-release.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)     3897 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/serve-all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      854 2023-07-14 11:31:18.000000 lmql-0.0.6.6/scripts/wheel.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)      868 2023-07-25 10:40:20.730274 lmql-0.0.6.6/setup.cfg
+-rw-r--r--   0 docker    (1000) docker    (1000)       37 2023-07-14 11:31:18.000000 lmql-0.0.6.6/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.670275 lmql-0.0.6.6/src/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.674275 lmql-0.0.6.6/src/lmql/
+-rw-r--r--   0 docker    (1000) docker    (1000)     7767 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.674275 lmql-0.0.6.6/src/lmql/algorithms/
+-rw-r--r--   0 docker    (1000) docker    (1000)       45 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/algorithms/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2696 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/algorithms/cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      926 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/algorithms/functools.py
+-rwxr-xr-x   0 docker    (1000) docker    (1000)     8313 2023-07-14 11:38:09.000000 lmql-0.0.6.6/src/lmql/cli.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1578 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/demo.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1531 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/http.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.678275 lmql-0.0.6.6/src/lmql/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/language/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    29360 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/language/compiler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11042 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/language/fragment_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4545 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/language/qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1804 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/language/validator.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.678275 lmql-0.0.6.6/src/lmql/models/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.682275 lmql-0.0.6.6/src/lmql/models/lmtp/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6156 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.682275 lmql-0.0.6.6/src/lmql/models/lmtp/backends/
+-rw-r--r--   0 docker    (1000) docker    (1000)      493 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      694 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/__main__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4362 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/llama_cpp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/lmtp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2002 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/random_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4327 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/models/lmtp/backends/transformers_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       42 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/errors.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4669 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_async.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5645 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_client.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    20135 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_dcmodel.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2283 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_inference_server.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5606 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_multiprocessing.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      298 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    15201 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_scheduler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6381 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_serve.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3562 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_threading.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      634 2023-07-14 15:36:31.000000 lmql-0.0.6.6/src/lmql/models/lmtp/utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3396 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/models/model.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.682275 lmql-0.0.6.6/src/lmql/ops/
+-rw-r--r--   0 docker    (1000) docker    (1000)       93 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ops/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     7542 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ops/follow_map.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    42177 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/ops/ops.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21170 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ops/token_set.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.686275 lmql-0.0.6.6/src/lmql/output/
+-rw-r--r--   0 docker    (1000) docker    (1000)       57 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2334 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/http.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1889 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/sse.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2282 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/output/ws.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/bopenai/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2236 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/bopenai/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    29628 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/bopenai/batched_openai.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21823 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/bopenai/openai_api.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2096 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/caching.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/dclib/
+-rw-r--r--   0 docker    (1000) docker    (1000)      494 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    18839 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_array.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    26354 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      592 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_global.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4970 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8589 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    32348 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_seq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    22035 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/dclib/decoders.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    39830 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/interpreter.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      250 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/interrupt.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1231 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/langchain.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    10237 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/lmql_runtime.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1940 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/loop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1245 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/maiohttp.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1726 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/masks.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3145 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/runtime/model_registry.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5943 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/multi_head_interpretation.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    44838 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/openai_integration.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2179 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/openai_secret.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4042 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/output_writer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/postprocessing/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/postprocessing/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3543 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      152 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/postprocessing/group_by.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2209 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/program_state.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1317 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/stats.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2220 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/token_distribution.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11565 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.690275 lmql-0.0.6.6/src/lmql/runtime/tokenizers/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4509 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizers/hf_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3427 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3207 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.694275 lmql-0.0.6.6/src/lmql/tests/
+-rw-r--r--   0 docker    (1000) docker    (1000)      319 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      907 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/tests/all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5914 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/tests/expr_test_utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1314 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/fin_and.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/tests/outdated/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1611 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/mask_product_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2789 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/monotonicity.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      546 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/one_of_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      758 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/sentences_op.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      984 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1236 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/stops_at.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      537 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4738 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/test_multi_head.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3036 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/outdated/token_set_test.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/tests/queryargs/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4489 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2072 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_query_str.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1095 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_run.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1066 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_sync.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1092 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/queryargs/test_var_errors.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/tests/system/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3402 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/system/basic_use_cases.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      842 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/tail_token_set.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      788 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_back2back_caching.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_beam_in.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2775 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_eq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1756 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_escaping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2370 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/tests/test_f.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1033 2023-07-25 10:16:53.000000 lmql-0.0.6.6/src/lmql/tests/test_local_model_python.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_minimal_syntax.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1139 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_multibyte_characters.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1171 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_multibyte_local_models.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      457 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_orop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2931 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      479 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_query_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2639 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_sample_queries.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1703 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_scoping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3647 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/test_stopping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      707 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/tests/tiktoken_tsets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/ui/
+-rw-r--r--   0 docker    (1000) docker    (1000)       27 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.698275 lmql-0.0.6.6/src/lmql/ui/live/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6747 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/live.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3475 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/live.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3885 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/livelib.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      349 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/package.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    33701 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/live/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.702275 lmql-0.0.6.6/src/lmql/ui/playground/
+-rw-r--r--   0 docker    (1000) docker    (1000)       31 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/.dockerignore
+-rw-r--r--   0 docker    (1000) docker    (1000)       34 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/.env
+-rw-r--r--   0 docker    (1000) docker    (1000)      310 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)      354 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)     3359 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1327 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.702275 lmql-0.0.6.6/src/lmql/ui/playground/public/
+-rw-r--r--   0 docker    (1000) docker    (1000)       90 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/_headers
+-rw-r--r--   0 docker    (1000) docker    (1000)     3870 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/favicon.ico
+-rw-r--r--   0 docker    (1000) docker    (1000)     1678 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/index.html
+-rw-r--r--   0 docker    (1000) docker    (1000)     2817 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)      306 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/manifest.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.718274 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/
+-rw-r--r--   0 docker    (1000) docker    (1000)  1227728 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   295285 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   160131 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    81768 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    22895 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    89531 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   265372 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/json-template.json
+-rw-r--r--   0 docker    (1000) docker    (1000)  1710847 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    52748 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/list.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   628184 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   264768 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   215050 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       67 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/robots.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.718274 lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/
+-rw-r--r--   0 docker    (1000) docker    (1000)   381736 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   184008 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       62 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/ref.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       80 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/run-in-docker.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.726274 lmql-0.0.6.6/src/lmql/ui/playground/src/
+-rw-r--r--   0 docker    (1000) docker    (1000)    75521 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/App.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      246 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/App.test.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    29983 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      807 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/Configuration.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1174 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/DataListView.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    21617 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/DecodingTree.js
+-rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/Embed.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)     9601 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/Explore.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      675 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/SharedState.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4819 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/State.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5871 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)     9360 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/browser_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1163 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/build_info.js
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.726274 lmql-0.0.6.6/src/lmql/ui/playground/src/editor/
+-rw-r--r--   0 docker    (1000) docker    (1000)     8696 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4758 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/editor/theme.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      889 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/explore.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     1345 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/graph-layout.css
+-rw-r--r--   0 docker    (1000) docker    (1000)     1698 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/index.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      489 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/index.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     2632 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/logo.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     8766 2023-07-20 09:50:34.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/queries.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5990 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/remote_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      362 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     9520 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/screenshot.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      241 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/setupTests.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3466 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/spinner.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     3200 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-r--r--   0 docker    (1000) docker    (1000)   449905 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/playground/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/ui/vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)       76 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.gitattributes
+-rw-r--r--   0 docker    (1000) docker    (1000)       19 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.gitignore
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/ui/vscode/.vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)      540 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.vscode/launch.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       66 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/.vscodeignore
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      959 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/language-configuration.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    11532 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/lmql-vscode.png
+-rw-r--r--   0 docker    (1000) docker    (1000)     1214 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/
+-rw-r--r--   0 docker    (1000) docker    (1000)      518 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      642 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      853 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.730274 lmql-0.0.6.6/src/lmql/utils/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2402 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/docstring_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4933 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/graph.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2715 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql/utils/nputil.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      114 2023-07-25 10:40:12.000000 lmql-0.0.6.6/src/lmql/version.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 10:40:20.674275 lmql-0.0.6.6/src/lmql.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)     9166 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       39 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/entry_points.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       95 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        5 2023-07-25 10:40:20.000000 lmql-0.0.6.6/src/lmql.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)   115785 2023-07-14 11:31:18.000000 lmql-0.0.6.6/src/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)       86 2023-07-14 11:31:18.000000 lmql-0.0.6.6/yarn.lock
```

### Comparing `lmql-0.0.6.5/.github/workflows/lmql-ci.yml` & `lmql-0.0.6.6/.github/workflows/lmql-ci.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/.github/workflows/lmql-tests.yml` & `lmql-0.0.6.6/.github/workflows/lmql-tests.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/.github/workflows/lmql-web.yml` & `lmql-0.0.6.6/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/.gitignore` & `lmql-0.0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/LICENSE` & `lmql-0.0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/PKG-INFO` & `lmql-0.0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.5
+Version: 0.0.6.6
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
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.5 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.6 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6.5/README.md` & `lmql-0.0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/Makefile` & `lmql-0.0.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/make.bat` & `lmql-0.0.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.6.6/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.6.6/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/_static/images/lmql.svg` & `lmql-0.0.6.6/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.6.6/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/blog/release-0.0.5.md` & `lmql-0.0.6.6/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/blog/release-0.0.6.1.md` & `lmql-0.0.6.6/docs/source/blog/release-0.0.6.1.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/blog/release-0.0.6.3.md` & `lmql-0.0.6.6/docs/source/blog/release-0.0.6.3.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/blog/release-0.0.6.4.md` & `lmql-0.0.6.6/docs/source/blog/release-0.0.6.4.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/blog/release-0.0.6.5.md` & `lmql-0.0.6.6/docs/source/blog/release-0.0.6.5.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 metadata:release: 2023-07-13 18:00:00 +0000
 metadata:authors: team
 
-# LMQL becomes simpler and more powerful
+# LMQL becomes simpler and adds llama.cpp
 
 Today we are releasing LMQL 0.0.6.5. This update contains a major simplification of the LMQL syntax, moving it much closer to standard Python. It also includes a `llama.cpp` based inference backend, several bug fixes and other minor improvements.
 
+You can try the latest version of LMQL in your browser at [lmql.ai/playground](https://lmql.ai/playground) or install it via `pip install lmql`.
+
 ## One Line Is All It Takes
 
 Most notably, 0.0.6.5 comes with several simplifications of the core syntax of LMQL. Of course, all changes are backwards compatible, so you can continue to use your existing query code and move to the new version without any changes.
 
-With this, we aim to minimize syntactic overhead, by employing sensible defaults to enable more concise query code like the following:
+With this, we aim to minimize syntactic overhead, employing sensible defaults to enable more concise programs like the following:
 
 ```{lmql}
 name::simple-syntax
 
 "One line is all it takes [CONTINUATION]"
 
 model-output::
@@ -126,16 +128,22 @@
 name::llama-cpp-blog
 
 argmax "Say 'this is a test':[RESPONSE]" from "llama.cpp:<PATH TO WEIGHTS>.bin"
 ```
 
 We support, both, in-process loading of `llama.cpp`, as well as remote inference via `lmql serve-model`. To learn more about `llama.cpp` and how to use it with LMQL, check out the corresponding chapter in the LMQL [documentation](https://docs.lmql.ai/en/latest/language/llama.cpp.html).
 
+<br/>
+
 ## Other Changes
 
 * LMQL now includes a `random` model backend, which randomly samples tokens from the GPT-2 vocabulary. This is useful for debugging and testing purposes and can be used for data generation in the context of highly constrained query programs.
 
 * Two caching issues have been fixed, avoiding cache collisions which could lead to repeated model outputs.
 
-* More robust query string parsing, allowing for robust escaping of special characters `[`, `]`, `{` and `}`.
+* More robust query string parsing, allowing for [robust escaping](https://docs.lmql.ai/en/stable/language/scripted_prompts.html#escaping) of special characters `[`, `]`, `{` and `}`.
 
 * Added support for `transformers` based Llama models and the associated (fast) implementation of HF tokenizers.
+
+* Simplified Azure OpenAI support, see the relevant chapter in the [documentation](https://docs.lmql.ai/en/stable/language/azure.html).
+
+We thank community members [@minosvasilias](https://github.com/minosvasilias) and [@CircArgs](https://github.com/CircArgs) for their contribution to this release.
```

### Comparing `lmql-0.0.6.5/docs/source/blog/release-0.0.6.md` & `lmql-0.0.6.6/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/conf.py` & `lmql-0.0.6.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/dev-setup.md` & `lmql-0.0.6.6/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/docker-setup.md` & `lmql-0.0.6.6/docs/source/docker-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/images/inference.svg` & `lmql-0.0.6.6/docs/source/images/inference.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/index.rst` & `lmql-0.0.6.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/installation.md` & `lmql-0.0.6.6/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/azure.md` & `lmql-0.0.6.6/docs/source/language/azure.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/constraints.md` & `lmql-0.0.6.6/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/decoders.md` & `lmql-0.0.6.6/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/functions.md` & `lmql-0.0.6.6/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/hf.md` & `lmql-0.0.6.6/docs/source/language/hf.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/llama.cpp.md` & `lmql-0.0.6.6/docs/source/language/llama.cpp.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/models.md` & `lmql-0.0.6.6/docs/source/language/models.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/openai.md` & `lmql-0.0.6.6/docs/source/language/openai.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/overview.md` & `lmql-0.0.6.6/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/language/scripted_prompts.md` & `lmql-0.0.6.6/docs/source/language/scripted_prompts.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Scripted Prompting
 
-In LMQL, programs are not just static tempaltes of text, as they also contain control flow (e.g. loops, conditions, function calls). This facilitates dynamic prompt construction and allows LMQL programs to respond dynamically to model output. This scripting mechanic is achieved by a combination of prompt templates, control flow and [output constraining](constraints.md).
+In LMQL, programs are not just static templates of text, as they also contain control flow (e.g. loops, conditions, function calls). This facilitates dynamic prompt construction and allows LMQL programs to respond dynamically to model output. This scripting mechanic is achieved by a combination of prompt templates, control flow and [output constraining](constraints.md).
 
 > Note: LMQL requires special escaping to use `[`, `]`, `{` and `}` in a literal way, see [](Escaping).
 
 **Packing List** For instance, let's say we want to generate a packing list before going on vacation. One way to do this would be the following query:
 
 ```{lmql}
```

### Comparing `lmql-0.0.6.5/docs/source/lmql.svg` & `lmql-0.0.6.6/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/logo.png` & `lmql-0.0.6.6/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/pending/release-next.md` & `lmql-0.0.6.6/docs/source/pending/release-next.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/comparison.md` & `lmql-0.0.6.6/docs/source/python/comparison.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/langchain.ipynb` & `lmql-0.0.6.6/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/lc.py` & `lmql-0.0.6.6/docs/source/python/lc.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/llama_index.ipynb` & `lmql-0.0.6.6/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/lmql.txt` & `lmql-0.0.6.6/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/output.ipynb` & `lmql-0.0.6.6/docs/source/python/output.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/pandas.ipynb` & `lmql-0.0.6.6/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/python/python.ipynb` & `lmql-0.0.6.6/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/quickstart.md` & `lmql-0.0.6.6/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/docs/source/releases/misc-snippets.md` & `lmql-0.0.6.6/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/scripts/Dockerfile` & `lmql-0.0.6.6/scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/scripts/pypi-release.sh` & `lmql-0.0.6.6/scripts/pypi-release.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/scripts/serve-all.py` & `lmql-0.0.6.6/scripts/serve-all.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/scripts/wheel.sh` & `lmql-0.0.6.6/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/setup.cfg` & `lmql-0.0.6.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.6.5
+version = 0.0.6.6
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.6.5/src/lmql/__init__.py` & `lmql-0.0.6.6/src/lmql/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/algorithms/cache.py` & `lmql-0.0.6.6/src/lmql/algorithms/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pickle
 import os
 import inspect
 
 from lmql.runtime.lmql_runtime import LMQLQueryFunction
-from lmql import LMQLResult
+from lmql import LMQLResult, F
 
 # cache query results by query code and arguments
 global cache_file
 cache_file = None
 global cache
 cache = None
 
@@ -42,17 +42,21 @@
 def persist_cache():
     global cache
     global cache_file
     if cache is not None and cache_file is not None:
         with open(cache_file, "wb") as f:
             pickle.dump(cache, f)
 
-async def apply(q, *args):
+async def apply(q, *args, **kwargs):
     global cache
 
+    if type(q) is str:
+        where = kwargs.pop("where", None)
+        q = F(q, constraints=where, is_async=True)
+
     # handle non-LMQL queries
     if type(q) is not LMQLQueryFunction:
         if inspect.iscoroutinefunction(q):
             return await q(*args)
         return q(*args)
 
     global stats
@@ -70,15 +74,15 @@
         key = str(q.lmql_code) + str(args)
     
     if cache is not None and key in cache.keys():
         stats["cached"] += 1
         return cache[key]
     else:
         try:
-            result = await q(*args)
+            result = await q(*args, **kwargs)
             if len(result) == 1:
                 result = result[0]
             if type(result) is LMQLResult:
                 if "RESULT" in result.variables.keys():
                     result = result.variables["RESULT"].strip()
 
             if cache is not None:
```

### Comparing `lmql-0.0.6.5/src/lmql/algorithms/functools.py` & `lmql-0.0.6.6/src/lmql/algorithms/functools.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     total_results = []
 
     if progress:
         import tqdm
         chunks = tqdm.tqdm(chunks, file=sys.stdout)
 
     for chunk in chunks:
-        results = await asyncio.gather(*[apply(q, x) for x in chunk])
+        results = await asyncio.gather(*[apply(q, x, **kwargs) for x in chunk])
         total_results += results
 
     return total_results
 
 async def reduce(f, items, initial=None):
     if initial is None:
         acc = items[0]
```

### Comparing `lmql-0.0.6.5/src/lmql/cli.py` & `lmql-0.0.6.6/src/lmql/cli.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/demo.py` & `lmql-0.0.6.6/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/http.py` & `lmql-0.0.6.6/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/language/compiler.py` & `lmql-0.0.6.6/src/lmql/language/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,78 +38,93 @@
     def visit_Name(self, node):
         if type(node.ctx) is ast.Load:
             if self.is_excluded(node.id):
                 return
             self.free_vars.add(node.id)
 
 class DefinedVarsCollector(ast.NodeVisitor):
-    def __init__(self, defined_vars):
+    def __init__(self, defined_vars, defined_constraints):
         self.defined_vars = defined_vars
+        self.defined_constraints = defined_constraints
 
     def visit_Name(self, node):
         if type(node.ctx) is ast.Store:
             self.defined_vars.add(node.id)
+        super().generic_visit(node)
 
     def visit_FunctionDef(self, node: FunctionDef) -> Any:
         self.defined_vars.add(node.name)
+        super().generic_visit(node)
 
     def visit_ClassDef(self, node: ClassDef) -> Any:
         self.defined_vars.add(node.name)
+        visit_potential_constraint_def(node, self)
+        super().generic_visit(node)
 
     def visit_Import(self, node: Import) -> Any:
         for alias in node.names:
             self.defined_vars.add(alias.asname or alias.name)
+        super().generic_visit(node)
 
     def visit_ImportFrom(self, node: ImportFrom) -> Any:
         for alias in node.names:
             self.defined_vars.add(alias.asname or alias.name)
+        super().generic_visit(node)
 
     def visit_AsyncFunctionDef(self, node: AsyncFunctionDef) -> Any:
         self.defined_vars.add(node.name)
+        super().generic_visit(node)
+
+    # visit LMQLOp decorator to collect defined variables
+    def visit_Call(self, node: ast.Call) -> Any:
+        return super().generic_visit(node)
 
 class PromptScope(ast.NodeVisitor):
     def __init__(self):
         self.distribution_vars = set()
         self.defined_vars = set()
         self.prologue_vars = set()
         self.free_vars = set()
         self.written_vars = set()
 
+        self.defined_constraints = set()
+
     def scope_prologue(self, query: LMQLQuery):
         if query.prologue is None: return
         
-        DefinedVarsCollector(self.prologue_vars).visit(ast.parse(query.prologue))
+        DefinedVarsCollector(self.prologue_vars, self.defined_constraints).visit(ast.parse(query.prologue))
 
     def scope(self, query: LMQLQuery):
         self.distribution_vars = set([query.distribution.variable_name]) if query.distribution is not None else set()    
         self.defined_vars = set()
         self.prologue_vars = set()
 
         # collect set of global query template variables
         self.free_vars = set()
         self.written_vars = set()
 
         # collect defined vars in prologue
         self.scope_prologue(query)
 
         # collect defined vars in prompt
-        for p in query.prompt: self.visit(p)
+        for p in query.prompt: 
+            self.visit(p)
 
         # also collect variable reads from where clause
         if query.where is not None:
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.where)
         if query.from_ast is not None:
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.from_ast)
         if query.decode is not None:
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.decode)
         if query.distribution is not None:
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.distribution.values)
 
         # remove all defined and prologue vars from free vars
-        self.free_vars = self.free_vars - self.defined_vars - self.prologue_vars
+        self.free_vars = self.free_vars - self.defined_vars - self.prologue_vars - self.defined_constraints
 
         query.scope = self
 
     def visit_Expr(self, expr):
         if type(expr.value) is ast.Constant:
             self.scope_Constant(expr.value)
         else:
@@ -195,19 +210,33 @@
         self.defined_vars.add(node.name)
     
     def visit_AsyncFunctionDef(self, node: AsyncFunctionDef) -> Any:
         self.defined_vars.add(node.name)
 
     def visit_ClassDef(self, node: ClassDef) -> Any:
         self.defined_vars.add(node.name)
+        visit_potential_constraint_def(node, self)
 
     def visit_ImportFrom(self, node: ImportFrom) -> Any:
         for alias in node.names:
             self.defined_vars.add(alias.asname or alias.name)
 
+def visit_potential_constraint_def(node: ClassDef, scope: PromptScope):
+    for d in node.decorator_list:
+        # detect LMQLOp calls
+        if type(d) is ast.Call:
+            if type(d.func) is ast.Name:
+                if d.func.id == "LMQLOp" and len(d.args) == 1:
+                    if type(d.args[0]) is ast.Constant:
+                        scope.defined_constraints.add(d.args[0].value)
+                    elif type(d.args[0]) is ast.List:
+                        for e in d.args[0].elts:
+                            if type(e) is ast.Constant:
+                                scope.defined_constraints.add(e.value)
+
 def is_query_string_with_constraints(node: ast.BoolOp):
     if len(node.values) < 1:
         return False
     left_most_operand = node.values[0]
     return type(left_most_operand) is ast.Constant and type(left_most_operand.value) is str and isinstance(node.op, ast.And)
 
 class QueryStringTransformation(ast.NodeTransformer):
@@ -427,19 +456,19 @@
             
             assert False, "operator {} is not supported.".format(astunparse.unparse(expr))
         elif type(expr) is ast.Constant:
             return self.default_transform_node(expr, snf).strip()
         elif type(expr) is ast.ListComp:
             return self.default_transform_node(expr, snf).strip()
         elif type(expr) is ast.Call:
-            bn = get_builtin_name(expr.func)
-            if bn is not None:
+            constraint_ref = get_builtin_name(expr.func) or get_inner_constraint_ref(expr.func, self.scope)
+            if constraint_ref is not None:
                 args = [self.transform_node(a, snf) for a in expr.args]
                 args_list = ", ".join(args)
-                return f"{bn}([{args_list}])"
+                return f"{constraint_ref}([{args_list}])"
             if is_allowed_builtin_python_call(expr.func):
                 return self.default_transform_node(expr, snf).strip()
         elif type(expr) is ast.List:
             return self.default_transform_node(expr, snf).strip()
 
         print(f"compiler warning: expressions of type {type(expr)} are not explicitly supported: '{astunparse.unparse(expr).strip()}'")
         return snf.add(self.default_transform_node(expr, snf))
@@ -506,25 +535,42 @@
 
 def is_allowed_builtin_python_call(node):
     if type(node) is not ast.Name:
         return False
     allowed_builtin_functions = set(["set", "all"])
     return node.id in allowed_builtin_functions
 
+def get_inner_constraint_ref(node, scope: PromptScope):
+    if type(node) is str:
+        n = node
+    else:
+        if type(node) is not ast.Name:
+            return None
+        n = node.id
+    
+    if n in scope.defined_constraints:
+        return OPS_NAMESPACE + ".lmql_operation_registry['" + n + "']"
+    
+    return None
+
 def get_builtin_name(node, plain_python=False):
     if type(node) is str:
         n = node
     else:
         if type(node) is not ast.Name:
             return None
         n = node.id
     
     if n in lmql_operation_registry.keys():
-        return OPS_NAMESPACE + "." + lmql_operation_registry[n]
-    
+        name = lmql_operation_registry[n]
+        if type(name) is type:
+            return OPS_NAMESPACE + ".lmql_operation_registry['" + n + "']"
+        else:
+            return OPS_NAMESPACE + "." + name
+
     return None
 
 def is_type_constraint(expr: ast.Expr):
     if not type(expr.left) is ast.Call:
         return False
     if not type(expr.left.func) is ast.Name:
         return False
```

### Comparing `lmql-0.0.6.5/src/lmql/language/fragment_parser.py` & `lmql-0.0.6.6/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/language/qstrings.py` & `lmql-0.0.6.6/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/language/validator.py` & `lmql-0.0.6.6/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/README.md` & `lmql-0.0.6.6/src/lmql/models/lmtp/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/backends/__main__.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/backends/__main__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/backends/llama_cpp_model.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/backends/llama_cpp_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 class LlamaCppModel(LMTPModel):
     def __init__(self, model_identifier, **kwargs):
         self.model_identifier = model_identifier
         self.kwargs = kwargs
 
         self.max_batch_size = 1
 
-        print("[Loading llama.cpp model from", self.model_identifier, "]", flush=True)
+        print("[Loading llama.cpp model from", self.model_identifier, " with ", kwargs, "]", flush=True)
         if not "verbose" in kwargs.keys():
             kwargs["verbose"] = False
-        self.llm = Llama(model_path=model_identifier.strip("llama.cpp:"), **kwargs)
+        self.llm = Llama(model_path=model_identifier[len("llama.cpp:"):], **kwargs)
 
     def eos_token_id(self):
         return 2
 
     def score(self, input_ids, attention_mask, **model_kwargs):
         import time
         # s = time.time()
@@ -63,14 +63,16 @@
 
         logits_processor = self.logits_processors(bias_tensor) if bias_tensor is not None else None
 
         for i, token in zip(range(max_new_tokens), self.llm.generate(input_ids, max_new_tokens, 
                                                             temp=temperature,
                                                             stopping_criteria=llama_streamer, 
                                                             logits_processor=logits_processor)):
+            assert i + len(input_ids) < self.llm.n_ctx(), "The requested number of tokens exceeds the llama.cpp model's context size. Please specify a higher n_ctx value."
+            
             if i > 0:
                 streamer(sq_ar.reshape(1, *sq_ar.shape), ts_ar.reshape(-1, 1, *ts_ar.shape[1:]))
             sequence += [token]
             sq_ar = np.array(sequence)
             ts_ar = np.stack(token_scores, axis=0)
 
         ts_ar = np.stack(token_scores, axis=0)
```

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/backends/lmtp_model.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/backends/lmtp_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/backends/random_model.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/backends/random_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/backends/transformers_model.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/backends/transformers_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from transformers import AutoModelForCausalLM
 from typing import Tuple
 import torch
 from lmql.models.lmtp.backends.lmtp_model import LMTPModel, LMTPModelResult, TokenStreamer
 import random
 
 class TransformersLLM(LMTPModel):
     def __init__(self, model_identifier, **kwargs):
         self.model_identifier = model_identifier
         self.model_args = kwargs
 
-        print("[Loading", self.model_identifier, "with", f"AutoModelForCausalLM.from_pretrained({self.model_identifier}, {str(self.model_args)[1:-1]})]", flush=True)
-        
-        self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, **kwargs)
+        if self.model_args.pop("loader", None) == "auto-gptq":
+            from auto_gptq import AutoGPTQForCausalLM
+            print("[Loading", self.model_identifier, "with", f"AutoGPTQForCausalLM.from_quantized({self.model_identifier}, {str(self.model_args)[1:-1]})]", flush=True)
+            self.model = AutoGPTQForCausalLM.from_quantized(self.model_identifier, **self.model_args)
+        else:
+            from transformers import AutoModelForCausalLM
+            print("[Loading", self.model_identifier, "with", f"AutoModelForCausalLM.from_pretrained({self.model_identifier}, {str(self.model_args)[1:-1]})]", flush=True)
+            self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, **self.model_args)
         
         print("[", self.model_identifier, " ready on device ", self.model.device, 
         flush=True, sep="", end="]\n")
 
         self.max_batch_size = kwargs.get("batch_size", 8)
 
     @property
```

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_async.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_async.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_client.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_dcmodel.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_dcmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,15 +443,16 @@
 
                 if this.inprocess:
                     lmtp_server_kwargs = this.kwargs
                     inprocess_client_constructor = this.inprocess_client_constructor_factory
                 else:
                     lmtp_server_kwargs = None
 
-                return LMTPModel(self, self.get_tokenizer(), inprocess=this.inprocess, endpoint=this.endpoint, lmtp_server_kwargs=lmtp_server_kwargs, inprocess_client_constructor=inprocess_client_constructor, **self.decoder_args)
+                return LMTPModel(self, self.get_tokenizer(), inprocess=this.inprocess, endpoint=this.endpoint, lmtp_server_kwargs=lmtp_server_kwargs, 
+                                 inprocess_client_constructor=inprocess_client_constructor, **self.decoder_args)
 
             async def tokenize(self, text):
                 return self.get_tokenizer().tokenize(text, asbytes=True)
             
             async def detokenize(self, input_ids):
                 return self.get_tokenizer().decode(input_ids)
```

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_inference_server.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_inference_server.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_multiprocessing.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_scheduler.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,19 @@
     def put(self, call: GenerateCall):
         self.queue.put(call)
 
     def batches(self, max_batch_size=8):
         start = time.time()
         calls = []
         # get as many calls from the queue as possible within 0.1 seconds
+        first = True
         while time.time() - start < 0.1:
             try:
-                calls.append(self.queue.get_nowait())
+                calls.append(self.queue.get(block=first, timeout=0.1))
+                first = False
             except QueueEmpty:
                 break
         # group calls into batches
         batches_by_mode = {}
         for c in calls:
             mode = c.generation_mode()
             batches_by_mode.setdefault(mode, []).append(c)
@@ -270,15 +272,14 @@
 
                     result = model.generate(**kwargs, streamer=streamer)
                     streamer.log_token(result.sequences, result.scores, last=True)
             except Exception as e:
                 print("[Error during generate()]", e, flush=True)
                 for c in batch:
                     c.error("failed to generate tokens '" + str(e) + "'")
-                raise e
 
     @staticmethod
     def instance(model_identifier, model_args, user, only_existing=False, sync=False):
         identifier = (model_identifier, pickle.dumps(model_args).hex())
 
         if identifier not in Scheduler._instances:
             if only_existing:
```

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_serve.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_serve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
 Command Line Interface for lmtp_inference_server.py.
 """
 
 from .lmtp_inference_server import *
 from .utils import rename_model_args
 
-def serve(model_name, host="localhost", port=8080, cuda=False, dtype=None, static=False, **kwargs):
+def serve(model_name, host="localhost", port=8080, cuda=False, dtype=None, static=False, loader=None, **kwargs):
     """
     Serves the provided model as an LMTP/LMQL inference endpoint.
 
     Args:
         model_name (str): The model to load or 'auto' if any model should automatically be loaded on client request.
         host (str, optional): The host to serve the model on. Defaults to "localhost".
         port (int, optional): The port to serve the model on. Defaults to 8080.
         single_thread (bool, optional): If set, the model and the inference server will run in the same thread. Defaults to False. This can lead to increased latency when processing multiple requests, but may be required depending on model implementation.
         cuda (bool, optional): If set, the model will be loaded on the GPU. Defaults to False.
         dtype (str, optional): What format to load the model weights. Options: 'float16' (not available on all models), '8bit' (requires bitsandbytes). Defaults to None.
         static (bool, optional): If set, the model cannot be switched on client request but remains fixed to the model specified in the model argument. Defaults to False.
+        loader (str, optional): If set, the model will be loaded using a library other than transformers. This is useful when loading quantized models in formats that are not yet supported by Transformers (like GTPQ). Defaults to None.
         **kwargs: Any other argument will be passed as a keyword argument to the AutoModelForCausalLM.from_pretrained function.
 
     """
     return lmtp_serve_main({
         "model": model_name,
         "host": host,
         "port": port,
         "cuda": cuda,
         "dtype": dtype,
         "static": static,
+        "loader": loader,
         **kwargs
     })
 
 def lmtp_serve_main(model_args):
     """
     CLI for starting an LMTP server with a given HuggingFace 'transformers' model.
     """
@@ -91,14 +93,18 @@
   -h, --help     show this help message and exit
   --port PORT
   --host HOST
   --cuda
   --static      If set, the model cannot be switched on client request but remains fixed to the model specified in the model argument.
   --dtype DTYPE  What format to load the model weights. Options: 'float16'
                  (not available on all models), '8bit' (requires bitsandbytes)
+  --loader OPT  If set, the model will be loaded using the corresponding option. Useful for loading quantized modules in formats not
+                supported by the transformers library, like GPTQ. Available options:
+                * auto-gptq (loads GPTQ based quantized models with auto-gptq. Consider adding `--use_safetensors true` if the model is
+                             distributed in the safetensor format)
   --[*] VALUE   Any other argument will be passed as a keyword argument to the AutoModelForCausalLM.from_pretrained function.
     """
 
     for arg in args:
         if arg == "-h" or arg == "--help":
             print(help_text)
             sys.exit(0)
```

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_threading.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/lmtp_threading.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/lmtp/utils.py` & `lmql-0.0.6.6/src/lmql/models/lmtp/utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/models/model.py` & `lmql-0.0.6.6/src/lmql/models/model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ops/follow_map.py` & `lmql-0.0.6.6/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ops/ops.py` & `lmql-0.0.6.6/src/lmql/ops/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,26 @@
 from lmql.ops.follow_map import *
 
 lmql_operation_registry = {}
 
 # @LMQLOp('function_name') decorator
 def LMQLOp(name):
     def class_transformer(cls):
+        # get full import path of cls
+        cls_name = cls.__name__
+        
+        # if not in lmql.ops.ops, then use direct cls reference
+        if cls.__module__ != "lmql.ops.ops":
+            cls_name = cls
+
         if type(name) is list:
             for n in name:
-                lmql_operation_registry[n] = f"{cls.__name__}"
+                lmql_operation_registry[n] = cls_name
             return cls
-        lmql_operation_registry[name] = f"{cls.__name__}"
+        lmql_operation_registry[name] = cls_name
         return cls
     return class_transformer
 
 class Node:
     def __init__(self, predecessors):
         assert type(predecessors) is list, "Predecessors must be a list, not {}".format(type(predecessors))
         self.predecessors = predecessors
```

### Comparing `lmql-0.0.6.5/src/lmql/ops/token_set.py` & `lmql-0.0.6.6/src/lmql/ops/token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/output/http.py` & `lmql-0.0.6.6/src/lmql/output/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/output/sse.py` & `lmql-0.0.6.6/src/lmql/output/sse.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/output/ws.py` & `lmql-0.0.6.6/src/lmql/output/ws.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.6.6/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.6.6/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,14 +686,16 @@
                         break
                     except Exception as e:
                         if type(e) is AssertionError:
                             raise e
                         self.stats.errors += 1
                         retries -= 1            
                         print("OpenAI:", str(e), '"' + str(type(e)) + '"', flush=True)
+                        # do not retry if the error is definitive (API configuration error)
+                        if "api.env" in str(e): raise e
                         if kwargs.get("api_config", {}).get("errors", None) == "raise":
                             raise e
                         await asyncio.sleep(0.5)
                         if retries <= 0 or self.is_definitive_error(e):
                             raise e
                         if type(e) is TimeoutError or type(e) is OpenAIRateLimitError:
                             t = (2.0 * random.random()) ** (self.maximum_retries - retries)
```

### Comparing `lmql-0.0.6.5/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.6.6/src/lmql/runtime/bopenai/openai_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,16 +127,16 @@
             endpoint += f"?api-version={api_version}"
 
         headers = {
             "Content-Type": "application/json",
             "api-key": api_key,
         }
 
-        if "verbose" in api_config and api_config["verbose"] or os.environ.get("OPENAI_VERBOSE", "0") == "1":
-            print(f"Using Azure API endpoint: {endpoint}", is_chat)
+        if api_config.get("verbose", False) or os.environ.get("OPENAI_VERBOSE", "0") == "1":
+            print(f"Using Azure API endpoint: {endpoint}", is_chat, flush=True)
 
         return endpoint, headers
 
     return None
 
 def get_endpoint_and_headers(kwargs):
     model = kwargs["model"]
```

### Comparing `lmql-0.0.6.5/src/lmql/runtime/caching.py` & `lmql-0.0.6.6/src/lmql/runtime/caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.6.6/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.6.6/src/lmql/runtime/dclib/decoders.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/interpreter.py` & `lmql-0.0.6.6/src/lmql/runtime/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,17 @@
             self.model = model_name
             self.model_identifier = model_name
         elif type(self.model_identifier) is not str:
             self.model_identifier = self.model.model_identifier
 
         client = LMQLModelRegistry.get(self.model, **model_args)
 
+        if callable(client):
+            client = client()
+
         # setup the VocabularyMatcher to use the concrete vocabulary of the model
         VocabularyMatcher.init(client.get_tokenizer())
         
         # for OpenAI models we optimize for compact logit masks
         if self.model_identifier.startswith("openai/"):
             self.prefers_compact_mask = True
```

### Comparing `lmql-0.0.6.5/src/lmql/runtime/langchain.py` & `lmql-0.0.6.6/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.6.6/src/lmql/runtime/lmql_runtime.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,14 +92,31 @@
     @property
     def output_keys(self) -> List[str]:
         return self.output_variables
 
     def force_model(self, model):
         self.model = model
 
+    def try_bind_positional_to_kwargs(self, signature, *args, **query_kwargs):
+        """
+        Best-effort attempt to bind positional arguments to keyword arguments in order of self.args. 
+
+        Only enabled for lmql.F for now, may have unexpected effects depending on the order query
+        arguments as determined by the compiler.
+        """
+        # only bind if kwargs are empty and no signature is provided (lmql.F or lmql.run)
+        if len(signature.parameters) != 0 or len(self.args) != len(args):
+            return
+        kwargs = {**{k:v for k,v in zip(self.args, args)}, **query_kwargs}
+
+        return inspect.BoundArguments(
+            signature=inspect.Signature(parameters=[inspect.Parameter(name=k, kind=inspect.Parameter.POSITIONAL_OR_KEYWORD) for k in self.args]),
+            arguments=kwargs
+        )
+
     def make_kwargs(self, *args, **kwargs):
         """
         Binds args and kwargs to the function signature and returns a dict of all user-defined kwargs.
 
         Resolves additional captured variables using the surrounding function context.
         """
         assert self.function_context is not None, "Cannot call @lmql.query function without context."
@@ -118,19 +135,27 @@
             if param.default is not inspect.Parameter.empty and name in args_of_query:
                 compiled_query_args[name] = param.default
 
         # bind args and kwargs to signature
         try:
             signature = signature.bind(*args, **query_kwargs)
         except TypeError as e:
-            if len(e.args) == 1 and e.args[0].startswith("missing "):
-                e.args = (f"Call to @lmql.query function is " + e.args[0] + "." + f" Expecting {signature}, but got positional args {args} and {kwargs}.",)
-            elif len(e.args) == 1:
-                e.args = (e.args[0] + "." + f" Expecting {signature}, but got positional args {args} and {kwargs}.",)
-            raise e
+            if "too many positional arguments" in str(e):
+                # this is different from Python behavior, but we allow it for lmql.F and lmql.run
+                pos_as_kw = self.try_bind_positional_to_kwargs(signature, *args, **kwargs)
+                if pos_as_kw is not None:
+                    signature = pos_as_kw
+                else:
+                    raise e
+            else:    
+                if len(e.args) == 1 and e.args[0].startswith("missing "):
+                    e.args = (f"Call to @lmql.query function is " + e.args[0] + "." + f" Expecting {signature}, but got positional args {args} and {kwargs}.",)
+                elif len(e.args) == 1:
+                    e.args = (e.args[0] + "." + f" Expecting {signature}, but got positional args {args} and {kwargs}.",)
+                raise e
         
         # special case, if signature is empty (no input variables provided)
         if len(signature.arguments) == 0:
             # bind kwargs dynamically in compiled_query_args
             for k,v in kwargs.items():
                 if k in args_of_query:
                     # compiled_query_args[k] = v
```

### Comparing `lmql-0.0.6.5/src/lmql/runtime/loop.py` & `lmql-0.0.6.6/src/lmql/runtime/loop.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/maiohttp.py` & `lmql-0.0.6.6/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/masks.py` & `lmql-0.0.6.6/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/model_registry.py` & `lmql-0.0.6.6/src/lmql/runtime/model_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             model = LMQLModelRegistry.default_model
 
         if model in model_name_aliases:
             model = model_name_aliases[model]
 
         if type(model) is LMQLModel:
             if model.model is not None:
-                return model
+                return model.model
             else:
                 kwargs = {**model.kwargs, **kwargs}
                 model = model.model_identifier
 
         client = LMQLModelRegistry.clients.get(model, None)
 
         if client is None:
```

### Comparing `lmql-0.0.6.5/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.6.6/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/openai_integration.py` & `lmql-0.0.6.6/src/lmql/runtime/openai_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,16 +978,14 @@
     def reset_stats(self):
         openai.AsyncConfiguration.get_stats().reset()
 
     def cost_estimate(self, model):
         return openai.AsyncConfiguration.get_stats().cost_estimate(model)
 
 def openai_model(model_identifier, endpoint=None, mock=False, **kwargs):
-    # make sure openai org and secret are available
-    if not mock: from lmql.runtime.openai_secret import openai_secret, openai_org
     class OpenAIModel:
         def __init__(self) -> None:
             self.model_identifier = model_identifier
             self.served_model = None
             self._tokenizer = None
 
             self.decoder_args = {}
```

### Comparing `lmql-0.0.6.5/src/lmql/runtime/openai_secret.py` & `lmql-0.0.6.6/src/lmql/runtime/openai_secret.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,25 @@
         openai_org = str(js.get_openai_organization())
         
         return openai_secret, openai_org
     elif "LMQL_OPENAI_SECRET" in os.environ and "LMQL_OPENAI_ORG" in os.environ:
         return os.environ["LMQL_OPENAI_SECRET"], os.environ["LMQL_OPENAI_ORG"]
     elif "OPENAI_API_KEY" in os.environ:
         return os.environ["OPENAI_API_KEY"], ""
+    elif any(k.startswith("OPENAI_API_KEY") for k in os.environ):
+        return os.environ.get("OPENAI_API_KEY", None), ""
     else:
         search_paths = [
             os.path.join(ROOT_DIR, "api.env"),
             os.path.join(os.getcwd(), "api.env"),
             os.path.join(os.getenv("HOME"), ".lmql", "api.env")
         ]
         
         if not any(os.path.exists(p) for p in search_paths):
-            m = """api.env not found in any of the following locations:\n\n{}\n\n To use OpenAI models you need to create an api.env file with the following contents:
+            m = """To use openai/<models> you have to set environment variable OPENAI_API_KEY or provide an api.env file in one of the following locations:\n\n{}\n\n To use OpenAI models you need to create an api.env file with the following contents:
         openai-secret: <your openai secret>
         openai-org: <your openai org>
         
 Alternatively, you may just define the environment variable OPENAI_API_KEY=sk-...
         """.format("\n".join(" - " + p for p in search_paths))
             raise FileNotFoundError(m)
```

### Comparing `lmql-0.0.6.5/src/lmql/runtime/output_writer.py` & `lmql-0.0.6.6/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.6.6/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/program_state.py` & `lmql-0.0.6.6/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/stats.py` & `lmql-0.0.6.6/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/token_distribution.py` & `lmql-0.0.6.6/src/lmql/runtime/token_distribution.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/tokenizer.py` & `lmql-0.0.6.6/src/lmql/runtime/tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/tokenizers/hf_tokenizer.py` & `lmql-0.0.6.6/src/lmql/runtime/tokenizers/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/tokenizers/pure_python_tokenizer.py` & `lmql-0.0.6.6/src/lmql/runtime/tokenizers/pure_python_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py` & `lmql-0.0.6.6/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/all.py` & `lmql-0.0.6.6/src/lmql/tests/all.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.6.6/src/lmql/tests/expr_test_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/fin_and.py` & `lmql-0.0.6.6/src/lmql/tests/fin_and.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/stops_at.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.0.6.6/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/queryargs/test_args.py` & `lmql-0.0.6.6/src/lmql/tests/queryargs/test_args.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_query_str.py` & `lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_query_str.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_run.py` & `lmql-0.0.6.6/src/lmql/tests/queryargs/test_args_run.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/queryargs/test_sync.py` & `lmql-0.0.6.6/src/lmql/tests/queryargs/test_sync.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/queryargs/test_var_errors.py` & `lmql-0.0.6.6/src/lmql/tests/queryargs/test_var_errors.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.6.6/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/tail_token_set.py` & `lmql-0.0.6.6/src/lmql/tests/tail_token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_back2back_caching.py` & `lmql-0.0.6.6/src/lmql/tests/test_back2back_caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_eq.py` & `lmql-0.0.6.6/src/lmql/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_escaping.py` & `lmql-0.0.6.6/src/lmql/tests/test_escaping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_local_model_python.py` & `lmql-0.0.6.6/src/lmql/tests/test_local_model_python.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,9 +40,16 @@
         """Hello[WHO]"""
     from
         m2
     where
         STOPS_AT(WHO, "\n") and len(TOKENS(WHO)) < 10
     '''
 
+@lmql.query(model=m2)
+def test_model_reference_cuda_decorator():
+    '''lmql
+    "Hello[WHO]" where STOPS_AT(WHO, "\n") and len(TOKENS(WHO)) < 10
+    '''
+
+
 if __name__ == "__main__":
     run_all_tests(locals())
```

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_minimal_syntax.py` & `lmql-0.0.6.6/src/lmql/tests/test_minimal_syntax.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_multibyte_characters.py` & `lmql-0.0.6.6/src/lmql/tests/test_multibyte_characters.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_multibyte_local_models.py` & `lmql-0.0.6.6/src/lmql/tests/test_multibyte_local_models.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_qstrings.py` & `lmql-0.0.6.6/src/lmql/tests/test_qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_sample_queries.py` & `lmql-0.0.6.6/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_scoping.py` & `lmql-0.0.6.6/src/lmql/tests/test_scoping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/test_stopping.py` & `lmql-0.0.6.6/src/lmql/tests/test_stopping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/tests/tiktoken_tsets.py` & `lmql-0.0.6.6/src/lmql/tests/tiktoken_tsets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/live/live.js` & `lmql-0.0.6.6/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/live/live.py` & `lmql-0.0.6.6/src/lmql/ui/live/live.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/live/livelib.py` & `lmql-0.0.6.6/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/live/yarn.lock` & `lmql-0.0.6.6/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/README.md` & `lmql-0.0.6.6/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/package.json` & `lmql-0.0.6.6/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.6.6/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/index.html` & `lmql-0.0.6.6/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.6.6/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/json-template.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/json-template.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.6.6/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.6.6/src/lmql/ui/playground/src/App.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.6.6/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.6.6/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/State.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.6.6/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.6.6/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.6.6/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.6.6/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/index.css` & `lmql-0.0.6.6/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.6.6/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/queries.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.6.6/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.6.6/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.6.6/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.6.6/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.6.6/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.6.6/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.6.6/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.6.6/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/package.json` & `lmql-0.0.6.6/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.6.6/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/utils/docstring_parser.py` & `lmql-0.0.6.6/src/lmql/utils/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/utils/graph.py` & `lmql-0.0.6.6/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql/utils/nputil.py` & `lmql-0.0.6.6/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.5/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.6.6/src/lmql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.5
+Version: 0.0.6.6
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
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.5 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.6 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6.5/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.6.6/src/lmql.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 src/lmql/tests/expr_test_utils.py
 src/lmql/tests/fin_and.py
 src/lmql/tests/tail_token_set.py
 src/lmql/tests/test_back2back_caching.py
 src/lmql/tests/test_beam_in.py
 src/lmql/tests/test_eq.py
 src/lmql/tests/test_escaping.py
+src/lmql/tests/test_f.py
 src/lmql/tests/test_local_model_python.py
 src/lmql/tests/test_minimal_syntax.py
 src/lmql/tests/test_multibyte_characters.py
 src/lmql/tests/test_multibyte_local_models.py
 src/lmql/tests/test_orop.py
 src/lmql/tests/test_qstrings.py
 src/lmql/tests/test_query_args.py
```

### Comparing `lmql-0.0.6.5/src/lmql.svg` & `lmql-0.0.6.6/src/lmql.svg`

 * *Files identical despite different names*

