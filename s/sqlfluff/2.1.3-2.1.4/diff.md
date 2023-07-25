# Comparing `tmp/sqlfluff-2.1.3.tar.gz` & `tmp/sqlfluff-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-dwfpmqae/sqlfluff-2.1.3.tar", last modified: Wed Jul 19 22:42:51 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-fzrqvhpn/sqlfluff-2.1.4.tar", last modified: Tue Jul 25 10:29:09 2023, max compression
```

## Comparing `sqlfluff-2.1.3.tar` & `sqlfluff-2.1.4.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)   394733 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    45672 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25234 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134008 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68489 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    94430 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    81269 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   165314 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36674 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69805 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   202085 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)   101470 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   178244 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:42:51.000000 sqlfluff-2.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-19 22:42:34.000000 sqlfluff-2.1.3/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)   397137 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46018 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45351 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51152 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42757 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19891 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74094 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25234 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135036 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22693 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68578 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94477 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81269 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165929 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36674 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69805 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202161 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101470 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178244 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/test/test_testing.py
```

### Comparing `sqlfluff-2.1.3/CHANGELOG.md` & `sqlfluff-2.1.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,48 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.1.4] - 2023-07-25
+
+## Highlights
+
+This release brings some meaningful performance improvements to the parsing of
+complex SQL statements. In files with deeply nested expressions, we have seen
+up to a 50% reduction on time spent in the parsing phase. These changes are all
+internal optimisations and have minimal implications for the parser. In a few
+isolated cases they did highlight inconsistencies in the parsing of literals
+and so if your use case relies on the specific structure of literal and
+expression parsing you may find some small differences in how some expressions
+are parsed.
+
+Additionally this release brings new validation steps to configuration.
+Layout configuration is now validated on load (and so users with invalid
+layout configurations may see some of these being caught now) and inline
+configuration statements in files are also now validated for both their
+layout rules and for any removed or deprecated settings.
+
+On top of both we've seen dialect improvements to Databricks, PostgreSQL,
+BigQuery, Snowflake & Athena.
+
+## What’s Changed
+
+* Databricks set time zone [#5000](https://github.com/sqlfluff/sqlfluff/pull/5000) [@greg-finley](https://github.com/greg-finley)
+* Terminator inheritance [#4981](https://github.com/sqlfluff/sqlfluff/pull/4981) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Reduce copying in the parse phase [#4988](https://github.com/sqlfluff/sqlfluff/pull/4988) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Validate layout configs #4578 [#4997](https://github.com/sqlfluff/sqlfluff/pull/4997) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix handling of keywords for roles in ALTER ROLE statement [#4994](https://github.com/sqlfluff/sqlfluff/pull/4994) [@anzelpwj](https://github.com/anzelpwj)
+* BigQuery: fixes parse error on some literals with data type and quoted [#4992](https://github.com/sqlfluff/sqlfluff/pull/4992) [@yoichi](https://github.com/yoichi)
+* Correct Snowflake `CROSS JOIN` syntax [#4996](https://github.com/sqlfluff/sqlfluff/pull/4996) [@tunetheweb](https://github.com/tunetheweb)
+* Remove broken 'fork me' banner from docs [#4989](https://github.com/sqlfluff/sqlfluff/pull/4989) [@greg-finley](https://github.com/greg-finley)
+* feat: support athena optional WITH ORDINALITY post UNNEST function [#4991](https://github.com/sqlfluff/sqlfluff/pull/4991) [@reata](https://github.com/reata)
+
 ## [2.1.3] - 2023-07-19
 
 ## Highlights
 
 This release is a fairly standard incremental release. Highlights include bugfixes
 to `RF05` and dialect improvements to Snowflake, Teradata, MySQL, TSQL, SparkSQL & Postgres.
```

### Comparing `sqlfluff-2.1.3/LICENSE.md` & `sqlfluff-2.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/PKG-INFO` & `sqlfluff-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.3
+Version: 2.1.4
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.3/README.md` & `sqlfluff-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/setup.cfg` & `sqlfluff-2.1.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.1.3
+version = 2.1.4
 description = The SQL Linter for Humans
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -110,13 +110,13 @@
 [options.package_data]
 sqlfluff = 
 	config.ini
 	core/default_config.cfg
 	py.typed
 
 [sqlfluff_docs]
-stable_version = 2.1.3
+stable_version = 2.1.4
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/api/simple.py` & `sqlfluff-2.1.4/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.1.4/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.1.4/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/cli/commands.py` & `sqlfluff-2.1.4/src/sqlfluff/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1169,14 +1169,22 @@
         "stdout logging."
     ),
 )
 @click.option(
     "--profiler", is_flag=True, help="Set this flag to engage the python profiler."
 )
 @click.option(
+    "--parse-statistics",
+    is_flag=True,
+    help=(
+        "Set this flag to enabled detailed debugging readout "
+        "on the use of terminators in the parser."
+    ),
+)
+@click.option(
     "--nofail",
     is_flag=True,
     help=(
         "If set, the exit code will always be zero, regardless of violations "
         "found. This is potentially useful during rollout."
     ),
 )
@@ -1188,14 +1196,15 @@
     write_output: Optional[str],
     profiler: bool,
     bench: bool,
     nofail: bool,
     logger: Optional[logging.Logger] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
+    parse_statistics: bool = False,
     **kwargs,
 ) -> None:
     """Parse SQL files and just spit out the result.
 
     PATH is the path to a sql file or directory to lint. This can be either a
     file ('path/to/file.sql'), a path ('directory/of/sql/files'), a single ('-')
     character to indicate reading from *stdin* or a dot/blank ('.'/' ') which will
@@ -1243,22 +1252,24 @@
         if "-" == path:
             parsed_strings = [
                 lnt.parse_string(
                     sys.stdin.read(),
                     "stdin",
                     recurse=recurse,
                     config=lnt.config,
+                    parse_statistics=parse_statistics,
                 ),
             ]
         else:
             # A single path must be specified for this command
             parsed_strings = list(
                 lnt.parse_path(
                     path=path,
                     recurse=recurse,
+                    parse_statistics=parse_statistics,
                 )
             )
 
     total_time = time.monotonic() - t0
     violations_count = 0
 
     # iterative print for human readout
@@ -1352,15 +1363,15 @@
             fname = "stdin"
             file_config = lnt.config
         else:
             raw_sql, file_config, _ = lnt.load_raw_file_and_config(path, lnt.config)
             fname = path
 
     # Get file specific config
-    file_config.process_raw_file_for_config(raw_sql)
+    file_config.process_raw_file_for_config(raw_sql, fname)
     rendered = lnt.render_string(raw_sql, fname, file_config, "utf8")
 
     if rendered.templater_violations:
         for v in rendered.templater_violations:
             click.echo(formatter.format_violation(v))
         sys.exit(EXIT_FAIL)
     else:
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.1.4/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.1.4/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.1.4/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/config.py` & `sqlfluff-2.1.4/src/sqlfluff/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 We define a global loader, so that between calls to load config, we
 can still cache appropriately
 """
 
 ConfigElemType = Tuple[Tuple[str, ...], Any]
 
 
+ALLOWABLE_LAYOUT_CONFIG_KEYS = (
+    "spacing_before",
+    "spacing_after",
+    "spacing_within",
+    "line_position",
+    "align_within",
+    "align_scope",
+)
+
+
 @dataclass
 class _RemovedConfig:
     old_path: Tuple[str, ...]
     warning: str
     new_path: Optional[Tuple[str, ...]] = None
     translation_func: Optional[Callable[[str], str]] = None
 
@@ -497,21 +507,27 @@
             r[n] = v
         return ctx
 
     @staticmethod
     def _validate_configs(
         configs: Iterable[ConfigElemType], file_path
     ) -> List[ConfigElemType]:
-        """Validate config elements against removed list."""
+        """Validate config elements.
+
+        We validate in two ways:
+        1. Are these config settings removed or deprecated.
+        2. Are these config elements in the layout section _valid_.
+        """
         config_map = {cfg.old_path: cfg for cfg in REMOVED_CONFIGS}
         # Materialise the configs into a list to we can iterate twice.
         new_configs = list(configs)
         defined_keys = {k for k, _ in new_configs}
         validated_configs = []
         for k, v in new_configs:
+            # First validate against the removed option list.
             if k in config_map.keys():
                 formatted_key = ":".join(k)
                 removed_option = config_map[k]
                 # Is there a mapping option?
                 if removed_option.translation_func and removed_option.new_path:
                     formatted_new_key = ":".join(removed_option.new_path)
                     # Before mutating, check we haven't _also_ set the new value.
@@ -545,20 +561,45 @@
                         f"\n\n{removed_option.warning}\n\n"
                         "See https://docs.sqlfluff.com/en/stable/configuration.html"
                         " for more details.\n"
                     )
                 else:
                     # Raise an error.
                     raise SQLFluffUserError(
-                        f"Config file {file_path} set an outdated config "
+                        f"Config file {file_path!r} set an outdated config "
                         f"value {formatted_key}.\n\n{removed_option.warning}\n\n"
                         "See https://docs.sqlfluff.com/en/stable/configuration.html"
                         " for more details."
                     )
 
+            # Second validate any layout configs for validity.
+            # NOTE: For now we don't check that the "type" is a valid one
+            # to reference, or that the values are valid. For the values,
+            # these are likely to be rejected by the layout routines at
+            # runtime. The last risk area is validating that the type is
+            # a valid one.
+            if k and k[0] == "layout":
+                # Check for:
+                # - Key length
+                # - Key values
+                if (
+                    # Key length must be 4
+                    (len(k) != 4)
+                    # Second value must (currently) be "type"
+                    or (k[1] != "type")
+                    # Last key value must be one of the allowable options.
+                    or (k[3] not in ALLOWABLE_LAYOUT_CONFIG_KEYS)
+                ):
+                    raise SQLFluffUserError(
+                        f"Config file {file_path!r} set an invalid `layout` option "
+                        f"value {':'.join(k)}.\n"
+                        "See https://docs.sqlfluff.com/en/stable/layout.html"
+                        "#configuring-layout for more details."
+                    )
+
             validated_configs.append((k, v))
         return validated_configs
 
     def load_config_file(
         self, file_dir: str, file_name: str, configs: Optional[dict] = None
     ) -> dict:
         """Load the default config file."""
@@ -1090,41 +1131,45 @@
             if isinstance(cfg[k], dict):
                 # First yield the dict label
                 yield (0, k, "")
                 # Then yield its content
                 for idnt, key, val in self.iter_vals(cfg=cfg[k]):
                     yield (idnt + 1, key, val)
 
-    def process_inline_config(self, config_line: str):
+    def process_inline_config(self, config_line: str, fname: str):
         """Process an inline config command and update self."""
         # Strip preceding comment marks
         if config_line.startswith("--"):
             config_line = config_line[2:].strip()
         # Strip preceding sqlfluff line.
         if not config_line.startswith("sqlfluff:"):  # pragma: no cover
             config_logger.warning(
                 "Unable to process inline config statement: %r", config_line
             )
             return
         config_line = config_line[9:].strip()
         # Divide on colons
         config_path = [elem.strip() for elem in config_line.split(":")]
+        config_val = (tuple(config_path[:-1]), config_path[-1])
+        # Validate the value
+        ConfigLoader._validate_configs([config_val], fname)
         # Set the value
-        self.set_value(config_path[:-1], config_path[-1])
+        self.set_value(*config_val)
         # If the config is for dialect, initialise the dialect
         if config_path[:-1] == ["dialect"]:
             self._initialise_dialect(config_path[-1])
 
-    def process_raw_file_for_config(self, raw_str: str):
+    def process_raw_file_for_config(self, raw_str: str, fname: str):
         """Process a full raw file for inline config and update self."""
         # Scan the raw file for config commands.
         for raw_line in raw_str.splitlines():
-            if raw_line.startswith("-- sqlfluff"):
+            # With or without a space.
+            if raw_line.startswith(("-- sqlfluff", "--sqlfluff")):
                 # Found a in-file config command
-                self.process_inline_config(raw_line)
+                self.process_inline_config(raw_line, fname)
 
 
 class ProgressBarConfiguration:
     """Singleton-esque progress bar configuration.
 
     It's expected to be set during starting with parameters coming from commands
     parameters, then to be just utilized as just
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.1.4/src/sqlfluff/core/default_config.cfg`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.1.4/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.1.4/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/enums.py` & `sqlfluff-2.1.4/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/errors.py` & `sqlfluff-2.1.4/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.1.4/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.1.4/src/sqlfluff/core/linter/linter.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                     "Users can increase this limit in their config by setting the "
                     "'large_file_skip_byte_limit' value, or disable by setting it "
                     "to zero."
                 )
         with open(fname, encoding=encoding, errors="backslashreplace") as target_file:
             raw_file = target_file.read()
         # Scan the raw file for config commands.
-        file_config.process_raw_file_for_config(raw_file)
+        file_config.process_raw_file_for_config(raw_file, fname)
         # Return the raw file and config
         return raw_file, file_config, encoding
 
     @staticmethod
     def _normalise_newlines(string: str) -> str:
         """Normalise newlines to unix-style line endings."""
         return regex.sub(r"\r\n|\r", "\n", string)
@@ -219,23 +219,25 @@
 
     @staticmethod
     def _parse_tokens(
         tokens: Sequence[BaseSegment],
         config: FluffConfig,
         recurse: bool = True,
         fname: Optional[str] = None,
+        parse_statistics: bool = False,
     ) -> Tuple[Optional[BaseSegment], List[SQLParseError]]:
         parser = Parser(config=config)
         violations = []
         # Parse the file and log any problems
         try:
             parsed: Optional[BaseSegment] = parser.parse(
                 tokens,
                 recurse=recurse,
                 fname=fname,
+                parse_statistics=parse_statistics,
             )
         except SQLParseError as err:
             linter_logger.info("PARSING FAILED! : %s", err)
             violations.append(err)
             return None, violations
 
         if parsed:
@@ -377,14 +379,15 @@
     # These compose the base static methods into useful recipes.
 
     @classmethod
     def parse_rendered(
         cls,
         rendered: RenderedFile,
         recurse: bool = True,
+        parse_statistics: bool = False,
     ) -> ParsedString:
         """Parse a rendered file."""
         t0 = time.monotonic()
         violations = cast(List[SQLBaseError], rendered.templater_violations)
         tokens: Optional[Sequence[BaseSegment]]
         if rendered.templated_file is not None:
             tokens, lvs, config = cls._lex_templated_file(
@@ -399,14 +402,15 @@
 
         if tokens:
             parsed, pvs = cls._parse_tokens(
                 tokens,
                 rendered.config,
                 recurse=recurse,
                 fname=rendered.fname,
+                parse_statistics=parse_statistics,
             )
             violations += pvs
         else:
             parsed = None
 
         time_dict = {
             **rendered.time_dict,
@@ -881,35 +885,38 @@
     def parse_string(
         self,
         in_str: str,
         fname: str = "<string>",
         recurse: bool = True,
         config: Optional[FluffConfig] = None,
         encoding: str = "utf-8",
+        parse_statistics: bool = False,
     ) -> ParsedString:
         """Parse a string."""
         violations: List[SQLBaseError] = []
 
         # Dispatch the output for the template header (including the config diff)
         if self.formatter:
             self.formatter.dispatch_template_header(fname, self.config, config)
 
         # Just use the local config from here:
         config = config or self.config
 
         # Scan the raw file for config commands.
-        config.process_raw_file_for_config(in_str)
+        config.process_raw_file_for_config(in_str, fname)
         rendered = self.render_string(in_str, fname, config, encoding)
         violations += rendered.templater_violations
 
         # Dispatch the output for the parse header
         if self.formatter:
             self.formatter.dispatch_parse_header(fname)
 
-        return self.parse_rendered(rendered, recurse=recurse)
+        return self.parse_rendered(
+            rendered, recurse=recurse, parse_statistics=parse_statistics
+        )
 
     def fix(
         self,
         tree: BaseSegment,
         config: Optional[FluffConfig] = None,
         fname: Optional[str] = None,
         templated_file: Optional[TemplatedFile] = None,
@@ -1234,14 +1241,15 @@
         result.stop_timer()
         return result
 
     def parse_path(
         self,
         path: str,
         recurse: bool = True,
+        parse_statistics: bool = False,
     ) -> Iterator[ParsedString]:
         """Parse a path of sql files.
 
         NB: This a generator which will yield the result of each file
         within the path iteratively.
         """
         for fname in self.paths_from_path(path):
@@ -1257,8 +1265,9 @@
                 continue
             yield self.parse_string(
                 raw_file,
                 fname=fname,
                 recurse=recurse,
                 config=config,
                 encoding=encoding,
+                parse_statistics=parse_statistics,
             )
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.1.4/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.1.4/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 context manager. https://flask.palletsprojects.com/en/1.1.x/
 
 The context acts as a way of keeping track of state, references
 to common configuration and dialects, logging and also the parse
 and match depth of the current operation.
 """
 
+from collections import defaultdict
 import logging
 import uuid
 from typing import Optional, TYPE_CHECKING, Dict
 
 if TYPE_CHECKING:  # pragma: no cover
     from sqlfluff.core.parser.match_result import MatchResult
 
@@ -43,14 +44,20 @@
         # This is the logger that child objects will latch onto.
         self.logger = parser_logger
         # A uuid for this parse context to enable cache invalidation
         self.uuid = uuid.uuid4()
         # A dict for parse caching. This is reset for each file,
         # but persists for the duration of an individual file parse.
         self._parse_cache = {}
+        # A dictionary for keeping track of some statistics on parsing
+        # for performance optimisation.
+        # Focused around BaseGrammar._longest_trimmed_match().
+        # Initialise only with "next_counts", the rest will be int
+        # and are dealt with in .increment().
+        self.parse_stats = {"next_counts": defaultdict(int)}
 
     @classmethod
     def from_config(cls, config, **overrides: Dict[str, bool]) -> "RootParseContext":
         """Construct a `RootParseContext` from a `FluffConfig`."""
         indentation_config = config.get_section("indentation") or {}
         try:
             indentation_config = {k: bool(v) for k, v in indentation_config.items()}
@@ -104,24 +111,32 @@
     at the top level stack config object and the persistent
     config values (stored as attributes of the ParseContext
     itself).
     """
 
     # We create and destroy many ParseContexts, so we limit the slots
     # to improve performance.
-    __slots__ = ["match_depth", "parse_depth", "match_segment", "recurse", "_root_ctx"]
+    __slots__ = [
+        "match_depth",
+        "parse_depth",
+        "match_segment",
+        "recurse",
+        "terminators",
+        "_root_ctx",
+    ]
 
     def __init__(self, root_ctx, recurse=True):
         self._root_ctx = root_ctx
         self.recurse = recurse
         # The following attributes are only accessible via a copy
         # and not in the init method.
         self.match_segment = None
         self.match_depth = 0
         self.parse_depth = 0
+        self.terminators = []  # NOTE: Includes inherited parent terminators.
 
     def __getattr__(self, name):
         """If the attribute doesn't exist on this, revert to the root."""
         try:
             return getattr(self._root_ctx, name)
         except AttributeError:  # pragma: no cover
             raise AttributeError(
@@ -130,15 +145,20 @@
                 )
             )
 
     def _copy(self):
         """Mimic the copy.copy() method but restrict only to local vars."""
         ctx = self.__class__(root_ctx=self._root_ctx)
         for key in self.__slots__:
-            setattr(ctx, key, getattr(self, key))
+            if key == "terminators":
+                # For terminators, make sure we actually copy the list.
+                # This makes sure we don't keep a reference to the parent list.
+                setattr(ctx, key, getattr(self, key).copy())
+            else:
+                setattr(ctx, key, getattr(self, key))
         return ctx
 
     def __enter__(self):
         """Enter into the context.
 
         For the ParseContext, this just returns itself, because
         we already have the right kind of object.
@@ -158,14 +178,16 @@
     def deeper_parse(self):
         """Return a copy with an incremented parse depth."""
         ctx = self._copy()
         if not isinstance(ctx.recurse, bool):  # pragma: no cover TODO?
             ctx.recurse -= 1
         ctx.parse_depth += 1
         ctx.match_depth = 0
+        # Clear terminators here. Inner parsing shouldn't inherit terminators.
+        ctx.clear_terminators()
         return ctx
 
     def may_recurse(self):
         """Return True if allowed to recurse."""
         return self.recurse > 1 or self.recurse is True
 
     def matching_segment(self, name):
@@ -186,14 +208,29 @@
         """
         return self._root_ctx._parse_cache.get((loc_key, matcher_key))
 
     def put_parse_cache(self, loc_key: tuple, matcher_key: str, match: "MatchResult"):
         """Store a match in the cache for later retrieval."""
         self._root_ctx._parse_cache[(loc_key, matcher_key)] = match
 
+    def increment(self, key: str, default: int = 0) -> None:
+        """Increment one of the parse stats by name."""
+        self._root_ctx.parse_stats[key] = self._root_ctx.parse_stats.get(key, 0) + 1
+
+    def push_terminators(self, new_terminators: list) -> None:
+        """Push any new terminators onto the stack."""
+        # Yes, inefficient for now.
+        for term in new_terminators:
+            if term not in self.terminators:
+                self.terminators.append(term)
+
+    def clear_terminators(self) -> None:
+        """Clear any inherited terminators from this context."""
+        self.terminators = []
+
 
 class ParseDenylist:
     """Acts as a cache to stop unnecessary matching."""
 
     def __init__(self):
         self._denylist_struct = {}
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         self.max_times_per_element = kwargs.pop("max_times_per_element", None)
         # Any patterns to _prevent_ a match.
         self.exclude = kwargs.pop("exclude", None)
         # The intent here is that if we match something, and then the _next_
         # item is one of these, we can safely conclude it's a "total" match.
         # In those cases, we return early without considering more options.
         self.terminators = kwargs.pop("terminators", None)
+        self.reset_terminators = kwargs.pop("reset_terminators", False)
         super().__init__(*args, **kwargs)
 
     @cached_method_for_parse_context
     def simple(self, parse_context: ParseContext, crumbs: Optional[List[str]] = None):
         """Does this matcher support a uppercase hash matching route?
 
         AnyNumberOf does provide this, as long as *all* the elements *also* do.
@@ -157,20 +158,23 @@
         available_options = self._prune_options(segments, parse_context=parse_context)
 
         # If we've pruned all the options, return unmatched (with some logging).
         if not available_options:
             return MatchResult.from_unmatched(segments), None
 
         with parse_context.deeper_match() as ctx:
+            if self.reset_terminators:
+                ctx.clear_terminators()
+            if self.terminators:
+                ctx.push_terminators(self.terminators)
             match, matched_option = self._longest_trimmed_match(
                 segments,
                 available_options,
                 parse_context=ctx,
                 trim_noncode=False,
-                terminators=self.terminators,
             )
 
         return match, matched_option
 
     @match_wrapper()
     @allow_ephemeral
     def match(
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -224,28 +224,39 @@
     @classmethod
     def _longest_trimmed_match(
         cls,
         segments: Tuple[BaseSegment, ...],
         matchers: List[MatchableType],
         parse_context: ParseContext,
         trim_noncode=True,
-        terminators: Optional[List[MatchableType]] = None,
     ) -> Tuple[MatchResult, Optional[MatchableType]]:
         """Return longest match from a selection of matchers.
 
         Prioritise the first match, and if multiple match at the same point the longest.
         If two matches of the same length match at the same time, then it's the first in
         the iterable of matchers.
 
         Returns:
             `tuple` of (match_object, matcher).
 
+        NOTE: This matching method is the workhorse of the parser. It's performance
+        can be monitored using the `parse_stats` object on the context.
         """
         terminated = False
 
+        parse_context.increment("ltm_calls")
+        # NOTE: The use of terminators is only available via the context.
+        # They are set in that way to allow appropriate inheritance rather
+        # than only being used in a per-grammar basis.
+        if parse_context.terminators:
+            parse_context.increment("ltm_calls_w_ctx_terms")
+            terminators = parse_context.terminators
+        else:
+            terminators = []
+
         # Have we been passed an empty list?
         if len(segments) == 0:  # pragma: no cover
             return MatchResult.from_empty(), None
 
         # If gaps are allowed, trim the ends.
         if trim_noncode:
             pre_nc, segments, post_nc = trim_non_code_segments(segments)
@@ -260,15 +271,15 @@
             segments[0].pos_marker.working_loc,
             segments[0].get_type(),
             len(segments),
         )
 
         best_match_length = 0
         # iterate at this position across all the matchers
-        for matcher in matchers:
+        for idx, matcher in enumerate(matchers):
             # Check parse cache.
             matcher_key = matcher.cache_key()
             res_match: Optional[MatchResult] = parse_context.check_parse_cache(
                 loc_key, matcher_key
             )
             if res_match:
                 parse_match_logging(
@@ -286,14 +297,15 @@
                 parse_context.put_parse_cache(loc_key, matcher_key, res_match)
 
             # By here we know that it's a MatchResult
             res_match = cast(MatchResult, res_match)
 
             if res_match.is_complete():
                 # Just return it! (WITH THE RIGHT OTHER STUFF)
+                parse_context.increment("complete_match")
                 if trim_noncode:
                     return (
                         MatchResult.from_matched(
                             pre_nc + res_match.matched_segments + post_nc
                         ),
                         matcher,
                     )
@@ -305,15 +317,20 @@
                     best_match = res_match, matcher
                     best_match_length = res_match.trimmed_matched_length
 
                     # If we've got a terminator next, it's an opportunity to
                     # end earlier, and claim an effectively "complete" match.
                     # NOTE: This means that by specifying terminators, we can
                     # significantly increase performance.
-                    if terminators:
+                    if idx == len(matchers) - 1:
+                        # If it's the last option - no need to check terminators.
+                        # We're going to end anyway, so we can skip that step.
+                        terminated = True
+                        break
+                    elif terminators:
                         _, segs, _ = trim_non_code_segments(
                             best_match[0].unmatched_segments
                         )
                         for terminator in terminators:
                             terminator_match: MatchResult = terminator.match(
                                 segs, parse_context=parse_context
                             )
@@ -326,17 +343,37 @@
                 break
 
             # We could stash segments here, but given we might have some successful
             # matches here, we shouldn't, because they'll be mutated in the wrong way.
             # Eventually there might be a performance gain from doing that sensibly
             # here.
 
+        if terminated:
+            parse_context.increment("terminated_match")
+        else:
+            parse_context.increment("unterminated_match")
+
         # If we get here, then there wasn't a complete match. If we
         # has a best_match, return that.
         if best_match_length > 0:
+            # If not terminated, keep track of what the next token would
+            # have been if we had been able to terminate using it.
+            if not terminated:
+                if best_match[0].unmatched_segments:
+                    for seg in best_match[0].unmatched_segments:
+                        if seg.is_code:
+                            break
+                    next_seg = seg.raw_segments[0].raw_upper
+                else:  # pragma: no cover
+                    # NOTE: I don't think this clause should ever
+                    # occur, but it's included so that if it does happen
+                    # we don't get an exception and can better debug.
+                    next_seg = "<NONE>"
+                parse_context.parse_stats["next_counts"][next_seg] += 1
+
             if trim_noncode:
                 return (
                     MatchResult(
                         pre_nc + best_match[0].matched_segments,
                         best_match[0].unmatched_segments + post_nc,
                     ),
                     best_match[1],
@@ -796,14 +833,22 @@
     # We can't allow keyword refs here, because it doesn't make sense
     # and it also causes infinite recursion.
     allow_keyword_string_refs = False
 
     def __init__(self, *args: str, **kwargs):
         # Any patterns to _prevent_ a match.
         self.exclude = kwargs.pop("exclude", None)
+        # The intent here is that if we match something, and then the _next_
+        # item is one of these, we can safely conclude it's a "total" match.
+        # In those cases, we return early without considering more options.
+        # Terminators don't take effect directly within this grammar, but
+        # the Ref grammar is an effective place to manage the terminators
+        # inherited via the context.
+        self.terminators = kwargs.pop("terminators", None)
+        self.reset_terminators = kwargs.pop("reset_terminators", False)
         super().__init__(*args, **kwargs)
 
     @cached_method_for_parse_context
     def simple(self, parse_context: ParseContext, crumbs: Optional[Tuple[str]] = None):
         """Does this matcher support a uppercase hash matching route?
 
         A ref is simple, if the thing it references is simple.
@@ -865,14 +910,20 @@
         """
         elem = self._get_elem(dialect=parse_context.dialect)
 
         # First if we have an *exclude* option, we should check that
         # which would prevent the rest of this grammar from matching.
         if self.exclude:
             with parse_context.deeper_match() as ctx:
+                # NOTE: Not covered because `exclude` and `teminators` aren't
+                # currently used together in any dialect.
+                if self.reset_terminators:  # pragma: no cover
+                    ctx.clear_terminators()
+                if self.terminators:  # pragma: no cover
+                    ctx.push_terminators(self.terminators)
                 if self.exclude.match(segments, parse_context=ctx):
                     return MatchResult.from_unmatched(segments)
 
         # First check against the efficiency Cache.
         # We rely on segments not being mutated within a given
         # match cycle and so the ids should continue to refer to unchanged
         # objects.
@@ -889,14 +940,18 @@
                 self_name=self_name,
             )
             return MatchResult.from_unmatched(segments)
 
         # Match against that. NB We're not incrementing the match_depth here.
         # References shouldn't really count as a depth of match.
         with parse_context.matching_segment(self._get_ref()) as ctx:
+            if self.reset_terminators:
+                ctx.clear_terminators()
+            if self.terminators:
+                ctx.push_terminators(self.terminators)
             resp = elem.match(segments=segments, parse_context=ctx)
         if not resp:
             parse_context.denylist.mark(self_name, seg_tuple)
         return resp
 
     @classmethod
     def keyword(cls, keyword, **kwargs):
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,23 +147,22 @@
                         terminated = True
                         unmatched_segments = (
                             pre_non_code + match.all_segments() + post_non_code
                         )
                         break
 
                 with parse_context.deeper_match() as ctx:
+                    if delimiter_matchers and elements != delimiter_matchers:
+                        ctx.push_terminators(delimiter_matchers)
                     match, _ = self._longest_trimmed_match(
                         segments=seg_content,
                         matchers=elements,
                         parse_context=ctx,
                         # We've already trimmed
                         trim_noncode=False,
-                        terminators=delimiter_matchers
-                        if elements != delimiter_matchers
-                        else None,
                     )
 
                 if match:
                     if elements == delimiter_matchers:
                         delimiters += 1
                         matched_delimiter = True
                         cached_matched_segments = matched_segments
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,20 @@
         # In either case, we're golden. Return successfully, with any leftovers as
         # the unmatched elements. Meta all go at the end regardless of wny trailing
         # whitespace.
 
         return MatchResult(
             BaseSegment._position_segments(
                 matched_segments.matched_segments + meta_pre_nc + meta_post_nc,
+                # Repositioning only meta segments at this stage does increase the
+                # risk of leakage a little (by not fully copying everything on
+                # return), but it does drastically improve performance. Future
+                # work may involve more immutable segments or a smarter way
+                # of isolating them.
+                metas_only=True,
             ),
             unmatched_segments,
         )
 
 
 class Bracketed(Sequence):
     """Match if a bracketed sequence, with content that matches one of the elements.
@@ -345,22 +351,26 @@
             if start_match:
                 seg_buff = start_match.unmatched_segments
             else:
                 # Can't find the opening bracket. No Match.
                 return MatchResult.from_unmatched(segments)
 
             # Look for the closing bracket
-            content_segs, end_match, _ = self._bracket_sensitive_look_ahead_match(
-                segments=seg_buff,
-                matchers=[end_bracket],
-                parse_context=parse_context,
-                start_bracket=start_bracket,
-                end_bracket=end_bracket,
-                bracket_pairs_set=self.bracket_pairs_set,
-            )
+            with parse_context.deeper_match() as ctx:
+                # Within the brackets, clear any inherited terminators.
+                ctx.clear_terminators()
+                content_segs, end_match, _ = self._bracket_sensitive_look_ahead_match(
+                    segments=seg_buff,
+                    matchers=[end_bracket],
+                    parse_context=ctx,
+                    start_bracket=start_bracket,
+                    end_bracket=end_bracket,
+                    bracket_pairs_set=self.bracket_pairs_set,
+                )
+
             if not end_match:  # pragma: no cover
                 raise SQLParseError(
                     "Couldn't find closing bracket for opening bracket.",
                     segment=start_match.matched_segments[0],
                 )
 
             # Construct a bracket segment
@@ -396,14 +406,16 @@
                 )
             else:
                 return MatchResult.from_unmatched(segments)
 
         # Match the content using super. Sequence will interpret the content of the
         # elements.
         with parse_context.deeper_match() as ctx:
+            # Within the brackets, clear any inherited terminators.
+            ctx.clear_terminators()
             content_match = super().match(content_segs, parse_context=ctx)
 
         # We require a complete match for the content (hopefully for obvious reasons)
         if content_match.is_complete():
             # Reconstruct the bracket segment post match.
             # We need to realign the meta segments so the pos markers are correct.
             # Have we already got indents?
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/match_logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,14 +585,15 @@
         return segs
 
     @classmethod
     def _position_segments(
         cls,
         segments: Tuple["BaseSegment", ...],
         parent_pos: Optional[PositionMarker] = None,
+        metas_only: bool = False,
     ) -> Tuple["BaseSegment", ...]:
         """Refresh positions of segments within a span.
 
         This does two things:
         - Assign positions to any segments without them.
         - Updates the working line_no and line_pos for all
           segments during fixing.
@@ -621,14 +622,35 @@
                 linter_logger.warning("SEG: %r, POS: %r", segments, parent_pos)
                 raise ValueError("Unable to find working position.")
 
         # Use the index so that we can look forward
         # and backward.
         segment_buffer: Tuple["BaseSegment", ...] = ()
         for idx, segment in enumerate(segments):
+            # NOTE: Repositioning can be very compute intensive to do
+            # completely (especially because of the copying required
+            # to do it safely), but during the parsing phase we may
+            # only need to reposition meta segments. Because they have
+            # no size in the templated file and also no children - they
+            # can be done safely without affecting the rest of the file.
+            if metas_only and not segment.is_meta:
+                # Assert that the segment already has position. Unless a
+                # fix has occured this should already be true.
+                assert segment.pos_marker, (
+                    "Non-meta segment found without position. Inappropriate "
+                    "use of `metas_only`."
+                )
+                # Add the original segment to the buffer.
+                segment_buffer += (segment,)
+                # Update working position
+                line_no, line_pos = segment.pos_marker.infer_next_position(
+                    segment.raw, line_no, line_pos
+                )
+                continue
+
             repositioned_seg = segment.copy()
             # Fill any that don't have a position.
             if not repositioned_seg.pos_marker:
                 # Can we get a position from the previous?
                 start_point = None
                 if idx > 0:
                     prev_seg = segment_buffer[idx - 1]
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.1.4/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.1.4/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.1.4/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.1.4/src/sqlfluff/core/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.1.4/src/sqlfluff/core/string_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.1.4/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.1.4/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.1.4/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.1.4/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/core/timing.py` & `sqlfluff-2.1.4/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,17 @@
     # NullSegment is defined separately to the keyword, so we can give it a different
     # type
     NullLiteralSegment=StringParser("null", LiteralKeywordSegment, type="null_literal"),
     TrueSegment=StringParser("true", LiteralKeywordSegment, type="boolean_literal"),
     FalseSegment=StringParser("false", LiteralKeywordSegment, type="boolean_literal"),
     # We use a GRAMMAR here not a Segment. Otherwise, we get an unnecessary layer
     SingleIdentifierGrammar=OneOf(
-        Ref("NakedIdentifierSegment"), Ref("QuotedIdentifierSegment")
+        Ref("NakedIdentifierSegment"),
+        Ref("QuotedIdentifierSegment"),
+        terminators=[Ref("DotSegment")],
     ),
     BooleanLiteralGrammar=OneOf(Ref("TrueSegment"), Ref("FalseSegment")),
     # We specifically define a group of arithmetic operators to make it easier to
     # override this if some dialects have different available operators
     ArithmeticBinaryOperatorGrammar=OneOf(
         Ref("PlusSegment"),
         Ref("MinusSegment"),
@@ -593,17 +595,16 @@
         # of a likely complete match if they come after a match. For
         # example "123," only needs to match against the LiteralGrammar
         # and because a comma follows, never be matched against
         # ExpressionSegment or FunctionSegment, which are both much
         # more complicated.
         terminators=[
             Ref("CommaSegment"),
-            # TODO: We can almost certainly add a few more here, but for
-            # now, the most reliable (and impactful) is the comma.
-            # Others could include some variant on AliasExpressionSegment.
+            Ref.keyword("AS"),
+            # TODO: We can almost certainly add a few more here.
         ],
     ),
     FilterClauseGrammar=Sequence(
         "FILTER", Bracketed(Sequence("WHERE", Ref("ExpressionSegment")))
     ),
     IgnoreRespectNullsGrammar=Sequence(OneOf("IGNORE", "RESPECT"), "NULLS"),
     FrameClauseUnitGrammar=OneOf("ROWS", "RANGE"),
@@ -1355,19 +1356,21 @@
     match_grammar: Matchable = Sequence(
         # Project name, schema identifier, etc.
         AnyNumberOf(
             Sequence(
                 Ref("SingleIdentifierGrammar"),
                 Ref("DotSegment"),
             ),
+            terminators=[Ref("BracketedSegment")],
         ),
         # Base function name
         OneOf(
             Ref("FunctionNameIdentifierSegment"),
             Ref("QuotedIdentifierSegment"),
+            terminators=[Ref("BracketedSegment")],
         ),
         allow_gaps=False,
     )
 
 
 class FunctionSegment(BaseSegment):
     """A scalar or aggregate function.
@@ -1555,22 +1558,24 @@
             OneOf(
                 # check first for MLTableExpression,
                 # because of possible FunctionSegment in
                 # MainTableExpression
                 Ref("MLTableExpressionSegment"),
                 Ref("FromExpressionElementSegment"),
                 Bracketed(Ref("FromExpressionSegment")),
+                terminators=[Ref.keyword("ORDER"), Ref.keyword("GROUP")],
             ),
             Dedent,
             Conditional(Indent, indented_joins=True),
             AnyNumberOf(
                 Sequence(
                     OneOf(Ref("JoinClauseSegment"), Ref("JoinLikeClauseGrammar")),
                 ),
                 optional=True,
+                terminators=[Ref.keyword("ORDER"), Ref.keyword("GROUP")],
             ),
             Conditional(Dedent, indented_joins=True),
         )
     )
 
 
 class TableExpressionSegment(BaseSegment):
@@ -1925,28 +1930,47 @@
     """A `CASE WHEN` clause."""
 
     type = "case_expression"
     match_grammar: Matchable = OneOf(
         Sequence(
             "CASE",
             ImplicitIndent,
-            AnyNumberOf(Ref("WhenClauseSegment")),
-            Ref("ElseClauseSegment", optional=True),
+            AnyNumberOf(
+                Ref("WhenClauseSegment"),
+                reset_terminators=True,
+                terminators=[Ref.keyword("ELSE"), Ref.keyword("END")],
+            ),
+            Ref(
+                "ElseClauseSegment",
+                optional=True,
+                reset_terminators=True,
+                terminators=[Ref.keyword("END")],
+            ),
             Dedent,
             "END",
         ),
         Sequence(
             "CASE",
             Ref("ExpressionSegment"),
             ImplicitIndent,
-            AnyNumberOf(Ref("WhenClauseSegment")),
-            Ref("ElseClauseSegment", optional=True),
+            AnyNumberOf(
+                Ref("WhenClauseSegment"),
+                reset_terminators=True,
+                terminators=[Ref.keyword("ELSE"), Ref.keyword("END")],
+            ),
+            Ref(
+                "ElseClauseSegment",
+                optional=True,
+                reset_terminators=True,
+                terminators=[Ref.keyword("END")],
+            ),
             Dedent,
             "END",
         ),
+        terminators=[Ref("CommaSegment"), Ref("BinaryOperatorGrammar")],
     )
 
 
 ansi_dialect.add(
     # Expression_A_Grammar
     # https://www.cockroachlabs.com/docs/v20.2/sql-grammar.html#a_expr
     # The upstream grammar is defined recursively, which if implemented naively
@@ -1967,15 +1991,18 @@
         "PRIOR",
     ),
     Tail_Recurse_Expression_A_Grammar=Sequence(
         # This should be used instead of a recursive call to Expression_A_Grammar
         # whenever the repeating element in Expression_A_Grammar makes a recursive
         # call to itself at the _end_.  If it's in the middle then you still need
         # to recurse into Expression_A_Grammar normally.
-        AnyNumberOf(Ref("Expression_A_Unary_Operator_Grammar")),
+        AnyNumberOf(
+            Ref("Expression_A_Unary_Operator_Grammar"),
+            terminators=[Ref("BinaryOperatorGrammar")],
+        ),
         Ref("Expression_C_Grammar"),
     ),
     Expression_A_Grammar=Sequence(
         # Grammar always starts with optional unary operator, plus c_expr.  This
         # section must always match the tail recurse grammar.
         Ref("Tail_Recurse_Expression_A_Grammar"),
         # As originally pictured in the diagram, the grammar then repeats itself
@@ -2089,14 +2116,15 @@
             OneOf(
                 Ref("Expression_D_Grammar"),
                 Ref("CaseExpressionSegment"),
             ),
             AnyNumberOf(Ref("TimeZoneGrammar"), optional=True),
         ),
         Ref("ShorthandCastSegment"),
+        terminators=[Ref("CommaSegment")],
     ),
     # Expression_D_Grammar
     # https://www.cockroachlabs.com/docs/v20.2/sql-grammar.htm#d_expr
     Expression_D_Grammar=Sequence(
         OneOf(
             Ref("BareFunctionSegment"),
             Ref("FunctionSegment"),
@@ -2146,14 +2174,15 @@
                     Ref("NumericLiteralSegment"),
                     Ref("BooleanLiteralGrammar"),
                     Ref("NullLiteralSegment"),
                     Ref("DateTimeLiteralGrammar"),
                 ),
             ),
             Ref("LocalAliasSegment"),
+            terminators=[Ref("CommaSegment")],
         ),
         Ref("Accessor_Grammar", optional=True),
         allow_gaps=True,
     ),
     Accessor_Grammar=AnyNumberOf(Ref("ArrayAccessorSegment")),
 )
 
@@ -2533,14 +2562,15 @@
                 # and Values() function (used in INSERT statements):
                 # https://dev.mysql.com/doc/refman/8.0/en/miscellaneous-functions.html#function_values
                 # TODO: split these out in future.
                 Ref.keyword("ROW", optional=True),
                 Bracketed(
                     Delimited(
                         "DEFAULT",
+                        Ref("LiteralGrammar"),
                         Ref("ExpressionSegment"),
                         ephemeral_name="ValuesClauseElements",
                     )
                 ),
             ),
         ),
     )
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,20 @@
         Ref("ArithmeticBinaryOperatorGrammar"),
         Ref("StringBinaryOperatorGrammar"),
         Ref("BooleanBinaryOperatorGrammar"),
         Ref("ComparisonOperatorGrammar"),
         # Add arrow operators for functions (e.g. filter)
         Ref("RightArrowOperator"),
     ),
+    PostFunctionGrammar=ansi_dialect.get_grammar("PostFunctionGrammar").copy(
+        # UNNEST can optionally have a WITH ORDINALITY clause
+        insert=[
+            Sequence("WITH", "ORDINALITY", optional=True),
+        ]
+    ),
 )
 
 
 class ArrayTypeSegment(ansi.ArrayTypeSegment):
     """Prefix for array literals specifying the type."""
 
     type = "array_type"
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,18 +472,15 @@
 
     type = "assert_statement"
     match_grammar: Matchable = Sequence(
         "ASSERT",
         Ref("ExpressionSegment"),
         Sequence(
             "AS",
-            OneOf(
-                Ref("SingleQuotedLiteralSegment"),
-                Ref("DoubleQuotedLiteralSegment"),
-            ),
+            Ref("QuotedLiteralSegment"),
             optional=True,
         ),
     )
 
 
 class ForInStatementsSegment(BaseSegment):
     """Statements within a FOR..IN...DO...END FOR statement.
@@ -704,15 +701,23 @@
 # BigQuery allows functions in INTERVAL
 class IntervalExpressionSegment(ansi.IntervalExpressionSegment):
     """An interval with a function as value segment."""
 
     match_grammar = Sequence(
         "INTERVAL",
         Ref("ExpressionSegment"),
-        OneOf(Ref("QuotedLiteralSegment"), Ref("DatetimeUnitSegment")),
+        OneOf(
+            Ref("QuotedLiteralSegment"),
+            Ref("DatetimeUnitSegment"),
+            Sequence(
+                Ref("DatetimeUnitSegment"),
+                "TO",
+                Ref("DatetimeUnitSegment"),
+            ),
+        ),
     )
 
 
 bigquery_dialect.replace(
     QuotedIdentifierSegment=TypedParser(
         "back_quote",
         ansi.IdentifierSegment,
@@ -720,18 +725,21 @@
         trim_chars=("`",),
     ),
     # Add ParameterizedSegment to the ansi NumericLiteralSegment
     NumericLiteralSegment=OneOf(
         TypedParser("numeric_literal", ansi.LiteralSegment, type="numeric_literal"),
         Ref("ParameterizedSegment"),
     ),
-    # Add three elements to the ansi LiteralGrammar
+    QuotedLiteralSegment=OneOf(
+        Ref("SingleQuotedLiteralSegment"),
+        Ref("DoubleQuotedLiteralSegment"),
+    ),
+    # Add elements to the ansi LiteralGrammar
     LiteralGrammar=ansi_dialect.get_grammar("LiteralGrammar").copy(
         insert=[
-            Ref("DoubleQuotedLiteralSegment"),
             Ref("ParameterizedSegment"),
         ]
     ),
     PostTableExpressionGrammar=Sequence(
         Sequence(
             "FOR", "SYSTEM_TIME", "AS", "OF", Ref("ExpressionSegment"), optional=True
         ),
@@ -850,19 +858,21 @@
             Sequence(
                 # BigQuery Function names can be prefixed by the keyword SAFE to
                 # return NULL instead of error.
                 # https://cloud.google.com/bigquery/docs/reference/standard-sql/functions-reference#safe_prefix
                 OneOf("SAFE", Ref("SingleIdentifierGrammar")),
                 Ref("DotSegment"),
             ),
+            terminators=[Ref("BracketedSegment")],
         ),
         # Base function name
         OneOf(
             Ref("FunctionNameIdentifierSegment"),
             Ref("QuotedIdentifierSegment"),
+            terminators=[Ref("BracketedSegment")],
         ),
         # BigQuery allows whitespaces between the `.` of a function refrence or
         # SAFE prefix. Keeping the explicit `allow_gaps=True` here to
         # make the distinction from `ansi.FunctionNameSegment` clear.
         allow_gaps=True,
     )
 
@@ -1765,16 +1775,15 @@
     """In BigQuery UNPIVOT alias's can be single or double quoted or numeric."""
 
     type = "alias_expression"
     match_grammar = Sequence(
         Indent,
         Ref.keyword("AS", optional=True),
         OneOf(
-            Ref("SingleQuotedLiteralSegment"),
-            Ref("DoubleQuotedLiteralSegment"),
+            Ref("QuotedLiteralSegment"),
             Ref("NumericLiteralSegment"),
         ),
         Dedent,
     )
 
 
 class FromUnpivotExpressionSegment(BaseSegment):
@@ -1997,18 +2006,15 @@
                         StringParser(
                             "uri",
                             CodeSegment,
                             type="export_option",
                         ),
                     ),
                     Ref("EqualsSegment"),
-                    OneOf(
-                        Ref("SingleQuotedLiteralSegment"),
-                        Ref("DoubleQuotedLiteralSegment"),
-                    ),
+                    Ref("QuotedLiteralSegment"),
                 ),
                 # Bool options
                 # Note: adding as own type, rather than keywords as convention with
                 # Bigquery, as per the docs, is to put Keywords in uppercase, and these
                 # in lowercase.
                 Sequence(
                     OneOf(
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,21 +120,37 @@
     match_grammar = Sequence(
         "USE",
         OneOf("DATABASE", "SCHEMA", optional=True),
         Ref("DatabaseReferenceSegment"),
     )
 
 
+class SetTimeZoneStatementSegment(BaseSegment):
+    """A `SET TIME ZONE` statement.
+
+    https://docs.databricks.com/sql/language-manual/sql-ref-syntax-aux-conf-mgmt-set-timezone.html
+    """
+
+    type = "set_timezone_statement"
+    match_grammar = Sequence(
+        "SET",
+        "TIME",
+        "ZONE",
+        OneOf("LOCAL", Ref("QuotedLiteralSegment"), Ref("IntervalExpressionSegment")),
+    )
+
+
 class StatementSegment(sparksql.StatementSegment):
     """Overriding StatementSegment to allow for additional segment parsing."""
 
     match_grammar = sparksql.StatementSegment.match_grammar
     parse_grammar = sparksql.StatementSegment.parse_grammar.copy(
         # Segments defined in Databricks SQL dialect
         insert=[
             # Unity Catalog
             Ref("AlterCatalogStatementSegment"),
             Ref("CreateCatalogStatementSegment"),
             Ref("DropCatalogStatementSegment"),
             Ref("UseCatalogStatementSegment"),
+            Ref("SetTimeZoneStatementSegment"),
         ]
     )
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,14 +454,15 @@
     match_grammar = Sequence(
         "VALUES",
         Delimited(
             OneOf(
                 Bracketed(
                     Delimited(
                         "DEFAULT",
+                        Ref("LiteralGrammar"),
                         Ref("ExpressionSegment"),
                         ephemeral_name="ValuesClauseElements",
                     )
                 ),
                 Delimited(
                     "DEFAULT",
                     Ref("ExpressionSegment"),
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -1556,34 +1556,55 @@
     """
 
     type = "alter_role_statement"
 
     match_grammar = Sequence(
         "ALTER",
         OneOf("ROLE", "USER"),
-        OneOf(Ref("RoleReferenceSegment"), "ALL"),
         OneOf(
+            # role_specification
             Sequence(
+                OneOf(
+                    "CURRENT_ROLE",
+                    "CURRENT_USER",
+                    "SESSION_USER",
+                    Ref("RoleReferenceSegment"),
+                ),
                 Ref.keyword("WITH", optional=True),
                 AnySetOf(
                     OneOf("SUPERUSER", "NOSUPERUSER"),
                     OneOf("CREATEDB", "NOCREATEDB"),
                     OneOf("CREATEROLE", "NOCREATEROLE"),
                     OneOf("INHERIT", "NOINHERIT"),
                     OneOf("LOGIN", "NOLOGIN"),
                     OneOf("REPLICATION", "NOREPLICATION"),
                     OneOf("BYPASSRLS", "NOBYPASSRLS"),
                     Sequence("CONNECTION", "LIMIT", Ref("NumericLiteralSegment")),
-                    Sequence("PASSWORD", OneOf(Ref("QuotedLiteralSegment"), "NULL")),
+                    Sequence(
+                        Ref.keyword("ENCRYPTED", optional=True),
+                        "PASSWORD",
+                        OneOf(Ref("QuotedLiteralSegment"), "NULL"),
+                    ),
                     Sequence("VALID", "UNTIL", Ref("QuotedLiteralSegment")),
                 ),
-                optional=True,
             ),
-            Sequence("RENAME", "TO", Ref("RoleReferenceSegment"), optional=True),
+            # name only
             Sequence(
+                Ref("RoleReferenceSegment"),
+                Sequence("RENAME", "TO", Ref("RoleReferenceSegment")),
+            ),
+            # role_specification | all
+            Sequence(
+                OneOf(
+                    "CURRENT_ROLE",
+                    "CURRENT_USER",
+                    "SESSION_USER",
+                    "ALL",
+                    Ref("RoleReferenceSegment"),
+                ),
                 Sequence(
                     "IN",
                     "DATABASE",
                     Ref("DatabaseReferenceSegment"),
                     optional=True,
                 ),
                 OneOf(
@@ -1607,15 +1628,14 @@
                                 "FROM",
                                 "CURRENT",
                             ),
                         ),
                     ),
                     Sequence("RESET", OneOf(Ref("ParameterNameSegment"), "ALL")),
                 ),
-                optional=True,
             ),
         ),
     )
 
 
 class ExplainStatementSegment(ansi.ExplainStatementSegment):
     """An `Explain` statement.
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,14 +769,15 @@
     match_grammar: Matchable = Sequence(
         # Project name, schema identifier, etc.
         AnyNumberOf(
             Sequence(
                 Ref("SingleIdentifierGrammar"),
                 Ref("DotSegment"),
             ),
+            terminators=[Ref("BracketedSegment")],
         ),
         # Base function name
         OneOf(
             Ref("FunctionNameIdentifierSegment"),
             Ref("QuotedIdentifierSegment"),
             # Snowflake's IDENTIFIER pseudo-function
             # https://docs.snowflake.com/en/sql-reference/identifier-literal.html
@@ -1088,14 +1089,15 @@
         Ref(
             "AliasExpressionSegment",
             exclude=OneOf(
                 Ref("FromClauseTerminatorGrammar"),
                 Ref("SamplingExpressionSegment"),
                 Ref("ChangesClauseSegment"),
                 Ref("JoinLikeClauseGrammar"),
+                "CROSS",
             ),
             optional=True,
         ),
         # https://cloud.google.com/bigquery/docs/reference/standard-sql/arrays#flattening_arrays
         Sequence("WITH", "OFFSET", Ref("AliasExpressionSegment"), optional=True),
         Ref("SamplingExpressionSegment", optional=True),
         Ref("PostTableExpressionGrammar", optional=True),
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.1.4/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.1.4/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.1.4/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.1.4/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.3
+Version: 2.1.4
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.3/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.1.4/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.1.4/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.3/test/test_testing.py` & `sqlfluff-2.1.4/test/test_testing.py`

 * *Files identical despite different names*

