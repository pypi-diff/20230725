# Comparing `tmp/cognite_neat-0.17.4.tar.gz` & `tmp/cognite_neat-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.17.4.tar", max compression
+gzip compressed data, was "cognite_neat-0.18.0.tar", max compression
```

## Comparing `cognite_neat-0.17.4.tar` & `cognite_neat-0.18.0.tar`

### file list

```diff
@@ -1,123 +1,124 @@
--rw-r--r--   0        0        0    11351 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/LICENSE
--rw-r--r--   0        0        0     8765 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/README.md
--rw-r--r--   0        0        0       61 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/_version.py
--rw-r--r--   0        0        0     9986 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/base_workflows/graph2assets_relationships.py
--rw-r--r--   0        0        0     7037 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/base_workflows/graphs_and_rules.py
--rw-r--r--   0        0        0    14391 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/base_workflows/sheet2cdf.py
--rw-r--r--   0        0        0    11824 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/base_workflows/sme_graph_capture.py
--rw-r--r--   0        0        0      871 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2792 2023-07-25 09:07:50.471196 cognite_neat-0.17.4/cognite/neat/core/app.py
--rw-r--r--   0        0        0     5616 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0     1276 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/exceptions.py
--rw-r--r--   0        0        0      586 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2837 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/labels.py
--rw-r--r--   0        0        0     5048 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/models.py
--rw-r--r--   0        0        0    39905 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py
--rw-r--r--   0        0        0    20940 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py
--rw-r--r--   0        0        0     5514 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0       99 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    11407 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12903 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0       73 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9594 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0     2026 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/__init__.py
--rw-r--r--   0        0        0    49672 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/_exceptions.py
--rw-r--r--   0        0        0     3060 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/_loader.py
--rw-r--r--   0        0        0     7054 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/_parser.py
--rw-r--r--   0        0        0     3506 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/_validation.py
--rw-r--r--   0        0        0     4782 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/analysis.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/__init__.py
--rw-r--r--   0        0        0       63 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/cdf/__init__.py
--rw-r--r--   0        0        0       48 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/cdf/rules2dms.py
--rw-r--r--   0        0        0      615 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/cdf/rules2labels.py
--rw-r--r--   0        0        0     5418 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2graph_sheet.py
--rw-r--r--   0        0        0     4788 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2graphql.py
--rw-r--r--   0        0        0    15668 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2ontology.py
--rw-r--r--   0        0        0     4029 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2rules.py
--rw-r--r--   0        0        0      636 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2triples.py
--rw-r--r--   0        0        0       63 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/importer/__init__.py
--rw-r--r--   0        0        0    12985 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/importer/ontology2excel.py
--rw-r--r--   0        0        0    24217 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/models.py
--rw-r--r--   0        0        0     8231 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/rules/to_rdf_path.py
--rw-r--r--   0        0        0    11890 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/utils/__init__.py
--rw-r--r--   0        0        0      314 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/utils/auxiliary.py
--rw-r--r--   0        0        0      741 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/utils/cdf.py
--rw-r--r--   0        0        0    10694 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/utils/utils.py
--rw-r--r--   0        0        0     2650 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      356 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    23380 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17845 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0    11664 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4907 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0     1008 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/step_model.py
--rw-r--r--   0        0        0      775 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6977 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      661 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/examples/__init__.py
--rw-r--r--   0        0        0      286 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    68445 2023-07-25 09:07:50.475196 cognite_neat-0.17.4/cognite/neat/examples/graph-sheets/power-grid-example.xlsx
--rw-r--r--   0        0        0    94607 2023-07-25 09:07:50.479196 cognite_neat-0.17.4/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    14930 2023-07-25 09:08:48.439725 cognite_neat-0.17.4/cognite/neat/examples/ontologies/report.txt
--rw-r--r--   0        0        0    12820 2023-07-25 09:08:48.355724 cognite_neat-0.17.4/cognite/neat/examples/ontologies/transformation_rules.xlsx
--rw-r--r--   0        0        0    64516 2023-07-25 09:07:50.479196 cognite_neat-0.17.4/cognite/neat/examples/ontologies/wind-energy.owl
--rw-r--r--   0        0        0    80218 2023-07-25 09:07:50.479196 cognite_neat-0.17.4/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77381 2023-07-25 09:07:50.479196 cognite_neat-0.17.4/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-07-25 09:07:50.479196 cognite_neat-0.17.4/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52650 2023-07-25 09:07:50.479196 cognite_neat-0.17.4/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79964 2023-07-25 09:07:50.479196 cognite_neat-0.17.4/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15698 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3549 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11456 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0      315 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8063 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0      270 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0      291 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1390 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    24068 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4622 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-07-25 09:07:50.483196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1370405 2023-07-25 09:07:50.491196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js
--rw-r--r--   0        0        0     2667 2023-07-25 09:07:50.491196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt
--rw-r--r--   0        0        0  5883860 2023-07-25 09:07:50.519196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.map
--rw-r--r--   0        0        0     2633 2023-07-25 09:07:50.519196 cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0      655 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/steps/data_contracts.py
--rw-r--r--   0        0        0     1992 2023-07-25 09:07:50.523196 cognite_neat-0.17.4/cognite/neat/steps/steps.py
--rw-r--r--   0        0        0     2711 2023-07-25 09:07:50.923200 cognite_neat-0.17.4/pyproject.toml
--rw-r--r--   0        0        0    10637 1970-01-01 00:00:00.000000 cognite_neat-0.17.4/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/LICENSE
+-rw-r--r--   0        0        0     8765 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/README.md
+-rw-r--r--   0        0        0       61 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0     2805 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/app.py
+-rw-r--r--   0        0        0     5611 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1390 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0    24132 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0     4622 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/main.py
+-rw-r--r--   0        0        0       16 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-07-25 10:06:52.432219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1370405 2023-07-25 10:06:52.440219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js
+-rw-r--r--   0        0        0     2667 2023-07-25 10:06:52.440219 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt
+-rw-r--r--   0        0        0  5883860 2023-07-25 10:06:52.472220 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map
+-rw-r--r--   0        0        0     2633 2023-07-25 10:06:52.472220 cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      884 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/constants.py
+-rw-r--r--   0        0        0     1276 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      711 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/config.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0     1213 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/graph.py
+-rw-r--r--   0        0        0      938 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    11427 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/graph_store.py
+-rw-r--r--   0        0        0       68 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/mocks/__init__.py
+-rw-r--r--   0        0        0    12883 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/extractors/mocks/graph.py
+-rw-r--r--   0        0        0      510 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/loaders/__init__.py
+-rw-r--r--   0        0        0     2837 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/__init__.py
+-rw-r--r--   0        0        0     2278 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/labels.py
+-rw-r--r--   0        0        0     5043 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/models.py
+-rw-r--r--   0        0        0    39901 2023-07-25 10:06:52.476220 cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/rdf_to_assets.py
+-rw-r--r--   0        0        0    20931 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5504 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/graph/loaders/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2650 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/graph/loaders/validator.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/graph/transformations/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0     9592 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    11892 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/graph/transformations/transformer.py
+-rw-r--r--   0        0        0     2027 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0    49672 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/_exceptions.py
+-rw-r--r--   0        0        0     3050 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/_loader.py
+-rw-r--r--   0        0        0     7047 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/_parser.py
+-rw-r--r--   0        0        0     3496 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/_validation.py
+-rw-r--r--   0        0        0     4777 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/cdf/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/cdf/rules2dms.py
+-rw-r--r--   0        0        0      610 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/cdf/rules2labels.py
+-rw-r--r--   0        0        0     5403 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2graph_sheet.py
+-rw-r--r--   0        0        0     4763 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2graphql.py
+-rw-r--r--   0        0        0    15643 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2ontology.py
+-rw-r--r--   0        0        0     4019 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2rules.py
+-rw-r--r--   0        0        0      631 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2triples.py
+-rw-r--r--   0        0        0       63 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0    13005 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/importer/ontology2excel.py
+-rw-r--r--   0        0        0    24210 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/models.py
+-rw-r--r--   0        0        0     8231 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/rules/to_rdf_path.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      741 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0    10682 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0    10004 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/graph2assets_relationships.py
+-rw-r--r--   0        0        0     7092 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/graphs_and_rules.py
+-rw-r--r--   0        0        0    14425 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/sheet2cdf.py
+-rw-r--r--   0        0        0    11809 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/sme_graph_capture.py
+-rw-r--r--   0        0        0      661 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/examples/__init__.py
+-rw-r--r--   0        0        0      286 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    68445 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/examples/graph-sheets/power-grid-example.xlsx
+-rw-r--r--   0        0        0    94607 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    14930 2023-07-25 10:07:44.837204 cognite_neat-0.18.0/cognite/neat/workflows/examples/ontologies/report.txt
+-rw-r--r--   0        0        0    12816 2023-07-25 10:07:44.585200 cognite_neat-0.18.0/cognite/neat/workflows/examples/ontologies/transformation_rules.xlsx
+-rw-r--r--   0        0        0    64516 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/examples/ontologies/wind-energy.owl
+-rw-r--r--   0        0        0    80218 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77381 2023-07-25 10:06:52.480220 cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-07-25 10:06:52.484220 cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52650 2023-07-25 10:06:52.484220 cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79964 2023-07-25 10:06:52.484220 cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1460 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15753 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3527 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11444 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0      325 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8063 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0      280 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0      301 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0      660 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0     1994 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/steps/steps.py
+-rw-r--r--   0        0        0      361 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/__init__.py
+-rw-r--r--   0        0        0    23404 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/base.py
+-rw-r--r--   0        0        0    17855 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/cdf_store.py
+-rw-r--r--   0        0        0    11684 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/manager.py
+-rw-r--r--   0        0        0     4907 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/model.py
+-rw-r--r--   0        0        0     1008 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/step_model.py
+-rw-r--r--   0        0        0      780 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/tasks.py
+-rw-r--r--   0        0        0     6987 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-07-25 10:06:52.488220 cognite_neat-0.18.0/cognite/neat/workflows/workflow/utils.py
+-rw-r--r--   0        0        0     2695 2023-07-25 10:06:52.912227 cognite_neat-0.18.0/pyproject.toml
+-rw-r--r--   0        0        0    10637 1970-01-01 00:00:00.000000 cognite_neat-0.18.0/PKG-INFO
```

### Comparing `cognite_neat-0.17.4/LICENSE` & `cognite_neat-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/README.md` & `cognite_neat-0.18.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -171,20 +171,21 @@
 
  Must implement `BaseWorkflow` class from `from cognite.neat.core.workflow.base`
 
  Each method that should be orchestrated by workflow engine must be prefixed with `step_` , each method must have single argument of `FlowMessage` type and return `FlowMessage` or `None`.
  FlowMessage is passed from one step to another and it's captured in execution log.
 
 Simplest `workflow.py`
+
 ````python
 
 import logging
 from cognite.client import CogniteClient
-from cognite.neat.core.workflow.base import BaseWorkflow
-from cognite.neat.core.workflow.model import FlowMessage
+from cognite.neat.workflows.workflow import BaseWorkflow
+from cognite.neat.workflows.workflow import FlowMessage
 
 
 class PlaygroundNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
 
     def step_run_experiment_1(self, flow_msg: FlowMessage = None):
```

### Comparing `cognite_neat-0.17.4/cognite/neat/base_workflows/graph2assets_relationships.py` & `cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/graph2assets_relationships.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import logging
 import time
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
-from cognite.neat.base_workflows.graphs_and_rules import GraphsAndRulesBaseWorkflow
-from cognite.neat.core.extractors.cdfcore.labels import upload_labels
-from cognite.neat.core.extractors.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
-from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
+from cognite.neat.workflows.base_workflows.graphs_and_rules import GraphsAndRulesBaseWorkflow
+from cognite.neat.graph.loaders.cdfcore.labels import upload_labels
+from cognite.neat.graph.loaders.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
+from cognite.neat.graph.loaders.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
-from cognite.neat.core.validator import validate_asset_hierarchy
-from cognite.neat.core.workflow.model import FlowMessage
+from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
+from cognite.neat.workflows.workflow.model import FlowMessage
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_graph_to_asset_hierarchy_wf_cdf_resource_stats",
         "CDF resource stats before and after running fast_graph workflow",
         ["resource_type", "state"],
     )
```

### Comparing `cognite_neat-0.17.4/cognite/neat/base_workflows/graphs_and_rules.py` & `cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/graphs_and_rules.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
-from cognite.neat.core import loader, rules
-from cognite.neat.core.configuration import PREFIXES
-from cognite.neat.core.loader.graph_store import NeatGraphStore, drop_graph_store
-from cognite.neat.core.rules.exporter.rules2triples import get_instances_as_triples
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.transformer import RuleProcessingReport, domain2app_knowledge_graph
-from cognite.neat.core.workflow import utils
-from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.core.workflow.cdf_store import CdfStore
+from cognite.neat import rules
+from cognite.neat.graph import extractors
+from cognite.neat.app.api.configuration import PREFIXES
+from cognite.neat.graph.extractors import NeatGraphStore, drop_graph_store
+from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.graph.transformations.transformer import RuleProcessingReport, domain2app_knowledge_graph
+from cognite.neat.workflows.workflow import utils
+from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.workflow.cdf_store import CdfStore
 
 
 class GraphsAndRulesBaseWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.dataset_id: int = 0
         self.source_graph: NeatGraphStore = None
@@ -58,29 +59,29 @@
         solution_store_dir = Path(self.data_store_path) / Path(solution_store_dir) if solution_store_dir else None
         logging.info(f"source_store_dir={source_store_dir}")
         logging.info(f"solution_store_dir={solution_store_dir}")
         if clean_start:
             drop_graph_store(self.source_graph, source_store_dir, force=True)
             drop_graph_store(self.solution_graph, solution_store_dir, force=True)
 
-        self.source_graph = loader.NeatGraphStore(
+        self.source_graph = extractors.NeatGraphStore(
             prefixes=self.transformation_rules.prefixes, base_prefix="neat", namespace=PREFIXES["neat"]
         )
 
         if self.get_config_item_value("source_rdf_store.type"):
             self.source_graph.init_graph(
                 self.get_config_item_value("source_rdf_store.type", self.graph_source_type),
                 self.get_config_item_value("source_rdf_store.query_url"),
                 self.get_config_item_value("source_rdf_store.update_url"),
                 "neat-tnt",
                 internal_storage_dir=source_store_dir,
             )
 
         if self.get_config_item_value("solution_rdf_store.type"):
-            self.solution_graph = loader.NeatGraphStore(
+            self.solution_graph = extractors.NeatGraphStore(
                 prefixes=self.transformation_rules.prefixes, base_prefix="neat", namespace=PREFIXES["neat"]
             )
 
             self.solution_graph.init_graph(
                 self.get_config_item_value("solution_rdf_store.type"),
                 self.get_config_item_value("solution_rdf_store.query_url"),
                 self.get_config_item_value("solution_rdf_store.update_url"),
```

### Comparing `cognite_neat-0.17.4/cognite/neat/base_workflows/sheet2cdf.py` & `cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/sheet2cdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
-from cognite.neat.core import loader, rules
-from cognite.neat.core.extractors.cdfcore.labels import upload_labels
-from cognite.neat.core.extractors.cdfcore.rdf_to_assets import (
+from cognite.neat import rules
+from cognite.neat.graph import extractors
+from cognite.neat.graph.loaders.cdfcore.labels import upload_labels
+from cognite.neat.graph.loaders.cdfcore.rdf_to_assets import (
     NeatMetadataKeys,
     categorize_assets,
     rdf2assets,
     remove_non_existing_labels,
     unique_asset_labels,
     upload_assets,
 )
-from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
+from cognite.neat.graph.loaders.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
-from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.rules.exporter.rules2triples import get_instances_as_triples
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.validator import validate_asset_hierarchy
-from cognite.neat.core.workflow import utils
-from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.core.workflow.cdf_store import CdfStore
+from cognite.neat.graph.extractors import NeatGraphStore
+from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
+from cognite.neat.workflows.workflow import utils
+from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.workflow.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_sheet2cdf_cdf_resource_stats",
         "CDF resource stats before and after running sheet2cdf workflow",
         ["resource_type", "state"],
     )
@@ -80,15 +81,15 @@
         logging.info(output_text)
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
 
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         return FlowMessage(output_text=output_text)
 
     def step_configuring_stores(self, flow_msg: FlowMessage = None, clean_start: bool = True):
-        self.source_graph = loader.NeatGraphStore(
+        self.source_graph = extractors.NeatGraphStore(
             prefixes=self.transformation_rules.prefixes, namespace=self.transformation_rules.metadata.namespace
         )
         self.source_graph.init_graph(base_prefix=self.transformation_rules.metadata.prefix)
 
         # this is fix to be able to display the graph in the UI
         # alex is working on a better solution
         self.solution_graph = self.source_graph
```

### Comparing `cognite_neat-0.17.4/cognite/neat/base_workflows/sme_graph_capture.py` & `cognite_neat-0.18.0/cognite/neat/workflows/base_workflows/sme_graph_capture.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import logging
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 
-from cognite.neat.core import extractors, loader, rules
-from cognite.neat.core.extractors.cdfcore.labels import upload_labels
-from cognite.neat.core.extractors.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
-from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
+from cognite.neat import rules
+from cognite.neat.graph import loaders, extractors
+from cognite.neat.graph.loaders.cdfcore.labels import upload_labels
+from cognite.neat.graph.loaders.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
+from cognite.neat.graph.loaders.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
-from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.utils.utils import add_triples
-from cognite.neat.core.validator import validate_asset_hierarchy
-from cognite.neat.core.workflow import utils
-from cognite.neat.core.workflow.base import BaseWorkflow
-from cognite.neat.core.workflow.cdf_store import CdfStore
-from cognite.neat.core.workflow.model import FlowMessage
+from cognite.neat.graph.extractors import NeatGraphStore
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.utils.utils import add_triples
+from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
+from cognite.neat.workflows.workflow import utils
+from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.workflow.cdf_store import CdfStore
 
 
 class SmeGraphCaptureBaseWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
         self.metrics.register_metric("counter_1", "", "counter", ["step"])
@@ -68,26 +68,26 @@
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_configure_graph_store(self, flow_msg: FlowMessage = None):
         logging.info("Configure graph store")
-        self.solution_graph = loader.NeatGraphStore(prefixes=self.transformation_rules.prefixes)
+        self.solution_graph = extractors.NeatGraphStore(prefixes=self.transformation_rules.prefixes)
         self.solution_graph.init_graph("memory")
         return FlowMessage(output_text="Graph store configured")
 
     def step_generate_graph_capture_sheet(self, flow_msg: FlowMessage = None):
         logging.info("Generate graph capture sheet")
         sheet_name = self.get_config_item_value("graph_capture.file", "graph_capture_sheet.xlsx")
         auto_identifier_type = self.get_config_item_value("graph_capture_sheet.auto_identifier_type", None)
         logging.info(f"Auto identifier type {auto_identifier_type}")
         data_capture_sheet_path = self.rules_storage_path.parent / "graph-sheets" / sheet_name
 
-        extractors.rules2graph_capturing_sheet(
+        loaders.rules2graph_capturing_sheet(
             self.transformation_rules, data_capture_sheet_path, auto_identifier_type=auto_identifier_type
         )
 
         output_text = (
             "Data capture sheet generated and can be downloaded here : "
             f'<a href="http://localhost:8000/data/graph-sheets/{sheet_name}?{time.time()}" target="_blank">'
             f"{sheet_name}</a>"
@@ -99,16 +99,16 @@
     # ------------------ Graph Capturing Sheet Processing ------------------------------
     # ----------------------------------------------------------------------------------
 
     def step_process_graph_capture_sheet(self, flow_msg: FlowMessage = None):
         data_capture_sheet_path = Path(self.upload_meta_object["full_path"])
         logging.info(f"Processing data capture sheet {data_capture_sheet_path}")
 
-        raw_sheets = loader.graph_capturing_sheet.excel_file_to_table_by_name(data_capture_sheet_path)
-        triples = extractors.sheet2triples(raw_sheets, self.transformation_rules)
+        raw_sheets = extractors.graph_capturing_sheet.excel_file_to_table_by_name(data_capture_sheet_path)
+        triples = loaders.sheet2triples(raw_sheets, self.transformation_rules)
         add_triples(self.solution_graph, triples)
         return FlowMessage(output_text="Data capture sheet processed")
 
     def step_create_cdf_labels(self, flow_msg: FlowMessage = None):
         logging.info("Creating CDF labels")
         upload_labels(self.cdf_client, self.transformation_rules, extra_labels=["non-historic", "historic"])
```

### Comparing `cognite_neat-0.17.4/cognite/neat/constants.py` & `cognite_neat-0.18.0/cognite/neat/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 
 from cognite import neat
 
 PACKAGE_DIRECTORY = Path(neat.__file__).parent
-EXAMPLES_DIRECTORY = PACKAGE_DIRECTORY / "examples"
+EXAMPLES_DIRECTORY = PACKAGE_DIRECTORY / "workflows" / "examples"
 EXAMPLE_RULES = EXAMPLES_DIRECTORY / "rules"
 EXAMPLE_SOURCE_GRAPHS = EXAMPLES_DIRECTORY / "source-graphs"
 EXAMPLE_WORKFLOWS = EXAMPLES_DIRECTORY / "workflows"
 EXAMPLE_GRAPH_CAPTURING = EXAMPLES_DIRECTORY / "graph-sheets"
 EXAMPLE_ONTOLOGIES = EXAMPLES_DIRECTORY / "ontologies"
 
 TNT_TRANSFORMATION_RULES = EXAMPLE_RULES / "Rules-Nordic44-to-TNT.xlsx"
 SIMPLE_TRANSFORMATION_RULES = EXAMPLE_RULES / "sheet2cdf-transformation-rules.xlsx"
 NORDIC44_KNOWLEDGE_GRAPH = EXAMPLE_SOURCE_GRAPHS / "Knowledge-Graph-Nordic44.xml"
 GRAPH_CAPTURING_SHEET = EXAMPLE_GRAPH_CAPTURING / "sheet2cdf-graph-capturing.xlsx"
 WIND_ONTOLOGY = EXAMPLE_ONTOLOGIES / "wind-energy.owl"
-UI_PATH = PACKAGE_DIRECTORY / "explorer-ui" / "neat-app" / "build"
+UI_PATH = PACKAGE_DIRECTORY / "app" / "ui" / "neat-app" / "build"
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/app.py` & `cognite_neat-0.18.0/cognite/neat/app/api/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
 from cognite.client import CogniteClient
 from fastapi import FastAPI
 
-from cognite.neat.core.configuration import Config
-from cognite.neat.core.utils.utils import get_cognite_client_from_config
-from cognite.neat.core.workflow.cdf_store import CdfStore
-from cognite.neat.core.workflow.manager import WorkflowManager
-from cognite.neat.core.workflow.triggers import TriggerManager
+from cognite.neat.app.api.configuration import Config
+from cognite.neat.utils.utils import get_cognite_client_from_config
+from cognite.neat.workflows.workflow.cdf_store import CdfStore
+from cognite.neat.workflows.workflow.manager import WorkflowManager
+from cognite.neat.workflows.workflow.triggers import TriggerManager
 
 
 class NeatApp:
     def __init__(self, config: Config, cdf_client: CogniteClient = None):
         self.config = config
         self.cdf_client: CogniteClient = None
         self.cdf_store: CdfStore = None
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/configuration.py` & `cognite_neat-0.18.0/cognite/neat/app/api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Literal, Optional, Self
 
 import yaml
 from pydantic import BaseModel, Field
 from rdflib import Namespace
 from yaml import safe_load
 
-from cognite.neat.core.utils.cdf import InteractiveCogniteClient, ServiceCogniteClient
+from cognite.neat.utils.cdf import InteractiveCogniteClient, ServiceCogniteClient
 
 PREFIXES = {
     # "rdf": Namespace("http://www.w3.org/1999/02/22-rdf-syntax-ns#"), # noqa
     # "rdfs": Namespace("http://www.w3.org/2000/01/rdf-schema#"),# noqa
     # "owl": Namespace("http://www.w3.org/2002/07/owl#"),# noqa
     # "sh": Namespace("http://www.w3.org/ns/shacl#"),
     "dct": Namespace("http://purl.org/dc/terms/"),
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.18.0/cognite/neat/graph/extractors/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.18.0/cognite/neat/graph/extractors/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/exceptions.py` & `cognite_neat-0.18.0/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/extractors/_exceptions.py` & `cognite_neat-0.18.0/cognite/neat/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/labels.py` & `cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import traceback
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelDefinition
 
-from cognite.neat.core.rules.exporter.cdf import get_labels
-from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.rules.exporter.cdf import get_labels
+from cognite.neat.rules.models import TransformationRules
 
 
 def upload_labels(
     client: CogniteClient,
     transformation_rules: TransformationRules,
     extra_labels: list = None,
     stop_on_exception: bool = False,
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/models.py` & `cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from typing import ClassVar, List, Optional
 
 from pydantic import BaseModel, ConfigDict, root_validator, validator
 from rdflib import Namespace
 
-from cognite.neat.core.rules.models import METADATA_VALUE_MAX_LENGTH
+from cognite.neat.rules.models import METADATA_VALUE_MAX_LENGTH
 
 
 class AssetClassMapping(BaseModel):
     external_id: str
     name: str
     parent_external_id: Optional[str] = None
     description: Optional[str] = None
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py` & `cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/rdf_to_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetHierarchy, AssetList
 from cognite.client.exceptions import CogniteDuplicatedError
 from deepdiff import DeepDiff
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
-from cognite.neat.core.configuration import EXCLUDE_PATHS
-from cognite.neat.core.extractors.cdfcore.models import AssetTemplate
-from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.rules.models import Property, TransformationRules
-from cognite.neat.core.utils.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
+from cognite.neat.app.api.configuration import EXCLUDE_PATHS
+from cognite.neat.graph.loaders.cdfcore.models import AssetTemplate
+from cognite.neat.graph.extractors.graph_store import NeatGraphStore
+from cognite.neat.rules.models import Property, TransformationRules
+from cognite.neat.utils.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
 
 
 @dataclass
 class NeatMetadataKeys:
     start_time: str = "start_time"
     end_time: str = "end_time"
     update_time: str = "update_time"
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py` & `cognite_neat-0.18.0/cognite/neat/graph/loaders/cdfcore/rdf_to_relationships.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from warnings import warn
 
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelFilter, Relationship, RelationshipUpdate
 from cognite.client.exceptions import CogniteDuplicatedError
 
-from cognite.neat.core.extractors.cdfcore.models import RelationshipDefinition, RelationshipDefinitions
-from cognite.neat.core.extractors.cdfcore.rdf_to_assets import _categorize_cdf_assets
-from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.utils.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace, retry_decorator
+from cognite.neat.graph.loaders.cdfcore.models import RelationshipDefinition, RelationshipDefinitions
+from cognite.neat.graph.loaders.cdfcore.rdf_to_assets import _categorize_cdf_assets
+from cognite.neat.graph.extractors.graph_store import NeatGraphStore
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.utils.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace, retry_decorator
 
 
 def define_relationships(rules: TransformationRules, stop_on_exception: bool = False) -> RelationshipDefinitions:
     relationships = {}
 
     # Unique ids used to check for redefinitions of relationships
     ids = set()
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.18.0/cognite/neat/graph/loaders/graph_sheet_to_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import warnings
 
 import pandas as pd
 from rdflib import RDF, XSD, Literal, Namespace
 
-from cognite.neat.core.rules.analysis import to_class_property_pairs, get_defined_classes
-from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.rules.analysis import to_class_property_pairs, get_defined_classes
+from cognite.neat.rules.models import TransformationRules
 
 
 def sheet2triples(
     graph_capturing_sheet: dict[str, pd.DataFrame],
     transformation_rule: TransformationRules,
     separator: str = ",",
     namespace: str = None,
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/loader/config.py` & `cognite_neat-0.18.0/cognite/neat/graph/extractors/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/loader/graph.py` & `cognite_neat-0.18.0/cognite/neat/graph/extractors/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from rdflib import Graph, Namespace
 
-from cognite.neat.core.configuration import DEFAULT_NAMESPACE, DEFAULT_URI, PREFIXES
+from cognite.neat.app.api.configuration import DEFAULT_NAMESPACE, DEFAULT_URI, PREFIXES
 
 __all__ = ["rdf_file_to_graph"]
 
 
 def rdf_file_to_graph(
     filepath: Path,
     base_prefix: str = DEFAULT_URI,
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.18.0/cognite/neat/graph/extractors/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.18.0/cognite/neat/graph/extractors/graph_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import pyoxigraph
 import requests
 from prometheus_client import Gauge, Summary
 from rdflib import Graph, Namespace
 from rdflib.plugins.stores.sparqlstore import SPARQLUpdateStore
 from rdflib.query import Result
 
-from cognite.neat.core.configuration import DEFAULT_NAMESPACE, PREFIXES, RdfStoreType
-from cognite.neat.core.data_stores import oxrdflib
-from cognite.neat.core.loader.graph import rdf_file_to_graph
+from cognite.neat.app.api.configuration import DEFAULT_NAMESPACE, PREFIXES, RdfStoreType
+from cognite.neat.graph.extractors.data_stores import oxrdflib
+from cognite.neat.graph.extractors.graph import rdf_file_to_graph
 
 prom_qsm = Summary("store_query_time_summary", "Time spent processing queries", ["query"])
 prom_sq = Gauge("store_single_query_time", "Time spent processing a single query", ["query"])
 
 
 class NeatGraphStore:
     """NeatGraphStore is a class that stores the graph and provides methods to read/write data it contains
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.18.0/cognite/neat/graph/extractors/mocks/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import warnings
 from collections import OrderedDict
 
 import pandas as pd
 from prometheus_client import Gauge
 from rdflib import RDF, Literal, Namespace, URIRef
 
-from cognite.neat.core.rules.analysis import (
+from cognite.neat.rules.analysis import (
     get_class_linkage,
     get_classes_with_properties,
     get_defined_classes,
     get_symmetric_pairs,
 )
-from cognite.neat.core.rules.exporter.rules2rules import subset_rules
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.utils.utils import remove_namespace
+from cognite.neat.rules.exporter.rules2rules import subset_rules
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.utils.utils import remove_namespace
 
 neat_total_processed_mock_triples = Gauge(
     "neat_total_processed_mock_triples", "Number of processed mock triples", ["state"]
 )
 neat_mock_triples_processing_timing = Gauge(
     "neat_mock_triples_processing_timing", "Generation of mock knowledge graph timing metrics", ["aggregation"]
 )
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.18.0/cognite/neat/graph/transformations/query_generator/sparql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
-from cognite.neat.core.configuration import PREFIXES
-from cognite.neat.core.rules.to_rdf_path import (
+from cognite.neat.app.api.configuration import PREFIXES
+from cognite.neat.rules.to_rdf_path import (
     AllProperties,
     AllReferences,
     Hop,
     SingleProperty,
     Traversal,
     Triple,
     parse_traversal,
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/__init__.py` & `cognite_neat-0.18.0/cognite/neat/rules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from typing import Literal, overload
 
 from pydantic_core import ErrorDetails
 
 from . import _loader, _parser, models
 
+
 __all__ = [
     "models",
     "load_rules_from_excel_file",
     "load_rules_from_google_sheet",
     "load_rules_from_yaml",
 ]
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/_exceptions.py` & `cognite_neat-0.18.0/cognite/neat/rules/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/_loader.py` & `cognite_neat-0.18.0/cognite/neat/rules/_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from io import BytesIO
 from pathlib import Path
 from zipfile import BadZipFile
 from openpyxl import Workbook, load_workbook
 import pandas as pd
 import requests
 
-from cognite.neat.core.utils.auxiliary import local_import
-from cognite.neat.core.rules import _exceptions
+from cognite.neat.utils.auxiliary import local_import
+from cognite.neat.rules import _exceptions
 
 
 def google_to_table_by_name(sheet_id: str) -> dict[str, pd.DataFrame]:
     # To trigger ImportError if gspread is not installed
     local_import("gspread", "google")
     import gspread
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/_parser.py` & `cognite_neat-0.18.0/cognite/neat/rules/_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from warnings import warn
 
 import pandas as pd
 from pydantic import field_validator
 from pydantic_core import ErrorDetails, ValidationError
 from rdflib import Namespace
 
-from cognite.neat.core.configuration import PREFIXES
-from cognite.neat.core.rules import _exceptions
-from cognite.neat.core.rules.models import Class, Metadata, Property, RuleModel, TransformationRules
+from cognite.neat.app.api.configuration import PREFIXES
+from cognite.neat.rules import _exceptions
+from cognite.neat.rules.models import Class, Metadata, Property, RuleModel, TransformationRules
 
 
 def from_tables(
     raw_dfs: dict[str, pd.DataFrame], return_report: bool = False
 ) -> tuple[TransformationRules | None, list[ErrorDetails] | None, list | None] | TransformationRules:
     # the only way to suppress warnings from pylense
     validation_warnings = []
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/_validation.py` & `cognite_neat-0.18.0/cognite/neat/rules/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import warnings
 
-from cognite.neat.core.rules import _exceptions
-from cognite.neat.core.rules.models import TransformationRules, data_model_name_compliance_regex
+from cognite.neat.rules import _exceptions
+from cognite.neat.rules.models import TransformationRules, data_model_name_compliance_regex
 
 
 def are_entity_names_dms_compliant(
     transformation_rules: TransformationRules, return_report: bool = False
 ) -> bool | tuple[bool, list[dict]]:
     """Check if data model definitions are valid."""
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/analysis.py` & `cognite_neat-0.18.0/cognite/neat/rules/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 import warnings
 import pandas as pd
 
-from cognite.neat.core.rules.models import Property, TransformationRules
+from cognite.neat.rules.models import Property, TransformationRules
 
 
 def get_defined_classes(transformation_rules: TransformationRules) -> set[str]:
     """Returns classes that have been defined in the data model."""
     return {property.class_id for property in transformation_rules.properties.values()}
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/exporter/cdf/rules2labels.py` & `cognite_neat-0.18.0/cognite/neat/rules/exporter/cdf/rules2labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.rules.models import TransformationRules
 
 
 def get_labels(transformation_rules: TransformationRules) -> set[str]:
     """Return CDF labels for classes and relationships."""
     class_labels = {class_.class_id for class_ in transformation_rules.classes.values()}
 
     property_labels = {property_.property_id for property_ in transformation_rules.properties.values()}
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2graph_sheet.py` & `cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2graph_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from pathlib import Path
 
 from openpyxl import Workbook
 from openpyxl.styles import Alignment, Border, Font, NamedStyle, PatternFill, Side
 from openpyxl.utils.cell import get_column_letter
 from openpyxl.worksheet.datavalidation import DataValidation
 
-from cognite.neat.core.rules.analysis import to_class_property_pairs
-from cognite.neat.core.rules.exporter.rules2rules import to_dms_name
-from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.rules.analysis import to_class_property_pairs
+from cognite.neat.rules.exporter.rules2rules import to_dms_name
+from cognite.neat.rules.models import TransformationRules
 
 
 def rules2graph_capturing_sheet(
     transformation_rules: TransformationRules,
     file_path: Path,
     no_rows: int = 1000,
     auto_identifier_type: str = "index-based",
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2graphql.py` & `cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dataclasses import dataclass
 from typing import Self
-from cognite.neat.core.rules import _exceptions
-from cognite.neat.core.rules._validation import (
+from cognite.neat.rules import _exceptions
+from cognite.neat.rules._validation import (
     are_entity_names_dms_compliant,
     are_properties_redefined,
 )
-from cognite.neat.core.rules.analysis import to_class_property_pairs
-from cognite.neat.core.rules.models import DATA_TYPE_MAPPING, TransformationRules
-from cognite.neat.core.utils.utils import generate_exception_report
+from cognite.neat.rules.analysis import to_class_property_pairs
+from cognite.neat.rules.models import DATA_TYPE_MAPPING, TransformationRules
+from cognite.neat.utils.utils import generate_exception_report
 
 
 _TYPE = (
     "{% include 'type_header' %}type {{ class_definition.class_id }} {{'{'}}"
     "{%-for property_definition in class_properties%}"
     "{% include 'field' %}"
     "{% endfor %}\n}\n"
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2ontology.py` & `cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2ontology.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import ClassVar, Optional, Self
 import warnings
 from pydantic import BaseModel, ConfigDict, FieldValidationInfo, field_validator
 from rdflib import OWL, RDF, RDFS, XSD, DCTERMS, BNode, Graph, Literal, URIRef, Namespace
 from rdflib.collection import Collection as GraphCollection
 
-from cognite.neat.core.rules.models import DATA_TYPE_MAPPING, Class, Property, TransformationRules, Metadata
-from cognite.neat.core.rules.analysis import to_property_dict, to_class_property_pairs
-from cognite.neat.core.rules._validation import are_properties_redefined
-from cognite.neat.core.rules import _exceptions
-from cognite.neat.core.utils.utils import generate_exception_report, remove_namespace
+from cognite.neat.rules.models import DATA_TYPE_MAPPING, Class, Property, TransformationRules, Metadata
+from cognite.neat.rules.analysis import to_property_dict, to_class_property_pairs
+from cognite.neat.rules._validation import are_properties_redefined
+from cognite.neat.rules import _exceptions
+from cognite.neat.utils.utils import generate_exception_report, remove_namespace
 
 
 class OntologyModel(BaseModel):
     model_config: ClassVar[ConfigDict] = ConfigDict(arbitrary_types_allowed=True, strict=False, extra="allow")
 
 
 class Ontology(OntologyModel):
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2rules.py` & `cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 - subsetting the data model to only include desired classes and their properties
 - converting classes/properties ids/names to DMS compliant format
 """
 import logging
 import re
 import warnings
 
-from cognite.neat.core.rules.analysis import get_defined_classes
-from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.rules.analysis import get_defined_classes
+from cognite.neat.rules.models import TransformationRules
 
 
 def subset_rules(
     transformation_rules: TransformationRules, desired_classes: set, skip_validation: bool = False
 ) -> TransformationRules:
     """Subset transformation rules to only include desired classes and their properties.
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/exporter/rules2triples.py` & `cognite_neat-0.18.0/cognite/neat/rules/exporter/rules2triples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.rules.models import TransformationRules
 
 
 def get_instances_as_triples(transformation_rules: TransformationRules) -> list[tuple]:
     """Converts transformation rules instances sheet to RDF triples
 
     Parameters
     ----------
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/importer/ontology2excel.py` & `cognite_neat-0.18.0/cognite/neat/rules/importer/ontology2excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import warnings
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from rdflib import DC, DCTERMS, OWL, RDF, RDFS, Graph
 
-from cognite.neat.core.rules import _exceptions, load_rules_from_excel_file
-from cognite.neat.core.utils.utils import generate_exception_report, get_namespace, remove_namespace
+from cognite.neat.rules import load_rules_from_excel_file
+from cognite.neat.rules import _exceptions
+from cognite.neat.utils.utils import generate_exception_report, get_namespace, remove_namespace
 
 
 def _create_default_metadata_parsing_config() -> dict[str, tuple[str, ...]]:
     # TODO: these are to be read from Metadata pydantic model
     return {
         "header": (
             "namespace",
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/models.py` & `cognite_neat-0.18.0/cognite/neat/rules/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     model_validator,
     parse_obj_as,
     validator,
 )
 from pydantic.fields import FieldInfo
 from rdflib import XSD, Literal, Namespace, URIRef
 
-from cognite.neat.core.configuration import PREFIXES
+from cognite.neat.app.api.configuration import PREFIXES
 
 # from . import _exceptions
-from cognite.neat.core.rules import _exceptions
-from cognite.neat.core.rules.to_rdf_path import Entity, RuleType, parse_rule
+from cognite.neat.rules import _exceptions
+from cognite.neat.rules.to_rdf_path import Entity, RuleType, parse_rule
 
 __all__ = ["Class", "Instance", "Metadata", "Prefixes", "Property", "Resource", "TransformationRules"]
 
 # mapping of XSD types to Python and GraphQL types
 DATA_TYPE_MAPPING = {
     "boolean": {"python": "bool", "GraphQL": "Boolean"},
     "float": {"python": "float", "GraphQL": "Float"},
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/rules/to_rdf_path.py` & `cognite_neat-0.18.0/cognite/neat/rules/to_rdf_path.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/transformer.py` & `cognite_neat-0.18.0/cognite/neat/graph/transformations/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import pandas as pd
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 from pydantic import BaseModel
 from rdflib import RDF, Graph
 from rdflib.term import Literal
 
-from cognite.neat.core.query_generator.sparql import build_sparql_query
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.rules.to_rdf_path import AllProperties, AllReferences, RawLookup, parse_rule
-from cognite.neat.core.utils.utils import remove_namespace
+from cognite.neat.graph.transformations.query_generator.sparql import build_sparql_query
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.rules.to_rdf_path import AllProperties, AllReferences, RawLookup, parse_rule
+from cognite.neat.utils.utils import remove_namespace
 
 prom_total_proc_rules_g = Gauge("neat_total_processed_rules", "Number of processed rules", ["state"])
 rules_processing_timing_metric = Gauge(
     "neat_rules_processing_timing", "Transformation rules processing timing metrics", ["aggregation"]
 )
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/utils/cdf.py` & `cognite_neat-0.18.0/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/utils/utils.py` & `cognite_neat-0.18.0/cognite/neat/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import pandas as pd
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client.credentials import CredentialProvider, OAuthClientCredentials, OAuthInteractive
 from cognite.client.exceptions import CogniteDuplicatedError, CogniteReadTimeout
 from rdflib import Literal
 from rdflib.term import URIRef
 
-from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.utils.cdf import InteractiveCogniteClient, ServiceCogniteClient, CogniteClientConfig
+from cognite.neat.graph.extractors import NeatGraphStore
+from cognite.neat.utils.cdf import InteractiveCogniteClient, ServiceCogniteClient, CogniteClientConfig
 
 Triple: TypeAlias = tuple[URIRef, URIRef, Literal | URIRef]
 
 
 def get_cognite_client_from_config(config: ServiceCogniteClient) -> CogniteClient:
     credentials = OAuthClientCredentials(
         token_url=config.token_url, client_id=config.client_id, client_secret=config.client_secret, scopes=config.scopes
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/validator.py` & `cognite_neat-0.18.0/cognite/neat/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/workflow/base.py` & `cognite_neat-0.18.0/cognite/neat/workflows/workflow/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,37 @@
 from threading import Event
 from typing import Type
 
 import yaml
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 
-from cognite.neat.core.data_stores.metrics import NeatMetricsCollector
-from cognite.neat.core.exceptions import InvalidWorkFlowError
-from cognite.neat.core.utils.utils import retry_decorator
-from cognite.neat.core.workflow import cdf_store
-from cognite.neat.core.workflow.model import (
+from cognite.neat.graph.extractors.data_stores.metrics import NeatMetricsCollector
+from cognite.neat.exceptions import InvalidWorkFlowError
+from cognite.neat.utils.utils import retry_decorator
+from cognite.neat.workflows.workflow.model import (
     FlowMessage,
     StepExecutionStatus,
     StepType,
     WorkflowConfigItem,
     WorkflowDefinition,
     WorkflowFullStateReport,
     WorkflowStartException,
     WorkflowState,
     WorkflowStepDefinition,
     WorkflowStepEvent,
     WorkflowSystemComponent,
 )
-from cognite.neat.core.workflow.tasks import WorkflowTaskBuilder
+from cognite.neat.workflows.workflow.tasks import WorkflowTaskBuilder
 
-from ..configuration import Config
-from ..utils.cdf import CogniteClientConfig
-from . import utils
+from cognite.neat.app.api.configuration import Config
+from cognite.neat.utils.cdf import CogniteClientConfig
+from . import utils, cdf_store
 from .step_model import DataContract
-import cognite.neat.steps.steps
+import cognite.neat.workflows.steps.steps
 
 summary_metrics = Gauge("neat_workflow_summary_metrics", "Workflow execution summary metrics", ["wf_name", "name"])
 steps_metrics = Gauge("neat_workflow_steps_metrics", "Workflow step level metrics", ["wf_name", "step_name", "name"])
 timing_metrics = Gauge("neat_workflow_timing_metrics", "Workflow timing metrics", ["wf_name", "component", "name"])
 
 
 class BaseWorkflow:
@@ -255,15 +254,15 @@
                     component_name=f"wf step runner , step.id = {step.id}",
                 )
                 def method_runner():
                     return method(flow_message)
 
                 new_flow_message = method_runner()
             elif step.stype == StepType.STD_STEP:
-                for name, step_cls in inspect.getmembers(cognite.neat.steps.steps):
+                for name, step_cls in inspect.getmembers(cognite.neat.workflows.steps.steps):
                     if inspect.isclass(step_cls):
                         if name == step.method:
                             step_obj = step_cls(self.metrics)
                             step_obj.set_global_configs(self.cdf_client, self.data_store_path, self.rules_storage_path)
                             signature = inspect.signature(step_obj.run)
                             parameters = signature.parameters
                             is_valid = True
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.18.0/cognite/neat/workflows/workflow/cdf_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Dict
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Event, FileMetadataUpdate, LabelDefinition, LabelFilter
 from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
 
-from cognite.neat.core.workflow.model import WorkflowFullStateReport, WorkflowState, WorkflowStepEvent
-from cognite.neat.core.workflow.utils import get_file_hash
+from cognite.neat.workflows.workflow.model import WorkflowFullStateReport, WorkflowState, WorkflowStepEvent
+from cognite.neat.workflows.workflow.utils import get_file_hash
 
 
 class NeatCdfResource(BaseModel):
     id: int = None
     name: str
     rtype: str
     last_updated_time: int = None
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.18.0/cognite/neat/workflows/workflow/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import traceback
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 from pydantic import BaseModel
 
-from cognite.neat.core.workflow import BaseWorkflow
-from cognite.neat.core.workflow.base import WorkflowDefinition
-from cognite.neat.core.workflow.model import FlowMessage, InstanceStartMethod, WorkflowState
-from cognite.neat.core.workflow.tasks import WorkflowTaskBuilder
+from cognite.neat.workflows.workflow import BaseWorkflow
+from cognite.neat.workflows.workflow.base import WorkflowDefinition
+from cognite.neat.workflows.workflow.model import FlowMessage, InstanceStartMethod, WorkflowState
+from cognite.neat.workflows.workflow.tasks import WorkflowTaskBuilder
 
 live_workflow_instances = Gauge("neat_workflow_live_instances", "Count of live workflow instances", ["itype"])
 
 
 class WorkflowStartStatus(BaseModel):
     workflow_instance: BaseWorkflow = None
     is_success: bool = True
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/workflow/model.py` & `cognite_neat-0.18.0/cognite/neat/workflows/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/workflow/step_model.py` & `cognite_neat-0.18.0/cognite/neat/workflows/workflow/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.18.0/cognite/neat/workflows/workflow/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from cognite.client import CogniteClient
 
-from cognite.neat.core.workflow.model import FlowMessage
+from cognite.neat.workflows.workflow.model import FlowMessage
 
 
 class WorkflowTaskBuilder:
     """Collection of all base tasks for workflows.All tasks must run in the context of a workflow including threads."""
 
     def __init__(self, cdf_client: CogniteClient, worflow_manager):
         # TODO : figure out ciclura import and set type to WorkflowManager
```

### Comparing `cognite_neat-0.17.4/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.18.0/cognite/neat/workflows/workflow/triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import threading
 import time
 
 import schedule
 from fastapi import Depends, FastAPI, Request
 
-from cognite.neat.core.workflow.manager import WorkflowManager
-from cognite.neat.core.workflow.model import FlowMessage, StepType, WorkflowState
+from cognite.neat.workflows.workflow.manager import WorkflowManager
+from cognite.neat.workflows.workflow.model import FlowMessage, StepType, WorkflowState
 
 
 async def get_body(request: Request):
     return await request.body()
 
 
 fast_api_depends = Depends(get_body)
```

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/__init__.py` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/graph-sheets/power-grid-example.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/graph-sheets/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/ontologies/report.txt` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/ontologies/report.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/ontologies/transformation_rules.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/ontologies/transformation_rules.xlsx`

 * *Files 22% similar despite different names*

```diff
@@ -1,802 +1,801 @@
-00000000: 504b 0304 1400 0000 0800 1849 f956 465a  PK.........I.VFZ
+00000000: 504b 0304 1400 0000 0800 f650 f956 465a  PK.........P.VFZ
 00000010: c10c 8200 0000 b100 0000 1000 0000 646f  ..............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 4d0b c230 1044 ff4a e9dd 6e55 f020 3120  M..0.D.J..nU. 1 
 00000040: d4a3 e0c9 7b48 3736 9064 4376 85fc 7c53  ....{H76.dCv..|S
 00000050: c18f db3c de30 8cba 15ca 58c4 2377 3586  ...<.0....X.#w5.
 00000060: c4a7 7e11 c947 00b6 0b46 c343 d3a9 1947  ..~..G...F.C...G
 00000070: 251a 6958 1e40 ce79 8b13 d967 c424 b01b  %.iX.@.y...g.$..
 00000080: c703 6015 4c33 ce9b fc1d ecb5 3ae7 1cbc  ..`.L3......:...
 00000090: 35e2 29e9 abb7 8598 9c74 976a 3128 f897  5.)......t.j1(..
 000000a0: 6bf3 8e85 d7bc 1fb6 6ff9 6105 bf93 fa05  k.......o.a.....
-000000b0: 504b 0304 1400 0000 0800 1849 f956 8068  PK.........I.V.h
-000000c0: a8bc ee00 0000 cb01 0000 1100 0000 646f  ..............do
-000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6c95  cProps/core.xml.
-000000e0: 91c1 4ec3 300c 865f 65ea bd75 da02 1b51  ..N.0.._e..u...Q
-000000f0: d60b 8813 4848 4c02 718b 1c6f 8b68 da28  ....HHL.q..o.h.(
-00000100: 316a f7f6 b465 eb86 e0c2 31fe 3f7f b615  1j...e....1.?...
-00000110: 855e 621b e839 b49e 025b 8a8b ded5 4d94  .^b..9...[....M.
-00000120: e8d7 c99e d94b 8088 7b72 3a66 03d1 0ce1  .....K..{r:f....
-00000130: b60d 4ef3 f00c 3bf0 1a3f f48e a010 e206  ..N...;..?......
-00000140: 1cb1 369a 358c c2d4 cfc6 e4a8 3438 2bfd  ..6.5.......48+.
-00000150: 67a8 2781 41a0 9a1c 351c 21cf 7238 b34c  g.'.A...5.!.r8.L
-00000160: c1c5 3f1b a664 26fb 6867 aaeb baac 2b27  ..?..d&.hg....+'
-00000170: 6ed8 2887 b7a7 c797 69f9 d436 9175 8394  n.(.....i..6.u..
-00000180: 54ca a0c4 409a db50 8d17 f943 5f2b b828  T...@..P...C_+.(
-00000190: aae3 ecef 0299 c530 41f2 c1d3 3a39 25af  .......0A...:9%.
-000001a0: e5dd fde6 21a9 0a51 94a9 58a6 c5f5 46dc  ....!..Q..X...F.
-000001b0: 4ab1 9257 cbf7 d1f5 a3ff 2c74 adb1 5bfb  J..W......,t..[.
-000001c0: 4fe3 eac2 7812 540a 7efd 5bf5 0550 4b03  O...x.T.~.[..PK.
-000001d0: 0414 0000 0008 0018 49f9 5699 5c9c 2310  ........I.V.\.#.
-000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
-000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
-00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
-00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
-00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
-00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
-00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
-00000250: b72f dee0 5732 2411 4130 19a7 aff0 c00a  ./..W2$.A0......
-00000260: a54c 5eb5 5a69 00c3 387d c913 12c3 dc82  .L^.Zi..8}......
-00000270: 8b08 4b78 14cb d65c e05b 1a2f 23d6 eab4  ..Kx...\.[./#...
-00000280: dbdd 5684 696c a118 4764 607d 5e2c 6840  ..V.il..Gd`}^,h@
-00000290: d054 515a 6f5f 20b4 e51f 33f8 15cb 548d  .TQZo_ ...3...T.
-000002a0: 65a3 0113 5741 26b9 88b4 f2f9 6cc5 fcda  e...WA&.....l...
-000002b0: de3e 65cf e93a 1d32 816e 301b 5820 7fce  .>e..:.2.n0.X ..
-000002c0: 6fa7 e44e 5a88 e154 c2c4 c06a 673f 566b  o..NZ..T...jg?Vk
-000002d0: c7d1 d248 8082 c97d 9405 ba49 f6a3 d315  ...H...}...I....
-000002e0: 0832 0d3b 3a9d 58ce 767c f6c4 ed9f 8cca  .2.;:.X.v|......
-000002f0: da74 346d 1ae0 e3f1 7838 b6cb d28b 701c  .t4m....x8....p.
-00000300: 04e0 51bb 9ec2 9df4 6cbf a441 09b4 a369  ..Q.....l..A...i
-00000310: d064 d8f6 daae 91a6 aa8d 534f d3f7 7ddf  .d........SO..}.
-00000320: eb9b 689c 0a8d 5b4f d36b 77dd d38e 89c6  ..h...[O.kw.....
-00000330: add0 780d bef1 4f87 c3ae 89c6 abd0 74eb  ..x...O.......t.
-00000340: 6926 27fd ae6b a4e9 1668 4246 e3eb 7a12  i&'..k...hBF..z.
-00000350: 15b5 e540 d320 0058 7076 d6cc d203 965e  ...@. .Xpv.....^
-00000360: 29fa 7594 1ad9 1dbb dd41 5cf0 58ee 3989  ).u......A\.X.9.
-00000370: 11fe c6c5 04d6 69d2 1996 3446 729d 9005  ......i...4Fr...
-00000380: 0e00 37c4 d14c 507c af41 b68a e0c2 92d2  ..7..LP|.A......
-00000390: 5c90 d6cf 29b5 501a 089a c881 f547 8221  \...).P......G.!
-000003a0: c5dc affd f597 bbc9 a433 7a9d 7d3a ce6b  .........3z.}:.k
-000003b0: 947f 69ab 01a7 edbb 9bcf 93fc 73e8 e49f  ..i.........s...
-000003c0: a793 d74d 42ce 70bc 2c09 f1fb 235b 6187  ...MB.p.,...#[a.
-000003d0: 276e 3b13 723a 1c67 427c cff6 f691 a525  'n;.r:.gB|.....%
-000003e0: 32cf eff9 0aeb 4e3c 671f 5696 b05d cfcf  2.....N<g.V..]..
-000003f0: e49e 8c72 23bb ddf6 587d f64f 476e 23d7  ...r#...X}.OGn#.
-00000400: a9c0 b322 d794 4624 459f c82d bae4 1138  ..."..F$E..-...8
-00000410: b549 0d32 133f 089d 8698 6a50 1c02 a409  .I.2.?....jP....
-00000420: 3196 a186 f8b4 c6ac 11e0 137d b7be 08c8  1..........}....
-00000430: df8d 88f7 ab6f 9a3d 57a1 5849 da84 f810  .....o.=W.XI....
-00000440: 461a e29c 73e6 73d1 6cfb 07a5 46d1 f655  F...s.s.l...F..U
-00000450: bcdc a397 5815 0197 18df 34aa 352c c5d6  ....X.....4.5,..
-00000460: 7895 c0f1 ad9c 3c1d 1312 cd94 0b06 4186  x.....<.......A.
-00000470: 9724 2612 a939 7e4d 4813 fe2b a5da fe9c  .$&..9~MH..+....
-00000480: d340 f094 2f24 fa4a 918f 69b3 23a7 7426  .@../$.J..i.#.t&
-00000490: cde8 331a c146 af1b 7587 68d2 3c7a fe05  ..3..F..u.h.<z..
-000004a0: f99c 350a 1c91 1b1d 0267 1bb3 4621 8469  ..5......g..F!.i
-000004b0: bbf0 1eaf 248e 9aad c211 2b42 3e62 1936  ....$.....+B>b.6
-000004c0: 1a72 b516 81b6 71a9 8460 5a12 c6d1 784e  .r....q..`Z...xN
-000004d0: d2b4 11fc 59ac 3593 3e60 c8ec cd91 75ce  ....Y.5.>`....u.
-000004e0: d691 0e11 925e 3742 3e62 ce8b 9011 bf1e  .....^7B>b......
-000004f0: 8638 4a9a eda2 7158 04fd 9e5e c349 c1e8  .8J...qX...^.I..
-00000500: 82cb 66fd b87e 86d5 336c 2c8e f747 d417  ..f..~..3l,..G..
-00000510: 4ae4 0f26 a73f e932 3407 a39a 5909 bd84  J..&.?.24...Y...
-00000520: 566a 9faa 8734 3ea8 1e32 0a05 f1b9 1e3e  Vj...4>..2.....>
-00000530: e57a 780a 3796 c6bc 50ae 827b 01ff d1da  .zx.7...P..{....
-00000540: 37c2 abf8 82c0 397f 2e7d cfa5 efb9 f43d  7.....9..}.....=
-00000550: a1d2 b737 237d 67c1 d38b 5bde 466e 5bc4  ...7#}g...[.Fn[.
-00000560: fbae 31da d734 2e28 6357 72cd c8c7 54af  ..1..4.(cWr...T.
-00000570: 9329 d839 9fc0 ecfd 683e 9ef1 edfa d924  .).9....h>.....$
-00000580: 84af 9a59 2d23 1690 4b81 b341 24b8 fc8b  ...Y-#..K..A$...
-00000590: caf0 2ac4 09e8 645b 2509 cb54 d365 378a  ..*...d[%..T.e7.
-000005a0: 129e 421b 6ee9 53f5 4a95 d7e5 afb9 28b8  ..B.n.S.J.....(.
-000005b0: 3c5b e4e9 afa1 743e 2ccf f93c 5fe7 b4cd  <[....t>,..<_...
-000005c0: 0b33 43b7 724b eab6 94be b526 384a f4b1  .3C.rK.....&8J..
-000005d0: cc70 4e1e cb0c 3b67 3c92 1db6 77a0 1d35  .pN...;g<...w..5
-000005e0: fbf6 5d76 e423 a530 5397 43b8 1a42 be03  ..]v.#.0S.C..B..
-000005f0: 6dba 9ddc 3a38 9e98 91b9 0ad3 5290 6fc3  m...:8......R.o.
-00000600: f9e9 c578 1ae2 39d9 04b9 7d98 576d e7d8  ...x..9...}.Wm..
-00000610: d1d1 fbe7 c151 b0a3 ef3c 961d c788 f2a2  .....Q...<......
-00000620: 21ee a186 98cf c343 8779 7b5f 9867 95c6  !......C.y{_.g..
-00000630: 5034 146d 6cac 242c 46b7 60b8 d7f1 2c14  P4.ml.$,F.`...,.
-00000640: e064 602d a007 83af 5102 f252 5560 315b  .d`-....Q..RU`1[
-00000650: c603 2b90 a27c 4c8c 45e8 70e7 975c 5fe3  ..+..|L.E.p..\_.
-00000660: d192 e3db a665 b56e af29 7719 6d22 5239  .....e.n.)w.m"R9
-00000670: c269 9813 67ab cade 65b1 c155 1dcf 555b  .i..g...e..U..U[
-00000680: f2b0 be6a 3db4 154e cffe 59ad c89f 0c11  ...j=..N..Y.....
-00000690: 4e16 0b12 4863 9417 a64a a2f3 1953 bee7  N...Hc...J...S..
-000006a0: 2b49 c455 38bf 4533 b612 9718 bce3 e6c7  +I.U8.E3........
-000006b0: 714e 53b8 1276 b60f 0232 b9bb 39a9 7a65  qNS..v...2..9.ze
-000006c0: 3167 a6f2 df2d 0c09 2c5b 8859 12e2 4d5d  1g...-..,[.Y..M]
-000006d0: edd5 e79b 9cae 7a22 76fa 9777 c160 f2fd  ......z"v..w.`..
-000006e0: 70c9 470f e53b e75f f45d 43ae 7ef6 dde3  p.G..;._.]C.~...
-000006f0: fa6e 933b 484c 9c79 c511 0174 4502 2395  .n.;HL.y...tE.#.
-00000700: 1c06 1617 32e4 50ee 9290 0613 01cd 94c9  ....2.P.........
-00000710: 44f0 0282 64a6 1c80 98fa 0bbd f20c b929  D...d..........)
-00000720: 15ce ad3e 397f 452c 8386 4e5e d225 1214  ...>9.E,..N^.%..
-00000730: 8ab0 0c05 2117 72e3 efef 936a 778c d7fa  ....!.r....jw...
-00000740: 2c81 6d84 5432 64d5 17ca 4389 c13d 3372  ,.m.T2d...C..=3r
-00000750: 43d8 5425 f3ae da26 0b85 dbe2 54cd bb1a  C.T%...&....T...
-00000760: be26 604b c37a 6e9d 2d27 ffdb 5ed4 3db4  .&`K.zn.-'..^.=.
-00000770: 173d 46f3 a399 e01e b387 739b 7ab8 c245  .=F.......s.z..E
-00000780: acff 58d6 1ef9 32df 3970 db3a de03 5ee6  ..X...2.9p.:..^.
-00000790: 132c 43a4 7ec1 7d8a 8a80 11ab 62be baaf  .,C.~.}.....b...
-000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
-000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
-000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
-000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
-000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
-000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
-00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 1849 f956 e0d9 6c24  .........I.V..l$
-00000820: 3d02 0000 a307 0000 1800 0000 786c 2f77  =...........xl/w
-00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00000840: 2e78 6d6c 8595 db72 9b30 1086 5f85 e101  .xml...r.0.._...
-00000850: 2ce3 b333 9899 da9d 4e7b 914e 269e 26d7  ,..3....N{.N&.&.
-00000860: 322c b6c6 42a2 d262 d2b7 afa4 38b2 9b82  2,..B..b....8...
-00000870: b842 a7dd 6f0f e257 da4a 75d6 2700 8cde  .B..o..W.Ju.'...
-00000880: 2a2e f426 3e21 d60f 84e8 fc04 15d5 2359  *..&>!........#Y
-00000890: 8330 3ba5 5415 4533 5547 a26b 05b4 7046  .0;.T.E3UG.k..pF
-000008a0: 1527 93f1 7841 2aca 449c a56e ed49 65a9  .'..xA*.D..n.Ie.
-000008b0: 6c90 3301 4f2a d24d 5551 f567 0b5c b69b  l.3.O*.MUQ.g.\..
-000008c0: 3889 3f16 9ed9 f184 6e81 6469 4d8f b007  8.?.....n.diM...
-000008d0: fc55 1b03 3325 de4f c12a 109a 4911 2928  .U..3%.O.*..I.)(
-000008e0: 37f1 97e4 619b cc9c 893b f2c2 a0d5 77e3  7...a....;....w.
-000008f0: c866 7390 f26c 273f 8a4d 3cb6 4101 871c  .fs..l'?.M<.A...
-00000900: ad0f 6a3e 17d8 01e7 d695 09e5 f7d5 6b7c  ..j>..........k|
-00000910: a35a cbfb f187 fb6f ae00 26be 03d5 b093  .Z.....o..&.....
-00000920: fc95 1578 dac4 ab38 2aa0 a40d c767 d97e  ...x...8*....g.~
-00000930: 876b 52f3 5b88 5f29 d22c 55b2 8d94 cd36  .kR.[._).,U....6
-00000940: 4b73 3b70 7497 bd39 ce84 add5 1e95 d965  Ks;pt..9.......e
-00000950: 8687 99a0 15e8 9ae6 9012 34c1 d845 925f  ..........4..E._
-00000960: 4db7 7d46 b671 da74 ee7c 1ce5 f228 18c2  M.}F.q.t.|...(..
-00000970: 8832 d232 5190 7fdd 1013 8d0f 69e2 439a  .2.2Q.......i.C.
-00000980: 0443 323d 2fd9 5b57 3c93 4f16 ae96 f788  .C2=/.[W<.O.....
-00000990: a947 4c83 88c2 94ea 5116 c07f 9af4 bb48  .GL.....Q......H
-000009a0: d321 d2cc 9366 4152 5e94 7b5b de3e d06c  .!...fAR^.{[.>.l
-000009b0: 0834 f7a0 7910 7401 656f 6f17 633e c458  .4..y.t.eoo.c>.X
-000009c0: 78c6 22c8 607a d728 0502 5ffa 610b 677b  x.".`z.(.._.a.g{
-000009d0: 3036 972c 49c9 a5e3 222c 3d6e 19ae 9df9  06.,I...",=n....
-000009e0: f911 8a2e ca72 28a5 9567 ac82 8ca6 2efa  .....r(..g......
-000009f0: 18ab 21c6 da33 d641 0632 e49d cd5f 0f11  ..!..3.A.2..._..
-00000a00: 92f1 ed37 1e87 6f34 e85c b11a 7bba 62ad  ...7..o4.\..{.b.
-00000a10: 0750 778a 1196 0cd7 16a9 3a31 9f6d fec7  .Pw.......:1.m..
-00000a20: dc54 2009 cb40 2e05 2a76 68fa 5083 6290  .T ..@..*vh.P.b.
-00000a30: dcd4 2009 cb81 b262 aa3b 2983 4290 dc94  .. ....b.;).B...
-00000a40: 2009 4b01 67b9 7961 ba85 b65f 06c8 9db6   .K.g.ya..._....
-00000a50: dbc7 eb91 aa23 133a e250 1a8b f168 69fe  .....#.:.P...hi.
-00000a60: 6ef5 fe18 bc4f 50d6 2e86 8344 9495 1b9e  n....OP....D....
-00000a70: cc23 0aca 1e30 fba5 94e8 2716 e3df e5ec  .#...0....'.....
-00000a80: 2f50 4b03 0414 0000 0008 0018 49f9 5619  /PK.........I.V.
-00000a90: c663 fc00 0e00 00bb 8300 0018 0000 0078  .c.............x
-00000aa0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00000ab0: 6574 322e 786d 6cad 9ddb 72da 4817 855f  et2.xml...r.H.._
-00000ac0: 85f2 0304 734c 66ca 71d5 60a1 ee74 2687  ....sLf.q.`..t&.
-00000ad0: 8a33 99aa ff4e 8636 a822 2422 449c ccd3  .3...N.6."$"D...
-00000ae0: ff12 8969 d9ea 4f4d cbbe 4acc 621f b417  ...i..OM..J.b...
-00000af0: 12e2 43b4 2eee b2fc eb6e ad75 d1fb b149  ..C......n.u...I
-00000b00: d2dd ebb3 7551 6cff ecf7 778b b5de 44bb  ....uQl...w...D.
-00000b10: 17d9 56a7 a572 9be5 9ba8 28ff cc57 fddd  ..V..r....(..W..
-00000b20: 36d7 d1f2 10b4 49fa c3f3 f369 7f13 c5e9  6.....I....i....
-00000b30: d9e5 c5e1 b18f f9e5 45b6 2f92 38d5 1ff3  ........E./.8...
-00000b40: de6e bfd9 44f9 cf99 4eb2 bbd7 6783 b3fb  .n..D...N...g...
-00000b50: 073e c5ab 7571 78a0 7f79 b18d 56fa 5a17  .>..uqx..y..V.Z.
-00000b60: ff6c cb80 f2cf fe31 cf32 dee8 7417 6769  .l.....1.2..t.gi
-00000b70: 2fd7 b7af cffe 1afc f9f6 e5f9 21e4 f094  /...........!...
-00000b80: 2fb1 bedb d5fe dfab b6e6 26cb be56 7fbc  /.........&..V..
-00000b90: 59be 3e3b af9a d289 5e14 558e a8fc e7bb  Y.>;....^.U.....
-00000ba0: bed2 4952 a52a 5bf9 f63b eb99 a95a 45d6  ..IR.*[..;...ZE.
-00000bb0: ff7f 9f3e 3c0c a0ec ef26 dae9 ab2c f937  ...><....&...,.7
-00000bc0: 5e16 ebd7 67af ce7a 4b7d 1bed 93e2 5376  ^...g..zK}....Sv
-00000bd0: 27f5 ef8d 9a98 1683 a888 2e2f f2ec ae97  '........../....
-00000be0: 575b 7b79 b1a8 fe53 952c 9f18 a7d5 94ae  W[{y...S.,......
-00000bf0: 8bbc 7c3c 2e2b 1597 d5d3 7bef b2a5 4e7a  ..|<.+....{...Nz
-00000c00: 81be 8dd3 b86a fca2 5f94 2d55 4fe8 2f7e  .....j.._.-UO./~
-00000c10: 2798 3d4e 5015 3c28 57a8 04a8 cca9 9deb  '.=NP.<(W.......
-00000c20: 222a b4a5 7c88 a904 2a92 8abc 4db3 bb44  "*..|...*...M..D
-00000c30: 2f57 ba34 e8db 3ede 1db6 b997 642b 4be1  /W.4..>.....d+K.
-00000c40: 3798 5ea1 f2d6 a6f4 4b4b 8ebe 0c8f be0c  7.^.....KK......
-00000c50: a1c7 ab24 daed 6c3e 50c0 fb68 631b dc15  ...$..l>P..hc...
-00000c60: 3d3f d0bb 451e 6fc1 ee80 c23e 46b9 4e8b  =?..E.o....>F.N.
-00000c70: 1eb5 37e7 72e5 4ebc 28cd 5dda dc75 4555  ..7.r.N.(.]..uEU
-00000c80: fe04 f657 86a0 d84f 7a9b 440b bdec cd7e  ...W...Oz.D....~
-00000c90: 5ac2 2485 5d67 fb7c 612b f4a6 3da2 374f  Z.$.]g.|a+..=.7O
-00000ca0: 8bb8 f8d9 031f 1445 bf8b 8ac5 da12 f016  .......E........
-00000cb0: 5f19 d9a6 3c46 150f 431e bcba 46c7 57d7  _...<F..C...F.W.
-00000cc0: 0872 8c82 c32e 6f7b 7d3d 0e31 fb39 2a01  .r....o{}=.1.9*.
-00000cd0: 95a9 0e2e d745 9697 47db 4f7a 7718 d3e7  .....E..G.Ozw...
-00000ce0: 9f5b db78 e698 3c44 45a0 22a9 a1ea bd66  .[.x..<DE."....f
-00000cf0: 57be d97c 5dbd 5864 abf2 60a7 5f44 71ff  W..|].Xd..`._Dq.
-00000d00: 2e4e 977d 9be3 fee3 5314 a27f 946f 0636  .N.}....S....o.6
-00000d10: 9b6d 1bf1 c0cd f1d1 cd31 e4fe 4be7 7164  .m.......1..K.qd
-00000d20: 35f3 7184 3113 9580 aabc 4977 4594 2487  5.q.1.....IwE.$.
-00000d30: 9d91 5cc4 ac21 2a02 1549 9d78 bae8 3d36  ..\..!*..I.x..=6
-00000d40: 4511 68a2 6d1b 1e98 3839 9a38 a16e 763b  E.h.m...89.8.nv;
-00000d50: 6dcb 3d7b 1c60 3c44 25a0 221e 3b24 260f  m.={.`<D%.".;$&.
-00000d60: 5111 a848 6ac8 d34a dfe1 290a 4027 6d9b  Q..Hj..J..).@'m.
-00000d70: f0c0 c9e9 d1c9 2935 f323 dec1 5467 8f63  ......)5.#..Tg.c
-00000d80: 8c99 a804 54e7 df72 4a9f f7f9 4df9 f0d5  ....T..rJ...M...
-00000d90: 3aca cb0d 2a5f d0bb 225e d8ec c4f4 212a  :...*_.."^....!*
-00000da0: 0215 492d 79da d961 828a 62d0 51db 563c  ..I-y..a..b.Q.V<
-00000db0: 70f4 e5d1 d197 f496 1b84 d59e 83ef 992d  p..............-
-00000dc0: 713d 7382 6d3b 3b7b 1c69 5c47 658e 4a88  q=s.m;;{.i\Ge.J.
-00000dd0: 8a40 4552 ef9e 5676 1c9d a238 b4d3 b625  .@ER..Vv...8...%
-00000de0: 0fec 7c75 b4f3 159e 4155 6f65 8f4f a17e  ..|u....AUoe.O.~
-00000df0: 59f9 38c6 eca0 a804 54e7 4b54 bec1 dc24  Y.8.....T.KT...$
-00000e00: fabe de3f e514 6dfb 2666 0e51 11a8 48ea  ...?..m.&f.Q..H.
-00000e10: c6d3 d00e c353 1483 66da b6e2 8199 7f1c  .....S..f.......
-00000e20: cdfc 83fa 29ae f6f9 77eb c1f6 7188 f112  ....)...w...q...
-00000e30: 9580 ca54 2fe2 8f79 b6dc 2f0a ebe7 1ecc  ...T/..y../.....
-00000e40: 18a2 2250 91d4 85a7 87fe 3353 1482 16da  .."P......3S....
-00000e50: 36e2 8185 8373 0321 ce5b a6fb 215f 4569  6....s.!.[..!_Ei
-00000e60: fcdf e1fc d271 7232 6b24 aad1 0894 022c  .....qr2k$.....,
-00000e70: ef3a 17e2 9c21 4b82 2589 9d78 1afc 5c03  .:...!K.%..x..\.
-00000e80: 5598 087d b76e dd43 e36b f4a9 0d3f b5ec  U..}.n.C.k...?..
-00000e90: 56b3 4660 cde8 16ee 44e5 aa53 a679 aaf3  V.F`....D..S.y..
-00000ea0: d5cf 2303 1279 b4b5 7dfe 9e73 fe90 25c1  ..#..y..}..s..%.
-00000eb0: 92c4 ae7c 4def 384c 8581 6cb2 9364 0d0c  ...|M.8L..l..d..
-00000ec0: ca1a 20c5 a93e 75d8 3fdc 3462 6afe a214  .. ..>u.?.4bj...
-00000ed0: b456 f278 d9cf b946 c892 6049 6267 be1e  .V.x...F..`Ibg..
-00000ee0: fbcf 5261 0cdb 6bdb 9087 f61a 9634 783a  ..Ra..k......4x:
-00000ef0: e599 3572 d4ec 66bc 8495 9df6 3255 6249  ..5r..f.....2UbI
-00000f00: b024 b113 5f7b 9f3e 4b85 39d8 6e27 6b1a  .$.._{.>K.9.n'k.
-00000f10: 18d8 3420 0812 6477 6975 1cb5 facb c089  ..4 ..dwiu......
-00000f20: a500 4b7d caca 517c c863 9d16 1180 ea39  ..K}..Q|.c.....9
-00000f30: e70d 5912 2c49 ecc6 d7e3 0e03 5418 c4a6  ..Y.,I......T...
-00000f40: 3ad9 d3c0 c0a7 01f1 90f9 f706 52fe ed28  :...........R..(
-00000f50: e327 9602 ace3 01a0 387d c892 6049 6253  .'......8}..`IbS
-00000f60: bec6 fa0e 5161 04bb eae4 5003 03a2 06c4  ....Qa....P.....
-00000f70: 44e6 3f16 c9be fa36 f37f 596a 3f1e 338f  D.?....6..Yj?.3.
-00000f80: 6229 c07a 5066 ceb9 4296 044b 123b f0b5  b).zPf..B..K.;..
-00000f90: b2eb e414 46b2 a54e 1035 3024 6a40 5c24  ....F..N.50$j@\$
-00000fa0: 8c13 bb93 4878 ae58 0ab0 8ccf 7eca 3c8a  ....Hx.X....~.<.
-00000fb0: 25c1 92c4 a67c cdf5 9ca1 c200 f6d4 49a3  %....|........I.
-00000fc0: 0606 470d 088f 84f1 0feb d7a2 b346 44cd  ..G..........FD.
-00000fd0: 54c6 5158 e77a bfdd 6679 513e 547e 42d8  T.QX.z..fyQ>T~B.
-00000fe0: e7ec 2803 2996 044b 123b f275 d477 820a  ..(.)..K.;.u.w..
-00000ff0: 23d8 5227 931a 1828 3520 5c12 2659 79c6  #.R'...(5 \.&Yy.
-00001000: 92da ae28 9835 826a ae32 98c2 5227 bbca  ...(.5.j.2..R'..
-00001010: 888a 25c1 92c4 8e7c 5ded 3044 8541 6cac  ..%....|].0D.Al.
-00001020: 9354 0d0d a91a 120f 9159 1eff 9795 e7a3  .T.......Y......
-00001030: 49f5 2585 f502 0d66 532c 0558 b0e5 bb90  I.%....fS,.X....
-00001040: 39e7 0b59 122c 49ec c2d3 d2ee e353 188a  9..Y.,I......S..
-00001050: c65a b7e7 a1b1 8644 0d89 81bc 995f f135  .Z.....D....._.5
-00001060: 374c a158 0ab0 94d7 1777 5c20 6449 b024  7L.X.....w\ dI.$
-00001070: b12d 5f8f 3b4c 5261 10bb ebbe 98aa 7635  .-_.;LRa......v5
-00001080: 1521 90fb 9e5e bcb1 facb 148a a5c0 59cc  .!...^........Y.
-00001090: 6a27 1327 9604 4b12 bbf0 b5b3 d3e8 1486  j'.'..K.........
-000010a0: b1a1 4ee8 3434 d069 4890 c374 6577 9441  ..N.44.iH..tew.A
-000010b0: 134b 81b3 9ad5 5186 4c2c 0996 2476 e1eb  .K....Q.L,..$v..
-000010c0: 68b7 d929 8c63 4b9d 6069 68c0 d210 2f30  h..).cK.`ih.../0
-000010d0: 326d d93d 65b8 c452 e02c 67f5 94a1 124b  2m.=e..R.,g....K
-000010e0: 8225 895d f87a da71 780a 03d9 5427 581a  .%.].z.qx...T'X.
-000010f0: 1ab0 3424 c251 ef2b b2ba ca80 89a5 e0a4  ..4$.Q.+........
-00001100: 7a56 6799 2ab1 2458 92d8 89af b35d 27a8  zVg.*.$X.....]'.
-00001110: 3092 ad75 d2a5 a1a1 4b43 221d f5c6 6eac  0..u....KC"...n.
-00001120: d632 5d62 2938 a99e d55a a64c 2c09 9624  .2]b)8...Z.L,..$
-00001130: 76e2 6b6d d709 2a8c 646b 9d94 6968 28d3  v.km..*.dk..ih(.
-00001140: 9080 47ad 31fb 4ecb b489 a5e0 9472 5663  ..G.1.N......rVc
-00001150: 9930 b124 5892 d888 afb1 1de7 a730 907d  .0.$X........0.}
-00001160: 7592 a6a1 214d 43a2 1eb5 beec 7b2c 0327  u...!MC.....{,.'
-00001170: 9682 53ca 597d 65ce c492 6049 6223 bebe  ..S.Y}e...`Ib#..
-00001180: 769c 9fc2 40f6 d589 9b86 0637 0d09 7a98  v...@......7..z.
-00001190: bebe 586d 65e2 c452 e0ac 66f5 9429 134b  ..Xme..R..f..).K
-000011a0: 8225 895d f87a da6d 760a e3d8 5227 681a  .%.].z.mv...R'h.
-000011b0: 19d0 3422 dc61 dab2 1e81 1b71 c652 9682  ..4".a.....q.R..
-000011c0: 13aa d94c e58c 214b 8225 897d f8fe 40a3  ...L..!K.%.}..@.
-000011d0: dbf4 14c6 f1cf 349c 9069 6420 d3c8 8546  ......4..id ...F
-000011e0: 5ed8 0fbf 8db8 9aa9 cc99 4ea8 6635 95c1  ^.........N.f5..
-000011f0: 124b 8225 897d f89a da6d 7a0a e3d8 5427  .K.%.}...mz...T'
-00001200: 5b1a 19b6 3442 4092 3abe 656d 44d6 6c65  [...4B@.:.emD.le
-00001210: bc84 f5e8 5b56 ce15 b224 5892 d881 afa1  ....[V...$X.....
-00001220: 5d27 a730 922d 75d2 a551 ede7 7148 48dc  ]'.0.-u..Q..qHH.
-00001230: bf75 9a35 826b aeb6 fc54 8e4a 7a41 612e  .u.5.k...T.JzAa.
-00001240: 10b2 2458 92d8 96af d54f 98a8 c260 76db  ..$X.....O...`v.
-00001250: 099e 4606 3c8d 0881 fc1d ddc0 6f21 9938  ..F.<.......o!.8
-00001260: b114 601d dfab 13b9 46c8 9260 4962 67be  ..`.....F..`Ibg.
-00001270: 2efb 4e52 6104 5beb c44f 2383 9f46 8440  ..NRa.[..O#..F.@
-00001280: fe8e d2e5 22fb ae73 abbd 8c9e 580a b096  ...."..s....X...
-00001290: eb27 029c 3364 49b0 24b1 135f 3bbb 4c4f  .'..3dI.$.._;.LO
-000012a0: 6114 5bea c44e 2383 9d46 843e de65 6976  a.[..N#..F.>.eiv
-000012b0: b830 d06a 2923 2796 02ac 75a8 83bb 27f3  .0.j)#'...u...'.
-000012c0: 2696 044b 12db f0f5 b3cb e814 46b1 9f4e  &..K........F..N
-000012d0: d634 32ac 6944 c8e3 dd3e 2962 3694 4913  .42.iD...>)b6.I.
-000012e0: 4b01 166b 3794 3913 4b82 2589 6df8 1ada  K..k7.9.K.%.m...
-000012f0: 6976 0ac3 d851 2765 1a19 ca34 22d8 f13e  iv...Q'e...4"..>
-00001300: a36b 231a 2135 3799 2f61 a1b6 6b23 385f  .k#.!57./a..k#8_
-00001310: c892 6049 6217 be66 7a8f 4d61 081b e9c4  ..`Ib..fz.Ma....
-00001320: 4a23 8395 4684 38de 67ed 175f cf1a 9135  J#..F.8.g.._...5
-00001330: 3f19 2c61 bd53 aef7 e6bc 214b 8225 89dd  ?.,a.S....!K.%..
-00001340: f8fa da75 8a0a 23d9 5e27 621a 1bc4 3426  ...u..#.^'b...4&
-00001350: d8f1 3e8b 771a 7f3d d908 33de b214 6031  ..>.w..=..3...`1
-00001360: d7d9 11e7 0c59 122c 49ec c477 f988 4ee3  .....Y.,I..w..N.
-00001370: 5318 c68b 4838 11d3 d820 a631 c18e f759  S...H8... .1...Y
-00001380: 3a4b a2a5 beff 3069 b596 3913 4b01 97dc  :K....0i..9.K...
-00001390: 6f6e 74fe e1f6 50d7 6e2e b326 9604 4b12  ont...P.n..&..K.
-000013a0: 7bf1 35f7 0963 5418 cc16 3b81 d3d8 00a7  {.5..cT...;.....
-000013b0: 31c1 0fe7 bc67 8dd0 9ac1 4c9c b0a0 179b  1....g....L.....
-000013c0: e002 214b 8225 896d f97a dd79 9e0a 43d9  ..!K.%.m.z.y..C.
-000013d0: 6927 871a 1b0e 3526 f0f1 e1f6 f67a 9de5  i'....5&.....z..
-000013e0: f69d 98f9 134b 0196 3a69 791f c64e 2c09  .....K..:iy..N,.
-000013f0: 9624 76e3 6b6d 8701 2a0c 6253 dd8b 35d5  .$v.km..*.bS..5.
-00001400: 566b 22e4 f121 654f 5b16 6c6a 59b1 e949  Vk"..!eO[.ljY..I
-00001410: 4b36 b5ac d9d4 b268 53cb aa4d cfb5 6c93  K6.....hS..M..l.
-00001420: fffc 14c6 b0a5 4ecc 3436 9869 4cc8 e343  ......N.46.iL..C
-00001430: 9ead aadf 91db 569a 9b35 a26a a632 66c2  ......V..5.j.2f.
-00001440: 5ace 1329 c64c 2c09 9624 76e2 6b68 97e9  Z..).L,..$v.kh..
-00001450: 298c 624b 9d98 696c 30d3 98a8 c7c7 ec4e  ).bK..il0......N
-00001460: e77c 72cc 9c89 a580 a539 4b21 4b82 2589  .|r......9K!K.%.
-00001470: 1be6 eb5a a701 290c 63db 9c34 696c 68d2  ...Z..).c..4ilh.
-00001480: 1801 8ffe 75b8 dbad e3ad d538 e649 2c05  ....u......8.I,.
-00001490: 58ce 17e9 738d 9025 c192 c4ce 7c6d ee38  X...s..%....|m.8
-000014a0: 5085 816c b413 328d 0d64 1a13 fa70 2d35  P..l..2..d...p-5
-000014b0: d008 ac19 cda8 09cb 39d6 b19a 73ce 9025  ........9...s..%
-000014c0: c192 c44e 7c8d ed38 4085 816c ac13 3a8d  ...N|..8@..l..:.
-000014d0: 0d74 1a3f 0102 cd1a c135 7399 3b61 49bf  .t.?.....5s.;aI.
-000014e0: cf37 0ca0 5812 2c49 6ccb d7e9 274c 5461  .7..X.,Il...'LTa
-000014f0: 30bb ed64 5013 c3a0 26b8 f452 0b90 9f35  0..dP...&..R...5
-00001500: a28c cd2c 0558 cbcb 662e 10b2 2458 92d8  ...,.X..f...$X..
-00001510: 96ef 1a98 5d46 a930 8a57 c274 e2a8 89c1  ....]F.0.W.t....
-00001520: 5113 5cd0 5b7f dbeb d4ba a0f2 ac11 54b3  Q.\.[.........T.
-00001530: 9731 1496 f259 dc94 7914 4b82 2589 4df9  .1...Y..y.K.%.M.
-00001540: 9adb 618e 0a83 d85b 2787 9a18 0e35 21f8  ..a....['....5!.
-00001550: 711d a7ab 441f a849 0b6c 6c84 d75c 6616  q...D..I.ll..\f.
-00001560: 8545 ddb0 91b3 862c 0996 24f6 e26b ee93  .E.....,..$..k..
-00001570: 06a9 309c 6d76 42a8 8981 5013 c221 27fe  ..0.mvB...P..!'.
-00001580: c07c d648 5033 9a81 1496 f53b 5a33 9962  .|.HP3.....;Z3.b
-00001590: 49b0 24b1 2d5f cf9f 3855 8509 d875 27a5  I.$.-_..8U...u'.
-000015a0: 9a18 4a35 2162 f279 9d6b f7be cdbc 8aa5  ..J5!b.y.k......
-000015b0: 006b 9eb0 6f33 ad62 49b0 24b1 175f 9f9f  .k..o3.bI.$.._..
-000015c0: 3247 85d1 6cb2 7bc9 f1da 9ae3 c450 3ec7  2G..l.{......P>.
-000015d0: 1b7d 5dee 5676 735b 561e 6f59 7afc 39d6  .}].Vvs[V.oYz.9.
-000015e0: 1e6f 597c bc65 f5f1 96e5 c79f 6bfd f12e  .oY|.e......k...
-000015f0: 8354 18c5 ee3a 11d6 c420 ac09 a196 6353  .T...:... ....cS
-00001600: d6ef 881a 6135 7b19 6161 3117 96e4 9c21  ....a5{.aa1....!
-00001610: 4b82 2589 9df8 7ada 697c 0ac3 d854 27e0  K.%...z.i|...T'.
-00001620: 9a18 c035 21ac f2f9 2e73 1e95 9971 b114  ...5!....s...q..
-00001630: 60c5 138e ca4c b558 122c 49ec c5d7 dbee  `....L.X.,I.....
-00001640: 5354 18cb 063b c1d6 c480 ad09 e115 5825  ST...;........X%
-00001650: 7cd6 08a8 b9ca 400b cb9c ba38 39e7 0e59  |.....@....89..Y
-00001660: 122c 49ec c8d7 5bcf 012a 0c60 439d 406b  .,I...[..*.`C.@k
-00001670: 6280 d684 08ca 3f5b 5a2e b311 52b3 9431  b.....?[Z...R..1
-00001680: 1616 3ae5 f229 ce1b b224 5892 d88d af9d  ..:..)...$X.....
-00001690: dee3 5318 c286 3a99 d5d4 30ab 2921 93fb  ..S...:...0.)!..
-000016a0: 5dc7 6669 23c8 58ca 52e0 2ce5 da4b 3977  ].fi#.X.R.,..K9w
-000016b0: c892 6049 6247 beb7 f8e8 3044 8541 7c93  ..`IbG....0D.A|.
-000016c0: 0f27 ac9a 1a58 3525 5e72 e2b4 678d 0435  .'...X5%^r..g..5
-000016d0: 9319 5c61 599f 55c9 397f c892 6049 6257  ..\aY.U.9...`IbW
-000016e0: be46 3f71 a80a 13b0 e94e 8a35 3514 6b4a  .F?q.....N.55.kJ
-000016f0: f4e4 8bce 8b78 c1eb b935 026b 6633 bfc2  .....x...5.kf3..
-00001700: 726d d72c 73be 9025 c192 c42e 7ccd ed38  rm.,s..%....|..8
-00001710: 3c85 816c aa93 594d 0db3 9ab6 c1a3 bf8a  <..l..YM........
-00001720: 24b2 3bca a08a a500 6bb9 3ef9 70ce 9025  $.;.....k.>.p..%
-00001730: c192 c44e 7c5d ed32 3d85 516c a913 484d  ...N|].2=.Ql..HM
-00001740: 0d90 9a12 0aa9 9aba 4ae2 8dfd 3690 b346  ........J...6..F
-00001750: 5ccd 5446 5158 cd69 2a83 2896 044b 123b  \.TFQX.i*.(..K.;
-00001760: f135 b5db fc14 c6b1 ad4e 0435 3508 6a4a  .5.......N.55.jJ
-00001770: 0cc4 e3cd 6fd6 9aa4 f72b 4bcf dcdd 95f2  ....o....+K.....
-00001780: 5c35 f2d4 5e10 28cd 590a 5912 2c49 dc1c  \5..^.(.Y.Y.,I..
-00001790: 5fcb 9f61 b60a 93b0 ffee 7be5 d56e 96d7  _..a......{..n..
-000017a0: 7617 bb30 ca37 56bf 5b6e 97d7 72bf bcb6  v..0.7V.[n..r...
-000017b0: 5227 9f67 b5dc 30af e58e 792d b7cc 7bae  R'.g..0...y-..{.
-000017c0: 7be6 7518 a4c2 2036 d709 aba6 0656 4d09  {.u... 6.....VM.
-000017d0: 9554 3ddd c35e 91c7 d60f c18d e09a c94c  .T=..^.........L
-000017e0: abb0 a4f3 c0cd ac8a 25c1 92c4 4e7c 8d7d  ........%...N|.}
-000017f0: c210 1506 b3c1 4e58 3535 b06a 4ae8 a4f6  ......NX55.jJ...
-00001800: 259d d55b 6656 2c05 add5 4ede 8199 5bb1  %..[fV,...N...[.
-00001810: 2458 92d8 95af cfdd 66a9 308e 2d76 e2ab  $X......f.0.-v..
-00001820: a9c1 57d3 e7b8 386a d6c8 5233 9c89 566b  ..W...8j..R3..Vk
-00001830: ed93 0d67 b2c5 9260 4962 57be 863f c764  ...g...`IbW..?.d
-00001840: 1566 61fb 9db0 eba5 815d 2f09 b9d0 a236  .fa......]/....6
-00001850: 8d00 e334 4b01 9671 1db6 3967 c892 6049  ...4K..q..9g..`I
-00001860: 6227 be37 3ef5 1c9c c200 bee5 29c3 adfe  b'.7>.......)...
-00001870: 6ead 7551 0def f262 1bad f4bb 285f c5e9  n.uQ...b....(_..
-00001880: ae97 e8db 32e2 fcc5 cbf2 1c2d 8f57 ebe3  ....2......-.W..
-00001890: 1f45 b67d 7d36 38eb dd64 4591 6d0e ff5d  .E.}}68..dE.m..]
-000018a0: eb68 a9f3 ea09 a57e 9b65 c5f1 8faa cc5d  .h.....~.e.....]
-000018b0: 967f 3d14 b9fc 3f50 4b03 0414 0000 0008  ..=...?PK.......
-000018c0: 0018 49f9 5691 02f1 6cc4 0e00 006f 8b00  ..I.V...l....o..
-000018d0: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-000018e0: 7473 2f73 6865 6574 332e 786d 6cad 9d5b  ts/sheet3.xml..[
-000018f0: 779b 4816 85ff 8a96 9fa6 5f62 ebe6 24bd  w.H......._b..$.
-00001900: 1caf 1549 405d ba92 2cbb 67fa 194b 659b  ...I@]..,.g..Ke.
-00001910: 892c d480 dac9 fcfa 01f9 0212 7caa 80fc  .,..........|...
-00001920: 14db 9ff7 a9aa 533b 086f 04ba 788c 93ef  ......S;.o..x...
-00001930: e9bd b559 efc7 c372 957e 3ab9 cfb2 f5ef  ...Y...r.~:.....
-00001940: a7a7 e9fc de3e 84e9 bb78 6d57 39b9 8d93  .....>...xmW9...
-00001950: 8730 cbbf 4dee 4ed3 7562 c3c5 56f4 b03c  .0..M.N.ub..V..<
-00001960: 1d9c 9d9d 9f3e 84d1 eae4 f262 fbb3 6fc9  .....>.....b..o.
-00001970: e545 bcc9 96d1 ca7e 4b7a e9e6 e121 4c7e  .E.....~Kz...!L~
-00001980: 4eec 327e fc74 d23f 79f9 c155 7477 9f6d  N.2~.t.?y..Utw.m
-00001990: 7f70 7a79 b10e efec b5cd febd ce05 f9b7  .pzy............
-000019a0: a7af 7516 d183 5da5 51bc ea25 f6f6 d3c9  ..u...].Q..%....
-000019b0: e7fe ef5f ce07 5bc9 f657 fe13 d9c7 b4f2  ..._..[..W......
-000019c0: 75af 58cd 4d1c 7f2f be91 8b4f 2767 c5a4  u.X.M../...O'g..
-000019d0: ecd2 ceb3 a246 98ff f38f 9dda e5b2 2895  .....F........(.
-000019e0: 4fe5 efe7 aa27 e5a8 85b2 faf5 4b79 7fdb  O....'......Ky..
-000019f0: 807c 7e37 616a a7f1 f2af 6891 dd7f 3af9  .|~7aj....h...:.
-00001a00: 70d2 5bd8 db70 b3cc aee2 4761 9f17 352e  p.[..p....Ga..5.
-00001a10: a738 0bb3 f0f2 2289 1f7b 49b1 dacb 8b79  .8...."..{I....y
-00001a20: f145 3164 fe8b d1aa e8d2 7596 e43f 8ff2  .E1d......u..?..
-00001a30: 91b2 cbe2 d77b 265e d865 6f66 6fa3 5554  .....{&^.eofo.UT
-00001a40: 4cfc e234 cba7 54fc c2e9 fcb9 c064 bf40  L..4..T......d.@
-00001a50: 31e0 964c 91cc 9078 487c 2401 1241 8bbb  1..L...xH|$..A..
-00001a60: cec2 cc36 2c46 6229 8544 d320 7a15 3f2e  ...6,Fb).D. z.?.
-00001a70: ede2 cee6 dbfd f726 4ab7 1dec 2de3 bb86  .......&J...-...
-00001a80: 81ff c0f2 06c9 9726 729a 6ff0 eb2e 0f5e  .......&r.o....^
-00001a90: 7779 0073 9c2e c334 6dda 5512 7c4b f2ff  wy.s...4m.U.|K..
-00001aa0: 8749 f6b3 4133 25cd 97f0 a1a9 d933 fafd  .I..A3%......3..
-00001ab0: 994d e749 b406 c379 24fb f3e7 ba69 189f  .M.I...y$....i..
-00001ac0: 7edf 44ab de34 deac b206 5180 a2f0 078a  ~.D..4....Q.....
-00001ad0: 042f 283f 50cd 73cb 2d9a 3ce7 5215 ae99  ./(?P.s.-.<.R...
-00001ae0: 35fb 5591 f6ca ae97 e1dc 2e7a 93a6 9dd2  5.U........z....
-00001af0: 24bb 8e37 c9bc 69a0 3f0e 2b7a de2a 8bb2  $..7..i.?.+z.*..
-00001b00: 9f3d d869 c3dd cce6 f70d 822f e8d7 f821  .=.i......./...!
-00001b10: 3f0e ef35 7fc7 f3c3 57cf 0fe9 3fce 649f  ?..5....W...?.d.
-00001b20: bc54 bf0f d3e9 cc1f ceb6 87bd 2687 63c9  .T..........&.c.
-00001b30: 1912 0f89 8f24 4022 9048 240a 89c6 46e4  .....$@".H$...F.
-00001b40: 2fbd 69fe dafb fdee dd3c becb 8ffd f65d  /.i......<.....]
-00001b50: 189d 3e46 abc5 6993 39ba f6d3 90d0 fec8  ..>F..i.9.......
-00001b60: 5f21 9b7c d1b4 949d ed1f bd6e ff08 b77f  _!.|.......n....
-00001b70: 9fec 4eb7 78e1 fb9a dc85 abe8 7fdb ff7b  ..N.x..........{
-00001b80: 5736 dd7a 1c0e 2f53 1c67 86c4 43e2 2309  W6.z../S.g..C.#.
-00001b90: 9008 2412 8942 a2b1 3bed 3cf1 a64d 3654  ..$..B..;.<..M6T
-00001ba0: 0d8d d2b4 be1d a38c 5f8d 3246 a3ec 93fa  ........_.2F....
-00001bb0: 1af2 73c5 264f 60c9 1912 0f89 8f24 4022  ..s.&O`......$@"
-00001bc0: 9048 240a 89c6 46b4 f344 d77e 1a12 e2f6  .H$...F..D.~....
-00001bd0: 372d 6567 fbcf 5fb7 ff1c b77f 9f34 4c37  7-eg.._......4L7
-00001be0: 8b93 fc2f 06d7 2102 8798 21f1 90f8 4802  .../..!...!...H.
-00001bf0: 2402 8944 a290 686c 4c3b 3bbc 557f 0d15  $..D..hlL;;.U...
-00001c00: 427b 342d 6dc7 1eef 5fed f11e edb1 4f76  B{4-m..._.....Ov
-00001c10: a7ef fd53 3b4f 7932 0316 9c21 f190 f848  ...S;Oy2...!...H
-00001c20: 0224 0289 44a2 9068 6c43 3b33 74eb a621  .$..D..hlC;3t..!
-00001c30: 196e 7dd3 4276 b6fe c3eb d67f c0ad df27  .n}.Bv.........'
-00001c40: bb93 f5a3 65e3 6100 ebcd 9078 487c 2401  ....e.a....xH|$.
-00001c50: 1281 4422 5148 3476 a1dd ce77 6aa6 2115  ..D"QH4v...wj.!.
-00001c60: 6e7c d33a 7636 fee3 ebc6 7fc4 8ddf 27bb  n|.:v6........'.
-00001c70: 73fd 23bc 69fe bb01 0bce 9078 487c 2401  s.#.i......xH|$.
-00001c80: 1281 4422 5148 34b6 a1dd ce77 eba6 2119  ..D"QH4....w..!.
-00001c90: 6e7d d342 76b6 be7f 56e6 6167 b8f9 35b4  n}.Bv...V.ag..5.
-00001ca0: 3bdf 2bbb dc9e cba6 f7d1 bac9 045c 79c6  ;.+..........\y.
-00001cb0: c863 e433 0a18 0946 9291 62a4 b92d eddc  .c.3...F..b..-..
-00001cc0: 705c 7b0d cad1 168d 6bda f545 2527 c51c  p\{.....k..E%'..
-00001cd0: 6e52 43fb 133f 7c76 c895 678c 3c46 3ea3  nRC..?|v..g.<F>.
-00001ce0: 8091 6024 1929 469a dbd2 d217 47b5 d7a0  ..`$.)F.....G...
-00001cf0: 9c7d e10c 56fb 65b2 dadf 8faa 2abe a014  .}..V.e.....*...
-00001d00: eb69 e27f 460f f6da 2651 b329 b0ec 8c91  .i..F...&Q.)....
-00001d10: c7c8 6714 3012 8c24 23c5 4873 4f5a 9aa2  ..g.0..$#.HsOZ..
-00001d20: 7b6f 0d6a d911 4d0b da75 4499 3bf6 3978  {o.j..M..uD.;.9x
-00001d30: aca1 caac 8bbf 77be 25f1 62d3 3885 2957  ......w.%.b.8.)W
-00001d40: 9d31 f218 f98c 0246 8291 64a4 1869 6e49  .1.....F..d..inI
-00001d50: 4b43 746e ad41 29fb c199 43f6 cb20 b2cf  KCtn.A)...C.. ..
-00001d60: 4964 0d55 26fd 2d7e b4c9 349b 6e92 7fac  Id.U&.-~..4.n...
-00001d70: b159 b8c8 17d1 680c 0e20 1979 8c7c 4601  .Y....h.. .y.|F.
-00001d80: 23c1 4832 528c 34f7 a6a5 318e efb1 c11a  #.H2R.4...1.....
-00001d90: ec10 6700 d92f 13c8 3e47 9035 5499 fd5f  ..g../..>G.5T.._
-00001da0: f992 ffdc 2437 3999 de87 493e 93fc 8897  ....$79...I>....
-00001db0: 66d1 bcd1 269c 4932 f218 f98c 0246 8291  f...&.I2.....F..
-00001dc0: 64a4 1869 6e50 4b9b bc51 a30d 1662 af38  d..inPK..Q...b.8
-00001dd0: d3ca 7e19 57f6 39af aca1 e625 b85e 6838  ..~.W.9....%.^h8
-00001de0: ad64 e431 f219 058c 0423 c948 31d2 dc9d  .d.1.....#.H1...
-00001df0: 9646 798b 2e1b acc2 2e71 8696 fd32 b5ec  .Fy......q...2..
-00001e00: 736c 5943 2f23 4795 8b75 5f6f 1bad c1d9  slYC/#G..u_o....
-00001e10: 2523 8f91 cf28 6024 1849 468a 91c6 96b4  %#...(`$.IF.....
-00001e20: b546 e7d6 1a94 b21f 9c49 66bf 8c32 fb9c  .F.......If..2..
-00001e30: 65d6 d0ce a40f 5da8 0393 70cc c9c8 63e4  e.....]...p...c.
-00001e40: 330a 1809 4692 9162 a4b1 4f6d 4df2 b6fd  3...F..b..OmM...
-00001e50: 3658 8f9d e38c 42fb 6516 dae7 30b4 866a  6X....B.e...0..j
-00001e60: 2bb9 b619 9884 1351 461e 239f 51c0 4830  +......QF.#.Q.H0
-00001e70: 928c 1423 8d2d 696b 92ce ad35 2865 3f38  ...#.-ik...5(e?8
-00001e80: f3d1 4199 8f0e 381f ada1 faa4 ebd7 f39a  ..A...8.........
-00001e90: fdc1 a3cc 1879 8c7c 4601 23c1 4832 528c  .....y.|F.#.H2R.
-00001ea0: 34b6 a8a5 3fde aed5 064b a15f 1ad7 b7eb  4...?....K._....
-00001eb0: 9732 371d 706e 5a43 3b8b d85e f203 7770  .27.pnZC;..^..wp
-00001ec0: 62ca c863 e433 0a18 0946 9291 62a4 b121  b..c.3...F..b..!
-00001ed0: 6ddd d1b1 b106 85ec 05f7 9b50 2bef 42e5  m..........P+.B.
-00001ee0: acb4 8676 a65c 5c04 042b 704e cac8 63e4  ...v.\\..+pN..c.
-00001ef0: 330a 1809 4692 9162 a4b1 1f6d add0 adaf  3...F..b...m....
-00001f00: 0675 ec04 6746 3a28 33d2 0167 a435 b433  .u..gF:(3..g.5.3
-00001f10: e3ed 4541 b002 27a4 8c3c 463e a380 9160  ..EA..'..<F>...`
-00001f20: 2419 2946 1a1b d2d6 0a1d 1b6b 50c8 5e70  $.)F.......kP.^p
-00001f30: e6a3 8332 1f1d 703e 5a43 3b53 ae5e 1104  ...2..p>ZC;S.^..
-00001f40: 4b70 36ca c863 e433 0a18 0946 9291 62a4  Kp6..c.3...F..b.
-00001f50: b12f 6d2d 715c 7f0d ead9 19ce 5c74 50e6  ./m-q\......\tP.
-00001f60: a203 ce45 6b68 6fe6 ce13 4c8e 4319 798c  ...Ekho...L.C.y.
-00001f70: 7c46 0123 c148 3252 8c34 f6a5 ad33 8eeb  |F.#.H2R.4...3..
-00001f80: af41 3d3b c399 820e ca14 74c0 2968 0ded  .A=;......t.)h..
-00001f90: ccfc f5c2 20d8 82c3 4f46 1e23 9f51 c048  .... ...OF.#.Q.H
-00001fa0: 3092 8c14 238d 4d69 6b8b 239a 6b50 cc9e  0...#.Mik.#.kP..
-00001fb0: 7066 9e83 32f3 1c70 e659 43e5 b42b 392d  pf..2..p.YC..+9-
-00001fc0: 5882 434f 461e 239f 51c0 4830 928c 1423  X.COF.#.Q.H0...#
-00001fd0: 8d3d 696b 89ee bd35 a865 4738 53cf 4199  .=ik...5.eG8S.A.
-00001fe0: 7a0e 38f5 aca1 72d6 78b5 07fc c179 2723  z.8...r.x....y'#
-00001ff0: 8f91 cf28 6024 1849 468a 91c6 0eb5 f5c7  ...(`$.IF.......
-00002000: 5b75 da60 2576 8b33 e91c 9449 e780 93ce  [u.`%v.3...I....
-00002010: 1a6a 5c83 fb50 c2a9 2723 8f91 cf28 6024  .j\..P..'#...(`$
-00002020: 1849 468a 91c6 f6b4 b5ca 9bb4 d960 19f6  .IF..........`..
-00002030: 8933 011d 9609 e890 02b3 cf69 da78 fbca  .3.........i.x..
-00002040: 0415 db57 cdad acd9 3028 9469 2f57 f6b6  ...W....0(.i/W..
-00002050: d25e a376 86da abe2 bed2 d4ae b2b4 973c  .^.v...........<
-00002060: 9fe1 f76e 6cf6 68ed aa17 56ca fe6b 1117  ...nl.h...V..k..
-00002070: 77d3 f7c2 bb55 5cfc a7ec c537 ffb5 f3ec  w....U\....7....
-00002080: b75e b85a f49e 59ba b6f3 e8f6 95f5 fe95  .^.Z..Y.........
-00002090: 6ee6 f7bd 30ed 15fb d57b deb0 dfde 35dd  n...0....{....5.
-000020a0: c68b f3ab 6c75 d3ed bc35 5de9 7946 8291  ....lu...5].yF..
-000020b0: 64a4 1869 9c7e db7b 273b 7ac3 a090 6f9e  d..i.~.{';z...o.
-000020c0: 74e6 b6c3 32b7 1d52 14f8 f947 94c2 7b2d  t...2..R...G..{-
-000020d0: 2728 8ad2 1719 189d 135d 461e 0ee7 b210  '(.......]F.....
-000020e0: c7bd 8c04 23c9 4831 d238 fdb6 16ea d875  ....#.H1.8.....u
-000020f0: 8342 b690 33ee 1d96 71ef 9032 c4e7 775c  .B..3...q..2..w\
-00002100: 353a 0873 cf30 9d66 9368 d5f4 b482 694d  5:.s.0.f.h....iM
-00002110: 55b1 0fa7 c038 569a 25d1 aae9 310d 3e57  U....8V.%...1.>W
-00002120: 0b18 0946 9291 62a4 b94b 2d9d d3a5 db06  ...F..b..K-.....
-00002130: 556c 1b67 363c acdc b74f 71e3 21db 70b6  Ul.g6<...Oq.!.p.
-00002140: 593d c97c 2a00 87a0 0337 f71f b8bb 9f06  Y=.|*....7......
-00002150: 761d 820e dcfc 7fe0 eeff 03b7 ff1f b8ff  v...............
-00002160: ffc0 0300 deea 0900 47f7 df60 0976 9533  ........G..`.v.3
-00002170: 651e 9629 f390 a24a e94d f129 2828 8ad2  e..)...J.M.)((..
-00002180: 1719 9889 8367 461e 0ee7 3213 a7d2 8c04  .....gF...2.....
-00002190: 23c9 4831 d238 fdb6 66ea d875 8342 b690  #.H1.8..f..u.B..
-000021a0: 338e 1e96 71f4 9032 4db9 4ab3 70f9 742a  3...q..2M.J.p.t*
-000021b0: 8da7 461c a8ee cbc1 529c 5833 f270 5897  ..F.....R.X3.pX.
-000021c0: a538 ce66 2418 4946 8a91 c6e9 b7b5 d491  .8.f$.IF........
-000021d0: dd37 5880 ade5 ccb3 8765 9e3d a468 f4cb  .7X......e.=.h..
-000021e0: e6e1 c626 5f6f 27cb 7061 9b8f 511c c9ee  ...&_o'.pa..Q...
-000021f0: 8ac1 569c 7833 f270 5097 ad38 0e67 2418  ..V.x3.pP..8.g$.
-00002200: 4946 8a91 c6e9 b7b5 d551 bd37 2867 5339  IF.......Q.7(gS9
-00002210: 03f1 6119 880f 295d 7dba ed01 cfa5 0edc  ..a...)]}.......
-00002220: 8abf 55e2 5938 27e5 8c3c 1cee c059 3827  ..U.Y8'..<...Y8'
-00002230: e88c 0423 c948 31d2 dca8 962e ead8 7083  ...#.H1.......p.
-00002240: 42f6 8f33 3e1f 96f1 f990 f256 877f 7e29  B..3>......V..~)
-00002250: f02d 6bc0 7189 6375 461e 8eed 3a2e 71e6  .-k.q.cuF...:.q.
-00002260: ce48 3092 8c14 238d d36f eba8 b7d8 0283  .H0...#..o......
-00002270: 55d8 5ece bc7d 58e6 ed43 8a69 afe2 2c4e  U.^..}X..C.i..,N
-00002280: be26 915d 6521 3d75 12c5 51ba 2f07 7f71  .&.]e!=u..Q./..q
-00002290: 16cf c8c3 615d fee2 a09e 9160 2419 2946  ....a].....`$.)F
-000022a0: 1aa7 dfd6 5f47 76df 6001 b696 33a2 1f95  ...._Gv.`...3...
-000022b0: 11fd 08b3 ef62 7674 8a8e aae7 55f1 b979  .....bvt....U..y
-000022c0: 4d59 9a89 9187 e339 ccc4 2503 4682 9164  MY.....9..%.F..d
-000022d0: a418 699c 7edb 27c5 756d bb41 253f 16ce  ..i.~.'.um.A%?..
-000022e0: 1981 8fca 087c 848f 8fb5 7f6f ecaa f141  .....|.....o...A
-000022f0: 9913 146d f3fc 1725 d888 5370 461e 8ef8  ...m...%..SpF...
-00002300: e5fc c3cd 7c7c 3e1f cedf cf07 a3f9 87c1  ....||>.........
-00002310: c7db f9e2 f6fd edcd 87f1 f06c 71f3 f17d  ...........lq..}
-00002320: a3b9 381b 6724 1849 468a 91c6 45b5 3557  ..8.g$.IF...E.5W
-00002330: f7ed 30a8 657b 39e3 f151 198f 8f28 46bd  ..0.e{9..Q...(F.
-00002340: deac d771 92e5 3fda ccb3 4d42 4fb6 9860  ...q..?...MBO..`
-00002350: 8128 6d2a 019e e3e8 9c91 8743 bb0e 5d9c  .(m*.......C..].
-00002360: 9f33 128c 2423 c548 e3f4 dbba eb0d 76c0  .3..$#.H......v.
-00002370: 6011 b699 334e 1f95 71fa a85b 423d 415d  `...3N..q..[B=A]
-00002380: fe57 c981 6b80 d39a ae62 28ce d171 b403  .W..k....b(..q..
-00002390: 43f9 5c2f 6024 1849 468a 91e6 4eb5 7453  C.\/`$.IF...N.tS
-000023a0: b78e 1bd4 b181 dccf d1ad 3c48 b75b 2a3d  ..........<H.[*=
-000023b0: 41dd d323 5ae8 dd12 d39a ae62 a003 8fd4  A..#Z......b....
-000023c0: a5d1 681c 9f8b 058c 0423 c948 31d2 dca6  ..h......#.H1...
-000023d0: 96ee e9d6 6e83 3a76 8f33 341f 95a1 f9a8  ....n.:v.34.....
-000023e0: 5b00 3d41 5db1 9c4d 2657 d76b dbf8 3cf5  [.=A]..M&W.k..<.
-000023f0: 694d 59f1 0f07 e538 deed 320e 9bfd c311  iMY....8..2.....
-00002400: 3923 c148 3252 8c34 37aa a57f ba36 dca0  9#.H2R.47....6..
-00002410: 921d e4cc c647 6536 3eea 9635 4f50 f7b4  .....Ge6>..5OP..
-00002420: a0af 9b8c 2dc4 a138 230f 0764 0b71 1cce  ....-..8#..d.q..
-00002430: 4830 928c 1423 cd9d 6a69 a1ce 1d37 2865  H0...#..ji...7(e
-00002440: 0f39 a3f0 5119 858f 2829 7579 e840 343b  .9..Q...()uy.@4;
-00002450: 8bc2 079b d9a4 d140 1c85 33f2 7034 3610  .......@..3.p46.
-00002460: 27e1 8c04 23c9 4831 d2dc a696 06ea d66e  '...#.H1.......n
-00002470: 833a 768f 3308 1f95 41f8 a85b aa3c 415d  .:v.3...A..[.<A]
-00002480: be1c ef47 be96 55b8 94cd 0720 4ebf 1979  ...G..U.... N..y
-00002490: 385e 8a97 52b8 5ac0 4830 928c 1423 cd9d  8^..R.Z.H0...#..
-000024a0: 6a69 a0ae 1d37 a864 0b39 c3ee 5119 768f  ji...7.d.9..Q.v.
-000024b0: ba05 c713 d4e5 0b12 9b9b a70f 7a6a 7410  ............zjt.
-000024c0: e7db 8c3c 1c8e 8f40 9c6c 3312 8c24 23c5  ...<...@.l3..$#.
-000024d0: 4873 9f5a 1aa8 63bf 0d0a d93f ce44 7b5c  Hs.Z..c....?.D{\
-000024e0: 26da e36e 59f1 0475 f97a 0ebc f369 5ad3  &..nY..u.z...iZ.
-000024f0: 95f6 61e4 e168 0786 f2b9 5ec0 4830 928c  ..a..h....^.H0..
-00002500: 1423 cd9d 6af9 2117 dd3a 6e50 c71f 72e1  .#..j.!..:nP..r.
-00002510: 0cb3 c765 983d eef6 5ee9 09ea 8ae5 b8df  ...e.=..^.......
-00002520: f734 ade9 2b46 e24c 1b47 fd85 217d ae1b  .4..+F.L.G..!}..
-00002530: 3012 8c24 23c5 4873 e75a 1aea b81d 30a8  0..$#.Hs.Z....0.
-00002540: 6763 3963 ec71 1963 8fbb 45c1 13d4 e5cb  gc9c.q.c..E.....
-00002550: 32e1 8feb 78b3 5a6c af50 37ba 8a53 6b46  2...x.Zl.P7..SkF
-00002560: 1e0e 89af 6e5c 2c60 2418 4946 8a91 e65e  ....n\,`$.IF...^
-00002570: b5b4 d211 3d37 2866 1f39 73ea 7199 538f  ....=7(f.9s.q.S.
-00002580: 3be6 d4a8 cbd7 e47c f7dc b4a6 ae18 89d3  ;......|........
-00002590: 6a1c d339 a0cf 5503 4682 9164 a418 69ee  j..9..U.F..d..i.
-000025a0: 5a4b 471d d37d 836a b694 33b9 1e97 c9f5  ZKG..}.j..3.....
-000025b0: b863 728d ba7c 5157 c5c7 38f2 7189 b36b  .cr..|QW..8.q..k
-000025c0: 461e 8ec7 c725 ceae 1909 4692 9162 a4b9  F....%....F..b..
-000025d0: 512d 5dd4 b5e1 0695 ec20 f747 c355 3e1b  Q-]...... .G.U>.
-000025e0: ae63 7a8d ba62 41ee b737 4d6b fa8a 8f0e  .cz..bA..7Mk....
-000025f0: 7c84 1c8d fa0b 43fa 5c37 6024 1849 468a  |.....C.\7`$.IF.
-00002600: 91e6 ceb5 b4d4 713b 6050 cfc6 7286 dae3  ......q;`P..r...
-00002610: 32d4 1e77 0cb5 51f7 b22c 3c0f e748 9b91  2..w..Q..,<..H..
-00002620: 87c3 1d1a cbe7 8201 23c1 4832 528c 34f7  ........#.H2R.4.
-00002630: aaa5 953a f6dc a090 3de4 0cb5 c765 a83d  ...:....=....e.=
-00002640: ee18 6aa3 2e5f cf2f bef7 645a ab51 b113  ..j.._./..dZ.Q..
-00002650: 07dc 38f2 2f0e eb73 ed80 9160 2419 2946  ..8./..s...`$.)F
-00002660: 9a3b d8d2 59c7 ef84 c11a 6c32 67f6 3d2e  .;..Y.....l2g.=.
-00002670: b3ef 71c7 ec1b 75c5 d21e ed3a fb9c d8c6  ..q...u....:....
-00002680: cfb3 a809 2bce e2e8 1b87 e353 284e be19  ....+......S(N..
-00002690: 0946 9291 62a4 b94f 2dad d4b1 df06 85ec  .F..b..O-.......
-000026a0: 1f67 f03d 2e83 ef71 c7e0 1b75 7b9f c780  .g.=...q...u{...
-000026b0: f704 4f6b 152a 46e2 041c c7e5 917c 2e17  ..Ok.*F......|..
-000026c0: 3012 8c24 23c5 4873 cb5a 5ae9 d8d6 1bac  0..$#.Hs.ZZ.....
-000026d0: c09e 7286 e1e7 6518 7ede 310c 47dd eec2  ..r...e.~.1.G...
-000026e0: 0e7d da4e ad44 692a 461e 239f 51c0 4830  .}.N.Di*F.#.Q.H0
-000026f0: 928c 1423 cdad 69f9 99be 47b7 d860 09fe  ...#..i...G..`..
-00002700: 385f 6710 7e5e 06e1 e71d 8370 d4ed ad0c  8_g.~^.....p....
-00002710: 3eeb 7e5a d357 9cc3 4138 8e9a e225 5dae  >.~Z.W..A8...%].
-00002720: 1630 128c 2423 c548 73bf 5a3a eab8 be1b  .0..$#.Hs.Z:....
-00002730: d4b3 9d9c f1f7 7919 7f9f 778c bf51 b7bb  ......y...w..Q..
-00002740: ac83 b7da 4d6b 452a 9ee2 181c 873e 3898  ....MkE*.....>8.
-00002750: cf15 0346 8291 64a4 1869 6e5c 4b5f bdc1  ...F..d..in\K_..
-00002760: 0618 2cc2 e6e2 4cfc 34bd b736 2b1e 6f76  ..,...L.4..6+.ov
-00002770: 79b1 0eef ac09 93bb 6895 f696 f636 579c  y.......h....6W.
-00002780: bd7b 3f3e e925 c5f5 e797 6fb2 78fd e924  .{?>.%....o.x..$
-00002790: 37eb 4d9c 65f1 c3f6 cb7b 1b2e 6c52 fc42  7.M.e....{..lR.B
-000027a0: ce6f e338 7bfd a618 e631 4ebe 6f07 b9fc  .o.8{....1N.o...
-000027b0: 3f50 4b03 0414 0000 0008 0018 49f9 56f7  ?PK.........I.V.
-000027c0: f68f 09a7 0200 006d 0b00 000d 0000 0078  .......m.......x
-000027d0: 6c2f 7374 796c 6573 2e78 6d6c dd56 db8e  l/styles.xml.V..
-000027e0: 9b30 10fd 15c4 0794 4d50 51a8 42a4 36d2  .0......MPQ.B.6.
-000027f0: 4a95 da6a a5dd 87be 9a60 8225 5fa8 31ab  J..j.....`.%_.1.
-00002800: 64bf be33 b613 92ec 0edd f6b1 a084 f11c  d..3............
-00002810: 9fb9 3b64 3db8 a3e4 8f1d e72e 3928 a987  ..;d=.......9(..
-00002820: 2aed 9ceb 3f65 d9b0 ebb8 62c3 07d3 730d  *...?e....b...s.
-00002830: 486b ac62 0e96 769f 0dbd e5ac 1990 a464  Hk.b..v........d
-00002840: b6bc bb2b 32c5 844e 376b 3daa 7be5 8664  ...+2..N7k=.{..d
-00002850: 6746 edaa f42e 4db2 cdba 357a 522d d3a0  gF....M...5zR-..
-00002860: 80bd 4cf1 e499 c92a dd32 296a 2bc2 66a6  ..L....*.2)j+.f.
-00002870: 843c 06fd d26b 7646 1a9b 3888 8657 e9c2  .<...kvF..8..W..
-00002880: ab86 97b0 6111 9718 6ab4 a584 36d6 6bb3  ....a...j...6.k.
-00002890: e026 7cd7 9170 89f8 c700 3b84 94d7 f181  .&|..p....;.....
-000028a0: 62b3 ee99 73dc ea7b 5804 92d7 bec6 a2fc  b...s..{X.......
-000028b0: 74ec 21be bd65 c7c5 f263 7ac1 f00f 7053  t.!..e...cz...pS
-000028c0: 1bdb 707b e528 a836 6bc9 5b87 0c2b f69d  ..p{.(.6k.[..+..
-000028d0: 179c e9f1 511b e78c 42a9 116c 6f34 0b91  ....Q...B..lo4..
-000028e0: 9c68 5774 dfc8 2a75 1d34 62b2 75ab 45c3  .hWt..*u.4b.u.E.
-000028f0: b7ba e8e5 567d 7613 0548 61c7 a57c c46d  ....V}v..Ha..|.m
-00002900: 3fdb 731e 0bc8 e3d0 26a1 f35f 1bdf 742c  ?.s.....&.._..t,
-00002910: ec49 84e4 a318 ccc4 053a b834 178c 5fd8  .I.......:.4.._.
-00002920: 5dfe 9bdd 5e3c 1bf7 6584 8cb4 5fff 1a8d  ]...^<..e..._...
-00002930: e30f 96b7 e2e0 d787 760a 8032 bf20 cc83  ........v..2. ..
-00002940: 9ef5 bd3c 7e96 62af 150f d9bf dbe3 66cd  ...<~.b.......f.
-00002950: 4ebc a433 56bc 8037 9cc9 1d28 388c ec33  N..3V..7...(8..3
-00002960: b74e ec50 034d 0a05 3ab4 b14a e702 f972  .N.P.M..:..J...r
-00002970: 5dd5 feac 4df0 4055 e90f 3ca8 f222 d17a  ]...M.@U..<..".z
-00002980: 14d2 091d 579d 681a ae5f b700 ec3b 56c3  ....W.h.._...;V.
-00002990: 4fc1 9503 d8d5 f096 8dd2 3d9d c12a 9de4  O.........=..*..
-000029a0: efbc 11a3 2acf bb1e b016 71d7 247f c351  ....*.....q.$..Q
-000029b0: 5c14 d369 0667 4237 fcc0 9b6d 5cda 7ded  \..i.gB7...m\.}.
-000029c0: c504 0470 1baf 30c8 37d0 bdbf 0888 6405  ...p..0.7.....d.
-000029d0: 9080 1024 7d91 6190 acc0 237d fd8f 79ad  ...$}.a...#}..y.
-000029e0: e8bc 0248 46b8 7a1b 5ad1 ac15 cd0a bc37  ...HF.z.Z......7
-000029f0: a1ad bf49 5f04 ab84 8b48 b92c f3bc 28c8  ...I_....H.,..(.
-00002a00: f26e b76f 87b1 256b 5814 f821 0c92 1122  .n.o..%kX..!..."
-00002a10: 87f4 85de feb6 f233 0330 3336 7f98 0db2  .......3.036....
-00002a20: cbb3 6343 a63c 33a2 64ca 3395 4788 a821  ..cC.<3.d.3.G..!
-00002a30: 72ca 9218 00d2 1772 c8a6 9013 8541 10be  r......r.....A..
-00002a40: 70d4 0856 9e63 9fc9 08c9 633e 0395 2509  p..V.c....c>..%.
-00002a50: e190 12d3 5b14 54a1 0abc 897e 9187 28cf  ....[.T....~..(.
-00002a60: cb92 8010 24c2 c873 12c2 033b 0391 6160  ....$..s...;..a`
-00002a70: 2024 94e7 e145 7af3 3ecb 4eef b96c fa83   $...Ez.>.N..l..
-00002a80: bdf9 0d50 4b03 0414 0000 0008 0018 49f9  ...PK.........I.
-00002a90: 56b7 47eb 8ac0 0000 0016 0200 000b 0000  V.G.............
-00002aa0: 005f 7265 6c73 2f2e 7265 6c73 9d92 4b6e  ._rels/.rels..Kn
-00002ab0: 0231 0c40 af12 655f 4ca9 c402 31ac d8b0  .1.@..e_L...1...
-00002ac0: 4388 0bb8 89e7 a399 c491 63c4 f4f6 8dd8  C.........c.....
-00002ad0: c020 6811 4bff 9e9e 2daf 0f34 a076 1c73  . h.K...-..4.v.s
-00002ae0: dba5 6cc6 30c4 5cd9 5635 ad00 b26b 2960  ..l.0.\.V5...k)`
-00002af0: 9e71 a258 2a35 4b40 2da1 3490 d0f5 d810  .q.X*5K@-.4.....
-00002b00: 2ce6 f325 c82d c36e d6b7 4c73 fc49 f40a  ,..%.-.n..Ls.I..
-00002b10: 91eb ba73 b465 770a 14f5 01f8 aec3 9a23  ...s.ew........#
-00002b20: 4a43 5ad9 7180 334b ffcd dccf 0ad4 9a9d  JCZ.q.3K........
-00002b30: afac ecfc a735 f0a6 ccf3 f520 90a2 4745  .....5..... ..GE
-00002b40: 702c f491 a44c 8b76 94af 3e9e ddbe a4f3  p,...L.v..>.....
-00002b50: a563 62b4 78df e8ff f3d0 a814 3df9 bf9d  .cb.x.......=...
-00002b60: 30a5 89d2 d745 0926 6fb0 f905 504b 0304  0....E.&o...PK..
-00002b70: 1400 0000 0800 1849 f956 b948 9c76 5201  .......I.V.H.vR.
-00002b80: 0000 ae02 0000 0f00 0000 786c 2f77 6f72  ..........xl/wor
-00002b90: 6b62 6f6f 6b2e 786d 6c8d 91dd 4e83 4010  kbook.xml...N.@.
-00002ba0: 855f 85ec 0308 a5da c4a6 f4a6 8dda c4bf  ._..............
-00002bb0: 58e3 fd00 4399 747f c8ee d06a 9fde 5d08  X...C.t....j..].
-00002bc0: 8a69 d278 b5cc 99d9 8f39 6717 4763 f7b9  .i.x.....9g.Gc..
-00002bd0: 31fb e853 49ed e636 1335 7333 8f63 57d4  1..SI..6.5s3.cW.
-00002be0: a8c0 5d99 06b5 ef55 c62a 605f da5d 6caa  ..]....U.*`_.]l.
-00002bf0: 8a0a 5c9b a255 a839 4e93 6416 5b94 c064  ..\..U.9N.d.[..d
-00002c00: b4ab a971 a2a7 fd87 e51a 8b50 ba1a 9195  ...q.......P....
-00002c10: ec51 0a48 8be5 62d8 ecd5 46f1 b832 8c45  .Q.H..b...F..2.E
-00002c20: f853 5083 f241 7874 bf03 a18c 0ee4 2827  .SP..Axt......('
-00002c30: 49fc 9589 ee5b a288 1469 5274 c232 1389  I....[...iRt.2..
-00002c40: 885c 6d8e 0fc6 d2c9 6806 b92d ac91 3213  .\m.....h..-..2.
-00002c50: 93be f181 96a9 3893 b761 cd77 c85d a730  ......8..a.w.].0
-00002c60: e46f c173 2666 8907 5664 1d77 131d 1ffc  .o.s&f..Vd.w....
-00002c70: 9207 f4c3 7dd5 b2b9 23c9 68d7 c078 6f4d  ....}...#.h..xoM
-00002c80: db90 de75 186f 231e f9e8 a218 ce48 83c2  ...u.o#......H..
-00002c90: 4c3c 2143 090c 610b af6e ca7e 23f6 a891  L<!C..a..n.~#...
-00002ca0: 3f3b 27df b09b b287 8e01 2b09 cea1 1bdd  ?;'.......+.....
-00002cb0: 4f2f dc4f cfee fbd4 9b10 c91f c4f4 0262  O/.O...........b
-00002cc0: dafb 1acc 9458 91c6 f2d9 c35c 68f8 680b  .....X.....\h.h.
-00002cd0: ffae e1e8 cca4 d737 935b 1f61 2be5 ca6b  .......7.[.a+..k
-00002ce0: 2ffa d140 f993 cef0 b4cb 6f50 4b03 0414  /..@......oPK...
-00002cf0: 0000 0008 0018 49f9 560b 085d 06bc 0000  ......I.V..]....
-00002d00: 001f 0300 001a 0000 0078 6c2f 5f72 656c  .........xl/_rel
-00002d10: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
-00002d20: 656c 73cd 9339 0e83 3010 45af 62f9 000c  els..9..0.E.b...
-00002d30: 4b92 2282 5469 6823 2e60 c1b0 88c5 9667  K.".Tih#.`.....g
-00002d40: a2c0 ed83 a000 4b29 d2a0 a4b2 fe58 7eff  ......K).....X~.
-00002d50: 15e3 f881 9de2 460f 5437 86c4 d877 0325  ......F.T7...w.%
-00002d60: b266 3657 00ca 6bec 1579 dae0 30df 94da  .f6W..k..y..0...
-00002d70: f68a e768 2b30 2a6f 5585 10fa fe05 ec9e  ...h+0*oU.......
-00002d80: 216f f19e 29b2 c9e0 3744 5d96 4d8e 779d  !o..)...7D].M.w.
-00002d90: 3f7b 1cf8 0318 5eda b654 23b2 1499 b215  ?{....^..T#.....
-00002da0: 7222 61ec b631 c172 04de 4c96 222d 1269  r"a..1.r..L."-.i
-00002db0: d322 9002 7e6d 143a 46e1 1f18 458e 5174  ."..~m.:F...E.Qt
-00002dc0: a411 f1d4 216d 3a6b 76fa 4f47 f6f3 fc16  ....!m:kv.OG....
-00002dd0: b7fa 25ae 4377 51ce 8b04 38ff e1f6 0650  ..%.CwQ...8....P
-00002de0: 4b03 0414 0000 0008 0018 49f9 56db fbce  K.........I.V...
-00002df0: 8f24 0100 00e9 0400 0013 0000 005b 436f  .$...........[Co
-00002e00: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-00002e10: cd54 cb4e c330 10fc 95c8 d72a 7129 1207  .T.N.0.....*q)..
-00002e20: d4f4 025c a107 7ec0 249b c68a 5ff2 6e4b  ...\..~.$..._.nK
-00002e30: faf7 6c12 1a09 545a aa20 d14b ac78 6767  ..l...TZ. .K.xgg
-00002e40: c63b b297 affb 0098 b4d6 38cc 454d 14ee  .;........8.EM..
-00002e50: a5c4 a206 ab30 f301 1c57 2a1f ad22 fe8d  .....0...W*.."..
-00002e60: 1b19 54d1 a80d c8c5 7c7e 270b ef08 1ca5  ..T.....|~'.....
-00002e70: d471 88d5 f211 2ab5 3594 3cb5 bc8d dabb  .q....*.5.<.....
-00002e80: 5c44 3028 9287 01d8 69e5 4285 6074 a188  \D0(....i.B.`t..
-00002e90: eb72 e7ca 6f2a e9a7 42c6 9d3d 066b 1d70  .r..o*..B..=.k.p
-00002ea0: c600 91c8 a312 7de9 4785 43e3 cb0e 62d4  ......}.G.C...b.
-00002eb0: 2524 6b15 e959 5986 c9d6 48a4 bd01 cc4e  %$k..YY...H....N
-00002ec0: 731c 71e9 ab4a 1750 fa62 6bb9 25c3 1041  s.q..J.P.bk.%..A
-00002ed0: 9558 0390 35d9 403a 3b23 4d3c 6418 be37  .X..5.@:;#M<d..7
-00002ee0: 930d f434 2715 19ba 8e3e 20a7 16e1 72bd  ...4'....> ...r.
-00002ef0: 432c 5d77 1a98 0822 e933 871c 2599 7bf2  C,]w...".3..%.{.
-00002f00: 09a1 4bbc 84f2 b7e2 3ce1 771f 9b3e 1394  ..K.....<.w..>..
-00002f10: fd32 7dcc 5f73 1ef9 2f35 b2b8 1623 b7ff  .2}._s../5...#..
-00002f20: 69e4 cdfb e6af 6f5e b766 5669 371a 90fd  i.....o^.fVi7...
-00002f30: 0bb7 fa00 504b 0102 1403 1400 0000 0800  ....PK..........
-00002f40: 1849 f956 465a c10c 8200 0000 b100 0000  .I.VFZ..........
-00002f50: 1000 0000 0000 0000 0000 0000 8001 0000  ................
-00002f60: 0000 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
-00002f70: 6d6c 504b 0102 1403 1400 0000 0800 1849  mlPK...........I
-00002f80: f956 8068 a8bc ee00 0000 cb01 0000 1100  .V.h............
-00002f90: 0000 0000 0000 0000 0000 8001 b000 0000  ................
-00002fa0: 646f 6350 726f 7073 2f63 6f72 652e 786d  docProps/core.xm
-00002fb0: 6c50 4b01 0214 0314 0000 0008 0018 49f9  lPK...........I.
-00002fc0: 5699 5c9c 2310 0600 009c 2700 0013 0000  V.\.#.....'.....
-00002fd0: 0000 0000 0000 0000 0080 01cd 0100 0078  ...............x
-00002fe0: 6c2f 7468 656d 652f 7468 656d 6531 2e78  l/theme/theme1.x
-00002ff0: 6d6c 504b 0102 1403 1400 0000 0800 1849  mlPK...........I
-00003000: f956 e0d9 6c24 3d02 0000 a307 0000 1800  .V..l$=.........
-00003010: 0000 0000 0000 0000 0000 8081 0e08 0000  ................
-00003020: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00003030: 6565 7431 2e78 6d6c 504b 0102 1403 1400  eet1.xmlPK......
-00003040: 0000 0800 1849 f956 19c6 63fc 000e 0000  .....I.V..c.....
-00003050: bb83 0000 1800 0000 0000 0000 0000 0000  ................
-00003060: 8081 810a 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-00003070: 6574 732f 7368 6565 7432 2e78 6d6c 504b  ets/sheet2.xmlPK
-00003080: 0102 1403 1400 0000 0800 1849 f956 9102  ...........I.V..
-00003090: f16c c40e 0000 6f8b 0000 1800 0000 0000  .l....o.........
-000030a0: 0000 0000 0000 8081 b718 0000 786c 2f77  ............xl/w
-000030b0: 6f72 6b73 6865 6574 732f 7368 6565 7433  orksheets/sheet3
-000030c0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-000030d0: 1849 f956 f7f6 8f09 a702 0000 6d0b 0000  .I.V........m...
-000030e0: 0d00 0000 0000 0000 0000 0000 8001 b127  ...............'
-000030f0: 0000 786c 2f73 7479 6c65 732e 786d 6c50  ..xl/styles.xmlP
-00003100: 4b01 0214 0314 0000 0008 0018 49f9 56b7  K...........I.V.
-00003110: 47eb 8ac0 0000 0016 0200 000b 0000 0000  G...............
-00003120: 0000 0000 0000 0080 0183 2a00 005f 7265  ..........*.._re
-00003130: 6c73 2f2e 7265 6c73 504b 0102 1403 1400  ls/.relsPK......
-00003140: 0000 0800 1849 f956 b948 9c76 5201 0000  .....I.V.H.vR...
-00003150: ae02 0000 0f00 0000 0000 0000 0000 0000  ................
-00003160: 8001 6c2b 0000 786c 2f77 6f72 6b62 6f6f  ..l+..xl/workboo
-00003170: 6b2e 786d 6c50 4b01 0214 0314 0000 0008  k.xmlPK.........
-00003180: 0018 49f9 560b 085d 06bc 0000 001f 0300  ..I.V..]........
-00003190: 001a 0000 0000 0000 0000 0000 0080 01eb  ................
-000031a0: 2c00 0078 6c2f 5f72 656c 732f 776f 726b  ,..xl/_rels/work
-000031b0: 626f 6f6b 2e78 6d6c 2e72 656c 7350 4b01  book.xml.relsPK.
-000031c0: 0214 0314 0000 0008 0018 49f9 56db fbce  ..........I.V...
-000031d0: 8f24 0100 00e9 0400 0013 0000 0000 0000  .$..............
-000031e0: 0000 0000 0080 01df 2d00 005b 436f 6e74  ........-..[Cont
-000031f0: 656e 745f 5479 7065 735d 2e78 6d6c 504b  ent_Types].xmlPK
-00003200: 0506 0000 0000 0b00 0b00 ca02 0000 342f  ..............4/
-00003210: 0000 0000                                ....
+000000b0: 504b 0304 1400 0000 0800 f650 f956 99aa  PK.........P.V..
+000000c0: f383 eb00 0000 cb01 0000 1100 0000 646f  ..............do
+000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6ca5  cProps/core.xml.
+000000e0: 91c1 4ec3 300c 865f 65ea bd75 da0e 2645  ..N.0.._e..u..&E
+000000f0: 5d2e 204e 2021 3109 b45b e478 5bb4 a68d  ]. N !1..[.x[...
+00000100: 12a3 766f 4f5b b66e 086e 1ce3 fff3 675b  ..voO[.n.n....g[
+00000110: a9d0 4b6c 03bd 86d6 5360 4b71 d1bb ba89  ..Kl....S`Kq....
+00000120: 12fd 3a39 307b 0910 f140 4ec7 6c20 9a21  ..:90{...@N.l .!
+00000130: dcb5 c169 1e9e 610f 5ee3 51ef 090a 21ee  ...i..a.^.Q...!.
+00000140: c111 6ba3 59c3 284c fd6c 4cce 4a83 b3d2  ..k.Y.(L.lL.J...
+00000150: 7f86 7a12 1804 aac9 51c3 11f2 2c87 2bcb  ..z.....Q...,.+.
+00000160: 145c fcb3 614a 66b2 8f76 a6ba aecb ba72  .\..aJf..v.....r
+00000170: e286 8d72 f878 797e 9b96 4f6d 1359 3748  ...r.xy~..Om.Y7H
+00000180: 89aa 0c4a 0ca4 b90d 6abc c89f faba 829b  ...J....j.......
+00000190: 6275 9efd 5d20 b318 2648 3e79 5a27 97e4  bu..] ..&H>yZ'..
+000001a0: bd7c 78dc 3c25 aa10 4599 8a55 5adc 6d72  .|x.<%..E..UZ.mr
+000001b0: 21c5 4a2e 97db d1f5 a3ff 2a74 adb1 3bfb  !.J.......*t..;.
+000001c0: 0fe3 45a0 2af8 f56f ea0b 504b 0304 1400  ..E.*..o..PK....
+000001d0: 0000 0800 f650 f956 995c 9c23 1006 0000  .....P.V.\.#....
+000001e0: 9c27 0000 1300 0000 786c 2f74 6865 6d65  .'......xl/theme
+000001f0: 2f74 6865 6d65 312e 786d 6ced 5a5b 73da  /theme1.xml.Z[s.
+00000200: 3814 7eef afd0 7867 f66d 0bc6 3681 b6b4  8.~...xg.m..6...
+00000210: 1373 6976 dbb4 9984 ed4e 1f85 1158 8d6c  .siv.....N...X.l
+00000220: 7964 9184 7fbf 4736 10cb 960d ed92 4dba  yd....G6......M.
+00000230: 9b3c 042c e9fb ce45 47e7 e838 79f3 ee2e  .<.,...EG..8y...
+00000240: 62e8 8688 94f2 7860 d92f dbd6 bbb7 2fde  b.....x`./..../.
+00000250: e057 3224 1141 3019 a7af f0c0 0aa5 4c5e  .W2$.A0.......L^
+00000260: b55a 6900 c338 7dc9 1312 c3dc 828b 084b  .Zi..8}........K
+00000270: 7814 cbd6 5ce0 5b1a 2f23 d6ea b4db dd56  x...\.[./#.....V
+00000280: 8469 6ca1 1847 6460 7d5e 2c68 40d0 5451  .il..Gd`}^,h@.TQ
+00000290: 5a6f 5f20 b4e5 1f33 f815 cb54 8d65 a301  Zo_ ...3...T.e..
+000002a0: 1357 4126 b988 b4f2 f96c c5fc dade 3e65  .WA&.....l....>e
+000002b0: cfe9 3a1d 3281 6e30 1b58 207f ce6f a7e4  ..:.2.n0.X ..o..
+000002c0: 4e5a 88e1 54c2 c4c0 6a67 3f56 6bc7 d1d2  NZ..T...jg?Vk...
+000002d0: 4880 82c9 7d94 05ba 49f6 a3d3 1508 320d  H...}...I.....2.
+000002e0: 3b3a 9d58 ce76 7cf6 c4ed 9f8c cada 7434  ;:.X.v|.......t4
+000002f0: 6d1a e0e3 f178 38b6 cbd2 8b70 1c04 e051  m....x8....p...Q
+00000300: bb9e c29d f46c bfa4 4109 b4a3 69d0 64d8  .....l..A...i.d.
+00000310: f6da ae91 a6aa 8d53 4fd3 f77d dfeb 9b68  .......SO..}...h
+00000320: 9c0a 8d5b 4fd3 6b77 ddd3 8e89 c6ad d078  ...[O.kw.......x
+00000330: 0dbe f14f 87c3 ae89 c6ab d074 eb69 2627  ...O.......t.i&'
+00000340: fdae 6ba4 e916 6842 46e3 eb7a 1215 b5e5  ..k...hBF..z....
+00000350: 40d3 2000 5870 76d6 ccd2 0396 5e29 fa75  @. .Xpv.....^).u
+00000360: 941a d91d bbdd 415c f058 ee39 8911 fec6  ......A\.X.9....
+00000370: c504 d669 d219 9634 4672 9d90 050e 0037  ...i...4Fr.....7
+00000380: c4d1 4c50 7caf 41b6 8ae0 c292 d25c 90d6  ..LP|.A......\..
+00000390: cf29 b550 1a08 9ac8 81f5 4782 21c5 dcaf  .).P......G.!...
+000003a0: fdf5 97bb c9a4 337a 9d7d 3ace 6b94 7f69  ......3z.}:.k..i
+000003b0: ab01 a7ed bb9b cf93 fc73 e8e4 9fa7 93d7  .........s......
+000003c0: 4d42 ce70 bc2c 09f1 fb23 5b61 8727 6e3b  MB.p.,...#[a.'n;
+000003d0: 1372 3a1c 6742 7ccf f6f6 91a5 2532 cfef  .r:.gB|.....%2..
+000003e0: f90a eb4e 3c67 1f56 96b0 5dcf cfe4 9e8c  ...N<g.V..].....
+000003f0: 7223 bbdd f658 7df6 4f47 6e23 d7a9 c0b3  r#...X}.OGn#....
+00000400: 22d7 9446 2445 9fc8 2dba e411 38b5 490d  "..F$E..-...8.I.
+00000410: 3213 3f08 9d86 986a 501c 02a4 0931 96a1  2.?....jP....1..
+00000420: 86f8 b4c6 ac11 e013 7db7 be08 c8df 8d88  ........}.......
+00000430: f7ab 6f9a 3d57 a158 49da 84f8 1046 1ae2  ..o.=W.XI....F..
+00000440: 9c73 e673 d16c fb07 a546 d1f6 55bc dca3  .s.s.l...F..U...
+00000450: 9758 1501 9718 df34 aa35 2cc5 d678 95c0  .X.....4.5,..x..
+00000460: f1ad 9c3c 1d13 12cd 940b 0641 8697 2426  ...<.......A..$&
+00000470: 12a9 397e 4d48 13fe 2ba5 dafe 9cd3 40f0  ..9~MH..+.....@.
+00000480: 942f 24fa 4a91 8f69 b323 a774 26cd e833  ./$.J..i.#.t&..3
+00000490: 1ac1 46af 1b75 8768 d23c 7afe 05f9 9c35  ..F..u.h.<z....5
+000004a0: 0a1c 911b 1d02 671b b346 2184 69bb f01e  ......g..F!.i...
+000004b0: af24 8e9a adc2 112b 423e 6219 361a 72b5  .$.....+B>b.6.r.
+000004c0: 1681 b671 a984 605a 12c6 d178 4ed2 b411  ...q..`Z...xN...
+000004d0: fc59 ac35 933e 60c8 eccd 9175 ced6 910e  .Y.5.>`....u....
+000004e0: 1192 5e37 423e 62ce 8b90 11bf 1e86 384a  ..^7B>b.......8J
+000004f0: 9aed a271 5804 fd9e 5ec3 49c1 e882 cb66  ...qX...^.I....f
+00000500: fdb8 7e86 d533 6c2c 8ef7 47d4 174a e40f  ..~..3l,..G..J..
+00000510: 26a7 3fe9 3234 07a3 9a59 09bd 8456 6a9f  &.?.24...Y...Vj.
+00000520: aa87 343e a81e 320a 05f1 b91e 3ee5 7a78  ..4>..2.....>.zx
+00000530: 0a37 96c6 bc50 ae82 7b01 ffd1 da37 c2ab  .7...P..{....7..
+00000540: f882 c039 7f2e 7dcf a5ef b9f4 3da1 d2b7  ...9..}.....=...
+00000550: 3723 7d67 c1d3 8b5b de46 6e5b c4fb ae31  7#}g...[.Fn[...1
+00000560: dad7 342e 2863 5772 cdc8 c754 af93 29d8  ..4.(cWr...T..).
+00000570: 399f c0ec fd68 3e9e f1ed fad9 2484 af9a  9....h>.....$...
+00000580: 592d 2316 904b 81b3 4124 b8fc 8bca f02a  Y-#..K..A$.....*
+00000590: c409 e864 5b25 09cb 54d3 6537 8a12 9e42  ...d[%..T.e7...B
+000005a0: 1b6e e953 f54a 95d7 e5af b928 b83c 5be4  .n.S.J.....(.<[.
+000005b0: e9af a174 3e2c cff9 3c5f e7b4 cd0b 3343  ...t>,..<_....3C
+000005c0: b772 4bea b694 beb5 2638 4af4 b1cc 704e  .rK.....&8J...pN
+000005d0: 1ecb 0c3b 673c 921d b677 a01d 35fb f65d  ...;g<...w..5..]
+000005e0: 76e4 23a5 3053 9743 b81a 42be 036d ba9d  v.#.0S.C..B..m..
+000005f0: dc3a 389e 9891 b90a d352 906f c3f9 e9c5  .:8......R.o....
+00000600: 781a e239 d904 b97d 9857 6de7 d8d1 d1fb  x..9...}.Wm.....
+00000610: e7c1 51b0 a3ef 3c96 1dc7 88f2 a221 eea1  ..Q...<......!..
+00000620: 8698 cfc3 4387 797b 5f98 6795 c650 3414  ....C.y{_.g..P4.
+00000630: 6d6c ac24 2c46 b760 b8d7 f12c 14e0 6460  ml.$,F.`...,..d`
+00000640: 2da0 0783 af51 02f2 5255 6031 5bc6 032b  -....Q..RU`1[..+
+00000650: 90a2 7c4c 8c45 e870 e797 5c5f e3d1 92e3  ..|L.E.p..\_....
+00000660: dba6 65b5 6eaf 2977 196d 2252 39c2 6998  ..e.n.)w.m"R9.i.
+00000670: 1367 abca de65 b1c1 551d cf55 5bf2 b0be  .g...e..U..U[...
+00000680: 6a3d b415 4ecf fe59 adc8 9f0c 114e 160b  j=..N..Y.....N..
+00000690: 1248 6394 17a6 4aa2 f319 53be e72b 49c4  .Hc...J...S..+I.
+000006a0: 5538 bf45 33b6 1297 18bc e3e6 c771 4e53  U8.E3........qNS
+000006b0: b812 76b6 0f02 32b9 bb39 a97a 6531 67a6  ..v...2..9.ze1g.
+000006c0: f2df 2d0c 092c 5b88 5912 e24d 5ded d5e7  ..-..,[.Y..M]...
+000006d0: 9b9c ae7a 2276 fa97 77c1 60f2 fd70 c947  ...z"v..w.`..p.G
+000006e0: 0fe5 3be7 5ff4 5d43 ae7e f6dd e3fa 6e93  ..;._.]C.~....n.
+000006f0: 3b48 4c9c 79c5 1101 7445 0223 951c 0616  ;HL.y...tE.#....
+00000700: 1732 e450 ee92 9006 1301 cd94 c944 f002  .2.P.........D..
+00000710: 8264 a61c 8098 fa0b bdf2 0cb9 2915 cead  .d..........)...
+00000720: 3e39 7f45 2c83 864e 5ed2 2512 148a b00c  >9.E,..N^.%.....
+00000730: 0521 1772 e3ef ef93 6a77 8cd7 fa2c 816d  .!.r....jw...,.m
+00000740: 8454 3264 d517 ca43 89c1 3d33 7243 d854  .T2d...C..=3rC.T
+00000750: 25f3 aeda 260b 85db e254 cdbb 1abe 2660  %...&....T....&`
+00000760: 4bc3 7a6e 9d2d 27ff db5e d43d b417 3d46  K.zn.-'..^.=..=F
+00000770: f3a3 99e0 1eb3 8773 9b7a b8c2 45ac ff58  .......s.z..E..X
+00000780: d61e f932 df39 70db 3ade 035e e613 2c43  ...2.9p.:..^..,C
+00000790: a47e c17d 8a8a 8011 ab62 beba af4f f925  .~.}.....b...O.%
+000007a0: 9c3b b47b f181 209b fcd6 dba4 f6dd e00c  .;.{.. .........
+000007b0: 7cd4 ab5a a564 2b11 3f4b 077c 1f92 0663  |..Z.d+.?K.|...c
+000007c0: 8c5b f434 5f8f 1462 ada6 b1ad c6da 310c  .[.4_..b......1.
+000007d0: 7980 58f3 0ca1 6638 df87 459a 1a33 d58b  y.X...f8..E..3..
+000007e0: ac39 8d0a 6f41 d540 e53f dbd4 0d68 f60d  .9..oA.@.?...h..
+000007f0: 341c 9105 5e31 99b6 36a3 e44e 0a3c dcfe  4...^1..6..N.<..
+00000800: ef0d b0c2 c48e e1ed 8bbf 0150 4b03 0414  ...........PK...
+00000810: 0000 0008 00f6 50f9 56e0 d96c 243d 0200  ......P.V..l$=..
+00000820: 00a3 0700 0018 0000 0078 6c2f 776f 726b  .........xl/work
+00000830: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
+00000840: 6c85 95db 729b 3010 865f 85e1 012c e3b3  l...r.0.._...,..
+00000850: 3398 99da 9d4e 7b91 4e26 9e26 d732 2cb6  3....N{.N&.&.2,.
+00000860: c642 a2d2 62d2 b7af a438 b29b 82b8 42a7  .B..b....8....B.
+00000870: dd6f 0fe2 57da 4a75 d627 008c de2a 2ef4  .o..W.Ju.'...*..
+00000880: 263e 21d6 0f84 e8fc 0415 d523 5983 303b  &>!........#Y.0;
+00000890: a554 1545 3355 47a2 6b05 b470 4615 2793  .T.E3UG.k..pF.'.
+000008a0: f178 412a ca44 9ca5 6eed 4965 a96c 9033  .xA*.D..n.Ie.l.3
+000008b0: 014f 2ad2 4d55 51f5 670b 5cb6 9b38 893f  .O*.MUQ.g.\..8.?
+000008c0: 169e d9f1 846e 8164 694d 8fb0 07fc 551b  .....n.diM....U.
+000008d0: 0333 25de 4fc1 2a10 9a49 1129 2837 f197  .3%.O.*..I.)(7..
+000008e0: e461 9bcc 9c89 3bf2 c2a0 d577 e3c8 6673  .a....;....w..fs
+000008f0: 90f2 6c27 3f8a 4d3c b641 0187 1cad 0f6a  ..l'?.M<.A.....j
+00000900: 3e17 d801 e7d6 9509 e5f7 d56b 7ca3 5acb  >..........k|.Z.
+00000910: fbf1 87fb 6fae 0026 be03 d5b0 93fc 9515  ....o..&........
+00000920: 78da c4ab 382a a0a4 0dc7 67d9 7e87 6b52  x...8*....g.~.kR
+00000930: f35b 885f 29d2 2c55 b28d 94cd 364b 733b  .[._).,U....6Ks;
+00000940: 7074 97bd 39ce 84ad d51e 95d9 6586 8799  pt..9.......e...
+00000950: a015 e89a e690 1234 c1d8 4592 5f4d b77d  .......4..E._M.}
+00000960: 46b6 71da 74ee 7c1c e5f2 2818 c288 32d2  F.q.t.|...(...2.
+00000970: 3251 907f dd10 138d 0f69 e243 9a04 4332  2Q.......i.C..C2
+00000980: 3d2f d95b 573c 934f 16ae 96f7 88a9 474c  =/.[W<.O......GL
+00000990: 8388 c294 ea51 16c0 7f9a f4bb 48d3 21d2  .....Q......H.!.
+000009a0: cc93 6641 525e 947b 5bde 3ed0 6c08 34f7  ..fAR^.{[.>.l.4.
+000009b0: a079 1074 0165 6f6f 1763 3ec4 5878 c622  .y.t.eoo.c>.Xx."
+000009c0: c860 7ad7 2805 025f fa61 0b67 7b30 3697  .`z.(.._.a.g{06.
+000009d0: 2c49 c9a5 e322 2c3d 6e19 ae9d f9f9 118a  ,I...",=n.......
+000009e0: 2eca 7228 a595 67ac 828c a62e fa18 ab21  ..r(..g........!
+000009f0: c6da 33d6 4106 32e4 9dcd 5f0f 1192 f1ed  ..3.A.2..._.....
+00000a00: 371e 876f 34e8 5cb1 1a7b ba62 ad07 5077  7..o4.\..{.b..Pw
+00000a10: 8a11 960c d716 a93a 319f 6dfe c7dc 5420  .......:1.m...T 
+00000a20: 09cb 402e 052a 7668 fa50 8362 90dc d420  ..@..*vh.P.b... 
+00000a30: 09cb 81b2 62aa 3b29 8342 90dc 9420 094b  ....b.;).B... .K
+00000a40: 0167 b979 61ba 85b6 5f06 c89d b6db c7eb  .g.ya..._.......
+00000a50: 91aa 2313 3ae2 501a 8bf1 6869 fe6e f5fe  ..#.:.P...hi.n..
+00000a60: 18bc 4f50 d62e 8683 4494 951b 9ecc 230a  ..OP....D.....#.
+00000a70: ca1e 30fb a594 e827 16e3 dfe5 ec2f 504b  ..0....'...../PK
+00000a80: 0304 1400 0000 0800 f650 f956 19c6 63fc  .........P.V..c.
+00000a90: 000e 0000 bb83 0000 1800 0000 786c 2f77  ............xl/w
+00000aa0: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00000ab0: 2e78 6d6c ad9d db72 da48 1785 5f85 f203  .xml...r.H.._...
+00000ac0: 0473 4c66 ca71 d560 a1ee 7426 878a 3399  .sLf.q.`..t&..3.
+00000ad0: aaff 4e86 36a8 2224 2244 9ccc d3ff 1289  ..N.6."$"D......
+00000ae0: 69d9 ea4f 4dcb be4a cc62 1fb4 1712 e243  i..OM..J.b.....C
+00000af0: b42e eeb2 fceb 6ead 75d1 fbb1 49d2 ddeb  ......n.u...I...
+00000b00: b375 516c ffec f777 8bb5 de44 bb17 d956  .uQl...w...D...V
+00000b10: a7a5 729b e59b a828 ffcc 57fd dd36 d7d1  ..r....(..W..6..
+00000b20: f210 b449 fac3 f3f3 697f 13c5 e9d9 e5c5  ...I....i.......
+00000b30: e1b1 8ff9 e545 b62f 9238 d51f f3de 6ebf  .....E./.8....n.
+00000b40: d944 f9cf 994e b2bb d767 83b3 fb07 3ec5  .D...N...g....>.
+00000b50: ab75 7178 a07f 79b1 8d56 fa5a 17ff 6ccb  .uqx..y..V.Z..l.
+00000b60: 80f2 cffe 31cf 32de e874 1767 692f d7b7  ....1.2..t.gi/..
+00000b70: afcf fe1a fcf9 f6e5 f921 e4f0 942f b1be  .........!.../..
+00000b80: dbd5 fedf abb6 e626 cbbe 567f bc59 be3e  .......&..V..Y.>
+00000b90: 3baf 9ad2 895e 1455 8ea8 fce7 bbbe d249  ;....^.U.......I
+00000ba0: 52a5 2a5b f9f6 3beb 99a9 5a45 d6ff 7f9f  R.*[..;...ZE....
+00000bb0: 3e3c 0ca0 ecef 26da e9ab 2cf9 375e 16eb  ><....&...,.7^..
+00000bc0: d767 afce 7a4b 7d1b ed93 e253 7627 f5ef  .g..zK}....Sv'..
+00000bd0: 8d9a 9816 83a8 882e 2ff2 ecae 9757 5b7b  ......../....W[{
+00000be0: 79b1 a8fe 5395 2c9f 18a7 d594 ae8b bc7c  y...S.,........|
+00000bf0: 3c2e 2b15 97d5 d37b efb2 a54e 7a81 be8d  <.+....{...Nz...
+00000c00: d3b8 6afc a25f 942d 554f e82f 7e27 983d  ..j.._.-UO./~'.=
+00000c10: 4e50 153c 2857 a804 a8cc a99d eb22 2ab4  NP.<(W......."*.
+00000c20: a57c 88a9 042a 928a bc4d b3bb 442f 57ba  .|...*...M..D/W.
+00000c30: 34e8 db3e de1d b6b9 9764 2b4b e137 985e  4..>.....d+K.7.^
+00000c40: a1f2 d6a6 f44b 4b8e be0c 8fbe 0ca1 c7ab  .....KK.........
+00000c50: 24da ed6c 3e50 c0fb 6863 1bdc 153d 3fd0  $..l>P..hc...=?.
+00000c60: bb45 1e6f c1ee 80c2 3e46 b94e 8b1e b537  .E.o....>F.N...7
+00000c70: e772 e54e bc28 cd5d dadc 7545 55fe 04f6  .r.N.(.]..uEU...
+00000c80: 5786 a0d8 4f7a 9b44 0bbd eccd 7e5a c224  W...Oz.D....~Z.$
+00000c90: 855d 67fb 7c61 2bf4 a63d a237 4f8b b8f8  .]g.|a+..=.7O...
+00000ca0: d903 1f14 45bf 8b8a c5da 12f0 165f 19d9  ....E........_..
+00000cb0: a63c 4615 0f43 1ebc ba46 c757 d708 728c  .<F..C...F.W..r.
+00000cc0: 82c3 2e6f 7b7d 3d0e 31fb 392a 0195 a90e  ...o{}=.1.9*....
+00000cd0: 2ed7 4596 9747 db4f 7a77 18d3 e79f 5bdb  ..E..G.Ozw....[.
+00000ce0: 78e6 983c 4445 a022 a9a1 eabd 6657 bed9  x..<DE."....fW..
+00000cf0: 7c5d bd58 64ab f260 a75f 4471 ff2e 4e97  |].Xd..`._Dq..N.
+00000d00: 7d9b e3fe e353 14a2 7f94 6f06 369b 6d1b  }....S....o.6.m.
+00000d10: f1c0 cdf1 d1cd 31e4 fe4b e771 6435 f371  ......1..K.qd5.q
+00000d20: 8431 1395 80aa bc49 7745 9424 879d 915c  .1.....IwE.$...\
+00000d30: c4ac 212a 0215 499d 78ba e83d 3645 1168  ..!*..I.x..=6E.h
+00000d40: a26d 1b1e 9838 399a 38a1 6e76 3b6d cb3d  .m...89.8.nv;m.=
+00000d50: 7b1c 603c 4425 a022 1e3b 2426 0f51 11a8  {.`<D%.".;$&.Q..
+00000d60: 486a c8d3 4adf e129 0a40 276d 9bf0 c0c9  Hj..J..).@'m....
+00000d70: e9d1 c929 35f3 23de c154 678f 638c 99a8  ...)5.#..Tg.c...
+00000d80: 0454 e7df 724a 9ff7 f94d f9f0 d53a cacb  .T..rJ...M...:..
+00000d90: 0d2a 5fd0 bb22 5ed8 ecc4 f421 2a02 1549  .*_.."^....!*..I
+00000da0: 2d79 dad9 6182 8a62 d051 db56 3c70 f4e5  -y..a..b.Q.V<p..
+00000db0: d1d1 97f4 961b 84d5 9e83 ef99 2d71 3d73  ............-q=s
+00000dc0: 826d 3b3b 7b1c 695c 4765 8e4a 888a 4045  .m;;{.i\Ge.J..@E
+00000dd0: 52ef 9e56 761c 9da2 38b4 d3b6 250f ec7c  R..Vv...8...%..|
+00000de0: 75b4 f315 9e41 556f 658f 4fa1 7e59 f938  u....AUoe.O.~Y.8
+00000df0: c6ec a0a8 0454 e74b 54be c1dc 24fa bede  .....T.KT...$...
+00000e00: 3fe5 146d fb26 660e 5111 a848 eac6 d3d0  ?..m.&f.Q..H....
+00000e10: 0ec3 5314 8366 dab6 e281 997f 1ccd fc83  ..S..f..........
+00000e20: fa29 aef6 f977 ebc1 f671 88f1 1295 80ca  .)...w...q......
+00000e30: 542f e28f 79b6 dc2f 0aeb e71e cc18 a222  T/..y../......."
+00000e40: 5091 d485 a787 fe33 5314 8216 da36 e281  P......3S....6..
+00000e50: 8583 7303 21ce 5ba6 fb21 5f45 69fc dfe1  ..s.!.[..!_Ei...
+00000e60: fcd2 7172 326b 24aa d108 9402 2cef 3a17  ..qr2k$.....,.:.
+00000e70: e29c 214b 8225 899d 781a fc5c 0355 9808  ..!K.%..x..\.U..
+00000e80: 7db7 6edd 43e3 6bf4 a90d 3fb5 ec56 b346  }.n.C.k...?..V.F
+00000e90: 60cd e816 ee44 e5aa 53a6 79aa f3d5 cf23  `....D..S.y....#
+00000ea0: 0312 79b4 b57d fe9e 73fe 9025 c192 c4ae  ..y..}..s..%....
+00000eb0: 7c4d ef38 4c85 816c b293 640d 0cca 1a20  |M.8L..l..d.... 
+00000ec0: c5a9 3e75 d83f dc34 626a fea2 14b4 56f2  ..>u.?.4bj....V.
+00000ed0: 78d9 cfb9 46c8 9260 4962 67be 1efb cf52  x...F..`Ibg....R
+00000ee0: 610c db6b db90 87f6 1a96 3478 3ae5 9935  a..k......4x:..5
+00000ef0: 72d4 ec66 bc84 959d f632 5562 49b0 24b1  r..f.....2UbI.$.
+00000f00: 135f 7b9f 3e4b 8539 d86e 276b 1a18 d834  ._{.>K.9.n'k...4
+00000f10: 2008 1264 7769 751c b5fa cbc0 89a5 004b   ..dwiu........K
+00000f20: 7dca ca51 7cc8 639d 1611 80ea 39e7 0d59  }..Q|.c.....9..Y
+00000f30: 122c 49ec c6d7 e30e 0354 18c4 a63a d9d3  .,I......T...:..
+00000f40: c0c0 a701 f190 f9f7 0652 feed 28e3 2796  .........R..(.'.
+00000f50: 02ac e301 a038 7dc8 9260 4962 53be c6fa  .....8}..`IbS...
+00000f60: 0e51 6104 bbea e450 0303 a206 c444 e63f  .Qa....P.....D.?
+00000f70: 16c9 befa 36f3 7f59 6a3f 1e33 8f62 29c0  ....6..Yj?.3.b).
+00000f80: 7a50 66ce b942 9604 4b12 3bf0 b5b2 ebe4  zPf..B..K.;.....
+00000f90: 1446 b2a5 4e10 3530 246a 405c 248c 13bb  .F..N.50$j@\$...
+00000fa0: 9348 78ae 580a b08c cf7e ca3c 8a25 c192  .Hx.X....~.<.%..
+00000fb0: c4a6 7ccd f59c a1c2 00f6 d449 a306 0647  ..|........I...G
+00000fc0: 0d08 8f84 f10f ebd7 a2b3 4644 cd54 c651  ..........FD.T.Q
+00000fd0: 58e7 7abf dd66 7951 3e54 7e42 d8e7 ec28  X.z..fyQ>T~B...(
+00000fe0: 0329 9604 4b12 3bf2 75d4 7782 0a23 d852  .)..K.;.u.w..#.R
+00000ff0: 2793 1a18 2835 205c 1226 5979 c692 daae  '...(5 \.&Yy....
+00001000: 2898 3582 6aae 3298 c252 27bb ca88 8a25  (.5.j.2..R'....%
+00001010: c192 c48e 7c5d ed30 4485 416c ac93 540d  ....|].0D.Al..T.
+00001020: 0da9 1a12 0f91 591e ff97 95e7 a349 f525  ......Y......I.%
+00001030: 85f5 020d 6653 2c05 58b0 e5bb 9039 e70b  ....fS,.X....9..
+00001040: 5912 2c49 ecc2 d3d2 eee3 5318 8ac6 5ab7  Y.,I......S...Z.
+00001050: e7a1 b186 440d 8981 bc99 5ff1 3537 4ca1  ....D....._.57L.
+00001060: 580a b094 d717 775c 2064 49b0 24b1 2d5f  X.....w\ dI.$.-_
+00001070: 8f3b 4c52 6110 bbeb be98 aa76 3515 2190  .;LRa......v5.!.
+00001080: fb9e 5ebc b1fa cb14 8aa5 c059 cc6a 2713  ..^........Y.j'.
+00001090: 2796 044b 12bb f0b5 b3d3 e814 86b1 a14e  '..K...........N
+000010a0: e834 34d0 6948 90c3 7465 7794 4113 4b81  .44.iH..tew.A.K.
+000010b0: b39a d551 864c 2c09 9624 76e1 eb68 b7d9  ...Q.L,..$v..h..
+000010c0: 298c 634b 9d60 6968 c0d2 102f 3032 6dd9  ).cK.`ih.../02m.
+000010d0: 3d65 b8c4 52e0 2c67 f594 a112 4b82 2589  =e..R.,g....K.%.
+000010e0: 5df8 7ada 7178 0a03 d954 2758 1a1a b034  ].z.qx...T'X...4
+000010f0: 24c2 51ef 2bb2 baca 8089 a5e0 a47a 5667  $.Q.+........zVg
+00001100: 992a b124 5892 d889 afb3 5d27 a830 92ad  .*.$X.....]'.0..
+00001110: 75d2 a5a1 a14b 4322 1df5 c66e acd6 325d  u....KC"...n..2]
+00001120: 6229 38a9 9ed5 5aa6 4c2c 0996 2476 e26b  b)8...Z.L,..$v.k
+00001130: 6dd7 092a 8c64 6b9d 9469 6828 d390 8047  m..*.dk..ih(...G
+00001140: ad31 fb4e cbb4 89a5 e094 7256 6399 30b1  .1.N......rVc.0.
+00001150: 2458 92d8 88af b11d e7a7 3090 7d75 92a6  $X........0.}u..
+00001160: a121 4d43 a21e b5be ec7b 2c03 2796 8253  .!MC.....{,.'..S
+00001170: ca59 7d65 cec4 9260 4962 23be be76 9c9f  .Y}e...`Ib#..v..
+00001180: c240 f6d5 899b 8606 370d 097a 98be be58  .@......7..z...X
+00001190: 6d65 e2c4 52e0 ac66 f594 2913 4b82 2589  me..R..f..).K.%.
+000011a0: 5df8 7ada 6d76 0ae3 d852 2768 1a19 d034  ].z.mv...R'h...4
+000011b0: 22dc 61da b21e 811b 71c6 5296 8213 aad9  ".a.....q.R.....
+000011c0: 4ce5 8c21 4b82 2589 7df8 fe40 a3db f414  L..!K.%.}..@....
+000011d0: c6f1 cf34 9c90 6964 20d3 c885 465e d80f  ...4..id ...F^..
+000011e0: bf8d b89a a9cc 994e a866 3595 c112 4b82  .......N.f5...K.
+000011f0: 2589 7df8 9ada 6d7a 0ae3 d854 275b 1a19  %.}...mz...T'[..
+00001200: b634 4240 923a be65 6d44 d66c 65bc 84f5  .4B@.:.emD.le...
+00001210: e85b 56ce 15b2 2458 92d8 81af a15d 27a7  .[V...$X.....]'.
+00001220: 3092 2d75 d2a5 51ed e771 4848 dcbf 759a  0.-u..Q..qHH..u.
+00001230: 3582 6bae b6fc 548e 4a7a 4161 2e10 b224  5.k...T.JzAa...$
+00001240: 5892 d896 afd5 4f98 a8c2 6076 db09 9e46  X.....O...`v...F
+00001250: 063c 8d08 81fc 1ddd c06f 2199 38b1 1460  .<.......o!.8..`
+00001260: 1ddf ab13 b946 c892 6049 6267 be2e fb4e  .....F..`Ibg...N
+00001270: 5261 045b ebc4 4f23 839f 4684 40fe 8ed2  Ra.[..O#..F.@...
+00001280: e522 fbae 73ab bd8c 9e58 0ab0 96eb 2702  ."..s....X....'.
+00001290: 9c33 6449 b024 b113 5f3b bb4c 4f61 145b  .3dI.$.._;.LOa.[
+000012a0: eac4 4e23 839d 4684 3ede 6569 76b8 30d0  ..N#..F.>.eiv.0.
+000012b0: 6a29 2327 9602 ac75 a883 bb27 f326 9604  j)#'...u...'.&..
+000012c0: 4b12 dbf0 f5b3 cbe8 1446 b19f 4ed6 3432  K........F..N.42
+000012d0: ac69 44c8 e3dd 3e29 6236 9449 134b 0116  .iD...>)b6.I.K..
+000012e0: 6b37 9439 134b 8225 896d f81a da69 760a  k7.9.K.%.m...iv.
+000012f0: c3d8 5127 651a 19ca 3422 d8f1 3ea3 6b23  ..Q'e...4"..>.k#
+00001300: 1a21 3537 992f 61a1 b66b 2338 5fc8 9260  .!57./a..k#8_..`
+00001310: 4962 17be 667a 8f4d 6108 1be9 c44a 2383  Ib..fz.Ma....J#.
+00001320: 9546 8438 de67 ed17 5fcf 1a91 353f 192c  .F.8.g.._...5?.,
+00001330: 61bd 53ae f7e6 bc21 4b82 2589 ddf8 fada  a.S....!K.%.....
+00001340: 758a 0a23 d95e 2762 1a1b c434 26d8 f13e  u..#.^'b...4&..>
+00001350: 8b77 1a7f 3dd9 0833 deb2 1460 31d7 d911  .w..=..3...`1...
+00001360: e70c 5912 2c49 ecc4 77f9 884e e353 18c6  ..Y.,I..w..N.S..
+00001370: 8b48 3811 d3d8 20a6 31c1 8ef7 593a 4ba2  .H8... .1...Y:K.
+00001380: a5be ff30 69b5 9639 134b 0197 dc6f 6e74  ...0i..9.K...ont
+00001390: fee1 f650 d76e 2eb3 2696 044b 127b f135  ...P.n..&..K.{.5
+000013a0: f709 6354 18cc 163b 81d3 d800 a731 c10f  ..cT...;.....1..
+000013b0: e7bc 678d d09a c14c 9cb0 a017 9be0 0221  ..g....L.......!
+000013c0: 4b82 2589 6df9 7add 799e 0a43 d969 2787  K.%.m.z.y..C.i'.
+000013d0: 1a1b 0e35 26f0 f1e1 f6f6 7a9d e5f6 9d98  ...5&.....z.....
+000013e0: f913 4b01 963a 6979 1fc6 4e2c 0996 2476  ..K..:iy..N,..$v
+000013f0: e36b 6d87 012a 0c62 53dd 8b35 d556 6b22  .km..*.bS..5.Vk"
+00001400: e4f1 2165 4f5b 166c 6a59 b1e9 494b 36b5  ..!eO[.ljY..IK6.
+00001410: acd9 d4b2 6853 cbaa 4dcf b56c 93ff fc14  ....hS..M..l....
+00001420: c6b0 a54e cc34 3698 694c c8e3 439e adaa  ...N.46.iL..C...
+00001430: df91 db56 9a9b 35a2 6aa6 3266 c25a ce13  ...V..5.j.2f.Z..
+00001440: 29c6 4c2c 0996 2476 e26b 6897 e929 8c62  ).L,..$v.kh..).b
+00001450: 4b9d 9869 6c30 d398 a8c7 c7ec 4ee7 7c72  K..il0......N.|r
+00001460: cc9c 89a5 80a5 394b 214b 8225 891b e6eb  ......9K!K.%....
+00001470: 5aa7 0129 0c63 db9c 3469 6c68 d218 018f  Z..).c..4ilh....
+00001480: fe75 b8db ade3 add5 38e6 492c 0558 ce17  .u......8.I,.X..
+00001490: e973 8d90 25c1 92c4 ce7c 6dee 3850 8581  .s..%....|m.8P..
+000014a0: 6cb4 1332 8d0d 641a 13fa 702d 35d0 08ac  l..2..d...p-5...
+000014b0: 19cd a809 cb39 d6b1 9a73 ce90 25c1 92c4  .....9...s..%...
+000014c0: 4e7c 8ded 3840 8581 6cac 133a 8d0d 741a  N|..8@..l..:..t.
+000014d0: 3f01 02cd 1ac1 3573 993b 6149 bfcf 370c  ?.....5s.;aI..7.
+000014e0: a058 122c 496c cbd7 e927 4c54 6130 bbed  .X.,Il...'LTa0..
+000014f0: 6450 13c3 a026 b8f4 520b 909f 35a2 8ccd  dP...&..R...5...
+00001500: 2c05 58cb cb66 2e10 b224 5892 d896 ef1a  ,.X..f...$X.....
+00001510: 985d 46a9 308a 57c2 74e2 a889 c151 135c  .]F.0.W.t....Q.\
+00001520: d05b 7fdb ebd4 baa0 f2ac 1154 b397 3114  .[.........T..1.
+00001530: 96f2 59dc 9479 144b 8225 894d f99a db61  ..Y..y.K.%.M...a
+00001540: 8e0a 83d8 5b27 879a 180e 3521 f871 1da7  ....['....5!.q..
+00001550: ab44 1fa8 490b 6c6c 84d7 5c66 1685 45dd  .D..I.ll..\f..E.
+00001560: b091 b386 2c09 9624 f6e2 6bee 9306 a930  ....,..$..k....0
+00001570: 9c6d 7642 a889 8150 13c2 2127 fec0 7cd6  .mvB...P..!'..|.
+00001580: 4850 339a 8114 96f5 3b5a 3399 6249 b024  HP3.....;Z3.bI.$
+00001590: b12d 5fcf 9f38 5585 09d8 7527 a59a 184a  .-_..8U...u'...J
+000015a0: 3521 62f2 799d 6bf7 becd bc8a a500 6b9e  5!b.y.k.......k.
+000015b0: b06f 33ad 6249 b024 b117 5f9f 9f32 4785  .o3.bI.$.._..2G.
+000015c0: d16c b27b c9f1 da9a e3c4 503e c71b 7d5d  .l.{......P>..}]
+000015d0: ee56 7673 5b56 1e6f 597a fc39 d61e 6f59  .Vvs[V.oYz.9..oY
+000015e0: 7cbc 65f5 f196 e5c7 9f6b fdf1 2e83 5418  |.e......k....T.
+000015f0: c5ee 3a11 d6c4 20ac 09a1 9663 53d6 ef88  ..:... ....cS...
+00001600: 1a61 357b 1961 6131 1796 e49c 214b 8225  .a5{.aa1....!K.%
+00001610: 899d f87a da69 7c0a c3d8 5427 e09a 18c0  ...z.i|...T'....
+00001620: 3521 acf2 f92e 731e 9599 71b1 1460 c513  5!....s...q..`..
+00001630: 8eca 4cb5 5812 2c49 ecc5 d7db ee53 5418  ..L.X.,I.....ST.
+00001640: cb06 3bc1 d6c4 80ad 09e1 1558 257c d608  ..;........X%|..
+00001650: a8b9 ca40 0bcb 9cba 3839 e70e 5912 2c49  ...@....89..Y.,I
+00001660: ecc8 d75b cf01 2a0c 6043 9d40 6b62 80d6  ...[..*.`C.@kb..
+00001670: 8408 ca3f 5b5a 2eb3 1152 b394 3116 163a  ...?[Z...R..1..:
+00001680: e5f2 29ce 1bb2 2458 92d8 8daf 9dde e353  ..)...$X.......S
+00001690: 18c2 863a 99d5 d430 ab29 2193 fb5d c766  ...:...0.)!..].f
+000016a0: 6923 c858 ca52 e02c e5da 4b39 77c8 9260  i#.X.R.,..K9w..`
+000016b0: 4962 47be b7f8 e830 4485 417c 930f 27ac  IbG....0D.A|..'.
+000016c0: 9a1a 5835 255e 72e2 b467 8d04 3593 195c  ..X5%^r..g..5..\
+000016d0: 6159 9f55 c939 7fc8 9260 4962 57be 463f  aY.U.9...`IbW.F?
+000016e0: 71a8 0a13 b0e9 4e8a 3535 146b 4af4 e48b  q.....N.55.kJ...
+000016f0: ce8b 78c1 ebb9 3502 6b66 33bf c272 6dd7  ..x...5.kf3..rm.
+00001700: 2c73 be90 25c1 92c4 2e7c cded 383c 8581  ,s..%....|..8<..
+00001710: 6caa 9359 4d0d b39a b6c1 a3bf 8a24 b23b  l..YM........$.;
+00001720: caa0 8aa5 006b b93e f970 ce90 25c1 92c4  .....k.>.p..%...
+00001730: 4e7c 5ded 323d 8551 6ca9 1348 4d0d 909a  N|].2=.Ql..HM...
+00001740: 120a a99a ba4a e28d fd36 90b3 465c cd54  .....J...6..F\.T
+00001750: 4651 58cd 692a 8328 9604 4b12 3bf1 35b5  FQX.i*.(..K.;.5.
+00001760: dbfc 14c6 b1ad 4e04 3535 086a 4a0c c4e3  ......N.55.jJ...
+00001770: cd6f d69a a4f7 2b4b cfdc dd95 f25c 35f2  .o....+K.....\5.
+00001780: d45e 1028 cd59 0a59 122c 49dc 1c5f cb9f  .^.(.Y.Y.,I.._..
+00001790: 61b6 0a93 b0ff ee7b e5d5 6e96 d776 17bb  a......{..n..v..
+000017a0: 30ca 3756 bf5b 6e97 d772 bfbc b652 279f  0.7V.[n..r...R'.
+000017b0: 67b5 dc30 afe5 8e79 2db7 cc7b ae7b e675  g..0...y-..{.{.u
+000017c0: 18a4 c220 36d7 09ab a606 564d 0995 543d  ... 6.....VM..T=
+000017d0: ddc3 5e91 c7d6 0fc1 8de0 9ac9 4cab b0a4  ..^.........L...
+000017e0: f3c0 cdac 8a25 c192 c44e 7c8d 7dc2 1015  .....%...N|.}...
+000017f0: 06b3 c14e 5835 35b0 6a4a e8a4 f625 9dd5  ...NX55.jJ...%..
+00001800: 5b66 562c 05ad d54e de81 995b b124 5892  [fV,...N...[.$X.
+00001810: d895 afcf dd66 a930 8e2d 76e2 aba9 c157  .....f.0.-v....W
+00001820: d3e7 b838 6ad6 c852 339c 8956 6bed 930d  ...8j..R3..Vk...
+00001830: 67b2 c592 6049 6257 be86 3fc7 6415 6661  g...`IbW..?.d.fa
+00001840: fb9d b0eb a581 5d2f 09b9 d0a2 368d 00e3  ......]/....6...
+00001850: 344b 0196 711d b639 67c8 9260 4962 27be  4K..q..9g..`Ib'.
+00001860: 373e f51c 9cc2 00be e529 c3ad fe6e ad75  7>.......)...n.u
+00001870: 510d eff2 621b adf4 bb28 5fc5 e9ae 97e8  Q...b....(_.....
+00001880: db32 e2fc c5cb f21c 2d8f 57eb e31f 45b6  .2......-.W...E.
+00001890: 7d7d 3638 ebdd 6445 916d 0eff 5deb 68a9  }}68..dE.m..].h.
+000018a0: f3ea 09a5 7e9b 65c5 f18f aacc 5d96 7f3d  ....~.e.....]..=
+000018b0: 14b9 fc3f 504b 0304 1400 0000 0800 f650  ...?PK.........P
+000018c0: f956 ba52 73fa c30e 0000 6f8b 0000 1800  .V.Rs.....o.....
+000018d0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+000018e0: 7368 6565 7433 2e78 6d6c ad9d 5b73 9bc8  sheet3.xml..[s..
+000018f0: 1685 ff8a ca4f 332f b175 7332 538e ab22  .....O3/.us2S.."
+00001900: 09e8 cb74 92b2 e79c 79c6 52db e644 161a  ...t....y.R..D..
+00001910: 40e3 647e fd01 f902 127c ea80 fc14 db9f  @.d~.....|......
+00001920: d7ee eedd 2b08 2f04 ba78 8c93 6fe9 bdb5  ....+./..x..o...
+00001930: 59ef fbc3 7295 7e3c b9cf b2f5 efa7 a7e9  Y...r.~<........
+00001940: fcde 3e84 e9bb 786d 5739 b98d 9387 30cb  ..>...xmW9....0.
+00001950: bf4d ee4e d375 62c3 c556 f4b0 3c1d 9c9d  .M.N.ub..V..<...
+00001960: 9d9f 3e84 d1ea e4f2 62fb b3af c9e5 45bc  ..>.....b.....E.
+00001970: c996 d1ca 7e4d 7ae9 e6e1 214c 7e4c ec32  ....~Mz...!L~L.2
+00001980: 7efc 78d2 3f79 f9c1 5574 779f 6d7f 707a  ~.x.?y..Utw.m.pz
+00001990: 79b1 0eef ecb5 cdfe b3ce 05f9 b7a7 af75  y..............u
+000019a0: 16d1 835d a551 bcea 25f6 f6e3 c9a7 feef  ...].Q..%.......
+000019b0: 9fcf 075b c9f6 57fe 1bd9 c7b4 f275 af58  ...[..W......u.X
+000019c0: cd4d 1c7f 2bbe 918b 8f27 67c5 a4ec d2ce  .M..+....'g.....
+000019d0: b3a2 4698 fff3 8f9d dae5 b228 954f e5ef  ..F........(.O..
+000019e0: e7aa 27e5 a885 b2fa f54b 797f db80 7c7e  ..'......Ky...|~
+000019f0: 3761 6aa7 f1f2 af68 91dd 7f3c f970 d25b  7aj....h...<.p.[
+00001a00: d8db 70b3 ccae e247 619f 1735 2ea7 380b  ..p....Ga..5..8.
+00001a10: b3f0 f222 891f 7b49 b1da cb8b 79f1 4531  ..."..{I....y.E1
+00001a20: 64fe 8bd1 aae8 d275 96e4 3f8f f291 b2cb  d......u..?.....
+00001a30: e2d7 7b26 5ed8 656f 666f a355 544c fce2  ..{&^.eofo.UTL..
+00001a40: 34cb a754 fcc2 e9fc b9c0 64bf 4031 e096  4..T......d.@1..
+00001a50: 4c91 cc90 7848 7c24 0112 418b bbce c2cc  L...xH|$..A.....
+00001a60: 362c 4662 2985 44d3 207a 153f 2eed e2ce  6,Fb).D. z.?....
+00001a70: e6db fdf7 264a b71d ec2d e3bb 8681 ffc0  ....&J...-......
+00001a80: f206 c9e7 2672 9a6f f0eb 2e0f 5e77 7900  ....&r.o....^wy.
+00001a90: 739c 2ec3 346d da55 127c 4df2 ff87 49f6  s...4m.U.|M...I.
+00001aa0: a341 3325 cde7 f0a1 a9d9 33fa fd99 4de7  .A3%......3...M.
+00001ab0: 49b4 06c3 7924 fbf3 c7ba 6918 9f7e df44  I...y$....i..~.D
+00001ac0: abde 34de acb2 0651 80a2 f03b 8a04 2f28  ..4....Q...;../(
+00001ad0: 3f50 cd73 cb2d 9a3c e752 15ae 9935 fb55  ?P.s.-.<.R...5.U
+00001ae0: 91f6 caae 97e1 dc2e 7a93 a69d d224 bb8e  ........z....$..
+00001af0: 37c9 bc69 a03f 0e2b 7ade 2a8b b21f 3dd8  7..i.?.+z.*...=.
+00001b00: 69c3 ddcc e6f7 0d82 cfe8 d7f8 213f 0eef  i...........!?..
+00001b10: 357f c7f3 c357 cf0f e93f ce64 9fbc 54bf  5....W...?.d..T.
+00001b20: 0fd3 e9cc 1fce b687 bd26 8763 c919 120f  .........&.c....
+00001b30: 898f 2440 2290 4824 0a89 c646 e42f bd69  ..$@".H$...F./.i
+00001b40: feda fbed eedd 3cbe cb8f fdf6 5d18 9d3e  ......<.....]..>
+00001b50: 46ab c569 9339 baf6 d390 d07e cf5f 219b  F..i.9.....~._!.
+00001b60: 7cd1 b494 9ded 1fbd 6eff 08b7 7f9f ec4e  |.......n......N
+00001b70: b778 e1fb 92dc 85ab e8df edff bd2b 9b6e  .x...........+.n
+00001b80: 3d0e 8797 298e 3343 e221 f191 0448 0412  =...).3C.!...H..
+00001b90: 8944 21d1 d89d 769e 78d3 261b aa86 4669  .D!...v.x.&...Fi
+00001ba0: 5adf 8e51 c6af 4619 a351 f649 7d0d f9b9  Z..Q..F..Q.I}...
+00001bb0: 6293 27b0 e40c 8987 c447 1220 1148 2412  b.'......G. .H$.
+00001bc0: 8544 6323 da79 a26b 3f0d 0971 fb9b 96b2  .Dc#.y.k?..q....
+00001bd0: b3fd e7af db7f 8edb bf4f 1aa6 9bc5 49fe  .........O....I.
+00001be0: 1783 eb10 8143 cc90 7848 7c24 0112 8144  .....C..xH|$...D
+00001bf0: 2251 4834 36a6 9d1d deaa bf86 0aa1 3d9a  "QH46.........=.
+00001c00: 96b6 638f f7af f678 8ff6 d827 bbd3 f7fe  ..c....x...'....
+00001c10: a99d a73c 9901 0bce 9078 487c 2401 1281  ...<.....xH|$...
+00001c20: 4422 5148 34b6 a19d 19ba 75d3 900c b7be  D"QH4.....u.....
+00001c30: 6921 3b5b ffe1 75eb 3fe0 d6ef 93dd c9fa  i!;[..u.?.......
+00001c40: d1b2 f130 80f5 6648 3c24 3e92 0089 4022  ...0..fH<$>...@"
+00001c50: 9128 241a bbd0 6ee7 3b35 d390 0a37 be69  .($...n.;5...7.i
+00001c60: 1d3b 1bff dbeb c6ff 861b bf4f 76e7 fa47  .;.........Ov..G
+00001c70: 78d3 fc77 0316 9c21 f190 f848 0224 0289  x..w...!...H.$..
+00001c80: 44a2 9068 6c43 bb9d efd6 4d43 32dc faa6  D..hlC....MC2...
+00001c90: 85ec 6c7d ffac ccc3 ce70 f36b 6877 be57  ..l}.....p.khw.W
+00001ca0: 76b9 3d97 4def a375 9309 b8f2 8c91 c7c8  v.=.M..u........
+00001cb0: 6714 3012 8c24 23c5 4873 5bda b9e1 b8f6  g.0..$#.Hs[.....
+00001cc0: 1a94 a32d 1ad7 b4eb 8b4a 4e8a 39dc a486  ...-.....JN.9...
+00001cd0: f627 7ef8 ec90 2bcf 1879 8c7c 4601 23c1  .'~...+..y.|F.#.
+00001ce0: 4832 528c 34b7 a5a5 2f8e 6aaf 4139 fbc2  H2R.4.../.j.A9..
+00001cf0: 19ac f6cb 64b5 bf1f 5555 7c41 29d6 d3c4  ....d...UU|A)...
+00001d00: ff8c 1eec b54d a266 5360 d919 238f 91cf  .....M.fS`..#...
+00001d10: 2860 2418 4946 8a91 e69e b434 45f7 de1a  (`$.IF.....4E...
+00001d20: d4b2 239a 16b4 eb88 3277 ec73 f058 4395  ..#.....2w.s.XC.
+00001d30: 5917 7fef 7c4d e2c5 a671 0a53 ae3a 63e4  Y...|M...q.S.:c.
+00001d40: 31f2 1905 8c04 23c9 4831 d2dc 9296 86e8  1.....#.H1......
+00001d50: dc5a 8352 f683 3387 ec97 4164 9f93 c81a  .Z.R..3...Ad....
+00001d60: aa4c fa6b fc68 9369 36dd 24ff 5863 b370  .L.k.h.i6.$.Xc.p
+00001d70: 912f a2d1 181c 4032 f218 f98c 0246 8291  ./....@2.....F..
+00001d80: 64a4 1869 ee4d 4b63 1cdf 6383 35d8 21ce  d..i.MKc..c.5.!.
+00001d90: 00b2 5f26 907d 8e20 6ba8 32fb bff2 25ff  .._&.}. k.2...%.
+00001da0: b949 6e72 32bd 0f93 7c26 f911 2fcd a279  .Inr2...|&../..y
+00001db0: a34d 3893 64e4 31f2 1905 8c04 23c9 4831  .M8.d.1.....#.H1
+00001dc0: d2dc a096 3679 a346 1b2c c45e 71a6 95fd  ....6y.F.,.^q...
+00001dd0: 32ae ec73 5e59 43cd 4b70 bdd0 705a c9c8  2..s^YC.Kp..pZ..
+00001de0: 63e4 330a 1809 4692 9162 a4b9 3b2d 8df2  c.3...F..b..;-..
+00001df0: 165d 3658 855d e20c 2dfb 656a d9e7 d8b2  .]6X.]..-.ej....
+00001e00: 865e 468e 2a17 ebbe dc36 5a83 b34b 461e  .^F.*....6Z..KF.
+00001e10: 239f 51c0 4830 928c 1423 8d2d 696b 8dce  #.Q.H0...#.-ik..
+00001e20: ad35 2865 3f38 93cc 7e19 65f6 39cb aca1  .5(e?8..~.e.9...
+00001e30: 9d49 1fba 5007 26e1 9893 91c7 c867 1430  .I..P.&......g.0
+00001e40: 128c 2423 c548 639f da9a e46d fb6d b01e  ..$#.Hc....m.m..
+00001e50: 3bc7 1985 f6cb 2cb4 cf61 680d d556 726d  ;.....,..ah..Vrm
+00001e60: 3330 0927 a28c 3c46 3ea3 8091 6024 1929  30.'..<F>...`$.)
+00001e70: 461a 5bd2 d624 9d5b 6b50 ca7e 70e6 a383  F.[..$.[kP.~p...
+00001e80: 321f 1d70 3e5a 43f5 49d7 afe7 35fb 8347  2..p>ZC.I...5..G
+00001e90: 9931 f218 f98c 0246 8291 64a4 1869 6c51  .1.....F..d..ilQ
+00001ea0: 4b7f bc5d ab0d 9642 bf34 ae6f d72f 656e  K..]...B.4.o./en
+00001eb0: 3ae0 dcb4 8676 16b1 bde4 07ee e0c4 9491  :....v..........
+00001ec0: c7c8 6714 3012 8c24 23c5 4863 43da baa3  ..g.0..$#.HcC...
+00001ed0: 6363 0d0a d90b ee37 a156 de85 ca59 690d  cc.....7.V...Yi.
+00001ee0: ed4c b9b8 0808 56e0 9c94 91c7 c867 1430  .L....V......g.0
+00001ef0: 128c 2423 c548 633f da5a a15b 5f0d ead8  ..$#.Hc?.Z.[_...
+00001f00: 09ce 8c74 5066 a403 ce48 6b68 67c6 db8b  ...tPf...Hkhg...
+00001f10: 8260 054e 4819 798c 7c46 0123 c148 3252  .`.NH.y.|F.#.H2R
+00001f20: 8c34 36a4 ad15 3a36 d6a0 90bd e0cc 4707  .46...:6......G.
+00001f30: 653e 3ae0 7cb4 8676 a65c bd22 0896 e06c  e>:.|..v.\."...l
+00001f40: 9491 c7c8 6714 3012 8c24 23c5 4863 5fda  ....g.0..$#.Hc_.
+00001f50: 5ae2 b8fe 1ad4 b333 9cb9 e8a0 cc45 079c  Z......3.....E..
+00001f60: 8bd6 d0de cc9d 2798 1c87 32f2 18f9 8c02  ......'...2.....
+00001f70: 4682 9164 a418 69ec 4b5b 671c d75f 837a  F..d..i.K[g.._.z
+00001f80: 7686 3305 1d94 29e8 8053 d01a da99 f9eb  v.3...)..S......
+00001f90: 8541 b005 879f 8c3c 463e a380 9160 2419  .A.....<F>...`$.
+00001fa0: 2946 1a9b d2d6 1647 34d7 a098 3de1 cc3c  )F.....G4...=..<
+00001fb0: 0765 e639 e0cc b386 ca69 5772 5ab0 0487  .e.9.....iWrZ...
+00001fc0: 9e8c 3c46 3ea3 8091 6024 1929 461a 7bd2  ..<F>...`$.)F.{.
+00001fd0: d612 dd7b 6b50 cb8e 70a6 9e83 32f5 1c70  ...{kP..p...2..p
+00001fe0: ea59 43e5 acf1 6a0f f883 f34e 461e 239f  .YC...j....NF.#.
+00001ff0: 51c0 4830 928c 1423 8d1d 6aeb 8fb7 eab4  Q.H0...#..j.....
+00002000: c14a ec16 67d2 3928 93ce 0127 9d35 d4b8  .J..g.9(...'.5..
+00002010: 06f7 a184 534f 461e 239f 51c0 4830 928c  ....SOF.#.Q.H0..
+00002020: 1423 8ded 696b 9537 69b3 c132 ec13 6702  .#..ik.7i..2..g.
+00002030: 3a2c 13d0 2105 669f d2b4 f1f6 9509 2ab6  :,..!.f.......*.
+00002040: af9a 5b59 b361 5028 d35e aeec 6da5 bd46  ..[Y.aP(.^..m..F
+00002050: ed0c b557 c57d a5a9 5d65 692f 793e c3ef  ...W.}..]ei/y>..
+00002060: ddd8 ecd1 da55 2fac 94fd 6511 1777 d3f7  .....U/...e..w..
+00002070: c2bb 555c fca7 ecc5 37ff b3f3 ecd7 5eb8  ..U\....7.....^.
+00002080: 5af4 9e59 bab6 f3e8 f695 f57e 4937 f3fb  Z..Y.......~I7..
+00002090: 5e98 f68a fdea 3d6f d8af ef9a 6ee3 c5f9  ^.....=o....n...
+000020a0: 55b6 bae9 76de 9aae f43c 23c1 4832 528c  U...v....<#.H2R.
+000020b0: 344e bfed bd93 1dbd 6150 c837 4f3a 73db  4N......aP.7O:s.
+000020c0: 6199 db0e 290a fcf4 3d4a e1bd 9613 1445  a...)...=J.....E
+000020d0: e98b 0c8c ce89 2e23 0f87 7359 88e3 5e46  .......#..sY..^F
+000020e0: 8291 64a4 1869 9c7e 5b0b 75ec ba41 215b  ..d..i.~[.u..A![
+000020f0: c819 f70e cbb8 7748 19e2 f33b ae1a 1d84  ......wH...;....
+00002100: b967 984e b349 b46a 7a5a c1b4 a6aa d887  .g.N.I.jzZ......
+00002110: 5360 1c2b cd92 68d5 f498 069f ab05 8c04  S`.+..h.........
+00002120: 23c9 4831 d2dc a596 cee9 d26d 832a b68d  #.H1.......m.*..
+00002130: 331b 1e56 eedb a7b8 f190 6d38 dbac 9e64  3..V......m8...d
+00002140: 3e15 8043 d081 9bfb 0fdc dd4f 03bb 0e41  >..C.......O...A
+00002150: 076e fe3f 70f7 ff81 dbff 0fdc ff7f e001  .n.?p...........
+00002160: 006f f504 80a3 fb6f b004 bbca 9932 0fcb  .o.....o.....2..
+00002170: 9479 4851 a5f4 a6f8 1414 1445 e98b 0ccc  .yHQ.......E....
+00002180: c4c1 3323 0f87 7399 8953 6946 8291 64a4  ..3#..s..SiF..d.
+00002190: 1869 9c7e 5b33 75ec ba41 215b c819 470f  .i.~[3u..A![..G.
+000021a0: cb38 7a48 99a6 5ca5 59b8 7c3a 95c6 5323  .8zH..\.Y.|:..S#
+000021b0: 0e54 f7e5 6029 4eac 1979 38ac cb52 1c67  .T..`)N..y8..R.g
+000021c0: 3312 8c24 23c5 48e3 f4db 5aea c8ee 1b2c  3..$#.H...Z....,
+000021d0: c0d6 72e6 d9c3 32cf 1e52 34fa 79f3 7063  ..r...2..R4.y.pc
+000021e0: 932f b793 65b8 b0cd c728 8e64 77c5 602b  ./..e....(.dw.`+
+000021f0: 4ebc 1979 38a8 cb56 1c87 3312 8c24 23c5  N..y8..V..3..$#.
+00002200: 48e3 f4db daea a8de 1b94 b3a9 9c81 f8b0  H...............
+00002210: 0cc4 8794 ae3e ddf6 80e7 5207 6ec5 df2a  .....>....R.n..*
+00002220: f12c 9c93 7246 1e0e 77e0 2c9c 1374 4682  .,..rF..w.,..tF.
+00002230: 9164 a418 696e 544b 1775 6cb8 4121 fbc7  .d..inTK.ul.A!..
+00002240: 199f 0fcb f87c 4879 abc3 3f3f 15f8 9635  .....|Hy..??...5
+00002250: e0b8 c4b1 3a23 0fc7 761d 9738 7367 2418  ....:#..v..8sg$.
+00002260: 4946 8a91 c6e9 b775 d45b 6c81 c12a 6c2f  IF.....u.[l..*l/
+00002270: 67de 3e2c f3f6 21c5 b457 7116 275f 92c8  g.>,..!..Wq.'_..
+00002280: aeb2 909e 3a89 e228 dd97 83bf 388b 67e4  ....:..(....8.g.
+00002290: e1b0 2e7f 7150 cf48 3092 8c14 238d d36f  ....qP.H0...#..o
+000022a0: ebaf 23bb 6fb0 005b cb19 d18f ca88 7e84  ..#.o..[......~.
+000022b0: d977 313b 3a45 47d5 f3aa f8dc bca6 2ccd  .w1;:EG.......,.
+000022c0: c4c8 c3f1 1c66 e292 0123 c148 3252 8c34  .....f...#.H2R.4
+000022d0: 4ebf ed93 e2ba b6dd a092 1f0b e78c c047  N..............G
+000022e0: 6504 3ec2 c7c7 dabf 3776 d5f8 a0cc 098a  e.>.....7v......
+000022f0: b679 fe8b 126c c429 3823 0f47 fc6c c30f  .y...l.)8#.G.l..
+00002300: efcf 47ef 6fc7 e1d9 6874 3e18 7f38 1f84  ..G.o...ht>..8..
+00002310: c3c1 f836 7c7f 7376 7633 1837 9a8b b371  ...6|.svv3.7...q
+00002320: 4682 9164 a418 695c 545b 7375 df0e 835a  F..d..i\T[su...Z
+00002330: b697 331e 1f95 f1f8 8862 d4eb cd7a 1d27  ..3......b...z.'
+00002340: 59fe a3cd 3cdb 24f4 648b 0916 88d2 a612  Y...<.$.d.......
+00002350: e039 8ece 1979 38b4 ebd0 c5f9 3923 c148  .9...y8.....9#.H
+00002360: 3252 8c34 4ebf adbb de60 070c 1661 9b39  2R.4N....`...a.9
+00002370: e3f4 5119 a78f ba25 d413 d4e5 7f95 1cb8  ..Q....%........
+00002380: 0638 ade9 2a86 e21c 1d47 3b30 94cf f502  .8..*....G;0....
+00002390: 4682 9164 a418 69ee 544b 3775 ebb8 411d  F..d..i.TK7u..A.
+000023a0: 1bc8 fd1c ddca 8374 bba5 d213 d43d 3da2  .......t.....==.
+000023b0: 85de 2d31 ade9 2a06 3af0 485d 1a8d c6f1  ..-1..*.:.H]....
+000023c0: b958 c048 3092 8c14 23cd 6d6a e99e 6eed  .X.H0...#.mj..n.
+000023d0: 36a8 63f7 3843 f351 199a 8fba 05d0 13d4  6.c.8C.Q........
+000023e0: 15cb d964 7275 bdb6 8dcf 539f d694 15ff  ...dru....S.....
+000023f0: 7050 8ee3 dd2e e3b0 d93f 1c91 3312 8c24  pP.......?..3..$
+00002400: 23c5 4873 a35a faa7 6bc3 0d2a d941 ce6c  #.Hs.Z..k..*.A.l
+00002410: 7c54 66e3 a36e 59f3 0475 4f0b fab2 c9d8  |Tf..nY..uO.....
+00002420: 421c 8a33 f270 40b6 10c7 e18c 0423 c948  B..3.p@......#.H
+00002430: 31d2 dca9 9616 eadc 7183 52f6 9033 0a1f  1.......q.R..3..
+00002440: 9551 f888 9252 9787 0e44 b3b3 287c b099  .Q...R...D..(|..
+00002450: 4d1a 0dc4 5138 230f 4763 0371 12ce 4830  M...Q8#.Gc.q..H0
+00002460: 928c 1423 cd6d 6a69 a06e ed36 a863 f738  ...#.mji.n.6.c.8
+00002470: 83f0 5119 848f baa5 ca13 d4e5 cbf1 bee7  ..Q.............
+00002480: 6b59 854b d97c 00e2 f49b 9187 e3a5 7829  kY.K.|........x)
+00002490: 85ab 058c 0423 c948 31d2 dca9 9606 eada  .....#.H1.......
+000024a0: 7183 4ab6 9033 ec1e 9561 f7a8 5b70 3c41  q.J..3...a..[p<A
+000024b0: 5dbe 20b1 b979 faa0 a746 0771 becd c8c3  ]. ..y...F.q....
+000024c0: e1f8 08c4 c936 23c1 4832 528c 34f7 a9a5  .....6#.H2R.4...
+000024d0: 813a f6db a090 fde3 4cb4 c765 a23d ee96  .:......L..e.=..
+000024e0: 154f 5097 afe7 c03b 9fa6 355d 691f 461e  .OP....;..5]i.F.
+000024f0: 8e76 6028 9feb 058c 0423 c948 31d2 dca9  .v`(.....#.H1...
+00002500: 961f 72d1 ade3 0675 fc21 17ce 307b 5c86  ..r....u.!..0{\.
+00002510: d9e3 6eef 959e a0ae 588e fb7d 4fd3 9abe  ..n.....X..}O...
+00002520: 6224 ceb4 71d4 9f18 d2e7 ba01 23c1 4832  b$..q.......#.H2
+00002530: 528c 3477 aea5 a18e db01 837a 3696 33c6  R.4w.......z6.3.
+00002540: 1e97 31f6 b85b 143c 415d be2c 137e bf8e  ..1..[.<A].,.~..
+00002550: 37ab c5f6 0a75 a3ab 38b5 66e4 e190 f8ea  7....u..8.f.....
+00002560: c6c5 0246 8291 64a4 1869 ee55 4b2b 1dd1  ...F..d..i.UK+..
+00002570: 7383 62f6 9133 a71e 9739 f5b8 634e 8dba  s.b..3...9..cN..
+00002580: 7c4d ce77 cf4d 6bea 8a91 38ad c631 9d03  |M.w.Mk...8..1..
+00002590: fa5c 3560 2418 4946 8a91 e6ae b574 d431  .\5`$.IF.....t.1
+000025a0: dd37 a866 4b39 93eb 7199 5c8f 3b26 d7a8  .7.fK9..q.\.;&..
+000025b0: cb17 7555 7c8c 231f 9738 bb66 e4e1 787c  ..uU|.#..8.f..x|
+000025c0: 5ce2 ec9a 9160 2419 2946 9a1b d5d2 455d  \....`$.)F....E]
+000025d0: 1b6e 50c9 0e72 7f34 5ce5 b3e1 3aa6 d7a8  .nP..r.4\...:...
+000025e0: 2b16 e47e 7bd3 b4a6 aff8 e8c0 47c8 d1a8  +..~{.......G...
+000025f0: 3f31 a4cf 7503 4682 9164 a418 69ee 5c4b  ?1..u.F..d..i.\K
+00002600: 4b1d b703 06f5 6c2c 67a8 3d2e 43ed 71c7  K.....l,g.=.C.q.
+00002610: 501b 752f cbc2 f370 8eb4 1979 38dc a1b1  P.u/...p...y8...
+00002620: 7c2e 1830 128c 2423 c548 73af 5a5a a963  |..0..$#.Hs.ZZ.c
+00002630: cf0d 0ad9 43ce 507b 5c86 dae3 8ea1 36ea  ....C.P{\.....6.
+00002640: f2f5 fce4 7b4f a6b5 1a15 3b71 c08d 23ff  ....{O....;q..#.
+00002650: e4b0 3ed7 0e18 0946 9291 62a4 b983 2d9d  ..>....F..b...-.
+00002660: 75fc 4e18 acc1 2673 66df e332 fb1e 77cc  u.N...&sf..2..w.
+00002670: be51 572c edd1 aeb3 4f89 6dfc 3c8b 9ab0  .QW,....O.m.<...
+00002680: e22c 8ebe 7138 3e85 e2e4 9b91 6024 1929  .,..q8>.....`$.)
+00002690: 469a fbd4 d24a 1dfb 6d50 c8fe 7106 dfe3  F....J..mP..q...
+000026a0: 32f8 1e77 0cbe 51b7 f779 0c78 4ff0 b456  2..w..Q..y.xO..V
+000026b0: a162 244e c071 5c1e c9e7 7201 23c1 4832  .b$N.q\...r.#.H2
+000026c0: 528c 34b7 aca5 958e 6dbd c10a ec29 6718  R.4.....m....)g.
+000026d0: 7e5e 86e1 e71d c370 d4ed 2eec d0a7 edd4  ~^.....p........
+000026e0: 4a94 a662 e431 f219 058c 0423 c948 31d2  J..b.1.....#.H1.
+000026f0: dc9a 969f e97b 748b 0d96 e08f f375 06e1  .....{t......u..
+00002700: e765 107e de31 0847 ddde cae0 b3ee a735  .e.~.1.G.......5
+00002710: 7dc5 391c 84e3 a829 5ed2 e56a 0123 c148  }.9....)^..j.#.H
+00002720: 3252 8c34 f7ab a5a3 8eeb bb41 3ddb c919  2R.4.......A=...
+00002730: 7f9f 97f1 f779 c7f8 1b75 bbcb 3a78 abdd  .....y...u..:x..
+00002740: b456 a4e2 298e c171 e883 83f9 5c31 6024  .V..)..q....\1`$
+00002750: 1849 468a 91e6 c6b5 f4d5 1b6c 80c1 226c  .IF........l.."l
+00002760: 2ece c44f d37b 6bb3 e2f1 6697 17eb f0ce  ...O.{k...f.....
+00002770: 9a30 b98b 5669 6f69 6f73 c5d9 bbf7 e393  .0..Vioios......
+00002780: 5e52 5c7f 7ef9 268b d71f 4f72 b3de c459  ^R\.~.&...Or...Y
+00002790: 163f 6cbf bcb7 e1c2 26c5 2fe4 fc36 8eb3  .?l.....&./..6..
+000027a0: d76f 8a61 1ee3 e4db 7690 cbff 0350 4b03  .o.a....v....PK.
+000027b0: 0414 0000 0008 00f6 50f9 56f7 f68f 09a7  ........P.V.....
+000027c0: 0200 006d 0b00 000d 0000 0078 6c2f 7374  ...m.......xl/st
+000027d0: 796c 6573 2e78 6d6c dd56 db8e 9b30 10fd  yles.xml.V...0..
+000027e0: 15c4 0794 4d50 51a8 42a4 36d2 4a95 da6a  ....MPQ.B.6.J..j
+000027f0: a5dd 87be 9a60 8225 5fa8 31ab 64bf be33  .....`.%_.1.d..3
+00002800: b613 92ec 0edd f6b1 a084 f11c 9fb9 3b64  ..............;d
+00002810: 3db8 a3e4 8f1d e72e 3928 a987 2aed 9ceb  =.......9(..*...
+00002820: 3f65 d9b0 ebb8 62c3 07d3 730d 486b ac62  ?e....b...s.Hk.b
+00002830: 0e96 769f 0dbd e5ac 1990 a464 b6bc bb2b  ..v........d...+
+00002840: 32c5 844e 376b 3daa 7be5 8664 6746 edaa  2..N7k=.{..dgF..
+00002850: f42e 4db2 cdba 357a 522d d3a0 80bd 4cf1  ..M...5zR-....L.
+00002860: e499 c92a dd32 296a 2bc2 66a6 843c 06fd  ...*.2)j+.f..<..
+00002870: d26b 7646 1a9b 3888 8657 e9c2 ab86 97b0  .kvF..8..W......
+00002880: 6111 9718 6ab4 a584 36d6 6bb3 e026 7cd7  a...j...6.k..&|.
+00002890: 9170 89f8 c700 3b84 94d7 f181 62b3 ee99  .p....;.....b...
+000028a0: 73dc ea7b 5804 92d7 bec6 a2fc 74ec 21be  s..{X.......t.!.
+000028b0: bd65 c7c5 f263 7ac1 f00f 7053 1bdb 707b  .e...cz...pS..p{
+000028c0: e528 a836 6bc9 5b87 0c2b f69d 179c e9f1  .(.6k.[..+......
+000028d0: 511b e78c 42a9 116c 6f34 0b91 9c68 5774  Q...B..lo4...hWt
+000028e0: dfc8 2a75 1d34 62b2 75ab 45c3 b7ba e8e5  ..*u.4b.u.E.....
+000028f0: 567d 7613 0548 61c7 a57c c46d 3fdb 731e  V}v..Ha..|.m?.s.
+00002900: 0bc8 e3d0 26a1 f35f 1bdf 742c ec49 84e4  ....&.._..t,.I..
+00002910: a318 ccc4 053a b834 178c 5fd8 5dfe 9bdd  .....:.4.._.]...
+00002920: 5e3c 1bf7 6584 8cb4 5fff 1a8d e30f 96b7  ^<..e..._.......
+00002930: e2e0 d787 760a 8032 bf20 cc83 9ef5 bd3c  ....v..2. .....<
+00002940: 7e96 62af 150f d9bf dbe3 66cd 4ebc a433  ~.b.......f.N..3
+00002950: 56bc 8037 9cc9 1d28 388c ec33 b74e ec50  V..7...(8..3.N.P
+00002960: 034d 0a05 3ab4 b14a e702 f972 5dd5 feac  .M..:..J...r]...
+00002970: 4df0 4055 e90f 3ca8 f222 d17a 14d2 091d  M.@U..<..".z....
+00002980: 579d 681a ae5f b700 ec3b 56c3 4fc1 9503  W.h.._...;V.O...
+00002990: d8d5 f096 8dd2 3d9d c12a 9de4 efbc 11a3  ......=..*......
+000029a0: 2acf bb1e b016 71d7 247f c351 5c14 d369  *.....q.$..Q\..i
+000029b0: 0667 4237 fcc0 9b6d 5cda 7ded c504 0470  .gB7...m\.}....p
+000029c0: 1baf 30c8 37d0 bdbf 0888 6405 9080 1024  ..0.7.....d....$
+000029d0: 7d91 6190 acc0 237d fd8f 79ad e8bc 0248  }.a...#}..y....H
+000029e0: 46b8 7a1b 5ad1 ac15 cd0a bc37 a1ad bf49  F.z.Z......7...I
+000029f0: 5f04 ab84 8b48 b92c f3bc 28c8 f26e b76f  _....H.,..(..n.o
+00002a00: 87b1 256b 5814 f821 0c92 1122 87f4 85de  ..%kX..!..."....
+00002a10: feb6 f233 0330 3336 7f98 0db2 cbb3 6343  ...3.036......cC
+00002a20: a63c 33a2 64ca 3395 4788 a821 72ca 9218  .<3.d.3.G..!r...
+00002a30: 00d2 1772 c8a6 9013 8541 10be 70d4 0856  ...r.....A..p..V
+00002a40: 9e63 9fc9 08c9 633e 0395 2509 e190 12d3  .c....c>..%.....
+00002a50: 5b14 54a1 0abc 897e 9187 28cf cb92 8010  [.T....~..(.....
+00002a60: 24c2 c873 12c2 033b 0391 6160 2024 94e7  $..s...;..a` $..
+00002a70: e145 7af3 3ecb 4eef b96c fa83 bdf9 0d50  .Ez.>.N..l.....P
+00002a80: 4b03 0414 0000 0008 00f6 50f9 56b7 47eb  K.........P.V.G.
+00002a90: 8ac0 0000 0016 0200 000b 0000 005f 7265  ............._re
+00002aa0: 6c73 2f2e 7265 6c73 9d92 4b6e 0231 0c40  ls/.rels..Kn.1.@
+00002ab0: af12 655f 4ca9 c402 31ac d8b0 4388 0bb8  ..e_L...1...C...
+00002ac0: 89e7 a399 c491 63c4 f4f6 8dd8 c020 6811  ......c...... h.
+00002ad0: 4bff 9e9e 2daf 0f34 a076 1c73 dba5 6cc6  K...-..4.v.s..l.
+00002ae0: 30c4 5cd9 5635 ad00 b26b 2960 9e71 a258  0.\.V5...k)`.q.X
+00002af0: 2a35 4b40 2da1 3490 d0f5 d810 2ce6 f325  *5K@-.4.....,..%
+00002b00: c82d c36e d6b7 4c73 fc49 f40a 91eb ba73  .-.n..Ls.I.....s
+00002b10: b465 770a 14f5 01f8 aec3 9a23 4a43 5ad9  .ew........#JCZ.
+00002b20: 7180 334b ffcd dccf 0ad4 9a9d afac ecfc  q.3K............
+00002b30: a735 f0a6 ccf3 f520 90a2 4745 702c f491  .5..... ..GEp,..
+00002b40: a44c 8b76 94af 3e9e ddbe a4f3 a563 62b4  .L.v..>......cb.
+00002b50: 78df e8ff f3d0 a814 3df9 bf9d 30a5 89d2  x.......=...0...
+00002b60: d745 0926 6fb0 f905 504b 0304 1400 0000  .E.&o...PK......
+00002b70: 0800 f650 f956 b948 9c76 5201 0000 ae02  ...P.V.H.vR.....
+00002b80: 0000 0f00 0000 786c 2f77 6f72 6b62 6f6f  ......xl/workboo
+00002b90: 6b2e 786d 6c8d 91dd 4e83 4010 855f 85ec  k.xml...N.@.._..
+00002ba0: 0308 a5da c4a6 f4a6 8dda c4bf 58e3 fd00  ............X...
+00002bb0: 4399 747f c8ee d06a 9fde 5d08 8a69 d278  C.t....j..]..i.x
+00002bc0: b5cc 99d9 8f39 6717 4763 f7b9 31fb e853  .....9g.Gc..1..S
+00002bd0: 49ed e636 1335 7333 8f63 57d4 a8c0 5d99  I..6.5s3.cW...].
+00002be0: 06b5 ef55 c62a 605f da5d 6caa 8a0a 5c9b  ...U.*`_.]l...\.
+00002bf0: a255 a839 4e93 6416 5b94 c064 b4ab a971  .U.9N.d.[..d...q
+00002c00: a2a7 fd87 e51a 8b50 ba1a 9195 ec51 0a48  .......P.....Q.H
+00002c10: 8be5 62d8 ecd5 46f1 b832 8c45 f853 5083  ..b...F..2.E.SP.
+00002c20: f241 7874 bf03 a18c 0ee4 2827 49fc 9589  .Axt......('I...
+00002c30: ee5b a288 1469 5274 c232 1389 885c 6d8e  .[...iRt.2...\m.
+00002c40: 0fc6 d2c9 6806 b92d ac91 3213 93be f181  ....h..-..2.....
+00002c50: 96a9 3893 b761 cd77 c85d a730 e46f c173  ..8..a.w.].0.o.s
+00002c60: 2666 8907 5664 1d77 131d 1ffc 9207 f4c3  &f..Vd.w........
+00002c70: 7dd5 b2b9 23c9 68d7 c078 6f4d db90 de75  }...#.h..xoM...u
+00002c80: 186f 231e f9e8 a218 ce48 83c2 4c3c 2143  .o#......H..L<!C
+00002c90: 090c 610b af6e ca7e 23f6 a891 3f3b 27df  ..a..n.~#...?;'.
+00002ca0: b09b b287 8e01 2b09 cea1 1bdd 4f2f dc4f  ......+.....O/.O
+00002cb0: cfee fbd4 9b10 c91f c4f4 0262 dafb 1acc  ...........b....
+00002cc0: 9458 91c6 f2d9 c35c 68f8 680b ffae e1e8  .X.....\h.h.....
+00002cd0: cca4 d737 935b 1f61 2be5 ca6b 2ffa d140  ...7.[.a+..k/..@
+00002ce0: f993 cef0 b4cb 6f50 4b03 0414 0000 0008  ......oPK.......
+00002cf0: 00f6 50f9 560b 085d 06bc 0000 001f 0300  ..P.V..]........
+00002d00: 001a 0000 0078 6c2f 5f72 656c 732f 776f  .....xl/_rels/wo
+00002d10: 726b 626f 6f6b 2e78 6d6c 2e72 656c 73cd  rkbook.xml.rels.
+00002d20: 9339 0e83 3010 45af 62f9 000c 4b92 2282  .9..0.E.b...K.".
+00002d30: 5469 6823 2e60 c1b0 88c5 9667 a2c0 ed83  Tih#.`.....g....
+00002d40: a000 4b29 d2a0 a4b2 fe58 7eff 15e3 f881  ..K).....X~.....
+00002d50: 9de2 460f 5437 86c4 d877 0325 b266 3657  ..F.T7...w.%.f6W
+00002d60: 00ca 6bec 1579 dae0 30df 94da f68a e768  ..k..y..0......h
+00002d70: 2b30 2a6f 5585 10fa fe05 ec9e 216f f19e  +0*oU.......!o..
+00002d80: 29b2 c9e0 3744 5d96 4d8e 779d 3f7b 1cf8  )...7D].M.w.?{..
+00002d90: 0318 5eda b654 23b2 1499 b215 7222 61ec  ..^..T#.....r"a.
+00002da0: b631 c172 04de 4c96 222d 1269 d322 9002  .1.r..L."-.i."..
+00002db0: 7e6d 143a 46e1 1f18 458e 5174 a411 f1d4  ~m.:F...E.Qt....
+00002dc0: 216d 3a6b 76fa 4f47 f6f3 fc16 b7fa 25ae  !m:kv.OG......%.
+00002dd0: 4377 51ce 8b04 38ff e1f6 0650 4b03 0414  CwQ...8....PK...
+00002de0: 0000 0008 00f6 50f9 56db fbce 8f24 0100  ......P.V....$..
+00002df0: 00e9 0400 0013 0000 005b 436f 6e74 656e  .........[Conten
+00002e00: 745f 5479 7065 735d 2e78 6d6c cd54 cb4e  t_Types].xml.T.N
+00002e10: c330 10fc 95c8 d72a 7129 1207 d4f4 025c  .0.....*q).....\
+00002e20: a107 7ec0 249b c68a 5ff2 6e4b faf7 6c12  ..~.$..._.nK..l.
+00002e30: 1a09 545a aa20 d14b ac78 6767 c63b b297  ..TZ. .K.xgg.;..
+00002e40: affb 0098 b4d6 38cc 454d 14ee a5c4 a206  ......8.EM......
+00002e50: ab30 f301 1c57 2a1f ad22 fe8d 1b19 54d1  .0...W*.."....T.
+00002e60: a80d c8c5 7c7e 270b ef08 1ca5 d471 88d5  ....|~'......q..
+00002e70: f211 2ab5 3594 3cb5 bc8d dabb 5c44 3028  ..*.5.<.....\D0(
+00002e80: 9287 01d8 69e5 4285 6074 a188 eb72 e7ca  ....i.B.`t...r..
+00002e90: 6f2a e9a7 42c6 9d3d 066b 1d70 c600 91c8  o*..B..=.k.p....
+00002ea0: a312 7de9 4785 43e3 cb0e 62d4 2524 6b15  ..}.G.C...b.%$k.
+00002eb0: e959 5986 c9d6 48a4 bd01 cc4e 731c 71e9  .YY...H....Ns.q.
+00002ec0: ab4a 1750 fa62 6bb9 25c3 1041 9558 0390  .J.P.bk.%..A.X..
+00002ed0: 35d9 403a 3b23 4d3c 6418 be37 930d f434  5.@:;#M<d..7...4
+00002ee0: 2715 19ba 8e3e 20a7 16e1 72bd 432c 5d77  '....> ...r.C,]w
+00002ef0: 1a98 0822 e933 871c 2599 7bf2 09a1 4bbc  ...".3..%.{...K.
+00002f00: 84f2 b7e2 3ce1 771f 9b3e 1394 fd32 7dcc  ....<.w..>...2}.
+00002f10: 5f73 1ef9 2f35 b2b8 1623 b7ff 69e4 cdfb  _s../5...#..i...
+00002f20: e6af 6f5e b766 5669 371a 90fd 0bb7 fa00  ..o^.fVi7.......
+00002f30: 504b 0102 1403 1400 0000 0800 f650 f956  PK...........P.V
+00002f40: 465a c10c 8200 0000 b100 0000 1000 0000  FZ..............
+00002f50: 0000 0000 0000 0000 8001 0000 0000 646f  ..............do
+00002f60: 6350 726f 7073 2f61 7070 2e78 6d6c 504b  cProps/app.xmlPK
+00002f70: 0102 1403 1400 0000 0800 f650 f956 99aa  ...........P.V..
+00002f80: f383 eb00 0000 cb01 0000 1100 0000 0000  ................
+00002f90: 0000 0000 0000 8001 b000 0000 646f 6350  ............docP
+00002fa0: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
+00002fb0: 0214 0314 0000 0008 00f6 50f9 5699 5c9c  ..........P.V.\.
+00002fc0: 2310 0600 009c 2700 0013 0000 0000 0000  #.....'.........
+00002fd0: 0000 0000 0080 01ca 0100 0078 6c2f 7468  ...........xl/th
+00002fe0: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
+00002ff0: 0102 1403 1400 0000 0800 f650 f956 e0d9  ...........P.V..
+00003000: 6c24 3d02 0000 a307 0000 1800 0000 0000  l$=.............
+00003010: 0000 0000 0000 8081 0b08 0000 786c 2f77  ............xl/w
+00003020: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00003030: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00003040: f650 f956 19c6 63fc 000e 0000 bb83 0000  .P.V..c.........
+00003050: 1800 0000 0000 0000 0000 0000 8081 7e0a  ..............~.
+00003060: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00003070: 7368 6565 7432 2e78 6d6c 504b 0102 1403  sheet2.xmlPK....
+00003080: 1400 0000 0800 f650 f956 ba52 73fa c30e  .......P.V.Rs...
+00003090: 0000 6f8b 0000 1800 0000 0000 0000 0000  ..o.............
+000030a0: 0000 8081 b418 0000 786c 2f77 6f72 6b73  ........xl/works
+000030b0: 6865 6574 732f 7368 6565 7433 2e78 6d6c  heets/sheet3.xml
+000030c0: 504b 0102 1403 1400 0000 0800 f650 f956  PK...........P.V
+000030d0: f7f6 8f09 a702 0000 6d0b 0000 0d00 0000  ........m.......
+000030e0: 0000 0000 0000 0000 8001 ad27 0000 786c  ...........'..xl
+000030f0: 2f73 7479 6c65 732e 786d 6c50 4b01 0214  /styles.xmlPK...
+00003100: 0314 0000 0008 00f6 50f9 56b7 47eb 8ac0  ........P.V.G...
+00003110: 0000 0016 0200 000b 0000 0000 0000 0000  ................
+00003120: 0000 0080 017f 2a00 005f 7265 6c73 2f2e  ......*.._rels/.
+00003130: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
+00003140: f650 f956 b948 9c76 5201 0000 ae02 0000  .P.V.H.vR.......
+00003150: 0f00 0000 0000 0000 0000 0000 8001 682b  ..............h+
+00003160: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
+00003170: 6c50 4b01 0214 0314 0000 0008 00f6 50f9  lPK...........P.
+00003180: 560b 085d 06bc 0000 001f 0300 001a 0000  V..]............
+00003190: 0000 0000 0000 0000 0080 01e7 2c00 0078  ............,..x
+000031a0: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+000031b0: 2e78 6d6c 2e72 656c 7350 4b01 0214 0314  .xml.relsPK.....
+000031c0: 0000 0008 00f6 50f9 56db fbce 8f24 0100  ......P.V....$..
+000031d0: 00e9 0400 0013 0000 0000 0000 0000 0000  ................
+000031e0: 0080 01db 2d00 005b 436f 6e74 656e 745f  ....-..[Content_
+000031f0: 5479 7065 735d 2e78 6d6c 504b 0506 0000  Types].xmlPK....
+00003200: 0000 0b00 0b00 ca02 0000 302f 0000 0000  ..........0/....
```

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/ontologies/wind-energy.owl` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/ontologies/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/basic/workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from cognite.client import CogniteClient
 
-from cognite.neat.core.workflow.base import BaseWorkflow
-from cognite.neat.core.workflow.model import FlowMessage
+from cognite.neat.workflows.workflow import BaseWorkflow
+from cognite.neat.workflows.workflow import FlowMessage
 
 
 class BasicNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
         self.metrics.register_metric("counter_1", "", "counter", ["step"])
```

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/default/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
-from cognite.neat.core import loader, rules
-from cognite.neat.core.extractors.cdfcore.labels import upload_labels
-from cognite.neat.core.extractors.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
-from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
+from cognite.neat import rules
+from cognite.neat.graph import extractors
+from cognite.neat.graph.loaders.cdfcore.labels import upload_labels
+from cognite.neat.graph.loaders.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
+from cognite.neat.graph.loaders.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
-from cognite.neat.core.loader.graph_store import NeatGraphStore, drop_graph_store
-from cognite.neat.core.rules.exporter.rules2triples import get_instances_as_triples
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.transformer import RuleProcessingReport, domain2app_knowledge_graph
-from cognite.neat.core.validator import validate_asset_hierarchy
-from cognite.neat.core.workflow import utils
-from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.core.workflow.cdf_store import CdfStore
+from cognite.neat.graph.extractors import NeatGraphStore, drop_graph_store
+from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.graph.transformations.transformer import RuleProcessingReport, domain2app_knowledge_graph
+from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
+from cognite.neat.workflows.workflow import utils
+from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.workflow.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_default_wf_cdf_resource_stats",
         "CDF resource stats before and after running default workflow",
         ["resource_type", "state"],
     )
@@ -78,26 +79,26 @@
         solution_store_dir = self.get_config_item_value("solution_rdf_store.disk_store_dir", None)
         source_store_dir = Path(source_store_dir) if source_store_dir else None
         solution_store_dir = Path(solution_store_dir) if solution_store_dir else None
         if clean_start:
             drop_graph_store(self.source_graph, source_store_dir)
             drop_graph_store(self.solution_graph, solution_store_dir)
 
-        self.source_graph = loader.NeatGraphStore(
+        self.source_graph = extractors.NeatGraphStore(
             prefixes=self.transformation_rules.prefixes, base_prefix="nordic44", namespace="http://purl.org/nordic44#"
         )
         self.graph_source_type = self.get_config_item_value("source_rdf_store.type", self.graph_source_type)
         self.source_graph.init_graph(
             self.graph_source_type,
             self.get_config_item_value("source_rdf_store.query_url"),
             self.get_config_item_value("source_rdf_store.update_url"),
             "neat-tnt",
             internal_storage_dir=source_store_dir,
         )
-        self.solution_graph = loader.NeatGraphStore(prefixes=self.transformation_rules.prefixes)
+        self.solution_graph = extractors.NeatGraphStore(prefixes=self.transformation_rules.prefixes)
         self.solution_graph.init_graph(
             self.get_config_item_value("solution_rdf_store.type"),
             self.get_config_item_value("solution_rdf_store.query_url"),
             self.get_config_item_value("solution_rdf_store.update_url"),
             "tnt-solution",
             internal_storage_dir=solution_store_dir,
         )
```

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
-from cognite.neat.core import extractors, rules
-from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.workflow import utils
-from cognite.neat.core.workflow.base import BaseWorkflow
-from cognite.neat.core.workflow.cdf_store import CdfStore
-from cognite.neat.core.workflow.model import FlowMessage
+from cognite.neat import rules
+from cognite.neat.graph import loaders
+from cognite.neat.graph.extractors import NeatGraphStore
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.workflows.workflow import utils
+from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.workflow.cdf_store import CdfStore
 
 
 class FDMSchemaGenerationNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
         self.metrics.register_metric("counter_1", "", "counter", ["step"])
@@ -54,15 +54,15 @@
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_generate_fdm_schema(self, flow_msg: FlowMessage = None):
         logging.info("Generating FDM schema")
-        self.data_model_gql = extractors.rules2graphql_schema(self.transformation_rules)
+        self.data_model_gql = loaders.rules2graphql_schema(self.transformation_rules)
 
         default_name = (
             f"{self.transformation_rules.metadata.prefix}-"
             f"v{self.transformation_rules.metadata.version.strip().replace('.', '_')}"
             ".graphql"
         )
         schema_name = self.get_config_item_value("fdm_schema.file", default_name)
```

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import time
 from pathlib import Path
 
 import requests
 from cognite.client import CogniteClient
 
-from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.rules.models import TransformationRules
-from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
+from cognite.neat.graph.extractors import NeatGraphStore
+from cognite.neat.rules.models import TransformationRules
+from cognite.neat.workflows.workflow import BaseWorkflow, FlowMessage
 
 
 class GraphDbImportNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.dataset_id: int = 0
         self.current_step: str = None
```

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.18.0/cognite/neat/workflows/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.18.0/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer/explorer.py` & `cognite_neat-0.18.0/cognite/neat/app/api/explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,34 +12,34 @@
 from fastapi import FastAPI, UploadFile
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse, RedirectResponse
 from fastapi.staticfiles import StaticFiles
 from prometheus_client import REGISTRY, Counter, make_asgi_app
 
 from cognite import neat
-from cognite.neat import constants
-from cognite.neat.core import query_generator
-from cognite.neat.core import rules as rules_module
-from cognite.neat.core.app import NeatApp
-from cognite.neat.core.configuration import Config, configure_logging
-from cognite.neat.core.loader.config import copy_examples_to_directory
-from cognite.neat.core.workflow import WorkflowFullStateReport, utils
-from cognite.neat.core.workflow.base import WorkflowDefinition
-from cognite.neat.core.workflow.model import FlowMessage, WorkflowConfigItem
-from cognite.neat.explorer.data_classes.rest import (
+from cognite.neat import constants, rules as rules_module
+from cognite.neat.graph.transformations import query_generator
+from cognite.neat.app.api.app import NeatApp
+from cognite.neat.app.api.configuration import Config, configure_logging
+from cognite.neat.graph.extractors.config import copy_examples_to_directory
+from cognite.neat.workflows.workflow import WorkflowFullStateReport
+from cognite.neat.workflows.workflow import utils
+from cognite.neat.workflows.workflow.base import WorkflowDefinition
+from cognite.neat.workflows.workflow.model import FlowMessage, WorkflowConfigItem
+from cognite.neat.app.api.data_classes.rest import (
     DownloadFromCdfRequest,
     NodesAndEdgesRequest,
     QueryRequest,
     RuleRequest,
     RunWorkflowRequest,
     UploadToCdfRequest,
 )
-from cognite.neat.explorer.utils.data_mapping import rdf_result_to_api_response
-from cognite.neat.explorer.utils.query_templates import query_templates
-from cognite.neat.migration.wf_manifests import migrate_wf_manifest
+from cognite.neat.app.api.utils.data_mapping import rdf_result_to_api_response
+from cognite.neat.app.api.utils.query_templates import query_templates
+from cognite.neat.workflows.migration.wf_manifests import migrate_wf_manifest
 
 logger = getLogger(__name__)  # temporary logger before config is loaded
 config_path = Path(os.environ.get("NEAT_CONFIG_PATH", "config.yaml"))
 
 if os.environ.get("NEAT_CDF_PROJECT"):
     logger.info("ENV NEAT_CDF_PROJECT is set, loading config from env.")
     config = Config.from_env()
```

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.18.0/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.map` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.18.0/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.18.0/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.4/cognite/neat/steps/steps.py` & `cognite_neat-0.18.0/cognite/neat/workflows/steps/steps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from pathlib import Path
 from typing import Optional, Tuple
 
-from cognite.neat.core import loader
-from cognite.neat.core.extractors import upload_labels
-from cognite.neat.core.rules import load_rules_from_excel_file
-from cognite.neat.core.workflow.model import FlowMessage
-from cognite.neat.core.workflow.step_model import Step
+from ...graph import extractors
+from cognite.neat.graph.loaders import upload_labels
+from cognite.neat.rules import load_rules_from_excel_file
+from cognite.neat.workflows.workflow.model import FlowMessage
+from cognite.neat.workflows.workflow.step_model import Step
 from .data_contracts import ClientData, PathData, RulesData, SourceGraphData
 
 __all__ = [
     "LoadTransformationRules",
     "ConfiguringStores",
     "LoadInstancesToGraph",
     "CreateCDFLabels",
@@ -25,15 +25,15 @@
         return (FlowMessage(output_text="Rules loaded successfully std step"), RulesData(rules=rules))
 
 
 class ConfiguringStores(Step):
     def run(self, input_data: RulesData) -> Tuple[FlowMessage, SourceGraphData]:
         logging.info("Configuring stores")
         rules = input_data.rules
-        graph = loader.NeatGraphStore(prefixes=rules.prefixes, namespace=rules.metadata.namespace)
+        graph = extractors.NeatGraphStore(prefixes=rules.prefixes, namespace=rules.metadata.namespace)
         graph.init_graph(base_prefix=rules.metadata.prefix)
         logging.info("Store configured")
         return (FlowMessage(output_text="Stores Configured"), SourceGraphData(graph=graph))
 
 
 class LoadInstancesToGraph(Step):
     def run(self, rules: RulesData, graph_data: SourceGraphData) -> None:
```

### Comparing `cognite_neat-0.17.4/pyproject.toml` & `cognite_neat-0.18.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.17.4"
+version = "0.18.0"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
 homepage = "https://cognite-neat.readthedocs-hosted.com/"
 repository = "https://github.com/cognitedata/neat"
 packages = [
     { include="cognite", from="." },
 ]
 exclude = [
-    "cognite/neat/explorer-ui/neat-app/public/**",
-    "cognite/neat/explorer-ui/neat-app/src/**",
-    "cognite/neat/explorer-ui/neat-app/node_modules/**",
-    "cognite/neat/explorer-ui/neat-app/*.json",
+    "cognite/neat/app/ui/neat-app/public/**",
+    "cognite/neat/app/ui/neat-app/src/**",
+    "cognite/neat/app/ui/neat-app/node_modules/**",
+    "cognite/neat/app/ui/neat-app/*.json",
 ]
 
 
 [tool.black]
 line-length = 120
 target_version = ['py311']
 include = '\.py$'
 
 [tool.mypy]
 explicit_package_bases = true
 
 [tool.poetry.scripts]
-neat = "cognite.neat.main:run"
+neat = "cognite.neat.app.main:run"
 
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 pandas = "*"
 rdflib = "*"
 pydantic = "^2"
```

### Comparing `cognite_neat-0.17.4/PKG-INFO` & `cognite_neat-0.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.17.4
+Version: 0.18.0
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -217,20 +217,21 @@
 
  Must implement `BaseWorkflow` class from `from cognite.neat.core.workflow.base`
 
  Each method that should be orchestrated by workflow engine must be prefixed with `step_` , each method must have single argument of `FlowMessage` type and return `FlowMessage` or `None`.
  FlowMessage is passed from one step to another and it's captured in execution log.
 
 Simplest `workflow.py`
+
 ````python
 
 import logging
 from cognite.client import CogniteClient
-from cognite.neat.core.workflow.base import BaseWorkflow
-from cognite.neat.core.workflow.model import FlowMessage
+from cognite.neat.workflows.workflow import BaseWorkflow
+from cognite.neat.workflows.workflow import FlowMessage
 
 
 class PlaygroundNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
 
     def step_run_experiment_1(self, flow_msg: FlowMessage = None):
```

