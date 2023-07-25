# Comparing `tmp/metldata-0.3.6.tar.gz` & `tmp/metldata-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metldata-0.3.6.tar", last modified: Fri Jun 23 14:24:21 2023, max compression
+gzip compressed data, was "metldata-0.3.7.tar", last modified: Tue Jul 25 08:41:00 2023, max compression
```

## Comparing `metldata-0.3.6.tar` & `metldata-0.3.7.tar`

### file list

```diff
@@ -1,188 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.121452 metldata-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-23 14:24:06.000000 metldata-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-06-23 14:24:21.121452 metldata-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-06-23 14:24:06.000000 metldata-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.089452 metldata-0.3.6/metldata/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.089452 metldata-0.3.6/metldata/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/accession_registry/accession_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/accession_registry/accession_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/accession_registry/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.093452 metldata-0.3.6/metldata/artifacts_rest/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/api_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/artifact_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/load_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/artifacts_rest/query_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.093452 metldata-0.3.6/metldata/builtin_transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.093452 metldata-0.3.6/metldata/builtin_transformations/add_accessions/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/add_accessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/add_accessions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/add_accessions/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/add_accessions/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/add_accessions/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.093452 metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.097452 metldata-0.3.6/metldata/builtin_transformations/delete_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/delete_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/delete_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/delete_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/delete_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/delete_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/delete_slots/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.097452 metldata-0.3.6/metldata/builtin_transformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.097452 metldata-0.3.6/metldata/builtin_transformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/path/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/path/path_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/path/path_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/path/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/infer_references/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.101452 metldata-0.3.6/metldata/builtin_transformations/merge_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/merge_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/merge_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/merge_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/merge_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/merge_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/merge_slots/model_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_transformations/merge_slots/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.101452 metldata-0.3.6/metldata/builtin_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/builtin_workflows/ghga_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.101452 metldata-0.3.6/metldata/event_handling/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/event_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/event_handling/artifact_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/event_handling/event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/event_handling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/event_handling/submission_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.101452 metldata-0.3.6/metldata/load/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.105452 metldata-0.3.6/metldata/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/model_utils/metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.105452 metldata-0.3.6/metldata/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/submission_registry/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/submission_registry/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/submission_registry/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/submission_registry/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/submission_registry/submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/submission_registry/submission_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.109452 metldata-0.3.6/metldata/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/transform/artifact_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/transform/handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/transform/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-23 14:24:06.000000 metldata-0.3.6/metldata/transform/source_event_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.089452 metldata-0.3.6/metldata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-06-23 14:24:21.000000 metldata-0.3.6/metldata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-23 14:24:21.000000 metldata-0.3.6/metldata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:24:21.000000 metldata-0.3.6/metldata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 14:24:21.000000 metldata-0.3.6/metldata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:24:20.000000 metldata-0.3.6/metldata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-23 14:24:21.000000 metldata-0.3.6/metldata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 14:24:21.000000 metldata-0.3.6/metldata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-23 14:24:21.121452 metldata-0.3.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-23 14:24:06.000000 metldata-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.109452 metldata-0.3.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.109452 metldata-0.3.6/tests/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/accession_registry/test_accession_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/accession_registry/test_accession_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.109452 metldata-0.3.6/tests/artifact_rest/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/artifact_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/artifact_rest/test_api_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/artifact_rest/test_artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/artifact_rest/test_load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/artifact_rest/test_query_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.109452 metldata-0.3.6/tests/builtin_tranformations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.109452 metldata-0.3.6/tests/builtin_tranformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/infer_references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.113452 metldata-0.3.6/tests/builtin_tranformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/infer_references/path/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/infer_references/path/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/infer_references/path/test_path_str.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.113452 metldata-0.3.6/tests/builtin_tranformations/merge_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/merge_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/merge_slots/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/merge_slots/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_tranformations/test_happy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.113452 metldata-0.3.6/tests/builtin_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/builtin_workflows/test_happy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.113452 metldata-0.3.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/metadata_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/fixtures/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.117452 metldata-0.3.6/tests/load/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/load/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/load/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.117452 metldata-0.3.6/tests/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/test_anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/test_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/test_essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/test_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/test_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/model_utils/test_metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.117452 metldata-0.3.6/tests/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/submission_registry/test_event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/submission_registry/test_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/submission_registry/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/submission_registry/test_submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/submission_registry/test_submission_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/test_event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/test_metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:24:21.121452 metldata-0.3.6/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/transform/test_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-23 14:24:06.000000 metldata-0.3.6/tests/transform/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.114096 metldata-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-25 08:40:48.000000 metldata-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-07-25 08:41:00.114096 metldata-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-07-25 08:40:48.000000 metldata-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.086095 metldata-0.3.7/metldata/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.086095 metldata-0.3.7/metldata/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/accession_registry/accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/accession_registry/accession_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/accession_registry/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.090095 metldata-0.3.7/metldata/artifacts_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/artifact_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/load_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/artifacts_rest/query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.090095 metldata-0.3.7/metldata/builtin_transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.090095 metldata-0.3.7/metldata/builtin_transformations/add_accessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/add_accessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/add_accessions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/add_accessions/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/add_accessions/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/add_accessions/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.090095 metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.090095 metldata-0.3.7/metldata/builtin_transformations/delete_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/delete_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/delete_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/delete_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/delete_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/delete_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/delete_slots/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.094096 metldata-0.3.7/metldata/builtin_transformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.094096 metldata-0.3.7/metldata/builtin_transformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/path/path_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/path/path_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/path/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/infer_references/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.094096 metldata-0.3.7/metldata/builtin_transformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/merge_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/merge_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/merge_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/merge_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/merge_slots/model_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_transformations/merge_slots/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.094096 metldata-0.3.7/metldata/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/builtin_workflows/ghga_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.098096 metldata-0.3.7/metldata/event_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/event_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/event_handling/artifact_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/event_handling/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/event_handling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/event_handling/submission_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.098096 metldata-0.3.7/metldata/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.098096 metldata-0.3.7/metldata/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/model_utils/metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.102096 metldata-0.3.7/metldata/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/submission_registry/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/submission_registry/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/submission_registry/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/submission_registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/submission_registry/submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/submission_registry/submission_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.102096 metldata-0.3.7/metldata/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/transform/artifact_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/transform/handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/transform/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-25 08:40:48.000000 metldata-0.3.7/metldata/transform/source_event_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.086095 metldata-0.3.7/metldata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-07-25 08:41:00.000000 metldata-0.3.7/metldata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-25 08:41:00.000000 metldata-0.3.7/metldata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:41:00.000000 metldata-0.3.7/metldata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 08:41:00.000000 metldata-0.3.7/metldata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:40:59.000000 metldata-0.3.7/metldata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-25 08:41:00.000000 metldata-0.3.7/metldata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:41:00.000000 metldata-0.3.7/metldata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/get_package_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/license_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/scripts/script_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/script_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/script_utils/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1461 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/update_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/update_config_docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/update_readme.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-25 08:40:48.000000 metldata-0.3.7/scripts/update_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 08:41:00.114096 metldata-0.3.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-25 08:40:48.000000 metldata-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/tests/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/accession_registry/test_accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/accession_registry/test_accession_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/tests/artifact_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/artifact_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/artifact_rest/test_api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/artifact_rest/test_artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/artifact_rest/test_load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/artifact_rest/test_query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/tests/builtin_tranformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/tests/builtin_tranformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/infer_references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.106096 metldata-0.3.7/tests/builtin_tranformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/infer_references/path/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/infer_references/path/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/infer_references/path/test_path_str.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.110096 metldata-0.3.7/tests/builtin_tranformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/merge_slots/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/merge_slots/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_tranformations/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.110096 metldata-0.3.7/tests/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/builtin_workflows/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.110096 metldata-0.3.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/metadata_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/fixtures/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.110096 metldata-0.3.7/tests/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/load/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/load/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.114096 metldata-0.3.7/tests/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/test_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/test_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/test_essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/test_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/model_utils/test_metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.114096 metldata-0.3.7/tests/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/submission_registry/test_event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/submission_registry/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/submission_registry/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/submission_registry/test_submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/submission_registry/test_submission_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/test_metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:41:00.114096 metldata-0.3.7/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/transform/test_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-25 08:40:48.000000 metldata-0.3.7/tests/transform/test_main.py
```

### Comparing `metldata-0.3.6/LICENSE` & `metldata-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/PKG-INFO` & `metldata-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metldata
-Version: 0.3.6
+Version: 0.3.7
 Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 Home-page: https://github.com/ghga-de/metldata
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -76,29 +76,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.3.6
+docker pull ghga/metldata:0.3.7
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.3.6 .
+docker build -t ghga/metldata:0.3.7 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.3.6 --help
+docker run -p 8080:8080 ghga/metldata:0.3.7 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.3.6/README.md` & `metldata-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.3.6
+docker pull ghga/metldata:0.3.7
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.3.6 .
+docker build -t ghga/metldata:0.3.7 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.3.6 --help
+docker run -p 8080:8080 ghga/metldata:0.3.7 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.3.6/metldata/__init__.py` & `metldata-0.3.7/metldata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Short description of package"""  # Please adapt to package
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
```

### Comparing `metldata-0.3.6/metldata/__main__.py` & `metldata-0.3.7/metldata/__main__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/accession_registry/__init__.py` & `metldata-0.3.7/metldata/accession_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/accession_registry/accession_registry.py` & `metldata-0.3.7/metldata/accession_registry/accession_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/accession_registry/accession_store.py` & `metldata-0.3.7/metldata/accession_registry/accession_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/accession_registry/config.py` & `metldata-0.3.7/metldata/accession_registry/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/__init__.py` & `metldata-0.3.7/metldata/artifacts_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/api_factory.py` & `metldata-0.3.7/metldata/artifacts_rest/api_factory.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/artifact_dao.py` & `metldata-0.3.7/metldata/artifacts_rest/artifact_dao.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/artifact_info.py` & `metldata-0.3.7/metldata/artifacts_rest/artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/config.py` & `metldata-0.3.7/metldata/artifacts_rest/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/load_resources.py` & `metldata-0.3.7/metldata/artifacts_rest/load_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/models.py` & `metldata-0.3.7/metldata/artifacts_rest/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/artifacts_rest/query_resources.py` & `metldata-0.3.7/metldata/artifacts_rest/query_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/__init__.py` & `metldata-0.3.7/metldata/builtin_transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/add_accessions/__init__.py` & `metldata-0.3.7/metldata/builtin_transformations/add_accessions/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/add_accessions/config.py` & `metldata-0.3.7/metldata/builtin_transformations/add_accessions/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/add_accessions/main.py` & `metldata-0.3.7/metldata/builtin_transformations/add_accessions/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/add_accessions/metadata_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/add_accessions/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/add_accessions/model_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/add_accessions/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/__init__.py` & `metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/config.py` & `metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/embedding_profile.py` & `metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/embedding_profile.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/main.py` & `metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/metadata_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/custom_embeddings/model_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/custom_embeddings/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/delete_slots/__init__.py` & `metldata-0.3.7/metldata/builtin_transformations/delete_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/delete_slots/assumptions.py` & `metldata-0.3.7/metldata/builtin_transformations/delete_slots/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/delete_slots/config.py` & `metldata-0.3.7/metldata/builtin_transformations/delete_slots/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/delete_slots/main.py` & `metldata-0.3.7/metldata/builtin_transformations/delete_slots/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/delete_slots/metadata_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/delete_slots/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/delete_slots/model_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/delete_slots/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/__init__.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/config.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/main.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/metadata_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/model_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/path/__init__.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/path/path.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/path/path.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/path/path_elements.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/path/path_elements.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/path/path_str.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/path/path_str.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/path/resolve.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/path/resolve.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/infer_references/reference.py` & `metldata-0.3.7/metldata/builtin_transformations/infer_references/reference.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/merge_slots/__init__.py` & `metldata-0.3.7/metldata/builtin_transformations/merge_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/merge_slots/assumptions.py` & `metldata-0.3.7/metldata/builtin_transformations/merge_slots/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/merge_slots/config.py` & `metldata-0.3.7/metldata/builtin_transformations/merge_slots/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/merge_slots/main.py` & `metldata-0.3.7/metldata/builtin_transformations/merge_slots/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/merge_slots/metadata_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/merge_slots/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/merge_slots/model_transform.py` & `metldata-0.3.7/metldata/builtin_transformations/merge_slots/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_transformations/merge_slots/models.py` & `metldata-0.3.7/metldata/builtin_transformations/merge_slots/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_workflows/__init__.py` & `metldata-0.3.7/metldata/builtin_workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/builtin_workflows/ghga_archive.py` & `metldata-0.3.7/metldata/builtin_workflows/ghga_archive.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/cli.py` & `metldata-0.3.7/metldata/cli.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/combined.py` & `metldata-0.3.7/metldata/combined.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/config.py` & `metldata-0.3.7/metldata/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/custom_types.py` & `metldata-0.3.7/metldata/custom_types.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/event_handling/__init__.py` & `metldata-0.3.7/metldata/event_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/event_handling/artifact_events.py` & `metldata-0.3.7/metldata/event_handling/artifact_events.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/event_handling/event_handling.py` & `metldata-0.3.7/metldata/event_handling/event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/event_handling/models.py` & `metldata-0.3.7/metldata/event_handling/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/event_handling/submission_events.py` & `metldata-0.3.7/metldata/event_handling/submission_events.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/__init__.py` & `metldata-0.3.7/metldata/load/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/api.py` & `metldata-0.3.7/metldata/load/api.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/auth.py` & `metldata-0.3.7/metldata/load/auth.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/client.py` & `metldata-0.3.7/metldata/load/client.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/collect.py` & `metldata-0.3.7/metldata/load/collect.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/config.py` & `metldata-0.3.7/metldata/load/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/load.py` & `metldata-0.3.7/metldata/load/load.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/main.py` & `metldata-0.3.7/metldata/load/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/load/models.py` & `metldata-0.3.7/metldata/load/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/metadata_utils.py` & `metldata-0.3.7/metldata/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/model_utils/__init__.py` & `metldata-0.3.7/metldata/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/model_utils/anchors.py` & `metldata-0.3.7/metldata/model_utils/anchors.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/model_utils/assumptions.py` & `metldata-0.3.7/metldata/model_utils/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/model_utils/config.py` & `metldata-0.3.7/metldata/model_utils/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/model_utils/essentials.py` & `metldata-0.3.7/metldata/model_utils/essentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,57 +18,57 @@
 
 from __future__ import annotations
 
 import dataclasses
 import json
 from contextlib import contextmanager
 from copy import copy, deepcopy
-from functools import lru_cache
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Any, Generator
 
 import jsonasobj2
 import yaml
 from linkml_runtime import SchemaView
 from linkml_runtime.linkml_model import SchemaDefinition
 
 # The name of the root class of a model:
 ROOT_CLASS = "Submission"
 
 
-@lru_cache
-def schema_view_from_model(model: MetadataModel) -> SchemaView:
-    """Get a schema view instance from the metadata model."""
-
-    return ExportableSchemaView(model)
-
-
 class MetadataModel(SchemaDefinition):
     """A dataclass for describing metadata models."""
 
+    _schema_view = None
+
     @classmethod
     def init_from_path(cls, model_path: Path) -> MetadataModel:
         """Initialize from a model file in yaml format."""
 
         with open(model_path, "r", encoding="utf-8") as file:
             model_json = yaml.safe_load(file)
 
         return cls(**model_json)
 
     @property
     def schema_view(self) -> ExportableSchemaView:
         """Get a schema view instance from the metadata model."""
-
-        return schema_view_from_model(self)
-
-    def copy(self) -> MetadataModel:
-        """Copy the model."""
-
-        return deepcopy(self)
+        schema_view = self._schema_view
+        if schema_view is None:
+            schema_view = ExportableSchemaView(self)
+            self._schema_view = schema_view
+        return schema_view
+
+    def __deepcopy__(self, memo: Any):
+        """Return a deep copy of the model."""
+        schema_view = self._schema_view
+        self._schema_view = None
+        copied_model = deepcopy(super())
+        self._schema_view = schema_view
+        return copied_model
 
     def __eq__(self, other: object):
         """For comparisons."""
 
         if not isinstance(other, MetadataModel):
             return NotImplemented
 
@@ -137,19 +137,14 @@
 
         with NamedTemporaryFile(mode="w", encoding="utf-8") as file:
             model_json = self.as_dict()
             yaml.safe_dump(model_json, file)
             file.flush()
             yield Path(file.name)
 
-    def __hash__(self):
-        """Return a hash of the model."""
-
-        return hash(self.as_json())
-
 
 class ExportableSchemaView(SchemaView):
     """Extend the SchemaView by adding a method for exporting a MetadataModel."""
 
     def __copy__(self):
         """Return a copy of the model.
```

### Comparing `metldata-0.3.6/metldata/model_utils/identifiers.py` & `metldata-0.3.7/metldata/model_utils/identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/model_utils/manipulate.py` & `metldata-0.3.7/metldata/model_utils/manipulate.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/model_utils/metadata_validator.py` & `metldata-0.3.7/metldata/model_utils/metadata_validator.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/submission_registry/__init__.py` & `metldata-0.3.7/metldata/submission_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/submission_registry/config.py` & `metldata-0.3.7/metldata/submission_registry/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/submission_registry/event_publisher.py` & `metldata-0.3.7/metldata/submission_registry/event_publisher.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/submission_registry/identifiers.py` & `metldata-0.3.7/metldata/submission_registry/identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/submission_registry/models.py` & `metldata-0.3.7/metldata/submission_registry/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/submission_registry/submission_registry.py` & `metldata-0.3.7/metldata/submission_registry/submission_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/submission_registry/submission_store.py` & `metldata-0.3.7/metldata/submission_registry/submission_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/transform/__init__.py` & `metldata-0.3.7/metldata/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/transform/artifact_publisher.py` & `metldata-0.3.7/metldata/transform/artifact_publisher.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/transform/base.py` & `metldata-0.3.7/metldata/transform/base.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/transform/config.py` & `metldata-0.3.7/metldata/transform/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/transform/handling.py` & `metldata-0.3.7/metldata/transform/handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     WorkflowConfig,
     WorkflowDefinition,
     WorkflowStep,
     WorkflowStepBase,
 )
 
 
-class WorkflowConfigMissmatchError(RuntimeError):
+class WorkflowConfigMismatchError(RuntimeError):
     """Raised when the provided workflow config does not match the config class of the
     workflow definition.
     """
 
     def __init__(
         self, workflow_definition: WorkflowDefinition, workflow_config: Config
     ):
@@ -136,19 +136,19 @@
 def check_workflow_config(
     *, workflow_definition: WorkflowDefinition, workflow_config: WorkflowConfig
 ):
     """Checks if the config is an instance of the config class of the workflow
     definition.
 
     Raises:
-        WorkflowConfigMissmatchError:
+        WorkflowConfigMismatchError:
     """
 
     if workflow_config.schema_json() == workflow_definition.schema_json():
-        raise WorkflowConfigMissmatchError(
+        raise WorkflowConfigMismatchError(
             workflow_definition=workflow_definition, workflow_config=workflow_config
         )
 
 
 def resolve_workflow_step(
     *,
     workflow_step: WorkflowStep,
```

### Comparing `metldata-0.3.6/metldata/transform/main.py` & `metldata-0.3.7/metldata/transform/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata/transform/source_event_subscriber.py` & `metldata-0.3.7/metldata/transform/source_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/metldata.egg-info/PKG-INFO` & `metldata-0.3.7/metldata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metldata
-Version: 0.3.6
+Version: 0.3.7
 Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 Home-page: https://github.com/ghga-de/metldata
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -76,29 +76,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.3.6
+docker pull ghga/metldata:0.3.7
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.3.6 .
+docker build -t ghga/metldata:0.3.7 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.3.6 --help
+docker run -p 8080:8080 ghga/metldata:0.3.7 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.3.6/metldata.egg-info/SOURCES.txt` & `metldata-0.3.7/metldata.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -98,14 +98,23 @@
 metldata/transform/__init__.py
 metldata/transform/artifact_publisher.py
 metldata/transform/base.py
 metldata/transform/config.py
 metldata/transform/handling.py
 metldata/transform/main.py
 metldata/transform/source_event_subscriber.py
+scripts/__init__.py
+scripts/get_package_name.py
+scripts/license_checker.py
+scripts/update_all.py
+scripts/update_config_docs.py
+scripts/update_readme.py
+scripts/update_template_files.py
+scripts/script_utils/__init__.py
+scripts/script_utils/cli.py
 tests/test_event_handling.py
 tests/test_metadata_utils.py
 tests/accession_registry/__init__.py
 tests/accession_registry/test_accession_registry.py
 tests/accession_registry/test_accession_store.py
 tests/artifact_rest/__init__.py
 tests/artifact_rest/test_api_factory.py
@@ -126,14 +135,15 @@
 tests/builtin_workflows/test_happy.py
 tests/fixtures/__init__.py
 tests/fixtures/artifact_info.py
 tests/fixtures/config.py
 tests/fixtures/event_handling.py
 tests/fixtures/metadata.py
 tests/fixtures/metadata_models.py
+tests/fixtures/mongodb.py
 tests/fixtures/transformations.py
 tests/fixtures/utils.py
 tests/fixtures/workflows.py
 tests/load/__init__.py
 tests/load/test_client.py
 tests/load/test_main.py
 tests/model_utils/__init__.py
```

### Comparing `metldata-0.3.6/setup.cfg` & `metldata-0.3.7/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	hexkit[mongodb]==0.10.0
-	ghga-service-commons[api,auth]==0.4.2
+	hexkit[mongodb]==0.10.2
+	ghga-service-commons[api,auth]==0.4.3
 	typer==0.7.0
-	linkml-runtime==1.4.2
+	linkml==1.5.6
+	linkml-runtime==1.5.5
 	linkml-validator==0.4.5
 python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	metldata = metldata.__main__:run
```

### Comparing `metldata-0.3.6/setup.py` & `metldata-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/accession_registry/__init__.py` & `metldata-0.3.7/tests/accession_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/accession_registry/test_accession_registry.py` & `metldata-0.3.7/tests/accession_registry/test_accession_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/accession_registry/test_accession_store.py` & `metldata-0.3.7/tests/accession_registry/test_accession_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/artifact_rest/__init__.py` & `metldata-0.3.7/tests/artifact_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/artifact_rest/test_api_factory.py` & `metldata-0.3.7/tests/artifact_rest/test_api_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 
 
 import httpx
 import pytest
 from fastapi import FastAPI
 from ghga_service_commons.api.testing import AsyncTestClient
 from hexkit.protocols.dao import DaoFactoryProtocol
-from hexkit.providers.mongodb.testutils import mongodb_fixture  # noqa: F401
-from hexkit.providers.mongodb.testutils import MongoDbFixture
 
 from metldata.artifacts_rest.api_factory import rest_api_factory
 from metldata.artifacts_rest.artifact_info import ArtifactInfo
 from tests.artifact_rest.test_load_artifacts import load_example_artifact_resources
 from tests.fixtures.artifact_info import EXAMPLE_ARTIFACT_INFOS, MINIMAL_ARTIFACT_INFO
+from tests.fixtures.mongodb import (  # noqa: F401; pylint: disable=unused-import
+    MongoDbFixture,
+    mongodb_fixture,
+)
 
 
 @pytest.mark.asyncio
 async def get_example_app_client(
     dao_factory: DaoFactoryProtocol,
     artifact_infos: list[ArtifactInfo] = EXAMPLE_ARTIFACT_INFOS,
 ) -> httpx.AsyncClient:
@@ -44,15 +46,17 @@
 
     app = FastAPI()
     app.include_router(router)
     return AsyncTestClient(app)
 
 
 @pytest.mark.asyncio
-async def test_artifacts_info_endpoint(mongodb_fixture: MongoDbFixture):  # noqa: F811
+async def test_artifacts_info_endpoint(
+    mongodb_fixture: MongoDbFixture,  # noqa: F811
+):
     """Test happy path of using the artifacts info endpoint."""
 
     expected_infos = EXAMPLE_ARTIFACT_INFOS
 
     async with await get_example_app_client(
         dao_factory=mongodb_fixture.dao_factory
     ) as client:
@@ -95,15 +99,16 @@
     await load_example_artifact_resources(dao_factory=mongodb_fixture.dao_factory)
 
     # Get an example resource:
     artifact_name = MINIMAL_ARTIFACT_INFO.name
     class_name = "File"
     resource_id = "test_sample_01_R1"
     async with await get_example_app_client(
-        dao_factory=mongodb_fixture.dao_factory, artifact_infos=[MINIMAL_ARTIFACT_INFO]
+        dao_factory=mongodb_fixture.dao_factory,
+        artifact_infos=[MINIMAL_ARTIFACT_INFO],
     ) as client:
         response = await client.get(
             f"/artifacts/{artifact_name}/classes/{class_name}/resources/{resource_id}"
         )
 
     assert response.status_code == 200
     observed_resource = response.json()
```

### Comparing `metldata-0.3.6/tests/artifact_rest/test_artifact_info.py` & `metldata-0.3.7/tests/artifact_rest/test_artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/artifact_rest/test_load_artifacts.py` & `metldata-0.3.7/tests/artifact_rest/test_load_artifacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 # limitations under the License.
 #
 
 """Test the load_artifacts module"""
 
 import pytest
 from hexkit.protocols.dao import DaoFactoryProtocol
-from hexkit.providers.mongodb.testutils import mongodb_fixture  # noqa: F401
-from hexkit.providers.mongodb.testutils import MongoDbFixture
 
 from metldata.artifacts_rest.artifact_dao import ArtifactDaoCollection
 from metldata.artifacts_rest.load_resources import load_artifact_resources
 from metldata.artifacts_rest.models import ArtifactResource
 from tests.fixtures.artifact_info import MINIMAL_ARTIFACT_INFO
 from tests.fixtures.metadata import VALID_MINIMAL_METADATA_EXAMPLE
+from tests.fixtures.mongodb import (  # noqa: F401; pylint: disable=unused-import
+    MongoDbFixture,
+    mongodb_fixture,
+)
 
 
 async def load_example_artifact_resources(
     dao_factory: DaoFactoryProtocol,
 ) -> ArtifactDaoCollection:
     """Load the example artifact using the load_artifact_resources function and
     returns a ArtifactDaoCollection for accessing the resources."""
@@ -47,15 +49,17 @@
         dao_collection=dao_collection,
     )
 
     return dao_collection
 
 
 @pytest.mark.asyncio
-async def test_load_artifact_resources(mongodb_fixture: MongoDbFixture):  # noqa: F811
+async def test_load_artifact_resources(
+    mongodb_fixture: MongoDbFixture,  # noqa: F811
+):
     """Test happy path of using load_artifact_resources function."""
 
     dao_collection = await load_example_artifact_resources(
         dao_factory=mongodb_fixture.dao_factory,
     )
 
     # check that artifact resources have been persisted to the database by testing for
```

### Comparing `metldata-0.3.6/tests/artifact_rest/test_query_resources.py` & `metldata-0.3.7/tests/artifact_rest/test_query_resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,24 +13,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Test the query_resource module."""
 
 import pytest
-from hexkit.providers.mongodb.testutils import mongodb_fixture  # noqa: F401
-from hexkit.providers.mongodb.testutils import MongoDbFixture
 
 from metldata.artifacts_rest.query_resources import query_artifact_resource
 from tests.artifact_rest.test_load_artifacts import load_example_artifact_resources
 from tests.fixtures.artifact_info import MINIMAL_ARTIFACT_INFO
+from tests.fixtures.mongodb import (  # noqa: F401; pylint: disable=unused-import
+    MongoDbFixture,
+    mongodb_fixture,
+)
 
 
 @pytest.mark.asyncio
-async def test_query_artifact_resource(mongodb_fixture: MongoDbFixture):  # noqa: F811
+async def test_query_artifact_resource(
+    mongodb_fixture: MongoDbFixture,  # noqa: F811
+):
     """Test happy path of using the query_artifact_resource function."""
 
     # load example resources and prepare client:
     dao_collection = await load_example_artifact_resources(
         dao_factory=mongodb_fixture.dao_factory
     )
```

### Comparing `metldata-0.3.6/tests/builtin_tranformations/__init__.py` & `metldata-0.3.7/tests/builtin_tranformations/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/infer_references/__init__.py` & `metldata-0.3.7/tests/builtin_tranformations/infer_references/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/infer_references/path/__init__.py` & `metldata-0.3.7/tests/builtin_tranformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/infer_references/path/test_config.py` & `metldata-0.3.7/tests/builtin_tranformations/infer_references/path/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/infer_references/path/test_path.py` & `metldata-0.3.7/tests/builtin_tranformations/infer_references/path/test_path.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/infer_references/path/test_path_str.py` & `metldata-0.3.7/tests/builtin_tranformations/infer_references/path/test_path_str.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/merge_slots/__init__.py` & `metldata-0.3.7/tests/builtin_tranformations/merge_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/merge_slots/test_config.py` & `metldata-0.3.7/tests/builtin_tranformations/merge_slots/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/merge_slots/test_models.py` & `metldata-0.3.7/tests/builtin_tranformations/merge_slots/test_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_tranformations/test_happy.py` & `metldata-0.3.7/tests/builtin_tranformations/test_happy.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_workflows/__init__.py` & `metldata-0.3.7/tests/builtin_workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/builtin_workflows/test_happy.py` & `metldata-0.3.7/tests/builtin_workflows/test_happy.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/__init__.py` & `metldata-0.3.7/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/artifact_info.py` & `metldata-0.3.7/tests/fixtures/artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/config.py` & `metldata-0.3.7/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/event_handling.py` & `metldata-0.3.7/tests/fixtures/event_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Event,
     FileSystemEventCollector,
     FileSystemEventConfig,
     FileSystemEventPublisher,
 )
 
 
-class EventExpectationMissmatch(RuntimeError):
+class EventExpectationMismatch(RuntimeError):
     """Raised when expected events where not found."""
 
     def __init__(self, expected_events: set[str], consumed_events: set[str]):
         message = f"Expected events '{expected_events}' but got '{consumed_events}'"
         super().__init__(message)
 
 
@@ -45,15 +45,15 @@
     publisher: FileSystemEventPublisher
     collector: FileSystemEventCollector
 
     def expect_events(self, expected_events: list[Event]) -> None:
         """Check if the events expected to be published can be consumed.
 
         Raises:
-            EventExpectationMissmatch: If the expected events are not consumed.
+            EventExpectationMismatch: If the expected events are not consumed.
         """
 
         topics = sorted({event.topic for event in expected_events})
         types = sorted({event.type_ for event in expected_events})
 
         observed_events: list[Event] = []
         for topic in topics:
@@ -62,15 +62,15 @@
             )
 
         # hashable versions for comparison:
         observed_event_jsons = {event.json() for event in observed_events}
         expected_event_jsons = {event.json() for event in expected_events}
 
         if expected_event_jsons != observed_event_jsons:
-            raise EventExpectationMissmatch(
+            raise EventExpectationMismatch(
                 expected_events=observed_event_jsons,
                 consumed_events=expected_event_jsons,
             )
 
     async def publish_events(self, events: list[Event]) -> None:
         """Publish a list of events."""
```

### Comparing `metldata-0.3.6/tests/fixtures/metadata.py` & `metldata-0.3.7/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/metadata_models.py` & `metldata-0.3.7/tests/fixtures/metadata_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/transformations.py` & `metldata-0.3.7/tests/fixtures/transformations.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/utils.py` & `metldata-0.3.7/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/fixtures/workflows.py` & `metldata-0.3.7/tests/fixtures/workflows.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/load/__init__.py` & `metldata-0.3.7/tests/load/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/load/test_client.py` & `metldata-0.3.7/tests/load/test_client.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/load/test_main.py` & `metldata-0.3.7/tests/load/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 #
 
 """Test the main modules."""
 
 import pytest
 from ghga_service_commons.api.testing import AsyncTestClient
 from hexkit.protocols.dao import ResourceNotFoundError
-from hexkit.providers.mongodb.testutils import mongodb_fixture  # noqa: F401
-from hexkit.providers.mongodb.testutils import MongoDbFixture
 
 from metldata.artifacts_rest.artifact_dao import ArtifactDaoCollection
 from metldata.artifacts_rest.models import ArtifactInfo
 from metldata.load.auth import generate_token, generate_token_and_hash
 from metldata.load.config import ArtifactLoaderAPIConfig
 from metldata.load.main import get_app
 from tests.fixtures.artifact_info import EXAMPLE_ARTIFACT_INFOS
+from tests.fixtures.mongodb import (  # noqa: F401; pylint: disable=unused-import
+    MongoDbFixture,
+    mongodb_fixture,
+)
 from tests.fixtures.workflows import EXAMPLE_ARTIFACTS
 
 
 async def get_configured_client(
     mongodb_fixture: MongoDbFixture,  # noqa: F811
     artifact_infos: list[ArtifactInfo],
 ) -> tuple[AsyncTestClient, str]:
@@ -77,15 +79,16 @@
     expected_resource_content = {
         "alias": "test_sample_01_R1",
         "format": "fastq",
         "size": 299943,
     }
 
     dao_collection = await ArtifactDaoCollection.construct(
-        dao_factory=mongodb_fixture.dao_factory, artifact_infos=EXAMPLE_ARTIFACT_INFOS
+        dao_factory=mongodb_fixture.dao_factory,
+        artifact_infos=EXAMPLE_ARTIFACT_INFOS,
     )
     dao = await dao_collection.get_dao(
         artifact_name=expected_artifact_name, class_name=expected_resource_class
     )
 
     observed_resource = await dao.get_by_id(expected_resource_id)
     assert observed_resource.content == expected_resource_content
```

### Comparing `metldata-0.3.6/tests/model_utils/__init__.py` & `metldata-0.3.7/tests/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/model_utils/test_anchor.py` & `metldata-0.3.7/tests/model_utils/test_anchor.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/model_utils/test_assumptions.py` & `metldata-0.3.7/tests/model_utils/test_assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/model_utils/test_config.py` & `metldata-0.3.7/tests/model_utils/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/model_utils/test_essentials.py` & `metldata-0.3.7/tests/model_utils/test_essentials.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/model_utils/test_identifiers.py` & `metldata-0.3.7/tests/model_utils/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/model_utils/test_manipulate.py` & `metldata-0.3.7/tests/model_utils/test_manipulate.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/model_utils/test_metadata_validator.py` & `metldata-0.3.7/tests/model_utils/test_metadata_validator.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/submission_registry/__init__.py` & `metldata-0.3.7/tests/submission_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/submission_registry/test_event_publisher.py` & `metldata-0.3.7/tests/submission_registry/test_event_publisher.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/submission_registry/test_identifiers.py` & `metldata-0.3.7/tests/submission_registry/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/submission_registry/test_models.py` & `metldata-0.3.7/tests/submission_registry/test_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/submission_registry/test_submission_registry.py` & `metldata-0.3.7/tests/submission_registry/test_submission_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/submission_registry/test_submission_store.py` & `metldata-0.3.7/tests/submission_registry/test_submission_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/test_event_handling.py` & `metldata-0.3.7/tests/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/test_metadata_utils.py` & `metldata-0.3.7/tests/test_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/transform/__init__.py` & `metldata-0.3.7/tests/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/transform/test_base.py` & `metldata-0.3.7/tests/transform/test_base.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/transform/test_handling.py` & `metldata-0.3.7/tests/transform/test_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.6/tests/transform/test_main.py` & `metldata-0.3.7/tests/transform/test_main.py`

 * *Files identical despite different names*

