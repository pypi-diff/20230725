# Comparing `tmp/pytakes-1.2.1.tar.gz` & `tmp/pytakes-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytakes-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytakes-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytakes-1.2.1.tar` & `pytakes-2.0.0.tar`

### file list

```diff
@@ -1,74 +1,77 @@
--rw-r--r--   0        0        0      990 2023-07-24 22:54:53.059655 pytakes-1.2.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     5068 2023-07-24 22:54:53.059655 pytakes-1.2.1/.gitignore
--rw-r--r--   0        0        0     1484 2023-07-24 22:54:53.059655 pytakes-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1136 2023-07-24 22:54:53.059655 pytakes-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0    16558 2023-07-24 22:54:53.063655 pytakes-1.2.1/README.md
--rw-r--r--   0        0        0     1560 2023-07-24 22:54:53.063655 pytakes-1.2.1/example/old/config.json
--rw-r--r--   0        0        0     1497 2023-07-24 22:54:53.063655 pytakes-1.2.1/example/simple/example.config.py
--rw-r--r--   0        0        0     1454 2023-07-24 22:54:53.063655 pytakes-1.2.1/pyproject.toml
--rw-r--r--   0        0        0        6 2023-07-24 22:54:53.063655 pytakes-1.2.1/requirements-db.txt
--rw-r--r--   0        0        0        6 2023-07-24 22:54:53.063655 pytakes-1.2.1/requirements-dev.txt
--rw-r--r--   0        0        0        8 2023-07-24 22:54:53.063655 pytakes-1.2.1/requirements-psql.txt
--rw-r--r--   0        0        0        8 2023-07-24 22:54:53.063655 pytakes-1.2.1/requirements-sas.txt
--rw-r--r--   0        0        0       48 2023-07-24 22:54:53.063655 pytakes-1.2.1/requirements.txt
--rw-r--r--   0        0        0      217 2023-07-24 22:54:53.063655 pytakes-1.2.1/scripts/run.py
--rw-r--r--   0        0        0      488 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/__init__.py
--rw-r--r--   0        0        0    13095 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/automate_run.py
--rw-r--r--   0        0        0    10495 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/build_dictionary.py
--rw-r--r--   0        0        0     2448 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/corpus.py
--rw-r--r--   0        0        0       31 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/dict/__init__.py
--rw-r--r--   0        0        0     5577 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/dict/rules.py
--rw-r--r--   0        0        0     1089 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/dict/textitem.py
--rw-r--r--   0        0        0      307 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/header.py
--rw-r--r--   0        0        0      232 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/__init__.py
--rw-r--r--   0        0        0     1758 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/base.py
--rw-r--r--   0        0        0      771 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/config.py
--rw-r--r--   0        0        0     5322 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/csv.py
--rw-r--r--   0        0        0     1623 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/jsonl.py
--rw-r--r--   0        0        0     1881 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/sas.py
--rw-r--r--   0        0        0     5656 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/sql.py
--rw-r--r--   0        0        0     5301 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/sqlai.py
--rw-r--r--   0        0        0     6729 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/templates.py
--rw-r--r--   0        0        0     1137 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/iolib/txt.py
--rw-r--r--   0        0        0     6069 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/negex_creator.py
--rw-r--r--   0        0        0      248 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/nlp/__init__.py
--rw-r--r--   0        0        0     1820 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/nlp/collections.py
--rw-r--r--   0        0        0    15087 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/nlp/conceptminer.py
--rw-r--r--   0        0        0     8353 2023-07-24 22:54:53.063655 pytakes-1.2.1/src/pytakes/nlp/convert.py
--rw-r--r--   0        0        0  2441216 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/data/ssplit.db
--rw-r--r--   0        0        0    98304 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/data/status.db
--rw-r--r--   0        0        0      390 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/miner.py
--rw-r--r--   0        0        0     3751 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/ngrams.py
--rw-r--r--   0        0        0    13706 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/sentence_boundary.py
--rw-r--r--   0        0        0    10668 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/statusminer.py
--rw-r--r--   0        0        0     7747 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/terms.py
--rw-r--r--   0        0        0     1893 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/nlp/utils.py
--rw-r--r--   0        0        0     1816 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/parser.py
--rw-r--r--   0        0        0     7013 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/postprocessor.py
--rw-r--r--   0        0        0     1657 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/processor.py
--rw-r--r--   0        0        0        0 2023-07-24 22:54:53.087655 pytakes-1.2.1/src/pytakes/run/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/run/runner.py
--rw-r--r--   0        0        0     4699 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/run/schema.py
--rw-r--r--   0        0        0     3203 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/run/simple_run.py
--rw-r--r--   0        0        0      856 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/sendmail.py
--rw-r--r--   0        0        0     6641 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/templates.py
--rw-r--r--   0        0        0        0 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/util/__init__.py
--rw-r--r--   0        0        0     5015 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/util/db_reader.py
--rw-r--r--   0        0        0     4041 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/util/email_utils.py
--rw-r--r--   0        0        0     4587 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/util/mylogger.py
--rw-r--r--   0        0        0     2977 2023-07-24 22:54:53.091655 pytakes-1.2.1/src/pytakes/util/utils.py
--rw-r--r--   0        0        0      183 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/concepts.csv
--rw-r--r--   0        0        0      932 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/config/run.config.py
--rw-r--r--   0        0        0    96091 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/files/file1.txt
--rw-r--r--   0        0        0    73681 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/files/file2.txt
--rw-r--r--   0        0        0     7199 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/files/file3.txt
--rw-r--r--   0        0        0      288 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/negation.csv
--rw-r--r--   0        0        0     2906 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/testout/expected.csv
--rw-r--r--   0        0        0     6920 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/testout/expected.jsonl
--rw-r--r--   0        0        0     6870 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/data/testout/expected.negex.jsonl
--rw-r--r--   0        0        0      575 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/test_load_negex.py
--rw-r--r--   0        0        0     2664 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/test_negation.py
--rw-r--r--   0        0        0      916 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/test_run.py
--rw-r--r--   0        0        0     1466 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/test_simple_run.py
--rw-r--r--   0        0        0     1511 2023-07-24 22:54:53.091655 pytakes-1.2.1/tests/test_statusminer.py
--rw-r--r--   0        0        0    17781 1970-01-01 00:00:00.000000 pytakes-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      990 2023-07-24 22:54:48.934057 pytakes-2.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     5113 2023-07-24 22:54:48.934057 pytakes-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1931 2023-07-24 22:54:48.934057 pytakes-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1136 2023-07-24 22:54:48.934057 pytakes-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0    19220 2023-07-24 22:54:48.934057 pytakes-2.0.0/README.md
+-rw-r--r--   0        0        0     1560 2023-07-24 22:54:48.934057 pytakes-2.0.0/example/old/config.json
+-rw-r--r--   0        0        0     1497 2023-07-24 22:54:48.934057 pytakes-2.0.0/example/simple/example.config.py
+-rw-r--r--   0        0        0     1514 2023-07-24 22:54:48.934057 pytakes-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-07-24 22:54:48.934057 pytakes-2.0.0/requirements-db.txt
+-rw-r--r--   0        0        0        6 2023-07-24 22:54:48.934057 pytakes-2.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0        8 2023-07-24 22:54:48.934057 pytakes-2.0.0/requirements-psql.txt
+-rw-r--r--   0        0        0        8 2023-07-24 22:54:48.934057 pytakes-2.0.0/requirements-sas.txt
+-rw-r--r--   0        0        0       55 2023-07-24 22:54:48.934057 pytakes-2.0.0/requirements.txt
+-rw-r--r--   0        0        0      217 2023-07-24 22:54:48.934057 pytakes-2.0.0/scripts/run.py
+-rw-r--r--   0        0        0      488 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/__init__.py
+-rw-r--r--   0        0        0    13095 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/automate_run.py
+-rw-r--r--   0        0        0    10495 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/build_dictionary.py
+-rw-r--r--   0        0        0     2448 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/corpus.py
+-rw-r--r--   0        0        0       31 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/dict/__init__.py
+-rw-r--r--   0        0        0     5577 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/dict/rules.py
+-rw-r--r--   0        0        0      908 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/dict/textitem.py
+-rw-r--r--   0        0        0      307 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/header.py
+-rw-r--r--   0        0        0      232 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/__init__.py
+-rw-r--r--   0        0        0     1870 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/base.py
+-rw-r--r--   0        0        0      771 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/config.py
+-rw-r--r--   0        0        0     5269 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/csv.py
+-rw-r--r--   0        0        0     1572 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/jsonl.py
+-rw-r--r--   0        0        0     1881 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/sas.py
+-rw-r--r--   0        0        0     5652 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/sql.py
+-rw-r--r--   0        0        0     5301 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/sqlai.py
+-rw-r--r--   0        0        0     6704 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/templates.py
+-rw-r--r--   0        0        0     1137 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/iolib/txt.py
+-rw-r--r--   0        0        0     6069 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/negex_creator.py
+-rw-r--r--   0        0        0      248 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/nlp/__init__.py
+-rw-r--r--   0        0        0     1814 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/nlp/collections.py
+-rw-r--r--   0        0        0    15079 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/nlp/conceptminer.py
+-rw-r--r--   0        0        0     8540 2023-07-24 22:54:48.934057 pytakes-2.0.0/src/pytakes/nlp/convert.py
+-rw-r--r--   0        0        0  2441216 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/data/ssplit.db
+-rw-r--r--   0        0        0    98304 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/data/status.db
+-rw-r--r--   0        0        0      390 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/miner.py
+-rw-r--r--   0        0        0     3751 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/ngrams.py
+-rw-r--r--   0        0        0    13474 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/sentence_boundary.py
+-rw-r--r--   0        0        0    10598 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/statusminer.py
+-rw-r--r--   0        0        0     6876 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/terms.py
+-rw-r--r--   0        0        0     1893 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/nlp/utils.py
+-rw-r--r--   0        0        0     1816 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/parser.py
+-rw-r--r--   0        0        0     7011 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/postprocessor.py
+-rw-r--r--   0        0        0     1641 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/processor.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/run/__init__.py
+-rw-r--r--   0        0        0     1377 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/run/runner.py
+-rw-r--r--   0        0        0     4875 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/run/schema.py
+-rw-r--r--   0        0        0     3431 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/run/simple_run.py
+-rw-r--r--   0        0        0      856 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/sendmail.py
+-rw-r--r--   0        0        0     6616 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/templates.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/util/__init__.py
+-rw-r--r--   0        0        0     5015 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/util/db_reader.py
+-rw-r--r--   0        0        0     4041 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/util/email_utils.py
+-rw-r--r--   0        0        0     4587 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/util/mylogger.py
+-rw-r--r--   0        0        0     2977 2023-07-24 22:54:48.954058 pytakes-2.0.0/src/pytakes/util/utils.py
+-rw-r--r--   0        0        0      192 2023-07-24 22:54:48.954058 pytakes-2.0.0/tests/data/concepts.csv
+-rw-r--r--   0        0        0      932 2023-07-24 22:54:48.954058 pytakes-2.0.0/tests/data/config/run.config.py
+-rw-r--r--   0        0        0      973 2023-07-24 22:54:48.954058 pytakes-2.0.0/tests/data/config/run.is_regex_false.config.py
+-rw-r--r--   0        0        0    96091 2023-07-24 22:54:48.954058 pytakes-2.0.0/tests/data/files/file1.txt
+-rw-r--r--   0        0        0    73681 2023-07-24 22:54:48.954058 pytakes-2.0.0/tests/data/files/file2.txt
+-rw-r--r--   0        0        0     7199 2023-07-24 22:54:48.954058 pytakes-2.0.0/tests/data/files/file3.txt
+-rw-r--r--   0        0        0      288 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/data/negation.csv
+-rw-r--r--   0        0        0     3209 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/data/testout/expected.csv
+-rw-r--r--   0        0        0     2222 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/data/testout/expected.is_regex_false.jsonl
+-rw-r--r--   0        0        0     7699 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/data/testout/expected.jsonl
+-rw-r--r--   0        0        0     7649 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/data/testout/expected.negex.jsonl
+-rw-r--r--   0        0        0     1498 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/test_keywords.py
+-rw-r--r--   0        0        0      575 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/test_load_negex.py
+-rw-r--r--   0        0        0     2612 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/test_negation.py
+-rw-r--r--   0        0        0     1779 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/test_run.py
+-rw-r--r--   0        0        0     1466 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/test_simple_run.py
+-rw-r--r--   0        0        0     1496 2023-07-24 22:54:48.958057 pytakes-2.0.0/tests/test_statusminer.py
+-rw-r--r--   0        0        0    20516 1970-01-01 00:00:00.000000 pytakes-2.0.0/PKG-INFO
```

### Comparing `pytakes-1.2.1/.github/workflows/publish-to-pypi.yml` & `pytakes-2.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/.gitignore` & `pytakes-2.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -308,7 +308,8 @@
 
 # Pyre type checker
 .pyre/
 
 # user-added
 tests/data/testout/concepts*
 /tests/data/testout/run.negex.jsonl
+/tests/data/testout/run.is_regex_false.jsonl
```

### Comparing `pytakes-1.2.1/CHANGELOG.md` & `pytakes-2.0.0/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,33 @@
 * `Deprecated`: for soon-to-be removed features.
 * `Removed`: for now removed features.
 * `Fixed`: for any bug fixes.
 * `Security`: in case of vulnerabilities.
 
 ## [Unreleased]
 
+
+## 2.0.0 - 2023-07-24
+
+### Added
+
+* Added option to specify when the included text is not a regex by setting `is_regex` to false in config
+* Logging
+
+### Changed
+
+* For `regex_variation` = -1, no additions are made.
+* Building concepts/keywords will no longer remove parentheses or expand an asterisk.
+* Renamed `logger` in schema to `log` to prevent clash with loguru's logger. 
+
+### Fixed
+
+* Cases were cleaning was removing certain matches.
+
+
 ## 1.2.1 - 2023-07-20
 
 ### Added
 
 * Better documentation to negation
 * Specify which terms caused change in Concept status (`jsonl` output only)
```

### Comparing `pytakes-1.2.1/LICENSE.txt` & `pytakes-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/README.md` & `pytakes-2.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This module will look for a pre-defined set of terms in a corpus of text, and use a variation of the negex/context
 algorithm to determine whether these terms express negation, historical, or various other qualifiers. (The set of
 negation terms is also configurable.)
 
 ## Requirements ##
 
-* Python 3.6+
+* Python 3.8+
 * See requirements.txt (`pip install -r requirements.txt`)
     * Various requirements-_.txt files are provided depending on your needs:
         * dev: for running tests, general development
         * db: for connecting to database using pyodbc
         * psql: connecting to postgres database
         * sas: if data is stored in SAS
 
@@ -62,15 +62,28 @@
 here: https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/negex/lexical_kb.csv
 
 Negation works by searching for the following word categories and then using a set of rules to determine which words
 should be 'qualified' in different ways. Within the recommended `jsonl` output, you'll find this included under
 the `qualifiers` key. Consider the following example:
 
 ```json
-"qualifiers": {"certainty": 0, "hypothetical": true, "historical": false, "other_subject": false, "terms": ["not", "afraid"]}
+{
+  ...
+  "qualifiers": {
+    "certainty": 0,
+    "hypothetical": true,
+    "historical": false,
+    "other_subject": false,
+    "terms": [
+      "not",
+      "afraid"
+    ]
+  },
+  ...
+}
 ```
 
 All values begin as `False` except `certainty` which starts as 4, meaning `definite`/`affirmative`. Here, `certainty` is
 0, meaning `negated`. This was done by the term 'not' which appears in the list of `terms`. `hypothetical` has been
 marked as `True` due to the term `afraid` (often in a context like 'afraid that he will catch a cold').
 
 **Certainty:**
@@ -117,22 +130,23 @@
     * 3: term applies negation, etc. **forward and/or backward** in the sentence (e.g., 'likely')
 
 #### Concept/Term Table ####
 
 This is the table containing the terms you want to search for (i.e., the entities you want extracted). I have added a
 script to autogenerate these based on some basic configuration files.
 
-    ​Column	​Type	​Description
-    ​ID	​int	​identity column; unique integer for each row
-    ​CUI	 string	​category identifier; can be used to "group" different     terms together
-    ​Text	​string	​term
-    ​RegexVariation	​int	​amount of variation: 0=none; 3=very; 1=default; -1=don't even allow suffixes, exact matches only; see #Rules#parameters below; I suggest you just use "0" or "-1"
-    ​WordOrder	​int	​how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order
-    MaxIntervening	int	how many intervening words to allow when locating words; 'how many intervening words do I allow?'
-    MaxWords	int	how many words to look ahead to find the next word; is ‘how far do I look ahead after each term?’ 
+| Column	         | Type	                                                                    | Description                                                                                                                                                       |       
+|-----------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ID	             | int	                                                                     | identity column; unique integer for each row                                                                                                                      |
+| CUI	 string	    | category identifier; can be used to "group" different     terms together |
+| Text	           | string	                                                                  | term                                                                                                                                                              |
+| RegexVariation	 | int	                                                                     | amount of variation: 0=none; 3=very; 1=default; -1=don't even allow suffixes, exact matches only; see #Rules#parameters below; I suggest you just use "0" or "-1" |
+| WordOrder	      | int	                                                                     | how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order                                                                         |
+| MaxIntervening  | int                                                                      | how many intervening words to allow when locating words; 'how many intervening words do I allow?'                                                                 |
+| MaxWords	       | int                                                                      | how many words to look ahead to find the next word; is ‘how far do I look ahead after each term?’                                                                 | 
 
 MaxIntervening and MaxWords should not be used together.
 
 To autogenerate this table format, use the `pytakes-build-dictionary` script installed into the Python Scripts
 directory. For an example, run this with the `--create-sample` option (optionally specify the output with
 the `--path C:\somewhere` option. For additional specifications, see the "Dictionary Builder" section below.
 
@@ -196,40 +210,39 @@
 For a simple example, run (you will first need to install this package, run `python setup.py install` in the base
 directory):
 
     pytakes-build-dictionary --create-sample --path OUTPUT_PATH
 
 ### COMMAND LINE ARGUMENTS ###
 
-    Short​	​Long	​Description
-    ​-p	​--path	​Specifies parent directory of folders; program will prompt if unable to locate the directory
-    ​-o	​--output	​Specify output CSV file; if ".csv" is not included, it will be added
-    ​-t	​--table	​Specify output table in specified database (See below)
-    ​-v	​--verbosity	​Specify amount of log output to show: 3-most verbose; 0-least verbose
-    --driver	If -t is specified, driver where table should be created. Defaults to SQL Server
-    --server	If -t is specified, server where table should be created. 
-    --database	If -t is specified, database where table should be created. 
+| Short | Long        | Description                                                                                  |
+|-------|-------------|----------------------------------------------------------------------------------------------|
+| -p    | --path      | Specifies parent directory of folders; program will prompt if unable to locate the directory |
+| -o    | --output    | Specify output CSV file; if ".csv" is not included, it will be added                         |
+| -t    | --table     | Specify output table in specified database (See below)                                       |
+| -v    | --verbosity | Specify amount of log output to show: 3-most verbose; 0-least verbose                        |
+|       | --driver    | If -t is specified, driver where table should be created. Defaults to SQL Server             |
+|       | --server    | If -t is specified, server where table should be created.                                    |
+|       | --database  | If -t is specified, database where table should be created.                                  |
 
 ### OUTPUT COLUMNS ####
 
 Not all of these output columns are required (most don't do anything). This was originally designed for building a
 dictionary using cTAKES.
 
-     Column	​Type	​Description
-     ID	​int	​identity column; unique integer for each row
-     CUI	​varchar(8)	​category identifier; can be used to "group" different terms together
-     Fword	​varchar(80)	​first word of term
-     Text	​varchar(8000)	​term
-     Code	​varchar(45)	​unimportant value required by cTAKES (legacy)
-     SourceType	​varchar(45)	​unimportant value required by cTAKES (legacy)
-     TUI	​varchar(4)	​​unimportant value required by cTAKES (legacy)
-     TextLength	​int	​length of term (all characters including spaces)
-     RegexVariation	​int	​amount of variation: 0=none; 3=very; 1=default; see #Rules#parameters below
-     WordOrder	​int	​how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order
-     Valence	​int	​this should just be "1"; program is  not designed to work with this correctly
+| Column         | Type          | Description                                                                               |
+|----------------|---------------|-------------------------------------------------------------------------------------------|
+| ID             | int           | identity column; unique integer for each row                                              |
+| CUI            | varchar(8)    | category identifier; can be used to "group" different terms together                      |
+| Fword          | varchar(80)   | first word of term                                                                        |
+| Text           | varchar(8000) | term                                                                                      |
+| TextLength     | int           | length of term (all characters including spaces)                                          |
+| RegexVariation | int           | amount of variation: 0=none; 3=very; 1=default; see #Rules#parameters below               |
+| WordOrder      | int           | how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order |
+| Valence        | int           | this should just be "1"; program is not designed to work with this correctly              |
 
 ### RULES ###
 
 Rules are the text entries in the cTAKES-like dictionary, however, they can include "categories" in addition to just
 text.A category is any string of text surrounded by "[" and "]". The intervening text string is the name of a "
 category". The category must have a definition, and each item (synonym) in the definition will be used in the rule.
 
@@ -250,30 +263,30 @@
 The rule file must be named "rules" or "rules.some-extension" (e.g., "rules.txt").
 
 #### Parameters ####
 
 Rules may also maintain configuration parameters.The configurations are indexed in the following order (bold indicates
 the default parameter):
 
-RegexVariation (integers)
-
-    **0: no variation in regular expression coverage**
-    1: minimal variation in regular expression coverage
-    2: moderate variation in regular expression coverage
-    3: high flexibility in regular expression coverage
-
-WordOrder
-
-    0: free word order
-    **1: enforce first word rule**
-    2: require precise word order
-
-Valence
-
-    **ALWAYS USE 1** or just ignore; NOT YET CORRECTLY IMPLEMENTED IN LCTAKES
+| RegexVariation | Description                                               |
+|----------------|-----------------------------------------------------------|
+| 0              | **(Default)** no variation in regular expression coverage |
+| 1              | minimal variation in regular expression coverage          |
+| 2              | moderate variation in regular expression coverage         |
+| 3              | high flexibility in regular expression coverage           |
+
+| WordOrder | Description                           |
+|-----------|---------------------------------------|
+| 0         | free word order                       |
+| 1         | **(Default)** enforce first word rule |
+| 2         | require precise word order            |
+
+| Valence | Description                |
+|---------|----------------------------|
+| 1       | **(Default)** Always use 1 |
 
 These are designated by the double percent ('%%') and follow the rule.
 
     [category]%%REGEX_VARIATION,WORD_ORDER,VALENCE
 
 For example:
```

### Comparing `pytakes-1.2.1/example/old/config.json` & `pytakes-2.0.0/example/old/config.json`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/example/simple/example.config.py` & `pytakes-2.0.0/example/simple/example.config.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/pyproject.toml` & `pytakes-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 dependencies = [
     'regex',
     'jinja2',
     'pyodbc',
     'sqlalchemy',
     'jsonschema',
     'pyyaml',
+    'loguru',
 ]
 requires-python = '>=3.8'
 keywords = [
     'nlp',
     'information extraction',
 ]
 classifiers = [# https://pypi.org/classifiers/
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Science/Research',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Text Processing :: Linguistic',
     'License :: OSI Approved :: MIT License',
     'Intended Audience :: Healthcare Industry',
 ]
 
 [project.urls]
 Home = 'https://github.com/dcronkite/pytakes'
```

### Comparing `pytakes-1.2.1/src/pytakes/automate_run.py` & `pytakes-2.0.0/src/pytakes/automate_run.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/build_dictionary.py` & `pytakes-2.0.0/src/pytakes/build_dictionary.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/corpus.py` & `pytakes-2.0.0/src/pytakes/corpus.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/dict/rules.py` & `pytakes-2.0.0/src/pytakes/dict/rules.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/iolib/base.py` & `pytakes-2.0.0/src/pytakes/iolib/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 import abc
 
 
 class Dictionary(metaclass=abc.ABCMeta):
     def __init__(self, name=None, **kwargs):
         self.name = name
+        self.is_regex = kwargs.get('is_regex', None)
+        self.convert_all = kwargs.get('convert_all', None)
 
     @abc.abstractmethod
     def read(self):
         pass
 
     def int_or_default(self, val, default):
         try:
```

### Comparing `pytakes-1.2.1/src/pytakes/iolib/config.py` & `pytakes-2.0.0/src/pytakes/iolib/config.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/iolib/csv.py` & `pytakes-2.0.0/src/pytakes/iolib/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,32 +104,32 @@
 
     def writerow(self, feat: Concept, meta=None, text=None):
         if not meta:
             meta = []
         if text:
             length = len(text)
             self.writer.writerow(meta +
-                                 [feat.id(),
-                                  feat.cat(),
-                                  self._get_text(text, feat.begin(), feat.end()),
-                                  self._get_text(text, self._get_index(length, feat.begin() - self.context_width),
-                                                 self._get_index(length, feat.end() + self.context_width)),
-                                  feat.get_certainty(),
-                                  feat.is_hypothetical(),
-                                  feat.is_historical(),
-                                  feat.is_not_patient(),
-                                  feat.get_absolute_begin(),
-                                  feat.get_absolute_end(),
+                                 [feat.id,
+                                  feat.cat,
+                                  self._get_text(text, feat.begin, feat.end),
+                                  self._get_text(text, self._get_index(length, feat.begin - self.context_width),
+                                                 self._get_index(length, feat.end + self.context_width)),
+                                  feat.certainty,
+                                  feat.hypothetical,
+                                  feat.historical,
+                                  feat.other,
+                                  feat.absolute_begin,
+                                  feat.absolute_end,
                                   self.hostname,
                                   self.batch_number
                                   ]
                                  )
         else:  # no text
             self.writer.writerow(meta +
-                                 [text[feat.begin():feat.end()].strip(),
+                                 [text[feat.begin:feat.begin].strip(),
                                   None,
                                   None,
                                   None,
                                   None,
                                   None,
                                   self.hostname,
                                   self.batch_number
```

### Comparing `pytakes-1.2.1/src/pytakes/iolib/jsonl.py` & `pytakes-2.0.0/src/pytakes/iolib/jsonl.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,28 @@
         self.batch_number = batch_number
         self.fh = open(path / self.name, 'w')
 
     def writerow(self, feat, meta=None, text=None):
         length = len(text)
         data = {
             'meta': meta,
-            'concept_id': feat.id(),
-            'concept': feat.cat(),
-            'captured': self._get_text(text, feat.begin(), feat.end()),
-            'context': self._get_text(text, self._get_index(length, feat.begin() - self.context_width),
-                                      self._get_index(length, feat.end() + self.context_width)),
+            'concept_id': feat.id,
+            'concept': feat.cat,
+            'captured': self._get_text(text, feat.begin, feat.end),
+            'context': self._get_text(text, self._get_index(length, feat.begin - self.context_width),
+                                      self._get_index(length, feat.end + self.context_width)),
             'qualifiers': {
-                'certainty': feat.get_certainty(),
-                'hypothetical': feat.is_hypothetical(),
-                'historical': feat.is_historical(),
-                'other_subject': feat.is_not_patient(),
+                'certainty': feat.certainty,
+                'hypothetical': feat.hypothetical,
+                'historical': feat.historical,
+                'other_subject': feat.other,
                 'terms': feat.qualifiers,
             },
-            'start_index': feat.get_absolute_begin(),
-            'end_index': feat.get_absolute_end(),
+            'start_index': feat.absolute_begin,
+            'end_index': feat.absolute_end,
             'tracking': {
                 'hostname': self.hostname,
                 'batch': self.batch_number,
             }
         }
         self.fh.write(json.dumps(data) + '\n')
```

### Comparing `pytakes-1.2.1/src/pytakes/iolib/sas.py` & `pytakes-2.0.0/src/pytakes/iolib/sas.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/iolib/sql.py` & `pytakes-2.0.0/src/pytakes/iolib/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,16 @@
             raise e
 
     def writerow(self, meta, feat, text=None):
         self.dbi.execute_commit(
             Template(templates.PROC_INSERT_INTO2_QUERY).render(
                 labels=self.labels, metas=meta,
                 destination_table=self.fullname, feature=feat, text=text,
-                captured=text[feat.begin():feat.end()].strip(),
-                context=text[self._get_index(len(text), feat.begin() - 75):self._get_index(len(text), feat.end() + 75)],
+                captured=text[feat.begin:feat.begin].strip(),
+                context=text[self._get_index(len(text), feat.begin - 75):self._get_index(len(text), feat.begin + 75)],
                 hostname=self.hostname, batch_number=self.batch_number
             )
         )
         self.dbi.execute_commit(
             Template(templates.PROC_INSERT_INTO3_QUERY).render(
                 labels=self.labels, metas=meta,
                 destination_table=self.fullname, feature=feat,
```

### Comparing `pytakes-1.2.1/src/pytakes/iolib/sqlai.py` & `pytakes-2.0.0/src/pytakes/iolib/sqlai.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/iolib/templates.py` & `pytakes-2.0.0/src/pytakes/iolib/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,24 +142,24 @@
 {%- for label in labels %}
 {{ label }}{% if not loop.last %},{% endif %}
 {%- endfor %}
 ) VALUES (
 {%- for meta in metas %}
 '{{ meta|replace("'", "''") }}',
 {%- endfor %}
-{{ feature.id() }},
+{{ feature.id }},
 '{{ captured|replace("'", "''") }}',
 '{{ context|replace("'", "''") }}',
 '{{ text|replace("'", "''") }}',
-{{ feature.get_certainty() }},
-{% if feature.is_hypothetical() %}1{% else %}0{% endif %},
-{% if feature.is_historical() %}1{% else %}0{% endif %},
-{% if feature.is_hypothetical() %}1{% else %}0{% endif %},
-{{ feature.begin() }},
-{{ feature.end() }},
+{{ feature.certainty }},
+{% if feature.hypothetical %}1{% else %}0{% endif %},
+{% if feature.historical %}1{% else %}0{% endif %},
+{% if feature.hypothetical %}1{% else %}0{% endif %},
+{{ feature.begin }},
+{{ feature.begin }},
 {{ feature.get_absolute_begin() }},
 {{ feature.get_absolute_end() }}
 {% if hostname %}, '{{ hostname|replace("'", "''") }}', {{ batch_number }}{% endif %}
 )
 '''
 
 PROC_INSERT_INTO3_QUERY = r'''INSERT INTO {{ destination_table }} (
```

### Comparing `pytakes-1.2.1/src/pytakes/iolib/txt.py` & `pytakes-2.0.0/src/pytakes/iolib/txt.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/negex_creator.py` & `pytakes-2.0.0/src/pytakes/negex_creator.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/nlp/collections.py` & `pytakes-2.0.0/src/pytakes/nlp/collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,11 +44,11 @@
         res = []
         for miner in self.miners:
             res += miner.extract(terms)
         return res, sentence
 
     def parse(self, doc):
         offset = 0
-        for sentence in self.ssplit(doc.get_text()):
+        for sentence in self.ssplit(doc.text):
             sent = self.clean_sentence(sentence)
             yield self.parse_sentence(sent, offset)
             offset += len(sent)
```

### Comparing `pytakes-1.2.1/src/pytakes/nlp/conceptminer.py` & `pytakes-2.0.0/src/pytakes/nlp/conceptminer.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 from . import convert
 from .miner import Miner
 from .terms import Term, Concept
 
 
 class ConceptMiner(Miner):
 
-    def __init__(self, dictionaries: List[Dictionary]):
+    def __init__(self, dictionaries: List[Dictionary], *, is_regex=True, convert_all=True):
         super().__init__()
-        self.entries = [entry for d in dictionaries for entry in d.read()]
+        if len(dictionaries) == 0:
+            raise ValueError('No dictionaries supplied!')
+        self.entries = dictionaries
         self.cid_to_cat = {}  # ConceptID -> category
         self.cid_to_tids = {}  # ConceptID to TermIDs
         self.cid_search_param = {}
         self.wordID = 0
         self.tid_to_tid = {}  # list of conversions of
         # new TermIDs to old TermIDs
         # this should be a one-to-many
@@ -43,17 +45,17 @@
         # older TermIDs
         # no reason to have it the other
         # way around
         self.cid_to_val = {}
         self.cid_word_order = {}  # word order constraints
         self.wordlist = []
 
-        self._unpack_concepts()
+        self._unpack_concepts(is_regex=is_regex, convert_all=convert_all)
 
-    def _unpack_concepts(self):
+    def _unpack_concepts(self, *, is_regex=True, convert_all=True):
         """
         Organizes input from database
         Parameters:
             id_term_cat_val_rxVar_wdOrder - list of (id, term, category, valence,
                                        regex_variation, word_order)
                 * id - number
                 * term - ctakes dictionary "text" field
@@ -64,35 +66,40 @@
                             2: require precise word order
                 * regex_variation-
                             0: no variation; words must be exact
                             1: minimal variation
                             2: moderate variation
                             3: flexible
         """
-        for cid, term, cat, val, rxVar, wdOrder, max_intervening, max_search in self.entries:
-            # update references of ConceptID (think "CUI")
-            self.cid_to_cat[cid] = cat
-            self.cid_to_val[cid] = val
-            self.cid_word_order[cid] = wdOrder
-            self.cid_search_param[cid] = (max_intervening, max_search)
-            if wdOrder == 0:  # free word order
-                self.cid_to_tids[cid] = set()
-            elif wdOrder > 0:  # restricted word order
-                self.cid_to_tids[cid] = list()
-
-            for word in term.split():
-                # give each word a unique id, and treated uniquely
-                self.wordlist.append((word, self.wordID, rxVar))
-                if wdOrder == 0:
-                    self.cid_to_tids[cid].add(self.wordID)
-                if wdOrder > 0:
-                    self.cid_to_tids[cid].append(self.wordID)
-                self.wordID += 1
-
-        self.wordlist, upd_ids = convert.convert_to_regex(self.wordlist)
+        for dictionary in self.entries:
+            for cid, term, cat, val, rxVar, wdOrder, max_intervening, max_search in dictionary.read():
+                # update references of ConceptID (think "CUI")
+                self.cid_to_cat[cid] = cat
+                self.cid_to_val[cid] = val
+                self.cid_word_order[cid] = wdOrder
+                self.cid_search_param[cid] = (max_intervening, max_search)
+                if wdOrder == 0:  # free word order
+                    self.cid_to_tids[cid] = set()
+                elif wdOrder > 0:  # restricted word order
+                    self.cid_to_tids[cid] = list()
+
+                for word in term.split():
+                    # give each word a unique id, and treated uniquely
+                    self.wordlist.append((word, self.wordID, rxVar))
+                    if wdOrder == 0:
+                        self.cid_to_tids[cid].add(self.wordID)
+                    if wdOrder > 0:
+                        self.cid_to_tids[cid].append(self.wordID)
+                    self.wordID += 1
+
+            self.wordlist, upd_ids = convert.convert_to_regex(
+                self.wordlist,
+                is_regex=is_regex if dictionary.is_regex is None else dictionary.is_regex,
+                convert_all=convert_all if dictionary.convert_all is None else dictionary.convert_all,
+            )
 
     def add_conversion(self, newtid_to_oldtids):
         """
         Adds new one-to-many relations between
         term_ids. Each term-id may only appear
         either on the RHS or the LHS of the dict
         (a.k.a., either keys or values, but not both)
@@ -196,49 +203,49 @@
         @return: all found concepts
 
         """
         concepts = []
         for i in range(len(terms)):
             cword = terms[i]
             if isinstance(cword, Term):
-                c_all_tids = set(self.get_original_term_id(cword.id()))
+                c_all_tids = set(self.get_original_term_id(cword.id))
                 for cid in self.cid_to_tids:  # look through concepts
                     max_intervening, max_search = self.cid_search_param[cid]
                     remain_set = self._get_remaining(c_all_tids, self.cid_to_tids[cid], self.cid_word_order[cid],
                                                      first_word=True)
 
                     if remain_set is None:
                         continue  # return type of None was not a match
 
                     # check if concept was completed
                     if remain_set:  # concept has additional terms (> 1 word)
                         concept = self._aggregate(terms[i:],
                                                   remain_set,
-                                                  cword.get_certainty(),
-                                                  cword.is_hypothetical(),
-                                                  cword.is_historical(),
-                                                  cword.is_not_patient(),
-                                                  cword.begin(),
+                                                  cword.certainty,
+                                                  cword.hypothetical,
+                                                  cword.historical,
+                                                  cword.other,
+                                                  cword.begin,
                                                   cid,
                                                   max_search,
                                                   max_intervening,
                                                   self.cid_word_order[cid],
                                                   qualifiers=cword.qualifiers,
                                                   )
                     else:  # one-term concept (remain_set is empty list/set)
-                        concept = Concept(cword.word(),
-                                          cword.begin(),
-                                          cword.end(),
+                        concept = Concept(cword.word,
+                                          cword.begin,
+                                          cword.end,
                                           cid,
                                           self.cid_to_cat[cid],
-                                          self._check_valence(cid, cword.get_certainty()),
-                                          cword.is_hypothetical(),
-                                          cword.is_historical(),
-                                          cword.is_not_patient(),
-                                          offset=cword.offset_,
+                                          self._check_valence(cid, cword.certainty),
+                                          cword.hypothetical,
+                                          cword.historical,
+                                          cword.other,
+                                          offset=cword.offset,
                                           qualifiers=cword.qualifiers,
                                           )
                     if concept:  # function might return "False"
                         concepts.append(concept)
             else:  # current word is not a Term
                 continue
         return concepts
@@ -268,44 +275,43 @@
         words = words[1:]
         # see if matching terms are available in the next couple terms
         for j in range(len(words)):
             if j < words_to_look_at and max_intervening_words >= 0:
                 nword = words[j]
                 if isinstance(nword, Term):
                     # check if current term is present in current concept
-                    n_all_tids = set(self.get_original_term_id(nword.id()))
+                    n_all_tids = set(self.get_original_term_id(nword.id))
                     temp_remain_set = self._get_remaining(n_all_tids, remain_set, word_order, first_word=False)
 
                     if temp_remain_set is None:  # term not in concept
                         max_intervening_words -= 1
                     else:  # term in concept
                         words_to_look_at += words_to_look_at_incr
                         # update negex status with more egregious form
-                        certainty = min(certainty, nword.get_certainty())
-                        hypothetical = max(hypothetical, nword.is_hypothetical())
-                        historical = max(historical, nword.is_historical())
-                        not_patient = max(not_patient, nword.is_not_patient())
+                        certainty = min(certainty, nword.certainty)
+                        hypothetical = hypothetical or nword.hypothetical
+                        historical = historical or nword.historical
+                        not_patient = not_patient or nword.other
                         if nword.qualifiers:
                             qualifiers += nword.qualifiers
                         if temp_remain_set:  # more terms to find
                             remain_set = temp_remain_set
                         else:  # empty list or set (cannot be None)
-                            return Concept(' '.join([w.word() for w in orig_words[:j + 2]]),
+                            return Concept(' '.join(w.word for w in orig_words[:j + 2]),
                                            start_idx,
-                                           words[j].end(),
+                                           words[j].end,
                                            cid,
                                            self.cid_to_cat[cid],
                                            self._check_valence(cid, certainty),
                                            hypothetical,
                                            historical,
                                            not_patient,
-                                           offset=nword.offset_,
+                                           offset=nword.offset,
                                            qualifiers=qualifiers,
                                            )
-
             else:
                 break
         return False
 
     def postprocess(self, terms):
         return terms  # no postprocessing
 
@@ -326,28 +332,16 @@
         """
         remove terms that are subsumed by other terms
         :param terms:
         """
         terms.sort(reverse=False)
         if len(terms) < 2:
             return terms
-        i = 1
-        curr = 0
-        while True:
-            if terms[curr] == terms[i]:
-                if len(terms[curr]) > len(terms[i]):
-                    del terms[i]
-                elif len(terms[curr]) < len(terms[i]):
-                    del terms[curr]
-                    curr = i - 1
-                elif terms[curr].begin() == terms[i].begin() and terms[curr].end() == terms[i].end():
-                    terms[curr].add_term(terms[i])
-                    del terms[i]
-                else:  # keep both representations
-                    curr = i
-                    i += 1
+        curr_idx = 0
+        next_idx = 1
+        while next_idx < len(terms):
+            if terms[curr_idx] == terms[next_idx]:  # has same indices
+                terms[curr_idx].add_term(terms.pop(next_idx))
             else:
-                curr = i
-                i += 1
-
-            if i >= len(terms):
-                return terms
+                curr_idx += 1
+                next_idx += 1
+        return terms
```

### Comparing `pytakes-1.2.1/src/pytakes/nlp/convert.py` & `pytakes-2.0.0/src/pytakes/nlp/convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     The identity of the terms is retained.
 """
 # regex should replace/expand re
 # may require a new flag to get
 # default regex behavior after this
 # transformation
 import regex as re
+from loguru import logger
 
 
 def get_affix_morphs():
     """
     list of tuple(regex, replacement string, count) for modifying 
         the front of a term
     count represents the number of letters which are becoming
@@ -65,15 +66,15 @@
         optional (not _new_ optional ones)
     """
     return [(re.compile(r'\b(\S+)s(\W*)\b'), r'\g<1>\g<2>s(es)?', 0),  # pl='es'
             (re.compile(r'\b(\S+)o(\W*)\b'), r'\g<1>\g<2>o(e?s)?', 0),  # pl='es'
             (re.compile(r'\b(\S+)(\W*)\b'), r'\g<1>\g<2>s?', 0)]  # pl='s'
 
 
-def convert_to_regex(strings_ids_rxvar, convert_all=True,
+def convert_to_regex(strings_ids_rxvar, convert_all=True, is_regex=True,
                      affixmorphs=None, suffixmorphs=None,
                      medialmorphs=None, finalmorphs=None):
     """
     Takes a list of string-id tuples which are the words which
         need to be converted to regular expressions.
         The id part should be a unique identifier.
     Duplicate regexes will not be included. Duplicates
@@ -84,15 +85,15 @@
         string_ids_settings: list of (string, id, wdOrder ) in which 
             string is to be converted to regex;
             order is important as the strings are
             converted to regexes in list order, and
             any following strings which are matched
             by the previous regexes will not be included
         degree of regex variation-
-                    -1: no variation at all (no prefixes/suffixes)
+                    -1: no variation at all -- is already a Python-style regex
                     0: no variation; words must be exact
                     1: minimal variation
                     2: moderate variation
                     3: flexible
         convert_all=True: if false, all strings will be
             converted to regexes regardless of a previous
             regex matching it
@@ -109,18 +110,16 @@
         medialmorphs = get_medial_morphs()
     if not suffixmorphs:
         suffixmorphs = get_suffix_morphs()
 
     regexes = []  # [(regex, id), ...]
     updated_ids = {}  # new_id -> old_id
     for string, id_, regex_variation in strings_ids_rxvar:
-        string = string.replace('(', '').replace(')', '')
-        string = string.replace('*', r'\w*')
         if regex_variation == -1:
-            regexes.append((re.compile(r'\b{}\b'.format(string), re.I), id_))
+            regexes.append((re.compile(string, re.I), id_))
             continue
 
         if not convert_all:
             # see if string is matched by previously-
             #    created RegEx
             found = False
             for rx, rx_id in regexes:
@@ -133,14 +132,16 @@
                     break
             if found:
                 continue  # Duplicate RegEx was found
 
         length = len(string)
         start_idx = 0  # ensure first letter is unable to change
         orig_string = string
+        if not is_regex:
+            string = re.escape(string, literal_spaces=True)
 
         # 1) convert string to regex
         # a) convert any prefix
         for morph, repl, L, rLen in affixmorphs:
             if morph.match(string):
                 string = morph.sub(repl, string)
                 length -= L
@@ -160,14 +161,16 @@
                 break
         # d) add final elements
         if len(orig_string) > 2:
             if orig_string[-1] == 's':
                 string += r'(es)?'
             elif orig_string[-1] == 'o':
                 string += r'(e?s)?'
+            elif orig_string[-2:] == 's?' or orig_string[-3:] in {r'\w+', r'\w*'}:
+                pass
             else:
                 string += r's?'
 
         # 2) add Error permissions
         length -= 1  # removing the first term
         # FLEXIBLE
         if regex_variation == 3:
@@ -203,9 +206,10 @@
         # 4) compile string to regex
         rx = re.compile(string, re.V1 | re.I)
         # try:
         #     assert rx.match(orig_string)
         # except AssertionError:
         #     raise ValueError(r'Regex {} failed to match original string "{}".'.format(rx, orig_string))
         regexes.append((rx, id_))
+        logger.debug(f'Converted "{orig_string}" to "{string}".')
 
     return regexes, updated_ids
```

### Comparing `pytakes-1.2.1/src/pytakes/nlp/data/ssplit.db` & `pytakes-2.0.0/src/pytakes/nlp/data/ssplit.db`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/nlp/data/status.db` & `pytakes-2.0.0/src/pytakes/nlp/data/status.db`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/nlp/ngrams.py` & `pytakes-2.0.0/src/pytakes/nlp/ngrams.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/nlp/sentence_boundary.py` & `pytakes-2.0.0/src/pytakes/nlp/sentence_boundary.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,14 +69,22 @@
 
         for el in config or []:
             setattr(self, el, self.load_set_lower(config[el]))
 
         self.abbrevs -= self.knuthus  # remove duplicates
         self.ignorecase = ignorecase
         self.debug = debug
+        # compile regexes
+        self.double_start_pat = re.compile(r'\*\*NAME\[.{0,20}\]')
+        self.space_pat = re.compile(r'\s+')
+        self.amp_pat = re.compile(r'&amp;')
+        self.gt_pat = re.compile(r'&gt;|&gt ;|&lt;|&lt ;')
+        self.apostr_pat = re.compile(r'\'s|\'S')
+        self.numlist_pat = re.compile(r'\d+\.$')
+        self.is_digit_pat = re.compile(r'[+-]?\d*[.]?\d+$')
 
     def ssplit(self, text, debug=False):
         # debug outputs print statements
         debug_ = (debug or self.debug)
 
         # sentences = []
         text = self.prepare_text(text)
@@ -101,32 +109,32 @@
                             if self.is_num_list(word):
                                 if j == 0:  # 1. Percocet 5/325 one p.o.
                                     tmp += word + ' '
                                 else:  # postoperative day 3.
                                     tmp += word[:-1] + ' .\n'
                             # afebrile .
                             elif (word[:-1].lower() not in self.abbrevs and
-                                    word.lower() not in self.abbrevs):
+                                  word.lower() not in self.abbrevs):
                                 tmp += (word[:-1] + ' .\n')
                             else:  # abbreviations
                                 if j + 1 < len(words):
                                     nword = words[j + 1]
                                 else:
                                     nword = ''
                                 # elevation MI. The patient was
                                 if (len(nword) > 0 and
                                         self.isupper(nword[0], True) and
-                                    # 1.0 MM. C) LEFT BREAST, ...
-                                    # added by djc 30jul13
+                                        # 1.0 MM. C) LEFT BREAST, ...
+                                        # added by djc 30jul13
                                         (nword.lower() in self.sentence_word or
-                                            (2 <= len(nword) <= 3 and
-                                             nword[0].isalpha() and
-                                             nword[-1] == ')'
-                                             )
-                                         )):
+                                         (2 <= len(nword) <= 3 and
+                                          nword[0].isalpha() and
+                                          nword[-1] == ')'
+                                         )
+                                        )):
                                     tmp += word + '\n'
                                 else:
                                     tmp += word + ' '
                         else:
                             lword, rword = word.split('.')
                             if (self.isupper(rword[0], True) and
                                     (rword in self.sentence_word or
@@ -163,17 +171,17 @@
             if i + 1 < len(text):
                 words = text[i + 1].split()
                 nword = words[0]
                 words = tmp.split()
                 eword = words[-1].lower()
                 # handle 'Page : '
                 if ((len(txt) > 6 and
-                        txt[:6].lower() == 'page :') or
+                     txt[:6].lower() == 'page :') or
                         (len(text[i + 1]) > 6 and
-                            text[i + 1].lower() == 'page :')):
+                         text[i + 1].lower() == 'page :')):
                     text[i] = (tmp.strip() + '\n')
                 elif tmp[-1] == '.':
                     if (len(tmp) >= 2 and
                             tmp[-2] != ' ' and
                             not (nword == '-' or
                                  self.is_num_list(nword) or
                                  self.isupper(nword[0]))):
@@ -224,15 +232,15 @@
     def num_dot(self, word):
         """
         return the number of dot in word
         :param word:
         """
         i = 0
         for w in word:
-            if w == '.' or word[i] == '!' or word[i] == '?' or word[i] == ';':
+            if w == '.' or word[i] in '!?;':
                 i += 1
         return i
 
     def has_dot(self, word):
         """
         Return the position of '.' in a word. -1 denote there are no '.' appeared
         :param word:
@@ -246,93 +254,77 @@
         return - 1
 
     def remove_double_star(self, line):
         """
         Some auto - inserted patterns in discharge summaries
         :param line:
         """
-        pattern1 = r'\*\*NAME\[.{0,20}\]'
-        return re.sub(pattern1, '**NAME**', line)
+        return self.double_start_pat.sub('**NAME**', line)
 
     def prepare_text(self, text):
         """
         Read text in to list,  remove the empty lines
         Parameters:
             text - string of text to be split
         Return:
             result - list of strings from text
             :param text:
         """
-        result = []
-        for line in text.split('\n'):
-            line = line.strip()
-            if len(line) > 0:
-                line = self.remove_double_star(line)
-                line = self.clean(line)
-                line = self.seperate_puncts(line)
-                line = re.sub(r'[ ]+', ' ', line)
-                line = line.strip()
-                if len(line) > 0:
-                    result.append(line)
-        return result
+        return [line for line in (
+            self.space_pat.sub(' ', self.seperate_puncts(self.clean(self.remove_double_star(line.strip()))))
+            for line in text.strip().split('\n')
+        ) if line]
 
     def seperate_puncts(self, line):
         """
         separate punctuations from words,  except '.'
         :param line:
         """
         linee = ''
         for w in line:
             if self.is_punct(w):
                 if len(linee) > 0 and linee[-1] != ' ':
-                    linee = linee + ' ' + w + ' '
+                    linee = f'{linee} {w} '
                 else:
-                    linee = linee + w + ' '
+                    linee = f'{linee}{w} '
             else:
-                linee = linee + w
+                linee = f'{linee}{w}'
         return linee.strip()
 
     def is_digit(self, word):
         """
         Identify all numbers
         :param word:
         """
-        if re.match(r'[+-]?\d*[.]?\d+$', word):  # all number
-            return True
-        return False
+        return self.is_digit_pat.match(word)  # all number
 
     def is_num_list(self, word):
         """
         for list like:  1.   2.
         :param word:
         """
-        if re.match(r'\d+\.$', word):  # num list
-            return True
-        return False
+        return self.numlist_pat.match(word)  # num list
 
     def is_punct(self, w):
         """
         indentify the punctuation
         :param w:
+        NB:  '.' and '+' used in ABBR
         """
-        if w == ',' or w == '?' or w == '!' or w == '"' or w == ';' or w == ':':
-            # '.' and '+' used in ABBR
-            return True
-        else:
-            return False
+        return w in ',?!";:'
 
     def clean(self, sentence):
         """
         Clean text: replace '[ ]+' into '[ ]'; remove '^[ ]+' and '[ ]+$'
         :param sentence:
         """
-        sentence = re.sub(r'&amp;', '&', sentence)
-        sentence = re.sub(r'&gt;|&gt[ ];|&lt;|&lt[ ];', ' ', sentence)
-        sentence = re.sub(r'\'s|\'S', ' \'s', sentence)
-        sentence = re.sub(r'[ ]+', ' ', sentence)
+        sentence = self.amp_pat.sub('&', sentence)
+        sentence = self.gt_pat.sub(' ', sentence)
+        sentence = self.apostr_pat.sub(' \'s', sentence)
+        sentence = self.space_pat.sub(' ', sentence)
         return sentence
 
     def get_ave_len(self, text):
         """
         get the average length of all the lines
         :param text:
         """
@@ -343,11 +335,8 @@
         return avel / lenn
 
     def is_stop_punct(self, w):
         """
         These puncts are definitely a sentence boundary
         :param w:
         """
-        if w == '?' or w == '!' or w == '.' or w == ';':
-            return True
-        else:
-            return False
+        return w in '?!.;'
```

### Comparing `pytakes-1.2.1/src/pytakes/nlp/statusminer.py` & `pytakes-2.0.0/src/pytakes/nlp/statusminer.py`

 * *Files 7% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                     :param text:
                     :param offset:
         """
         negations = []
         # rules already sorted by length of negation expression
         for negex, pattern, _type, direction in self._rules:
             for m in pattern.finditer(text):
-                n = Negation(negex, m.start(), m.end(), _type=_type, direction=direction, offset=offset)
+                n = Negation(negex, m.start(), m.end(), kind=_type, direction=direction, offset=offset)
                 # longer sequences will trump smaller ones
                 if n not in negations:
                     negations.append(n)
         return negations
 
     # noinspection PyPep8Naming
     def postprocess(self, terms):
@@ -195,19 +195,19 @@
         STRING = 4
 
         def found_term(ind, term_):
             """ updates ind[icator] when a term is found
             :param ind:
             :param _type:
             """
-            ind[TYPE] = term_.type()
+            ind[TYPE] = term_.kind
             ind[STATUS] = 1
             ind[OVERLAP] = 0
             ind[COUNTER] = 0
-            ind[STRING] = term_.word()
+            ind[STRING] = term_.word
 
         def overlap_term(ind):
             """ updates ind[icator] when overlap found
             :param ind:
             """
             ind[OVERLAP] = 1
 
@@ -224,75 +224,69 @@
             negtype = ['', 0, 0, 0, None]
             hypotype = ['', 0, 0, 0, None]
             temptype = ['', 0, 0, 0, None]
             subjtype = ['', 0, 0, 0, None]
             types = [negtype, hypotype, temptype, subjtype]
             for idx, term in enumerate(sentence):
 
-                if term.direction() in directions:
-                    if term.type() in self.NEGATION_TAGS:
+                if term.direction in directions:
+                    if term.kind in self.NEGATION_TAGS:
                         found_term(negtype, term)
-                    elif term.type() in self.HYPOTHETICAL_TAGS:
+                    elif term.kind in self.HYPOTHETICAL_TAGS:
                         found_term(hypotype, term)
-                    elif term.type() in self.TEMPORAL_TAGS:
+                    elif term.kind in self.TEMPORAL_TAGS:
                         found_term(temptype, term)
-                    elif term.type() in self.SUBJECT_TAGS:
+                    elif term.kind in self.SUBJECT_TAGS:
                         found_term(subjtype, term)
 
-                elif term.type() in self.STOP_TAGS:
+                elif term.kind in self.STOP_TAGS:
                     for _type in types:
                         overlap_term(_type)
 
-                elif term.type() in self.NEGATION_TAGS:
+                elif term.kind in self.NEGATION_TAGS:
                     overlap_term(negtype)
 
-                elif term.type() in self.TEMPORAL_TAGS:
+                elif term.kind in self.TEMPORAL_TAGS:
                     overlap_term(temptype)
 
-                elif term.type() in self.HYPOTHETICAL_TAGS:
+                elif term.kind in self.HYPOTHETICAL_TAGS:
                     overlap_term(hypotype)
 
-                elif term.type() in self.SUBJECT_TAGS:
+                elif term.kind in self.SUBJECT_TAGS:
                     overlap_term(subjtype)
 
                 else:
                     for _type in types:
                         _type[COUNTER] += 1
 
                 # check if term should be updated with any types
                 for _type in types:
                     if _type[STATUS] == 1 and _type[OVERLAP] == 0 and _type[COUNTER] <= self._maxscope:
                         # ignoring affirmation tag (affm)
                         if _type[TYPE] == 'negn':
                             term.negate(_type[STRING])
                         elif _type[TYPE] == 'impr':
-                            term.improbable(_type[STRING])
+                            term.set_improbable(_type[STRING])
                         elif _type[TYPE] == 'poss':
-                            term.possible(_type[STRING])
+                            term.set_possible(_type[STRING])
                         elif _type[TYPE] == 'prob':
-                            term.probable(_type[STRING])
+                            term.set_probable(_type[STRING])
                         if _type[TYPE] == 'hypo':
-                            term.hypothetical(_type[STRING])
+                            term.set_hypothetical(_type[STRING])
                         if _type[TYPE] == 'futp':
-                            term.hypothetical(_type[STRING])
+                            term.set_hypothetical(_type[STRING])
                         if _type[TYPE] == 'hist':
-                            term.historical(_type[STRING])
+                            term.set_historical(_type[STRING])
                         if _type[TYPE] == 'othr':
-                            term.other_subject(_type[STRING])
+                            term.set_other_subject(_type[STRING])
 
             return sentence
             # end inner function
 
-        # check all FORWARD (direction=2 or 3)
-        sentence = analyze_direction(terms, [2, 3])
-
-        # reverse and check all BACKWARD/BIDIRECTIONAL (1 or 3)      
-        sentence.reverse()  # reverse sentence
-        sentence = analyze_direction(terms, [1, 3])
-
-        # put sentence back in correct order
-        sentence.reverse()  # sentence correctly ordered
-
+        sentence = analyze_direction(terms, {2, 3})  # check Forward, bidirectional
+        sentence.reverse()  # reverse sentence to check BACKWARD
+        sentence = analyze_direction(sentence, {1, 3})  # check backward, bidirectional
+        sentence.reverse()  # sentence back into correct order
         return sentence
 
     def clean(self, text):
         return text
```

### Comparing `pytakes-1.2.1/src/pytakes/nlp/terms.py` & `pytakes-2.0.0/src/pytakes/nlp/terms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,222 +1,183 @@
 """
 
 
 Edit:
     2013-11-26    added direction, probability, hypothetical, etc. to Word and children
 """
-
+import re
 from functools import total_ordering
 
+from regex import Pattern
+
 
 @total_ordering
 class Word(object):
-    def __init__(self, word, begin, end, _type='term', offset=0):
-        self.word_ = word
-        self.begin_ = begin
-        self.end_ = end
-        self.type_ = _type.lower()
-        self.offset_ = offset
-        self.certainty_ = 4  # 0-4 (neg to affm)
-        self.hypothetical_ = False  # for status only
-        self.other_ = False  # for status only
-        self.historical_ = False  # for status only
-        self.direction_ = 0
-        self.qualifiers = []
-
-    def get_absolute_begin(self):
-        return self.begin() + self.offset_
-
-    def get_absolute_end(self):
-        return self.end() + self.offset_
-
-    def is_negated(self, normal=True):
-        if normal:
-            return self.certainty_ == 0
+    __slots__ = ['word', 'begin', 'end', 'kind', 'offset',
+                 'certainty', 'hypothetical', 'other', 'historical',
+                 'direction', 'qualifiers']
+
+    def __init__(self, word, begin, end, kind='term', offset=0):
+        if isinstance(word, Pattern):
+            self.word = word.pattern
         else:
-            return not self.negated_
-
-    def is_improbable(self):
-        return self.certainty_ == 1
-
-    def is_possible(self):
-        return self.certainty_ == 2
-
-    def is_probable(self):
-        return self.certainty_ == 3
-
-    def is_affirmed(self):
-        return self.certainty_ == 4
-
-    def get_certainty(self):
-        return self.certainty_
-
-    def set_certainty(self, level):
-        self.certainty_ = level
-
-    def is_hypothetical(self):
-        return self.hypothetical_
-
-    def is_historical(self):
-        return self.historical_
+            self.word = str(word)
+        self.begin = begin
+        self.end = end
+        self.kind = kind.lower()
+        self.offset = offset
+        self.certainty = 4  # 0-4 (neg to affm)
+        self.hypothetical = False  # for status only
+        self.other = False  # for status only
+        self.historical = False  # for status only
+        self.direction = 0
+        self.qualifiers = []
 
-    def is_not_patient(self):
-        return self.other_
+    @property
+    def absolute_begin(self):
+        return self.begin + self.offset
+
+    @property
+    def absolute_end(self):
+        return self.end + self.offset
+
+    @property
+    def negated(self):
+        return self.certainty == 0
+
+    @property
+    def improbable(self):
+        return self.certainty == 1
+
+    @property
+    def possible(self):
+        return self.certainty == 2
+
+    @property
+    def probable(self):
+        return self.certainty == 3
+
+    @property
+    def affirmed(self):
+        return self.certainty == 4
 
     def negate(self, qualifier=None):
-        self.certainty_ = 0
+        self.certainty = 0
         if qualifier:
             self.qualifiers.append(qualifier)
 
-    def improbable(self, qualifier=None):
-        if self.certainty_ > 1:  # added 20140109
-            self.certainty_ = 1
+    def set_improbable(self, qualifier=None):
+        if self.certainty > 1:  # added 20140109
+            self.certainty = 1
             if qualifier:
                 self.qualifiers.append(qualifier)
 
-    def possible(self, qualifier=None):
-        if self.certainty_ > 2:  # added 20140109
-            self.certainty_ = 2
+    def set_possible(self, qualifier=None):
+        if self.certainty > 2:  # added 20140109
+            self.certainty = 2
             if qualifier:
                 self.qualifiers.append(qualifier)
 
-    def probable(self, qualifier=None):
-        if self.certainty_ > 3:  # added 20140109
-            self.certainty_ = 3
+    def set_probable(self, qualifier=None):
+        if self.certainty > 3:  # added 20140109
+            self.certainty = 3
             if qualifier:
                 self.qualifiers.append(qualifier)
 
-    def hypothetical(self, qualifier=None):
-        self.hypothetical_ = True
+    def set_hypothetical(self, qualifier=None):
+        self.hypothetical = True
         if qualifier:
             self.qualifiers.append(qualifier)
 
-    def historical(self, qualifier=None):
-        self.historical_ = True
+    def set_historical(self, qualifier=None):
+        self.historical = True
         if qualifier:
             self.qualifiers.append(qualifier)
 
-    def other_subject(self, qualifier=None):
-        self.other_ = True
+    def set_other_subject(self, qualifier=None):
+        self.other = True
         if qualifier:
             self.qualifiers.append(qualifier)
 
-    def direction(self):
-        return self.direction_
-
-    def begin(self):
-        return self.begin_
-
-    def set_begin(self, begin):
-        self.begin_ = begin
-
-    def end(self):
-        return self.end_
-
-    def set_end(self, end):
-        self.end_ = end
-
-    def word(self):
-        return str(self.word_)
-
-    def type(self):
-        return self.type_
-
     def __len__(self):
-        return self.end_ - self.begin_
+        return self.end - self.begin
 
     ''' Comparisons defined by relative location
         in the sentence. First term < last term. '''
 
     def __gt__(self, other):
-        return self.begin_ > other.begin_ and self.end_ > other.end_  # must account for eq implementation
+        return self.begin > other.begin and self.end > other.end  # must account for eq implementation
 
     def __eq__(self, other):
         """ equal if any overlap in indices """
-        return (self.begin_ == other.begin_ or
-                self.end_ == other.end_ or
-                (self.begin_ > other.begin_ and self.end_ < other.end_) or
-                (self.begin_ < other.begin_ and self.end_ > other.end_)
+        return (self.begin == other.begin or
+                self.end == other.end or
+                (self.begin > other.begin and self.end < other.end) or
+                (self.begin < other.begin and self.end > other.end)
                 )
 
     def __unicode__(self):
-        return str(self.word_)
+        return str(self.word)
 
     def __str__(self):
         return str(self).encode('utf-8')
 
     def __repr__(self):
-        return ('<' + str(self.word_) + ',' + str(self.begin_) + ':' +
-                str(self.end_) +
-                (',NEG' if self.is_negated() else ',POS' if self.is_possible else '') +
-                ', <' + self.type_ + '>>')
+        return ('<' + str(self.word) + ',' + str(self.begin) + ':' +
+                str(self.end) +
+                (',NEG' if self.negated else ',POS' if self.possible else '') +
+                ', <' + self.kind + '>>')
 
 
 class Term(Word):
-    def __init__(self, word, begin, end, _type, id_, offset=0):
-        super(Term, self).__init__(word, begin, end, _type, offset)
-        self.id_ = id_
+    __slots__ = ['id']
 
-    def id(self):
-        return self.id_
+    def __init__(self, word, begin, end, kind, id_, offset=0):
+        super(Term, self).__init__(word, begin, end, kind, offset)
+        self.id = id_
 
     def id_as_list(self):
-        if isinstance(self.id_, list):
-            return self.id_
-        else:
-            return [self.id_]
+        return self.id if isinstance(self.id, list) else [self.id]
 
     def add_term(self, other):
-        self.id_ = self.id_as_list() + other.id_as_list()
+        self.id = self.id_as_list() + other.id_as_list()
 
 
 class Concept(Term):
+    __slots__ = ['cat']
+
     def __init__(self, word, begin, end, id_, cat, certainty=4,
                  hypothetical=0, historical=0, not_patient=0, offset=0,
                  qualifiers=None):
         """
         For backwards compatibility:
             certainty used to be neg(ated), boolean
             hypothetical used to be pos(sible), boolean
         """
-        super(Concept, self).__init__(word, begin, end, "concept", id_, offset=offset)
-        self.cat_ = cat
-
-        if isinstance(certainty, bool):  # old way
-            neg = certainty
-            pos = hypothetical
-            if neg:
-                self.negate()
-            if pos:
-                self.possible()
-
-        else:  # new way
-            self.set_certainty(certainty)
-            if hypothetical:
-                self.hypothetical()
-            if historical:
-                self.historical()
-            if not_patient:
-                self.other_subject()
+        super(Concept, self).__init__(word, begin, end, 'concept', id_, offset=offset)
+        self.cat = cat
+        self.certainty = certainty
+        self.hypothetical = hypothetical
+        self.historical = historical
+        self.other = not_patient
         self.qualifiers = qualifiers or []
 
-    def cat(self):
-        return self.cat_
-
 
 class Negation(Word):
-    def __init__(self, word, begin, end, _type='negn', direction=0, offset=0):
-        super(Negation, self).__init__(word, begin, end, _type, offset=offset)
-        self.direction_ = direction
+    __slots__ = ['direction']
+
+    def __init__(self, word, begin, end, kind='negn', direction=0, offset=0):
+        super(Negation, self).__init__(word, begin, end, kind, offset=offset)
+        self.direction = direction
         self.negate()
 
 
 def find_terms(terms, text, offset=0):
     """
-    Paramters:
+    Parameters:
         terms - list of (term,id) where unique id for each term
         :param terms:
         :param text:
         :param offset:
     """
     results = []
     for term, id_ in terms:
@@ -238,15 +199,15 @@
     while True:
         if terms[curr] == terms[i]:
             if len(terms[curr]) > len(terms[i]):
                 del terms[i]
             elif len(terms[curr]) < len(terms[i]):
                 del terms[curr]
                 curr = i - 1
-            elif terms[curr].begin() == terms[i].begin() and terms[curr].end() == terms[i].end():
+            elif terms[curr].begin == terms[i].begin and terms[curr].begin == terms[i].begin:
                 terms[curr].add_term(terms[i])
                 del terms[i]
             else:  # keep both representations
                 curr = i
                 i += 1
         else:
             curr = i
@@ -266,14 +227,13 @@
     :param terms:
     :param text:
     :param offset:
     """
     curr = 0
     words = []
     for term in sorted(terms):
-        if term.begin() > curr:
-            for word in text[curr:term.begin()].split():
+        if term.begin > curr:
+            for word in text[curr:term.begin].split():
                 words.append(Word(word, curr + 1, curr + 1 + len(word), offset=offset))
                 curr = curr + 1 + len(word)
-        curr = term.end()
-    # ignoring extraneous words at end of sentence
+        curr = term.end
     return words
```

### Comparing `pytakes-1.2.1/src/pytakes/nlp/utils.py` & `pytakes-2.0.0/src/pytakes/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/parser.py` & `pytakes-2.0.0/src/pytakes/parser.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/postprocessor.py` & `pytakes-2.0.0/src/pytakes/postprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                     new_row.append(el)
                 else:
                     new_row.append(el.encode('utf-8').decode('utf-8', 'ignore'))
             row = new_row
             text = row[col_idx]
             orig_row = copy.copy(row)
             for negConcept in tagger.find_negation(text):
-                _type = negConcept.type().lower()
+                _type = negConcept.kind.lower()
                 if _type == header.NEGATION_TYPE:
                     row[out_columns.index(header.CERTAINTY)] = 0
                 elif _type == header.IMPROBABLE_TYPE:
                     row[out_columns.index(header.CERTAINTY)] = 1
                 elif _type == header.POSSIBLE_TYPE:
                     row[out_columns.index(header.CERTAINTY)] = 2
                 elif _type == header.PROBABLE_TYPE:
```

### Comparing `pytakes-1.2.1/src/pytakes/processor.py` & `pytakes-2.0.0/src/pytakes/processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         for num, doc in enumerate(document.read_next()):
             if num % 100 == 0:
                 logging.info(f'Completed: {num:>5}.')
 
             for sent_no, (sentence, cleaned_text) in enumerate(mc.parse(doc)):
                 for feat, new in sentence:
                     for out in outputs:
-                        out.writerow(doc.get_metalist(), feat, text=doc.get_text())
+                        out.writerow(doc.meta, feat, text=doc.text)
     logging.info('Completed: 100%')
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('-j', '--json-config',
                         help='Json file containing configuration information.')
```

### Comparing `pytakes-1.2.1/src/pytakes/run/runner.py` & `pytakes-2.0.0/src/pytakes/run/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from datetime import datetime
 from typing import List
 
+from loguru import logger
+
 from pytakes import MinerCollection, SentenceBoundary
 from pytakes.corpus import get_next_from_corpus
 from pytakes.dict.textitem import process_textitem
 from pytakes.run.schema import validate_config
 from pytakes.run.simple_run import load_keywords, load_negation, output_context_manager
 
 
-def run(corpus=None, output=None, keywords: List = None, negation=None, logger=None):
+def run(corpus=None, output=None, keywords: List = None, negation=None, log=None):
     """
 
     :return:
     """
+    if log and log.get('file', None):
+        logger.add(log['file'], level=log.get('level', 'DEBUG'))
     mc = MinerCollection(ssplit=SentenceBoundary().ssplit)
     mc.add(load_keywords(*keywords))
     mc.add(load_negation(**negation))
     default_output = {
         'outfile': 'extracted_concepts_{}.jsonl'.format(datetime.now().strftime('%Y%m%d_%H%M%S')),
         'metalabels': ['file'],
     }
     with output_context_manager(**{**default_output, **output}) as out:
-        for i, ti in enumerate(get_next_from_corpus(**corpus)):
+        for i, ti in enumerate(get_next_from_corpus(**corpus), start=1):
             for results, sent in process_textitem(ti, mc):
                 for result in results:
                     out.writerow(result, meta=list(ti.meta.values()), text=sent)
+            if i % 10000 == 0:
+                logger.info(f'Completed processing of {i} records.')
 
 
 def run_config(config_file):
     run(**validate_config(config_file))
```

### Comparing `pytakes-1.2.1/src/pytakes/run/schema.py` & `pytakes-2.0.0/src/pytakes/run/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
                 'type': 'object',
                 'properties': {
                     'path': {'type': 'string'},
                     'regex_variation': {'type': 'integer'},  # -1 to 3
                     'word_order': {'type': 'integer'},
                     'max_search': {'type': 'integer'},
                     'max_intervening': {'type': 'integer'},
+                    'is_regex': {'type': 'boolean'},
+                    'convert_all': {'type': 'boolean'},
                 }
             }
         },
         'negation': {
             'type': 'object',
             'properties': {
                 'version': {'type': 'integer'},  # built-in version
@@ -63,20 +65,21 @@
             'type': 'object',
             'properties': {
                 'outfile': {'type': 'string'},
                 'path': {'type': 'string'},
                 'hostname': {'type': 'string'},
             }
         },
-        'logger': {
+        'log': {
             'type': 'object',
             'properties': {
-                'verbose': {'type': 'boolean'}
+                'level': {'type': 'string'},
+                'file': {'type': 'string'},  # 'INFO', 'DEBUG', 'WARN'
             }
-        }
+        },
     }
 }
 
 
 def myexec(code):
     import warnings
     warnings.warn('Executing python external file: only do this if you trust it')
```

### Comparing `pytakes-1.2.1/src/pytakes/run/simple_run.py` & `pytakes-2.0.0/src/pytakes/run/simple_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from datetime import datetime
 
+from loguru import logger
+
 from pytakes import CsvDictionary, CsvOutput, JsonlOutput
 from pytakes import ConceptMiner, SentenceBoundary, MinerCollection, StatusMiner
 from pytakes.corpus import get_next_from_corpus
 from pytakes.dict.textitem import process_textitem
 
 
 def output_context_manager(outfile, **kwargs):
@@ -11,16 +13,16 @@
         return JsonlOutput(outfile, **kwargs)
     elif outfile.endswith('csv'):
         return CsvOutput(outfile, **kwargs)
     else:
         raise ValueError(f'Unrecognized file type: {outfile}')
 
 
-def load_keywords(*paths):
-    return ConceptMiner([CsvDictionary(**file) for file in paths])
+def load_keywords(*paths, is_regex=True, convert_all=True):
+    return ConceptMiner([CsvDictionary(**file) for file in paths], is_regex=is_regex, convert_all=convert_all)
 
 
 def load_negation(version=None, path=None, skip=False, variation=0):
     if skip:
         return None
     elif path:  # requirement: must precede version as sometimes 'path' is always specified
         return StatusMiner(path=path, rx_var=variation)
@@ -46,18 +48,21 @@
     """
     mc = MinerCollection(ssplit=SentenceBoundary().ssplit)
     mc.add(load_keywords(*({'path': path} for path in keyword_files)))
     mc.add(load_negation(negex_version, negex_path, skip=skip_negex))
     if not outfile:
         outfile = 'extracted_concepts_{}.jsonl'.format(datetime.now().strftime('%Y%m%d_%H%M%S'))
     with output_context_manager(outfile, path=output_dir, metalabels=['file'], hostname=hostname) as out:
-        for ti in get_next_from_corpus(input_dir):
+        for i, ti in enumerate(get_next_from_corpus(input_dir), start=1):
             for results, sent in process_textitem(ti, mc):
                 for result in results:
                     out.writerow(result, meta=list(ti.meta.values()), text=sent)
+            if i % 10000 == 0:
+                logger.info(f'Completed processing of {i} records.')
+
 
 
 if __name__ == '__main__':
     import argparse
 
     parser = argparse.ArgumentParser(fromfile_prefix_chars='@')
     parser.add_argument('-i', '--input-dir', dest='input_dir', required=True)
```

### Comparing `pytakes-1.2.1/src/pytakes/sendmail.py` & `pytakes-2.0.0/src/pytakes/sendmail.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/templates.py` & `pytakes-2.0.0/src/pytakes/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,24 +139,24 @@
 {%- for label in labels %}
 {{ label }}{% if not loop.last %},{% endif %}
 {%- endfor %}
 ) VALUES (
 {%- for meta in metas %}
 '{{ meta|replace("'", "''") }}',
 {%- endfor %}
-{{ feature.id() }},
+{{ feature.id }},
 '{{ captured|replace("'", "''") }}',
 '{{ context|replace("'", "''") }}',
 '{{ text|replace("'", "''") }}',
-{{ feature.get_certainty() }},
-{% if feature.is_hypothetical() %}1{% else %}0{% endif %},
-{% if feature.is_historical() %}1{% else %}0{% endif %},
-{% if feature.is_hypothetical() %}1{% else %}0{% endif %},
-{{ feature.begin() }},
-{{ feature.end() }},
+{{ feature.certainty }},
+{% if feature.hypothetical %}1{% else %}0{% endif %},
+{% if feature.historical %}1{% else %}0{% endif %},
+{% if feature.hypothetical %}1{% else %}0{% endif %},
+{{ feature.begin }},
+{{ feature.begin }},
 {{ feature.get_absolute_begin() }},
 {{ feature.get_absolute_end() }}
 {% if hostname %}, '{{ hostname|replace("'", "''") }}', {{ batch_number }}{% endif %}
 )
 '''
 
 PROC_INSERT_INTO3_QUERY = r'''INSERT INTO {{ destination_table }} (
```

### Comparing `pytakes-1.2.1/src/pytakes/util/db_reader.py` & `pytakes-2.0.0/src/pytakes/util/db_reader.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/util/email_utils.py` & `pytakes-2.0.0/src/pytakes/util/email_utils.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/util/mylogger.py` & `pytakes-2.0.0/src/pytakes/util/mylogger.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/src/pytakes/util/utils.py` & `pytakes-2.0.0/src/pytakes/util/utils.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/tests/data/config/run.config.py` & `pytakes-2.0.0/tests/data/config/run.config.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/tests/data/files/file1.txt` & `pytakes-2.0.0/tests/data/files/file1.txt`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/tests/data/files/file2.txt` & `pytakes-2.0.0/tests/data/files/file2.txt`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/tests/data/files/file3.txt` & `pytakes-2.0.0/tests/data/files/file3.txt`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/tests/data/testout/expected.csv` & `pytakes-2.0.0/tests/data/testout/expected.csv`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 file1,0,WRITING,letter,"ng , and Miss Bingley , seated near him , was watching the progress of his letter , and repeatedly calling off his attention by messages to his sister .",4,False,False,True,76277,76283,Eumaeus,
 file1,0,WRITING,letter,"s hand-writing , or on the evenness of his lines , or on the length of his letter , with the perfect unconcern with which her praises were received , formed",4,False,False,False,76690,76696,Eumaeus,
 file1,0,WRITING,letter,""" How delighted Miss Darcy will be to receive such a letter !",4,False,False,False,76898,76904,Eumaeus,
 file1,0,WRITING,letters,""" How many letters you must have occasion to write in the course of the year !",4,False,False,False,77014,77021,Eumaeus,
 file1,0,WRITING,Letters,Letters of business too !,4,False,False,False,77081,77088,Eumaeus,
 file1,1,WRITING,pen,""" I am afraid you do not like your pen .",0,True,False,False,77354,77357,Eumaeus,
 file1,1,WRITING,pens,I mend pens remarkably well .,4,False,False,False,77390,77394,Eumaeus,
+file1,0,WRITING,letters,"But do you always write such charming long letters to her , Mr. Darcy ?",4,False,False,False,77964,77971,Eumaeus,
 file1,0,WRITING,letter,""" It is a rule with me , that a person who can write a long letter , with ease , cannot write ill .",4,False,False,False,78144,78150,Eumaeus,
 file1,0,WRITING,letters,as flow so rapidly that I have not time to express them--by which means my letters sometimes convey no ideas at all to my correspondents .,4,False,False,False,78651,78658,Eumaeus,
 file1,0,WRITING,letter,and Mr. Darcy had much better finish his letter .,4,False,False,False,83983,83989,Eumaeus,
 file1,0,WRITING,letter,"Mr. Darcy took her advice , and did finish his letter .",4,False,False,False,84040,84046,Eumaeus,
 file2,5,WEATHER,weather,"llers of the heavy lands adjacent to Paris , there were sheltered from the weather that very day , rude carts , bespattered with rustic mire , snuffed about ",3,False,False,False,2897,2904,Eumaeus,
 file2,5,WEATHER,weather,""" Yes , sir , if the weather holds and the wind sets tolerable fair .",4,True,False,False,27273,27280,Eumaeus,
+file2,0,WRITING,letter,""" I received a letter from the Bank , sir , yesterday , informing me that some intelligence--or ",4,False,False,False,36459,36465,Eumaeus,
 file3,0,WRITING,letter,"There is a letter , written in the name of the church over which he himself presided , to th",4,False,False,False,247,253,Eumaeus,
 file3,4,FATHER,his father,"And he was met by Herod , the captain of police , and by his father Nicetes , who took him into their carriage , and sitting beside him endeav",4,False,False,True,5576,5586,Eumaeus,
```

### Comparing `pytakes-1.2.1/tests/data/testout/expected.jsonl` & `pytakes-2.0.0/tests/data/testout/expected.jsonl`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "ng , and Miss Bingley , seated near him , was watching the progress of his letter , and repeatedly calling off his attention by messages to his sister .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": true, "terms": ["sister"]}, "start_index": 76277, "end_index": 76283, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "s hand-writing , or on the evenness of his lines , or on the length of his letter , with the perfect unconcern with which her praises were received , formed", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 76690, "end_index": 76696, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "\" How delighted Miss Darcy will be to receive such a letter !", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 76898, "end_index": 76904, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letters", "context": "\" How many letters you must have occasion to write in the course of the year !", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77014, "end_index": 77021, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "Letters", "context": "Letters of business too !", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77081, "end_index": 77088, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "1", "concept": "WRITING", "captured": "pen", "context": "\" I am afraid you do not like your pen .", "qualifiers": {"certainty": 0, "hypothetical": true, "historical": false, "other_subject": false, "terms": ["not", "afraid"]}, "start_index": 77354, "end_index": 77357, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "1", "concept": "WRITING", "captured": "pens", "context": "I mend pens remarkably well .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77390, "end_index": 77394, "tracking": {"hostname": "Eumaeus", "batch": null}}
+{"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letters", "context": "But do you always write such charming long letters to her , Mr. Darcy ?", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77964, "end_index": 77971, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "\" It is a rule with me , that a person who can write a long letter , with ease , cannot write ill .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 78144, "end_index": 78150, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letters", "context": "as flow so rapidly that I have not time to express them--by which means my letters sometimes convey no ideas at all to my correspondents .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 78651, "end_index": 78658, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "and Mr. Darcy had much better finish his letter .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 83983, "end_index": 83989, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "Mr. Darcy took her advice , and did finish his letter .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 84040, "end_index": 84046, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file2"], "concept_id": "5", "concept": "WEATHER", "captured": "weather", "context": "llers of the heavy lands adjacent to Paris , there were sheltered from the weather that very day , rude carts , bespattered with rustic mire , snuffed about ", "qualifiers": {"certainty": 3, "hypothetical": false, "historical": false, "other_subject": false, "terms": ["likely"]}, "start_index": 2897, "end_index": 2904, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file2"], "concept_id": "5", "concept": "WEATHER", "captured": "weather", "context": "\" Yes , sir , if the weather holds and the wind sets tolerable fair .", "qualifiers": {"certainty": 4, "hypothetical": true, "historical": false, "other_subject": false, "terms": ["if"]}, "start_index": 27273, "end_index": 27280, "tracking": {"hostname": "Eumaeus", "batch": null}}
+{"meta": ["file2"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "\" I received a letter from the Bank , sir , yesterday , informing me that some intelligence--or ", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 36459, "end_index": 36465, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file3"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "There is a letter , written in the name of the church over which he himself presided , to th", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 247, "end_index": 253, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file3"], "concept_id": "4", "concept": "FATHER", "captured": "his father", "context": "And he was met by Herod , the captain of police , and by his father Nicetes , who took him into their carriage , and sitting beside him endeav", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": true, "terms": ["father", "father"]}, "start_index": 5576, "end_index": 5586, "tracking": {"hostname": "Eumaeus", "batch": null}}
```

### Comparing `pytakes-1.2.1/tests/data/testout/expected.negex.jsonl` & `pytakes-2.0.0/tests/data/testout/expected.negex.jsonl`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "ng , and Miss Bingley , seated near him , was watching the progress of his letter , and repeatedly calling off his attention by messages to his sister .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 76277, "end_index": 76283, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "s hand-writing , or on the evenness of his lines , or on the length of his letter , with the perfect unconcern with which her praises were received , formed", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 76690, "end_index": 76696, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "\" How delighted Miss Darcy will be to receive such a letter !", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 76898, "end_index": 76904, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letters", "context": "\" How many letters you must have occasion to write in the course of the year !", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77014, "end_index": 77021, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "Letters", "context": "Letters of business too !", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77081, "end_index": 77088, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "1", "concept": "WRITING", "captured": "pen", "context": "\" I am afraid you do not like your pen .", "qualifiers": {"certainty": 0, "hypothetical": false, "historical": false, "other_subject": false, "terms": ["not"]}, "start_index": 77354, "end_index": 77357, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "1", "concept": "WRITING", "captured": "pens", "context": "I mend pens remarkably well .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77390, "end_index": 77394, "tracking": {"hostname": "Eumaeus", "batch": null}}
+{"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letters", "context": "But do you always write such charming long letters to her , Mr. Darcy ?", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 77964, "end_index": 77971, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "\" It is a rule with me , that a person who can write a long letter , with ease , cannot write ill .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 78144, "end_index": 78150, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letters", "context": "as flow so rapidly that I have not time to express them--by which means my letters sometimes convey no ideas at all to my correspondents .", "qualifiers": {"certainty": 0, "hypothetical": false, "historical": false, "other_subject": false, "terms": ["not", "no"]}, "start_index": 78651, "end_index": 78658, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "and Mr. Darcy had much better finish his letter .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 83983, "end_index": 83989, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file1"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "Mr. Darcy took her advice , and did finish his letter .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 84040, "end_index": 84046, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file2"], "concept_id": "5", "concept": "WEATHER", "captured": "weather", "context": "llers of the heavy lands adjacent to Paris , there were sheltered from the weather that very day , rude carts , bespattered with rustic mire , snuffed about ", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 2897, "end_index": 2904, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file2"], "concept_id": "5", "concept": "WEATHER", "captured": "weather", "context": "\" Yes , sir , if the weather holds and the wind sets tolerable fair .", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 27273, "end_index": 27280, "tracking": {"hostname": "Eumaeus", "batch": null}}
+{"meta": ["file2"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "\" I received a letter from the Bank , sir , yesterday , informing me that some intelligence--or ", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 36459, "end_index": 36465, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file3"], "concept_id": "0", "concept": "WRITING", "captured": "letter", "context": "There is a letter , written in the name of the church over which he himself presided , to th", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 247, "end_index": 253, "tracking": {"hostname": "Eumaeus", "batch": null}}
 {"meta": ["file3"], "concept_id": "4", "concept": "FATHER", "captured": "his father", "context": "And he was met by Herod , the captain of police , and by his father Nicetes , who took him into their carriage , and sitting beside him endeav", "qualifiers": {"certainty": 4, "hypothetical": false, "historical": false, "other_subject": false, "terms": []}, "start_index": 5576, "end_index": 5586, "tracking": {"hostname": "Eumaeus", "batch": null}}
```

### Comparing `pytakes-1.2.1/tests/test_load_negex.py` & `pytakes-2.0.0/tests/test_load_negex.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/tests/test_negation.py` & `pytakes-2.0.0/tests/test_negation.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,42 +8,42 @@
     terms = [
         Term('I', 0, 1, 'C01', 1),
         Word('have', 2, 6),
         Negation('no', 7, 9, 'negn', 3),
         Term('beer', 10, 14, 'C02', 2),
     ]
     miner.postprocess(terms)
-    assert terms[0].is_negated()
-    assert terms[-1].is_negated()
+    assert terms[0].negated
+    assert terms[-1].negated
 
 
 def test_negation_forward():
     miner = StatusMiner(rules=[])
     terms = [
         Term('I', 0, 1, 'C01', 1),
         Word('have', 2, 6),
         Negation('no', 7, 9, 'negn', 2),
         Term('beer', 10, 14, 'C02', 2),
     ]
     miner.postprocess(terms)
-    assert not terms[0].is_negated()
-    assert terms[-1].is_negated()
+    assert not terms[0].negated
+    assert terms[-1].negated
 
 
 def test_negation_backward():
     miner = StatusMiner(rules=[])
     terms = [
         Term('I', 0, 1, 'C01', 1),
         Word('have', 2, 6),
         Negation('no', 7, 9, 'negn', 1),
         Term('beer', 10, 14, 'C02', 2),
     ]
     miner.postprocess(terms)
-    assert terms[0].is_negated()
-    assert not terms[-1].is_negated()
+    assert terms[0].negated
+    assert not terms[-1].negated
 
 
 def test_negation_with_punct():
     miner = StatusMiner(rules=[('c/o', 'negn', 3)])
     assert len(miner.mine('pt c/o', 0)) == 1
     assert len(miner.mine('pt c / o', 0)) == 0
 
@@ -67,22 +67,22 @@
         Word('have', 2, 6),
         Negation('no', 7, 9, 'negn', 3),
         Term('beer', 10, 14, 'C02', 2),
         Negation('or', 15, 17, 'conj', 0),
         Term('wine', 18, 22, 'C02', 3),
     ]
     miner.postprocess(terms)
-    assert terms[0].is_negated()
-    assert terms[-3].is_negated()  # negates 'beer'
-    assert not terms[-1].is_negated()  # 'or' blocks 'wine' from being negated
+    assert terms[0].negated
+    assert terms[-3].negated  # negates 'beer'
+    assert not terms[-1].negated  # 'or' blocks 'wine' from being negated
 
 
 def test_default_negation():
     ti = TextItem(['I am not happy.'])
     mc = MinerCollection()
     mc.add(ConceptMiner([TxtDictionary('happy', 'sad')]))
     mc.add(StatusMiner())
     concepts = [found for found, sentence in process_textitem(ti, mc)][0]
     assert len(concepts) == 1  # 'happy'
-    assert concepts[0].type_ == 'concept'
-    assert concepts[0].get_certainty() == 0
+    assert concepts[0].kind == 'concept'
+    assert concepts[0].certainty == 0
     assert concepts[0].qualifiers == ['not']
```

### Comparing `pytakes-1.2.1/tests/test_simple_run.py` & `pytakes-2.0.0/tests/test_simple_run.py`

 * *Files identical despite different names*

### Comparing `pytakes-1.2.1/tests/test_statusminer.py` & `pytakes-2.0.0/tests/test_statusminer.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 def test_negated_sentence(concept_file):
     mc = MinerCollection()
     mc.add(ConceptMiner([CsvDictionary(concept_file)]))
     mc.add(StatusMiner())
     concepts, sentence = mc.parse_sentence('no bad weather', offset=0)
     for concept in concepts:
-        assert concept.is_negated()
+        assert concept.negated
 
 
 def test_improbable_sentence(concept_file):
     mc = MinerCollection()
     mc.add(ConceptMiner([CsvDictionary(concept_file)]))
     mc.add(StatusMiner())
     concepts, sentence = mc.parse_sentence('no evidence of bad weather', offset=0)
     for concept in concepts:
-        assert concept.is_improbable()
+        assert concept.improbable
 
 
 def test_hypothetical_sentence(concept_file):
     mc = MinerCollection()
     mc.add(ConceptMiner([CsvDictionary(concept_file)]))
     mc.add(StatusMiner())
     concepts, sentence = mc.parse_sentence('if there is bad weather', offset=0)
     for concept in concepts:
-        assert concept.is_hypothetical()
+        assert concept.hypothetical
```

### Comparing `pytakes-1.2.1/PKG-INFO` & `pytakes-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: pytakes
-Version: 1.2.1
+Version: 2.0.0
 Summary: Simple entity extraction module from a lexicon.
 Keywords: nlp,information extraction
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Healthcare Industry
 Requires-Dist: regex
 Requires-Dist: jinja2
 Requires-Dist: pyodbc
 Requires-Dist: sqlalchemy
 Requires-Dist: jsonschema
 Requires-Dist: pyyaml
+Requires-Dist: loguru
 Requires-Dist: pyodbc ; extra == "db"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: psycopg2 ; extra == "postgres"
 Requires-Dist: sas7bdat ; extra == "sas"
 Project-URL: Home, https://github.com/dcronkite/pytakes
 Provides-Extra: db
 Provides-Extra: dev
@@ -40,15 +42,15 @@
 
 This module will look for a pre-defined set of terms in a corpus of text, and use a variation of the negex/context
 algorithm to determine whether these terms express negation, historical, or various other qualifiers. (The set of
 negation terms is also configurable.)
 
 ## Requirements ##
 
-* Python 3.6+
+* Python 3.8+
 * See requirements.txt (`pip install -r requirements.txt`)
     * Various requirements-_.txt files are provided depending on your needs:
         * dev: for running tests, general development
         * db: for connecting to database using pyodbc
         * psql: connecting to postgres database
         * sas: if data is stored in SAS
 
@@ -96,15 +98,28 @@
 here: https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/negex/lexical_kb.csv
 
 Negation works by searching for the following word categories and then using a set of rules to determine which words
 should be 'qualified' in different ways. Within the recommended `jsonl` output, you'll find this included under
 the `qualifiers` key. Consider the following example:
 
 ```json
-"qualifiers": {"certainty": 0, "hypothetical": true, "historical": false, "other_subject": false, "terms": ["not", "afraid"]}
+{
+  ...
+  "qualifiers": {
+    "certainty": 0,
+    "hypothetical": true,
+    "historical": false,
+    "other_subject": false,
+    "terms": [
+      "not",
+      "afraid"
+    ]
+  },
+  ...
+}
 ```
 
 All values begin as `False` except `certainty` which starts as 4, meaning `definite`/`affirmative`. Here, `certainty` is
 0, meaning `negated`. This was done by the term 'not' which appears in the list of `terms`. `hypothetical` has been
 marked as `True` due to the term `afraid` (often in a context like 'afraid that he will catch a cold').
 
 **Certainty:**
@@ -151,22 +166,23 @@
     * 3: term applies negation, etc. **forward and/or backward** in the sentence (e.g., 'likely')
 
 #### Concept/Term Table ####
 
 This is the table containing the terms you want to search for (i.e., the entities you want extracted). I have added a
 script to autogenerate these based on some basic configuration files.
 
-    ​Column	​Type	​Description
-    ​ID	​int	​identity column; unique integer for each row
-    ​CUI	 string	​category identifier; can be used to "group" different     terms together
-    ​Text	​string	​term
-    ​RegexVariation	​int	​amount of variation: 0=none; 3=very; 1=default; -1=don't even allow suffixes, exact matches only; see #Rules#parameters below; I suggest you just use "0" or "-1"
-    ​WordOrder	​int	​how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order
-    MaxIntervening	int	how many intervening words to allow when locating words; 'how many intervening words do I allow?'
-    MaxWords	int	how many words to look ahead to find the next word; is ‘how far do I look ahead after each term?’ 
+| Column	         | Type	                                                                    | Description                                                                                                                                                       |       
+|-----------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ID	             | int	                                                                     | identity column; unique integer for each row                                                                                                                      |
+| CUI	 string	    | category identifier; can be used to "group" different     terms together |
+| Text	           | string	                                                                  | term                                                                                                                                                              |
+| RegexVariation	 | int	                                                                     | amount of variation: 0=none; 3=very; 1=default; -1=don't even allow suffixes, exact matches only; see #Rules#parameters below; I suggest you just use "0" or "-1" |
+| WordOrder	      | int	                                                                     | how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order                                                                         |
+| MaxIntervening  | int                                                                      | how many intervening words to allow when locating words; 'how many intervening words do I allow?'                                                                 |
+| MaxWords	       | int                                                                      | how many words to look ahead to find the next word; is ‘how far do I look ahead after each term?’                                                                 | 
 
 MaxIntervening and MaxWords should not be used together.
 
 To autogenerate this table format, use the `pytakes-build-dictionary` script installed into the Python Scripts
 directory. For an example, run this with the `--create-sample` option (optionally specify the output with
 the `--path C:\somewhere` option. For additional specifications, see the "Dictionary Builder" section below.
 
@@ -230,40 +246,39 @@
 For a simple example, run (you will first need to install this package, run `python setup.py install` in the base
 directory):
 
     pytakes-build-dictionary --create-sample --path OUTPUT_PATH
 
 ### COMMAND LINE ARGUMENTS ###
 
-    Short​	​Long	​Description
-    ​-p	​--path	​Specifies parent directory of folders; program will prompt if unable to locate the directory
-    ​-o	​--output	​Specify output CSV file; if ".csv" is not included, it will be added
-    ​-t	​--table	​Specify output table in specified database (See below)
-    ​-v	​--verbosity	​Specify amount of log output to show: 3-most verbose; 0-least verbose
-    --driver	If -t is specified, driver where table should be created. Defaults to SQL Server
-    --server	If -t is specified, server where table should be created. 
-    --database	If -t is specified, database where table should be created. 
+| Short | Long        | Description                                                                                  |
+|-------|-------------|----------------------------------------------------------------------------------------------|
+| -p    | --path      | Specifies parent directory of folders; program will prompt if unable to locate the directory |
+| -o    | --output    | Specify output CSV file; if ".csv" is not included, it will be added                         |
+| -t    | --table     | Specify output table in specified database (See below)                                       |
+| -v    | --verbosity | Specify amount of log output to show: 3-most verbose; 0-least verbose                        |
+|       | --driver    | If -t is specified, driver where table should be created. Defaults to SQL Server             |
+|       | --server    | If -t is specified, server where table should be created.                                    |
+|       | --database  | If -t is specified, database where table should be created.                                  |
 
 ### OUTPUT COLUMNS ####
 
 Not all of these output columns are required (most don't do anything). This was originally designed for building a
 dictionary using cTAKES.
 
-     Column	​Type	​Description
-     ID	​int	​identity column; unique integer for each row
-     CUI	​varchar(8)	​category identifier; can be used to "group" different terms together
-     Fword	​varchar(80)	​first word of term
-     Text	​varchar(8000)	​term
-     Code	​varchar(45)	​unimportant value required by cTAKES (legacy)
-     SourceType	​varchar(45)	​unimportant value required by cTAKES (legacy)
-     TUI	​varchar(4)	​​unimportant value required by cTAKES (legacy)
-     TextLength	​int	​length of term (all characters including spaces)
-     RegexVariation	​int	​amount of variation: 0=none; 3=very; 1=default; see #Rules#parameters below
-     WordOrder	​int	​how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order
-     Valence	​int	​this should just be "1"; program is  not designed to work with this correctly
+| Column         | Type          | Description                                                                               |
+|----------------|---------------|-------------------------------------------------------------------------------------------|
+| ID             | int           | identity column; unique integer for each row                                              |
+| CUI            | varchar(8)    | category identifier; can be used to "group" different terms together                      |
+| Fword          | varchar(80)   | first word of term                                                                        |
+| Text           | varchar(8000) | term                                                                                      |
+| TextLength     | int           | length of term (all characters including spaces)                                          |
+| RegexVariation | int           | amount of variation: 0=none; 3=very; 1=default; see #Rules#parameters below               |
+| WordOrder      | int           | how accurate must the given word order be; 2=exactly; 1=fword constraint; 0=no word order |
+| Valence        | int           | this should just be "1"; program is not designed to work with this correctly              |
 
 ### RULES ###
 
 Rules are the text entries in the cTAKES-like dictionary, however, they can include "categories" in addition to just
 text.A category is any string of text surrounded by "[" and "]". The intervening text string is the name of a "
 category". The category must have a definition, and each item (synonym) in the definition will be used in the rule.
 
@@ -284,30 +299,30 @@
 The rule file must be named "rules" or "rules.some-extension" (e.g., "rules.txt").
 
 #### Parameters ####
 
 Rules may also maintain configuration parameters.The configurations are indexed in the following order (bold indicates
 the default parameter):
 
-RegexVariation (integers)
-
-    **0: no variation in regular expression coverage**
-    1: minimal variation in regular expression coverage
-    2: moderate variation in regular expression coverage
-    3: high flexibility in regular expression coverage
-
-WordOrder
-
-    0: free word order
-    **1: enforce first word rule**
-    2: require precise word order
-
-Valence
-
-    **ALWAYS USE 1** or just ignore; NOT YET CORRECTLY IMPLEMENTED IN LCTAKES
+| RegexVariation | Description                                               |
+|----------------|-----------------------------------------------------------|
+| 0              | **(Default)** no variation in regular expression coverage |
+| 1              | minimal variation in regular expression coverage          |
+| 2              | moderate variation in regular expression coverage         |
+| 3              | high flexibility in regular expression coverage           |
+
+| WordOrder | Description                           |
+|-----------|---------------------------------------|
+| 0         | free word order                       |
+| 1         | **(Default)** enforce first word rule |
+| 2         | require precise word order            |
+
+| Valence | Description                |
+|---------|----------------------------|
+| 1       | **(Default)** Always use 1 |
 
 These are designated by the double percent ('%%') and follow the rule.
 
     [category]%%REGEX_VARIATION,WORD_ORDER,VALENCE
 
 For example:
```

