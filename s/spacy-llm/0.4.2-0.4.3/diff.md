# Comparing `tmp/spacy-llm-0.4.2.tar.gz` & `tmp/spacy-llm-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.4.2.tar", last modified: Fri Jul 14 09:43:35 2023, max compression
+gzip compressed data, was "spacy-llm-0.4.3.tar", last modified: Tue Jul 25 13:55:56 2023, max compression
```

## Comparing `spacy-llm-0.4.2.tar` & `spacy-llm-0.4.3.tar`

### file list

```diff
@@ -1,170 +1,172 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)   101733 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      918 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1827 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10379 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/hf/
--rw-r--r--   0 vsts      (1001) docker     (122)      264 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4886 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2439 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2814 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3332 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4816 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/langchain/
--rw-r--r--   0 vsts      (1001) docker     (122)      227 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/langchain/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4540 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/langchain/model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/
--rw-r--r--   0 vsts      (1001) docker     (122)      476 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4627 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10902 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5971 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/base.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3722 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/models/rest/noop/
--rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/noop/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      865 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/noop/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)      351 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/noop/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/models/rest/openai/
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6093 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/openai/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19421 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/openai/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11251 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2940 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4725 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8738 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9184 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4807 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/sentiment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6944 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/span.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9497 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5720 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/summarization.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/lemma.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/sentiment.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/summarization.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)    16409 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4042 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/util/serialization.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1350 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2323 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3068 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1618 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1508 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1865 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3299 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2085 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8914 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.json
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/rel.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/sentiment.json
--rw-r--r--   0 vsts      (1001) docker     (122)      186 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/sentiment.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      174 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/sentiment.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     3126 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.json
--rw-r--r--   0 vsts      (1001) docker     (122)     3093 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)     3089 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_binary.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_binary.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/lemma.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/ner.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/sentiment.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/summarization.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/textcat.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24355 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6774 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6983 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_sentiment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17549 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13777 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_summarization.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23930 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9200 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1694 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9252 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     5129 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3361 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)   101733 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      918 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1827 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.096675 spacy-llm-0.4.3/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10379 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.096675 spacy-llm-0.4.3/spacy_llm/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.096675 spacy-llm-0.4.3/spacy_llm/models/hf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      311 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4886 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2439 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3012 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/hf/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2654 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/hf/llama2.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3332 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4816 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.096675 spacy-llm-0.4.3/spacy_llm/models/langchain/
+-rw-r--r--   0 vsts      (1001) docker     (122)      227 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/langchain/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4540 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/langchain/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/models/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/models/rest/anthropic/
+-rw-r--r--   0 vsts      (1001) docker     (122)      476 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/anthropic/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4587 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/anthropic/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12656 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/anthropic/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5971 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/base.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/models/rest/cohere/
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/cohere/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3722 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/cohere/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/cohere/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/models/rest/noop/
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/noop/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      865 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/noop/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      351 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/noop/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/models/rest/openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6093 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/openai/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19421 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/models/rest/openai/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11251 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2940 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.100674 spacy-llm-0.4.3/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4725 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8738 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9184 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4807 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6944 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/span.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9497 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5720 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/summarization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.104675 spacy-llm-0.4.3/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/lemma.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/sentiment.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/summarization.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)    16409 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.104675 spacy-llm-0.4.3/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4042 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tasks/util/serialization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.104675 spacy-llm-0.4.3/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1350 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.104675 spacy-llm-0.4.3/spacy_llm/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2323 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3068 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1618 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1508 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1510 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_llama2.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1865 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3299 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2085 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/models/test_stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.104675 spacy-llm-0.4.3/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8914 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.108675 spacy-llm-0.4.3/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.108675 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/lemma.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/lemma.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/lemma.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/ner.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/ner.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/ner.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/rel.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/sentiment.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      186 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/sentiment.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      174 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/sentiment.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3126 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/summarization.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     3093 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/summarization.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)     3089 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/summarization.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_binary.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_binary.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.108675 spacy-llm-0.4.3/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/templates/lemma.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/templates/ner.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/templates/sentiment.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/templates/summarization.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/templates/textcat.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24355 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6774 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6983 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/test_sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17549 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13777 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/test_summarization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23930 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9200 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1694 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9252 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.096675 spacy-llm-0.4.3/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-25 13:55:56.000000 spacy-llm-0.4.3/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     5197 2023-07-25 13:55:56.000000 spacy-llm-0.4.3/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-25 13:55:56.000000 spacy-llm-0.4.3/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-07-25 13:55:56.000000 spacy-llm-0.4.3/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-25 13:55:55.000000 spacy-llm-0.4.3/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-07-25 13:55:56.000000 spacy-llm-0.4.3/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-07-25 13:55:56.000000 spacy-llm-0.4.3/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.108675 spacy-llm-0.4.3/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3361 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-25 13:55:56.112675 spacy-llm-0.4.3/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-07-25 13:55:39.000000 spacy-llm-0.4.3/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.4.2/LICENSE` & `spacy-llm-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/PKG-INFO` & `spacy-llm-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.4.2
+Version: 0.4.3
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -169,15 +169,15 @@
     "llm",
     config={
         "task": {
             "@llm_tasks": "spacy.NER.v2",
             "labels": ["PERSON", "ORGANISATION", "LOCATION"]
         },
         "model": {
-            "@llm_models": "spacy.gpt-3.5.v1",
+            "@llm_models": "spacy.GPT-3-5.v1",
         },
     },
 )
 nlp.initialize()
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.2 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.3 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -99,15 +99,15 @@
 (https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by
 setting the environmental variable `HF_HOME`. Also, you can upgrade the model
 to be `"databricks/dolly-v2-12b"` for better performance. ### Example 3: Create
 the component directly in Python The `llm` component behaves as any other spaCy
 component does, so adding it to an existing pipeline follows the same pattern:
 ```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config=
 { "task": { "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
-"LOCATION"] }, "model": { "@llm_models": "spacy.gpt-3.5.v1", }, }, )
+"LOCATION"] }, "model": { "@llm_models": "spacy.GPT-3-5.v1", }, }, )
 nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
 usage of resources, typically you would use [`nlp.pipe(docs)`](https://
 spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
 single document. ### Example 4: Implement your own custom task To write a
 [`task`](#tasks), you need to implement two functions: `generate_prompts` that
 takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
```

### Comparing `spacy-llm-0.4.2/README.md` & `spacy-llm-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     "llm",
     config={
         "task": {
             "@llm_tasks": "spacy.NER.v2",
             "labels": ["PERSON", "ORGANISATION", "LOCATION"]
         },
         "model": {
-            "@llm_models": "spacy.gpt-3.5.v1",
+            "@llm_models": "spacy.GPT-3-5.v1",
         },
     },
 )
 nlp.initialize()
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
```

#### html2text {}

```diff
@@ -83,15 +83,15 @@
 (https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by
 setting the environmental variable `HF_HOME`. Also, you can upgrade the model
 to be `"databricks/dolly-v2-12b"` for better performance. ### Example 3: Create
 the component directly in Python The `llm` component behaves as any other spaCy
 component does, so adding it to an existing pipeline follows the same pattern:
 ```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config=
 { "task": { "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
-"LOCATION"] }, "model": { "@llm_models": "spacy.gpt-3.5.v1", }, }, )
+"LOCATION"] }, "model": { "@llm_models": "spacy.GPT-3-5.v1", }, }, )
 nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
 usage of resources, typically you would use [`nlp.pipe(docs)`](https://
 spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
 single document. ### Example 4: Implement your own custom task To write a
 [`task`](#tasks), you need to implement two functions: `generate_prompts` that
 takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
```

### Comparing `spacy-llm-0.4.2/pyproject.toml` & `spacy-llm-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/setup.cfg` & `spacy-llm-0.4.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.4.2
+version = 0.4.3
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `spacy-llm-0.4.2/spacy_llm/cache.py` & `spacy-llm-0.4.3/spacy_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/compat.py` & `spacy-llm-0.4.3/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/hf/base.py` & `spacy-llm-0.4.3/spacy_llm/models/hf/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/hf/dolly.py` & `spacy-llm-0.4.3/spacy_llm/models/hf/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/hf/falcon.py` & `spacy-llm-0.4.3/spacy_llm/models/hf/falcon.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,24 @@
         name: MODEL_NAMES,
         config_init: Optional[Dict[str, Any]],
         config_run: Optional[Dict[str, Any]],
     ):
         self._tokenizer: Optional["transformers.AutoTokenizer"] = None
         self._device: Optional[str] = None
         super().__init__(name=name, config_init=config_init, config_run=config_run)
+
         assert isinstance(self._tokenizer, transformers.PreTrainedTokenizerBase)
-        self._config_run["eos_token_id"] = self._tokenizer.eos_token_id
+        self._config_run["pad_token_id"] = self._tokenizer.pad_token_id
+
+        # Instantiate GenerationConfig object from config dict.
+        self._hf_config_run = transformers.GenerationConfig.from_pretrained(
+            self._name, **self._config_run
+        )
+        # To avoid deprecation warning regarding usage of `max_length`.
+        self._hf_config_run.max_new_tokens = self._hf_config_run.max_length
 
     def init_model(self) -> Any:
         self._tokenizer = transformers.AutoTokenizer.from_pretrained(self._name)
         return transformers.pipeline(
             "text-generation",
             model=self._name,
             tokenizer=self._tokenizer,
@@ -35,32 +43,27 @@
 
     @property
     def hf_account(self) -> str:
         return "tiiuae"
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:  # type: ignore[override]
         return [
-            self._model(pr, **self._config_run)[0]["generated_text"] for pr in prompts
+            self._model(pr, generation_config=self._hf_config_run)[0]["generated_text"]
+            for pr in prompts
         ]
 
     @staticmethod
     def compile_default_configs() -> Tuple[Dict[str, Any], Dict[str, Any]]:
         default_cfg_init, default_cfg_run = HuggingFace.compile_default_configs()
         return (
             {
                 **default_cfg_init,
                 "trust_remote_code": True,
             },
-            {
-                **default_cfg_run,
-                "max_length": 200,
-                "do_sample": True,
-                "top_k": 10,
-                "num_return_sequences": 1,
-            },
+            default_cfg_run,
         )
 
 
 @registry.llm_models("spacy.Falcon.v1")
 def falcon_hf(
     name: Falcon.MODEL_NAMES,
     config_init: Optional[Dict[str, Any]] = SimpleFrozenDict(),
```

### Comparing `spacy-llm-0.4.2/spacy_llm/models/hf/openllama.py` & `spacy-llm-0.4.3/spacy_llm/models/hf/openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/hf/stablelm.py` & `spacy-llm-0.4.3/spacy_llm/models/hf/stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/langchain/model.py` & `spacy-llm-0.4.3/spacy_llm/models/langchain/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/model.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/anthropic/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Sized, Tuple
 
 import requests  # type: ignore[import]
 import srsly  # type: ignore[import]
 from requests import HTTPError
 
-from ....compat import Literal
 from ..base import REST
 
 
 class Endpoints(str, Enum):
     COMPLETIONS = "https://api.anthropic.com/v1/complete"
 
 
@@ -21,18 +20,14 @@
     """
 
     HUMAN = "\n\nHuman:"
     ASST = "\n\nAssistant:"
 
 
 class Anthropic(REST):
-    MODEL_NAMES = {
-        "claude-1": Literal["claude-1", "claude-1-100k"],
-    }
-
     @property
     def credentials(self) -> Dict[str, str]:
         # Fetch and check the key, set up headers
         api_key = os.getenv("ANTHROPIC_API_KEY")
         if api_key is None:
             warnings.warn(
                 "Could not find the API key to access the Anthropic Claude API. Ensure you have an API key "
@@ -112,14 +107,17 @@
         assert len(api_responses) == len(prompts)
         return api_responses
 
     @classmethod
     def get_model_names(cls) -> Tuple[str, ...]:
         return (
             # claude-1
+            "claude-2",
+            "claude-2-100k",
+            # claude-1
             "claude-1",
             "claude-1-100k",
             # claude-instant-1
             "claude-instant-1",
             "claude-instant-1-100k",
             # claude-instant-1.1
             "claude-instant-1.1",
```

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/registry.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/anthropic/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,48 @@
 from spacy.util import SimpleFrozenDict
 
 from ....compat import Literal
 from ....registry import registry
 from .model import Anthropic, Endpoints
 
 
+@registry.llm_models("spacy.Claude-2.v1")
+def anthropic_claude_2(
+    config: Dict[Any, Any] = SimpleFrozenDict(),
+    name: Literal["claude-2", "claude-2-100k"] = "claude-2",  # noqa: F722
+    strict: bool = Anthropic.DEFAULT_STRICT,
+    max_tries: int = Anthropic.DEFAULT_MAX_TRIES,
+    interval: float = Anthropic.DEFAULT_INTERVAL,
+    max_request_time: float = Anthropic.DEFAULT_MAX_REQUEST_TIME,
+) -> Callable[[Iterable[str]], Iterable[str]]:
+    """Returns Anthropic instance for 'claude-2' model using REST to prompt API.
+    config (Dict[Any, Any]): LLM config arguments passed on to the initialization of the model instance.
+    name (Literal["claude-2", "claude-2-100k"]): Model to use.
+    strict (bool): If True, ValueError is raised if the LLM API returns a malformed response (i. e. any kind of JSON
+        or other response object that does not conform to the expectation of how a well-formed response object from
+        this API should look like). If False, the API error responses are returned by __call__(), but no error will
+        be raised.
+    max_tries (int): Max. number of tries for API request.
+    interval (float): Time interval (in seconds) for API retries in seconds. We implement a base 2 exponential backoff
+        at each retry.
+    max_request_time (float): Max. time (in seconds) to wait for request to terminate before raising an exception.
+    RETURNS (Callable[[Iterable[str]], Iterable[str]]]): Anthropic instance for 'claude-1' model using REST to
+        prompt API.
+    """
+    return Anthropic(
+        name=name,
+        endpoint=Endpoints.COMPLETIONS,
+        config=config,
+        strict=strict,
+        max_tries=max_tries,
+        interval=interval,
+        max_request_time=max_request_time,
+    )
+
+
 @registry.llm_models("spacy.Claude-1.v1")
 def anthropic_claude_1(
     config: Dict[Any, Any] = SimpleFrozenDict(),
     name: Literal["claude-1", "claude-1-100k"] = "claude-1",  # noqa: F722
     strict: bool = Anthropic.DEFAULT_STRICT,
     max_tries: int = Anthropic.DEFAULT_MAX_TRIES,
     interval: float = Anthropic.DEFAULT_INTERVAL,
```

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/base.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/cohere/model.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/cohere/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/cohere/registry.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/cohere/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/noop/model.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/noop/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/openai/__init__.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/openai/model.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/openai/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/models/rest/openai/registry.py` & `spacy-llm-0.4.3/spacy_llm/models/rest/openai/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/pipeline/llm.py` & `spacy-llm-0.4.3/spacy_llm/pipeline/llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/registry/normalizer.py` & `spacy-llm-0.4.3/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/registry/reader.py` & `spacy-llm-0.4.3/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/__init__.py` & `spacy-llm-0.4.3/spacy_llm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/lemma.py` & `spacy-llm-0.4.3/spacy_llm/tasks/lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/ner.py` & `spacy-llm-0.4.3/spacy_llm/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/noop.py` & `spacy-llm-0.4.3/spacy_llm/tasks/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/rel.py` & `spacy-llm-0.4.3/spacy_llm/tasks/rel.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/sentiment.py` & `spacy-llm-0.4.3/spacy_llm/tasks/sentiment.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/span.py` & `spacy-llm-0.4.3/spacy_llm/tasks/span.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/spancat.py` & `spacy-llm-0.4.3/spacy_llm/tasks/spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/summarization.py` & `spacy-llm-0.4.3/spacy_llm/tasks/summarization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/lemma.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/lemma.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/sentiment.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/sentiment.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/summarization.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/summarization.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/textcat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy-llm-0.4.3/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/textcat.py` & `spacy-llm-0.4.3/spacy_llm/tasks/textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.4.3/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tasks/util/serialization.py` & `spacy-llm-0.4.3/spacy_llm/tasks/util/serialization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/conftest.py` & `spacy-llm-0.4.3/spacy_llm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_anthropic.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_cohere.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_cohere.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_dolly.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_falcon.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_falcon.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_langchain.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_openllama.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_rest.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/models/test_stablelm.py` & `spacy-llm-0.4.3/spacy_llm/tests/models/test_stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.4.3/spacy_llm/tests/pipeline/test_llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.json` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/lemma.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.jsonl` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/lemma.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.yml` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/lemma.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/rel.jsonl` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/rel.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.json` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/summarization.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.jsonl` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/summarization.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.yml` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/examples/summarization.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_lemma.py` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/test_lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/test_ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_rel.py` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/test_rel.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_sentiment.py` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/test_spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_summarization.py` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/test_summarization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.4.3/spacy_llm/tests/tasks/test_textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/test_cache.py` & `spacy-llm-0.4.3/spacy_llm/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.4.3/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/ty.py` & `spacy-llm-0.4.3/spacy_llm/ty.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm/util.py` & `spacy-llm-0.4.3/spacy_llm/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.4.3/spacy_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.4.2
+Version: 0.4.3
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -169,15 +169,15 @@
     "llm",
     config={
         "task": {
             "@llm_tasks": "spacy.NER.v2",
             "labels": ["PERSON", "ORGANISATION", "LOCATION"]
         },
         "model": {
-            "@llm_models": "spacy.gpt-3.5.v1",
+            "@llm_models": "spacy.GPT-3-5.v1",
         },
     },
 )
 nlp.initialize()
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.2 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.3 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -99,15 +99,15 @@
 (https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by
 setting the environmental variable `HF_HOME`. Also, you can upgrade the model
 to be `"databricks/dolly-v2-12b"` for better performance. ### Example 3: Create
 the component directly in Python The `llm` component behaves as any other spaCy
 component does, so adding it to an existing pipeline follows the same pattern:
 ```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config=
 { "task": { "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
-"LOCATION"] }, "model": { "@llm_models": "spacy.gpt-3.5.v1", }, }, )
+"LOCATION"] }, "model": { "@llm_models": "spacy.GPT-3-5.v1", }, }, )
 nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
 usage of resources, typically you would use [`nlp.pipe(docs)`](https://
 spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
 single document. ### Example 4: Implement your own custom task To write a
 [`task`](#tasks), you need to implement two functions: `generate_prompts` that
 takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
```

### Comparing `spacy-llm-0.4.2/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.4.3/spacy_llm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 spacy_llm.egg-info/requires.txt
 spacy_llm.egg-info/top_level.txt
 spacy_llm/models/__init__.py
 spacy_llm/models/hf/__init__.py
 spacy_llm/models/hf/base.py
 spacy_llm/models/hf/dolly.py
 spacy_llm/models/hf/falcon.py
+spacy_llm/models/hf/llama2.py
 spacy_llm/models/hf/openllama.py
 spacy_llm/models/hf/stablelm.py
 spacy_llm/models/langchain/__init__.py
 spacy_llm/models/langchain/model.py
 spacy_llm/models/rest/__init__.py
 spacy_llm/models/rest/base.py
 spacy_llm/models/rest/anthropic/__init__.py
@@ -78,14 +79,15 @@
 spacy_llm/tests/test_registry.py
 spacy_llm/tests/models/__init__.py
 spacy_llm/tests/models/test_anthropic.py
 spacy_llm/tests/models/test_cohere.py
 spacy_llm/tests/models/test_dolly.py
 spacy_llm/tests/models/test_falcon.py
 spacy_llm/tests/models/test_langchain.py
+spacy_llm/tests/models/test_llama2.py
 spacy_llm/tests/models/test_openllama.py
 spacy_llm/tests/models/test_rest.py
 spacy_llm/tests/models/test_stablelm.py
 spacy_llm/tests/pipeline/__init__.py
 spacy_llm/tests/pipeline/test_llm.py
 spacy_llm/tests/tasks/__init__.py
 spacy_llm/tests/tasks/test_lemma.py
```

### Comparing `spacy-llm-0.4.2/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.4.3/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.4.3/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.4.3/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.4.3/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.4.3/usage_examples/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.4.3/usage_examples/tests/test_usage_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.2/usage_examples/textcat_openai/run_pipeline.py` & `spacy-llm-0.4.3/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

