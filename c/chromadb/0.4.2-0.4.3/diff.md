# Comparing `tmp/chromadb-0.4.2.tar.gz` & `tmp/chromadb-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-0.4.2.tar", last modified: Wed Jul 19 05:00:29 2023, max compression
+gzip compressed data, was "chromadb-0.4.3.tar", last modified: Tue Jul 25 05:11:15 2023, max compression
```

## Comparing `chromadb-0.4.2.tar` & `chromadb-0.4.3.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.919031 chromadb-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-19 05:00:14.000000 chromadb-0.4.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.843031 chromadb-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.859031 chromadb-0.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.863031 chromadb-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/workflows/chroma-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/workflows/chroma-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-19 05:00:14.000000 chromadb-0.4.2/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 05:00:14.000000 chromadb-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-19 05:00:14.000000 chromadb-0.4.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.863031 chromadb-0.4.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-19 05:00:14.000000 chromadb-0.4.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-19 05:00:14.000000 chromadb-0.4.2/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-19 05:00:14.000000 chromadb-0.4.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 05:00:14.000000 chromadb-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-19 05:00:29.919031 chromadb-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-19 05:00:14.000000 chromadb-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-19 05:00:14.000000 chromadb-0.4.2/RELEASE_PROCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.867031 chromadb-0.4.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/build
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/docker_entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/generate_cloudformation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/integration-test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.867031 chromadb-0.4.2/bin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/templates/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/test-package.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/test-remote
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-19 05:00:14.000000 chromadb-0.4.2/bin/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.867031 chromadb-0.4.2/chromadb/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.871031 chromadb-0.4.2/chromadb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/api/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.871031 chromadb-0.4.2/chromadb/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/api/models/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/api/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.871031 chromadb-0.4.2/chromadb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.871031 chromadb-0.4.2/chromadb/db/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/impl/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/impl/sqlite_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.871031 chromadb-0.4.2/chromadb/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/db/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/experimental/density_relevance.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/migrations/embeddings_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/migrations/metadb/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/migrations/sysdb/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.847031 chromadb-0.4.2/chromadb/segment/impl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/segment/impl/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.875031 chromadb-0.4.2/chromadb/segment/impl/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.879031 chromadb-0.4.2/chromadb/segment/impl/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/impl/vector/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/impl/vector/brute_force_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/impl/vector/hnsw_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/impl/vector/local_hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/segment/impl/vector/local_persistent_hnsw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.879031 chromadb-0.4.2/chromadb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.879031 chromadb-0.4.2/chromadb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.879031 chromadb-0.4.2/chromadb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.883031 chromadb-0.4.2/chromadb/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.883031 chromadb-0.4.2/chromadb/test/db/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.887031 chromadb-0.4.2/chromadb/test/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/db/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.887031 chromadb-0.4.2/chromadb/test/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.887031 chromadb-0.4.2/chromadb/test/property/
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.891031 chromadb-0.4.2/chromadb/test/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/segment/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/test_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/test_multithreaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.891031 chromadb-0.4.2/chromadb/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.891031 chromadb-0.4.2/chromadb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/utils/distance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/utils/messageid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-19 05:00:14.000000 chromadb-0.4.2/chromadb/utils/read_write_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.867031 chromadb-0.4.2/chromadb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-19 05:00:29.000000 chromadb-0.4.2/chromadb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-19 05:00:29.000000 chromadb-0.4.2/chromadb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:00:29.000000 chromadb-0.4.2/chromadb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-19 05:00:29.000000 chromadb-0.4.2/chromadb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 05:00:29.000000 chromadb-0.4.2/chromadb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.851031 chromadb-0.4.2/clients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.895031 chromadb-0.4.2/clients/js/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.851031 chromadb-0.4.2/clients/js/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.899031 chromadb-0.4.2/clients/js/examples/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/browser/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/browser/app.ts
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/browser/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/browser/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.899031 chromadb-0.4.2/clients/js/examples/node/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/node/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/node/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/genapi.sh
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/openapitools.json
--rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.903031 chromadb-0.4.2/clients/js/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/ChromaClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/Collection.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.903031 chromadb-0.4.2/clients/js/src/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.911031 chromadb-0.4.2/clients/js/src/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/generated/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/generated/api.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/generated/configuration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/generated/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/generated/models.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/generated/runtime.ts
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/types.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/src/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.915031 chromadb-0.4.2/clients/js/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/add.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/collection.client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/get.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/initClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/query.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/update.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/tsconfig.module.json
--rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/js/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.915031 chromadb-0.4.2/clients/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/python/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/python/integration-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/python/is_thin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-19 05:00:14.000000 chromadb-0.4.2/clients/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-19 05:00:14.000000 chromadb-0.4.2/docker-compose.server.example.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-19 05:00:14.000000 chromadb-0.4.2/docker-compose.test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-19 05:00:14.000000 chromadb-0.4.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.915031 chromadb-0.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.915031 chromadb-0.4.2/examples/basic_functionality/
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/basic_functionality/alternative_embeddings.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/basic_functionality/local_persistence.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/basic_functionality/where_filtering.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.855031 chromadb-0.4.2/examples/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.919031 chromadb-0.4.2/examples/deployments/google-cloud-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/deployments/google-cloud-compute/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.855031 chromadb-0.4.2/examples/use_with/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:00:29.919031 chromadb-0.4.2/examples/use_with/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/use_with/cohere/cohere_js.js
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/use_with/cohere/cohere_python.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 05:00:14.000000 chromadb-0.4.2/examples/use_with/cohere/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-19 05:00:14.000000 chromadb-0.4.2/log_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-19 05:00:14.000000 chromadb-0.4.2/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-19 05:00:14.000000 chromadb-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-19 05:00:14.000000 chromadb-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-19 05:00:14.000000 chromadb-0.4.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:00:29.919031 chromadb-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.670656 chromadb-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-25 05:10:58.000000 chromadb-0.4.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.610655 chromadb-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.622655 chromadb-0.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.622655 chromadb-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 05:10:58.000000 chromadb-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 05:10:58.000000 chromadb-0.4.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.622655 chromadb-0.4.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 05:10:58.000000 chromadb-0.4.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-25 05:10:58.000000 chromadb-0.4.3/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-25 05:10:58.000000 chromadb-0.4.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 05:10:58.000000 chromadb-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-25 05:11:15.670656 chromadb-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-25 05:10:58.000000 chromadb-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-25 05:10:58.000000 chromadb-0.4.3/RELEASE_PROCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/integration-test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22439 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/db/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/impl/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/impl/sqlite_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/experimental/density_relevance.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/embeddings_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/metadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/sysdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.614655 chromadb-0.4.3/chromadb/segment/impl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/impl/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/impl/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/impl/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/brute_force_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/hnsw_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/local_hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/local_persistent_hnsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.638655 chromadb-0.4.3/chromadb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.638655 chromadb-0.4.3/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.638655 chromadb-0.4.3/chromadb/test/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/property/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_multithreaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.646655 chromadb-0.4.3/chromadb/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.646655 chromadb-0.4.3/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/distance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/messageid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/read_write_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/chromadb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.650655 chromadb-0.4.3/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.654655 chromadb-0.4.3/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.654655 chromadb-0.4.3/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/genapi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.658656 chromadb-0.4.3/clients/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/Collection.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.658656 chromadb-0.4.3/clients/js/src/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.662655 chromadb-0.4.3/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/models.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/types.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/initClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/clients/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/integration-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/is_thin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 05:10:58.000000 chromadb-0.4.3/docker-compose.server.example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-25 05:10:58.000000 chromadb-0.4.3/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 05:10:58.000000 chromadb-0.4.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/examples/basic_functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/basic_functionality/alternative_embeddings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/basic_functionality/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/basic_functionality/where_filtering.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/examples/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.670656 chromadb-0.4.3/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/examples/use_with/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.670656 chromadb-0.4.3/examples/use_with/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/use_with/cohere/cohere_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/use_with/cohere/cohere_python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/use_with/cohere/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 05:10:58.000000 chromadb-0.4.3/log_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-25 05:10:58.000000 chromadb-0.4.3/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-25 05:10:58.000000 chromadb-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 05:10:58.000000 chromadb-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 05:10:58.000000 chromadb-0.4.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:11:15.670656 chromadb-0.4.3/setup.cfg
```

### Comparing `chromadb-0.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-0.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-0.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-0.4.3/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/workflows/chroma-client-integration-test.yml` & `chromadb-0.4.3/.github/workflows/chroma-client-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/workflows/chroma-integration-test.yml` & `chromadb-0.4.3/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/workflows/chroma-release-python-client.yml` & `chromadb-0.4.3/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/workflows/chroma-release.yml` & `chromadb-0.4.3/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/workflows/chroma-test.yml` & `chromadb-0.4.3/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.github/workflows/pr-review-checklist.yml` & `chromadb-0.4.3/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.pre-commit-config.yaml` & `chromadb-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/.vscode/settings.json` & `chromadb-0.4.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/DEVELOP.md` & `chromadb-0.4.3/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/LICENSE` & `chromadb-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/PKG-INFO` & `chromadb-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.4.2
+Version: 0.4.3
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb Version: 0.4.2 Summary: Chroma. Author-
+Metadata-Version: 2.1 Name: chromadb Version: 0.4.3 Summary: Chroma. Author-
 email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-0.4.2/README.md` & `chromadb-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/RELEASE_PROCESS.md` & `chromadb-0.4.3/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/bin/generate_cloudformation.py` & `chromadb-0.4.3/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/__init__.py` & `chromadb-0.4.3/chromadb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chromadb.config import Settings, System
 from chromadb.api import API
 
 logger = logging.getLogger(__name__)
 
 __settings = Settings()
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 # Workaround to deal with Colab's old sqlite3 version
 try:
     import google.colab  # noqa: F401
 
     IN_COLAB = True
 except ImportError:
@@ -30,15 +30,15 @@
         subprocess.check_call(
             [sys.executable, "-m", "pip", "install", "pysqlite3-binary"]
         )
         __import__("pysqlite3")
         sys.modules["sqlite3"] = sys.modules.pop("pysqlite3")
     else:
         raise RuntimeError(
-            "\033[91mYour system has an unsupported version of sqlite3. Chroma requires sqlite3 >= 3.35.0.\033[0m"
+            "\033[91mYour system has an unsupported version of sqlite3. Chroma requires sqlite3 >= 3.35.0.\033[0m\n"
             "\033[94mPlease visit https://docs.trychroma.com/troubleshooting#sqlite to learn how to upgrade.\033[0m"
         )
 
 
 def configure(**kwargs) -> None:  # type: ignore
     """Override Chroma's default settings, environment variables or .env files"""
     global __settings
```

### Comparing `chromadb-0.4.2/chromadb/api/__init__.py` & `chromadb-0.4.3/chromadb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/api/fastapi.py` & `chromadb-0.4.3/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/api/models/Collection.py` & `chromadb-0.4.3/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/api/segment.py` & `chromadb-0.4.3/chromadb/api/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,8 +611,10 @@
     metadata map."""
     if not metadata:
         return None
     result = {}
     for k, v in metadata.items():
         if not k.startswith("chroma:"):
             result[k] = v
+    if len(result) == 0:
+        return None
     return result
```

### Comparing `chromadb-0.4.2/chromadb/api/types.py` & `chromadb-0.4.3/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/config.py` & `chromadb-0.4.3/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/__init__.py` & `chromadb-0.4.3/chromadb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/base.py` & `chromadb-0.4.3/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/impl/sqlite.py` & `chromadb-0.4.3/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/impl/sqlite_pool.py` & `chromadb-0.4.3/chromadb/db/impl/sqlite_pool.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/migrations.py` & `chromadb-0.4.3/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/mixins/embeddings_queue.py` & `chromadb-0.4.3/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/mixins/sysdb.py` & `chromadb-0.4.3/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/db/system.py` & `chromadb-0.4.3/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/errors.py` & `chromadb-0.4.3/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/experimental/density_relevance.ipynb` & `chromadb-0.4.3/chromadb/experimental/density_relevance.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/ingest/__init__.py` & `chromadb-0.4.3/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `chromadb-0.4.3/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/__init__.py` & `chromadb-0.4.3/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/impl/manager/local.py` & `chromadb-0.4.3/chromadb/segment/impl/manager/local.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/impl/metadata/sqlite.py` & `chromadb-0.4.3/chromadb/segment/impl/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/impl/vector/batch.py` & `chromadb-0.4.3/chromadb/segment/impl/vector/batch.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/impl/vector/brute_force_index.py` & `chromadb-0.4.3/chromadb/segment/impl/vector/brute_force_index.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/impl/vector/hnsw_params.py` & `chromadb-0.4.3/chromadb/segment/impl/vector/hnsw_params.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/impl/vector/local_hnsw.py` & `chromadb-0.4.3/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/segment/impl/vector/local_persistent_hnsw.py` & `chromadb-0.4.3/chromadb/segment/impl/vector/local_persistent_hnsw.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/server/fastapi/__init__.py` & `chromadb-0.4.3/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/server/fastapi/types.py` & `chromadb-0.4.3/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/telemetry/__init__.py` & `chromadb-0.4.3/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/telemetry/events.py` & `chromadb-0.4.3/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/telemetry/posthog.py` & `chromadb-0.4.3/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/conftest.py` & `chromadb-0.4.3/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/db/test_base.py` & `chromadb-0.4.3/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/db/test_migrations.py` & `chromadb-0.4.3/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/db/test_system.py` & `chromadb-0.4.3/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/ingest/test_producer_consumer.py` & `chromadb-0.4.3/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/property/invariants.py` & `chromadb-0.4.3/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/property/strategies.py` & `chromadb-0.4.3/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/property/test_add.py` & `chromadb-0.4.3/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/property/test_collections.py` & `chromadb-0.4.3/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/property/test_cross_version_persist.py` & `chromadb-0.4.3/chromadb/test/property/test_cross_version_persist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,34 @@
 from multiprocessing.connection import Connection
 import sys
 import os
 import shutil
 import subprocess
 import tempfile
 from types import ModuleType
-from typing import Callable, Generator, List, Tuple
+from typing import Generator, List, Tuple
 from hypothesis import given, settings
 import hypothesis.strategies as st
 import pytest
 import json
 from urllib import request
+from chromadb import config
 from chromadb.api import API
 from chromadb.api.types import Documents, EmbeddingFunction, Embeddings
 import chromadb.test.property.strategies as strategies
 import chromadb.test.property.invariants as invariants
 from packaging import version as packaging_version
 import re
 import multiprocessing
-from chromadb import Client
 from chromadb.config import Settings
 
-MINIMUM_VERSION = "0.3.20"
-COLLECTION_NAME_LOWERCASE_VERSION = "0.3.21"
+MINIMUM_VERSION = "0.4.1"
 version_re = re.compile(r"^[0-9]+\.[0-9]+\.[0-9]+$")
 
 
-def _patch_uppercase_coll_name(
-    collection: strategies.Collection, embeddings: strategies.RecordSet
-) -> None:
-    """Old versions didn't handle uppercase characters in collection names"""
-    collection.name = collection.name.lower()
-
-
-def _patch_empty_dict_metadata(
-    collection: strategies.Collection, embeddings: strategies.RecordSet
-) -> None:
-    """Old versions do the wrong thing when metadata is a single empty dict"""
-    if embeddings["metadatas"] == {}:
-        embeddings["metadatas"] = None
-
-
-version_patches: List[
-    Tuple[str, Callable[[strategies.Collection, strategies.RecordSet], None]]
-] = [
-    ("0.3.21", _patch_uppercase_coll_name),
-    ("0.3.21", _patch_empty_dict_metadata),
-]
-
-
-def patch_for_version(
-    version: str, collection: strategies.Collection, embeddings: strategies.RecordSet
-) -> None:
-    """Override aspects of the collection and embeddings, before testing, to account for
-    breaking changes in old versions."""
-
-    for patch_version, patch in version_patches:
-        if packaging_version.Version(version) <= packaging_version.Version(
-            patch_version
-        ):
-            patch(collection, embeddings)
-
-
 def versions() -> List[str]:
     """Returns the pinned minimum version and the latest version of chromadb."""
     url = "https://pypi.org/pypi/chromadb/json"
     data = json.load(request.urlopen(request.Request(url)))
     versions = list(data["releases"].keys())
     # Older versions on pypi contain "devXYZ" suffixes
     versions = [v for v in versions if version_re.match(v)]
@@ -81,15 +44,15 @@
                 chroma_api_impl="chromadb.api.segment.SegmentAPI",
                 chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
                 chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
                 chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
                 chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
                 allow_reset=True,
                 is_persistent=True,
-                persist_directory=tempfile.gettempdir(),
+                persist_directory=tempfile.gettempdir() + "/persistence_test_chromadb",
             ),
         )
         for version in versions
     ]
 
 
 test_old_versions = versions()
@@ -178,36 +141,43 @@
     settings: Settings,
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
     conn: Connection,
 ) -> None:
     try:
         old_module = switch_to_version(version)
-        api: API = old_module.Client(settings)
+        system = old_module.config.System(settings)
+        api: API = system.instance(API)
+        system.start()
+
         api.reset()
         coll = api.create_collection(
             name=collection_strategy.name,
             metadata=collection_strategy.metadata,
             # In order to test old versions, we can't rely on the not_implemented function
             embedding_function=not_implemented_ef(),
         )
         coll.add(**embeddings_strategy)
-        # We can't use the invariants module here because it uses the current version
+
         # Just use some basic checks for sanity and manual testing where you break the new
         # version
 
         check_embeddings = invariants.wrap_all(embeddings_strategy)
         # Check count
         assert coll.count() == len(check_embeddings["embeddings"] or [])
         # Check ids
         result = coll.get()
         actual_ids = result["ids"]
         embedding_id_to_index = {id: i for i, id in enumerate(check_embeddings["ids"])}
         actual_ids = sorted(actual_ids, key=lambda id: embedding_id_to_index[id])
         assert actual_ids == check_embeddings["ids"]
+
+        # Shutdown system
+        system.stop()
+
     except Exception as e:
         conn.send(e)
         raise e
 
 
 # Since we can't pickle the embedding function, we always generate record sets with embeddings
 collection_st: st.SearchStrategy[strategies.Collection] = st.shared(
@@ -215,34 +185,37 @@
 )
 
 
 @given(
     collection_strategy=collection_st,
     embeddings_strategy=strategies.recordsets(collection_st),
 )
-@pytest.mark.skipif(
-    sys.version_info.major < 3
-    or (sys.version_info.major == 3 and sys.version_info.minor <= 7),
-    reason="The mininum supported versions of chroma do not work with python <= 3.7",
-)
-@pytest.mark.xfail(
-    reason="As we migrate to sqlite, we will not support old versions of chromadb and instead require manual migration. The minimum version will be increased to 0.4.0 and this test will be expected to pass."
-)
 @settings(deadline=None)
 def test_cycle_versions(
     version_settings: Tuple[str, Settings],
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
 ) -> None:
-    # # Test backwards compatibility
-    # # For the current version, ensure that we can load a collection from
-    # # the previous versions
+    # Test backwards compatibility
+    # For the current version, ensure that we can load a collection from
+    # the previous versions
     version, settings = version_settings
 
-    patch_for_version(version, collection_strategy, embeddings_strategy)
+    # The strategies can generate metadatas of malformed inputs. Other tests
+    # will error check and cover these cases to make sure they error. Here we
+    # just convert them to valid values since the error cases are already tested
+    if embeddings_strategy["metadatas"] == {}:
+        embeddings_strategy["metadatas"] = None
+    if embeddings_strategy["metadatas"] is not None and isinstance(
+        embeddings_strategy["metadatas"], list
+    ):
+        embeddings_strategy["metadatas"] = [
+            m if m is None or len(m) > 0 else None  # type: ignore
+            for m in embeddings_strategy["metadatas"]
+        ]
 
     # Can't pickle a function, and we won't need them
     collection_strategy.embedding_function = None
     collection_strategy.known_metadata_keys = {}
 
     # Run the task in a separate process to avoid polluting the current process
     # with the old version. Using spawn instead of fork to avoid sharing the
@@ -258,17 +231,22 @@
 
     if conn1.poll():
         e = conn1.recv()
         raise e
 
     # Switch to the current version (local working directory) and check the invariants
     # are preserved for the collection
-    api = Client(settings)
+    system = config.System(settings)
+    api = system.instance(API)
+    system.start()
     coll = api.get_collection(
         name=collection_strategy.name,
         embedding_function=not_implemented_ef(),
     )
     invariants.count(coll, embeddings_strategy)
     invariants.metadatas_match(coll, embeddings_strategy)
     invariants.documents_match(coll, embeddings_strategy)
     invariants.ids_match(coll, embeddings_strategy)
     invariants.ann_accuracy(coll, embeddings_strategy)
+
+    # Shutdown system
+    system.stop()
```

### Comparing `chromadb-0.4.2/chromadb/test/property/test_embeddings.py` & `chromadb-0.4.3/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/property/test_filtering.py` & `chromadb-0.4.3/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/property/test_persist.py` & `chromadb-0.4.3/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/segment/test_metadata.py` & `chromadb-0.4.3/chromadb/test/segment/test_metadata.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/segment/test_vector.py` & `chromadb-0.4.3/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/test_api.py` & `chromadb-0.4.3/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/test_chroma.py` & `chromadb-0.4.3/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/test_client.py` & `chromadb-0.4.3/chromadb/test/test_client.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/test_config.py` & `chromadb-0.4.3/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/test_multithreaded.py` & `chromadb-0.4.3/chromadb/test/test_multithreaded.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/test/utils/test_messagid.py` & `chromadb-0.4.3/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/types.py` & `chromadb-0.4.3/chromadb/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/utils/distance_functions.py` & `chromadb-0.4.3/chromadb/utils/distance_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/utils/embedding_functions.py` & `chromadb-0.4.3/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/utils/messageid.py` & `chromadb-0.4.3/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb/utils/read_write_lock.py` & `chromadb-0.4.3/chromadb/utils/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/chromadb.egg-info/PKG-INFO` & `chromadb-0.4.3/chromadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.4.2
+Version: 0.4.3
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb Version: 0.4.2 Summary: Chroma. Author-
+Metadata-Version: 2.1 Name: chromadb Version: 0.4.3 Summary: Chroma. Author-
 email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-0.4.2/chromadb.egg-info/SOURCES.txt` & `chromadb-0.4.3/chromadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/DEVELOP.md` & `chromadb-0.4.3/clients/js/DEVELOP.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 `yarn test` will launch a test docker backend.
 `yarn test:run` will run against the docker backend you have running. But CAUTION, it will delete data.
 
 ### Pushing to npm
 
 The goal of the design is that this will be added to our github action releases so that the JS API is always up to date and pinned against the python backend API.
 
-`yarn release` pushes the `package.json` defined packaged to the package manager for authenticated users. It will build, test, and then publish the new version.
+`npm run release` pushes the `package.json` defined packaged to the package manager for authenticated users. It will build, test, and then publish the new version.
 
 ### Useful links
 
 https://gaganpreet.in/posts/hyperproductive-apis-fastapi/
```

### Comparing `chromadb-0.4.2/clients/js/LICENSE` & `chromadb-0.4.3/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/README.md` & `chromadb-0.4.3/clients/js/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,27 @@
 
 Chroma needs to be running in order for this client to talk to it. Please see the [🧪 Usage Guide](https://docs.trychroma.com/usage-guide) to learn how to quickly stand this up.
 
 ## Small example
 
 ```js
 import { ChromaClient } from "chromadb";
-const chroma = new ChromaClient("http://localhost:8000");
-const collection = await chroma.createCollection("test-from-js");
+const chroma = new ChromaClient({ path: "http://localhost:8000" });
+const collection = await chroma.createCollection({ name: "test-from-js" });
 for (let i = 0; i < 20; i++) {
-  await collection.add("test-id-" + i.toString(), [1, 2, 3, 4, 5], {
-    test: "test",
+  await collection.add({
+    ids: ["test-id-" + i.toString()],
+    embeddings, [1, 2, 3, 4, 5],
+    documents: ["test"],
   });
 }
-const queryData = await collection.query([1, 2, 3, 4, 5], 5, { test: "test" });
+const queryData = await collection.query({
+  queryEmbeddings: [1, 2, 3, 4, 5],
+  queryTexts: ["test"],
+});
 ```
 
 ## Local development
 
 [View the Development Readme](./DEVELOP.md)
 
 ## License
```

### Comparing `chromadb-0.4.2/clients/js/examples/browser/app.ts` & `chromadb-0.4.3/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/examples/browser/index.html` & `chromadb-0.4.3/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/examples/browser/yarn.lock` & `chromadb-0.4.3/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/examples/node/app.js` & `chromadb-0.4.3/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/examples/node/yarn.lock` & `chromadb-0.4.3/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/genapi.sh` & `chromadb-0.4.3/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/package-lock.json` & `chromadb-0.4.3/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/package.json` & `chromadb-0.4.3/clients/js/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'1.5.5'"}*

```diff
@@ -38,9 +38,9 @@
         "release": "run-s build test:run && npm publish",
         "test": "run-s db:clean db:run test:runfull db:clean",
         "test:run": "jest --runInBand",
         "test:runfull": "PORT=8001 jest --runInBand",
         "test:set-port": "cross-env URL=localhost:8001",
         "test:update": "run-s db:clean db:run && jest --runInBand --updateSnapshot && run-s db:clean"
     },
-    "version": "1.5.3"
+    "version": "1.5.5"
 }
```

### Comparing `chromadb-0.4.2/clients/js/src/ChromaClient.ts` & `chromadb-0.4.3/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/Collection.ts` & `chromadb-0.4.3/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-0.4.3/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-0.4.3/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `chromadb-0.4.3/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `chromadb-0.4.3/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/generated/README.md` & `chromadb-0.4.3/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/generated/api.ts` & `chromadb-0.4.3/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/generated/configuration.ts` & `chromadb-0.4.3/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/generated/models.ts` & `chromadb-0.4.3/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/generated/runtime.ts` & `chromadb-0.4.3/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/types.ts` & `chromadb-0.4.3/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/src/utils.ts` & `chromadb-0.4.3/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/add.collections.test.ts` & `chromadb-0.4.3/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/client.test.ts` & `chromadb-0.4.3/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/collection.client.test.ts` & `chromadb-0.4.3/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/collection.test.ts` & `chromadb-0.4.3/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/delete.collection.test.ts` & `chromadb-0.4.3/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/get.collection.test.ts` & `chromadb-0.4.3/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/peek.collection.test.ts` & `chromadb-0.4.3/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/query.collection.test.ts` & `chromadb-0.4.3/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/update.collection.test.ts` & `chromadb-0.4.3/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/test/upsert.collections.test.ts` & `chromadb-0.4.3/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/js/yarn.lock` & `chromadb-0.4.3/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/python/README.md` & `chromadb-0.4.3/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/python/build_python_thin_client.sh` & `chromadb-0.4.3/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/python/integration-test.sh` & `chromadb-0.4.3/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/clients/python/pyproject.toml` & `chromadb-0.4.3/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/docker-compose.test.yml` & `chromadb-0.4.3/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/README.md` & `chromadb-0.4.3/examples/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/basic_functionality/alternative_embeddings.ipynb` & `chromadb-0.4.3/examples/basic_functionality/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/basic_functionality/local_persistence.ipynb` & `chromadb-0.4.3/examples/basic_functionality/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/basic_functionality/where_filtering.ipynb` & `chromadb-0.4.3/examples/basic_functionality/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/deployments/google-cloud-compute/README.md` & `chromadb-0.4.3/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/deployments/google-cloud-compute/chroma.tf` & `chromadb-0.4.3/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-0.4.3/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/use_with/cohere/cohere_js.js` & `chromadb-0.4.3/examples/use_with/cohere/cohere_js.js`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/examples/use_with/cohere/cohere_python.ipynb` & `chromadb-0.4.3/examples/use_with/cohere/cohere_python.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.2/pyproject.toml` & `chromadb-0.4.3/pyproject.toml`

 * *Files identical despite different names*

