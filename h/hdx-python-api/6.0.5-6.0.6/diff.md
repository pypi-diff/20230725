# Comparing `tmp/hdx_python_api-6.0.5.tar.gz` & `tmp/hdx_python_api-6.0.6.tar.gz`

## Comparing `hdx_python_api-6.0.5.tar` & `hdx_python_api-6.0.6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    43789 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/documentation/main.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/_version.py
--rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/configuration.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/hdx_base_configuration.yaml
--rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/locations.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/__init__.py
--rwxr-xr-x   0        0        0   112228 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/dataset.py
--rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0        0        0     5798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/date_helper.py
--rwxr-xr-x   0        0        0     3770 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0    28580 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/hdxobject.py
--rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/indicator_resource_view_template.yaml
--rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/organization.py
--rwxr-xr-x   0        0        0    26488 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/resource.py
--rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/resource_view.py
--rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/showcase.py
--rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/user.py
--rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/vocabulary.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/simple.py
--rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/Tag_Mapping_ChainRuleError.csv
--rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/dataset_search_results.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/empty.csv
--rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/organization_show_results.yaml
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/resource_formats.json
--rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/showcase_all_search_results.yaml
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/test_data.zip
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_base_config.yaml
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_email_configuration.yaml
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_organization_static.yaml
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_static.yaml
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_view_static.yaml
--rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_showcase_static.yaml
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_user_static.yaml
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_vocabulary_static.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/test_data_no_years.csv
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
--rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources.yaml
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources_new.yaml
--rwxr-xr-x   0        0        0    45085 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/api/test_locations.py
--rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/__init__.py
--rwxr-xr-x   0        0        0    49383 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_organization.py
--rwxr-xr-x   0        0        0    46355 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_resource.py
--rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_showcase.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_user.py
--rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_vocabulary.py
--rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/test_simple.py
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/my_code.py
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/my_resource.csv
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/my_resource.xlsx
--rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/run.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/LICENSE
--rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/README.md
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/pyproject.toml
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    44094 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/documentation/main.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/_version.py
+-rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/configuration.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/hdx_base_configuration.yaml
+-rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/locations.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0   112315 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/dataset.py
+-rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0        0        0     6263 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/date_helper.py
+-rwxr-xr-x   0        0        0     3777 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0    28580 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/indicator_resource_view_template.yaml
+-rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/organization.py
+-rwxr-xr-x   0        0        0    27463 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/resource.py
+-rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/resource_view.py
+-rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/showcase.py
+-rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/user.py
+-rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/vocabulary.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/simple.py
+-rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+-rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/dataset_search_results.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/empty.csv
+-rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/organization_show_results.yaml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/showcase_all_search_results.yaml
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/test_data.zip
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_base_config.yaml
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_email_configuration.yaml
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_organization_static.yaml
+-rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_static.yaml
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_view_static.yaml
+-rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_showcase_static.yaml
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_user_static.yaml
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_vocabulary_static.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/test_data_no_years.csv
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources.yaml
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources_new.yaml
+-rwxr-xr-x   0        0        0    45085 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0    49390 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0        0        0    47090 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_showcase.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_user.py
+-rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_vocabulary.py
+-rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/test_simple.py
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/my_code.py
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/my_resource.csv
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/my_resource.xlsx
+-rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/run.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/LICENSE
+-rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/README.md
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/PKG-INFO
```

### Comparing `hdx_python_api-6.0.5/CONTRIBUTING.md` & `hdx_python_api-6.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/requirements.txt` & `hdx_python_api-6.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/.config/pre-commit-config.yaml` & `hdx_python_api-6.0.6/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/.github/workflows/publish.yaml` & `hdx_python_api-6.0.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/.github/workflows/run-python-tests.yaml` & `hdx_python_api-6.0.6/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/documentation/main.md` & `hdx_python_api-6.0.6/documentation/main.md`

 * *Files 0% similar despite different names*

```diff
@@ -918,14 +918,24 @@
     dataset.update_in_hdx()
 
 Alternatively, when calling **create_in_hdx** or **update_in_hdx** on the 
 resource, it is possible to supply the parameter `data_updated` eg.
 
     resource.update_in_hdx(data_updated=True)
 
+If you need to set a specific date for date of update (`last_modified`), you
+can call the following:
+
+    resource.set_date_data_updated(date)
+
+`date` can be a datetime object or string. You can retrieve the date of update
+(`last_modified`) using the getter:
+
+    date = resource.get_date_data_updated()
+
 If the method **set_file_to_upload** is used to supply a file, the resource 
 `last_modified` field is set to now automatically regardless of the value of 
 `data_updated` or whether **mark_data_updated** has been called.
 
 ## Showcase Management
 
 The **Showcase** class enables you to manage showcases, creating, deleting and updating
```

### Comparing `hdx_python_api-6.0.5/documentation/pydoc-markdown.yaml` & `hdx_python_api-6.0.6/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/api/configuration.py` & `hdx_python_api-6.0.6/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/api/hdx_base_configuration.yaml` & `hdx_python_api-6.0.6/src/hdx/api/hdx_base_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/api/locations.py` & `hdx_python_api-6.0.6/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/dataset.py` & `hdx_python_api-6.0.6/src/hdx/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
             updated_resource = merge_two_dictionaries(
                 self.resources[resource_index], resource
             )
             if resource.get_file_to_upload():
                 updated_resource.set_file_to_upload(
                     resource.get_file_to_upload()
                 )
-            if resource.is_data_updated():
+            if resource.is_marked_data_updated():
                 updated_resource.mark_data_updated()
 
     def add_update_resources(
         self,
         resources: ListTuple[Union["Resource", Dict, str]],
         ignore_datasetid: bool = False,
     ) -> None:
@@ -330,15 +330,15 @@
             updated_resource = merge_two_dictionaries(
                 self.resources[resource_index], resource
             )
             if resource.get_file_to_upload():
                 updated_resource.set_file_to_upload(
                     resource.get_file_to_upload()
                 )
-            if resource.is_data_updated():
+            if resource.is_marked_data_updated():
                 updated_resource.mark_data_updated()
         for resource_index in updated_resource_no_matches:
             resource = resource_objects[resource_index]
             resource.check_url_filetoupload()
             self.resources.append(resource)
 
     def delete_resource(
@@ -1252,15 +1252,15 @@
         Args:
             date_format (Optional[str]): Date format. None is taken to be ISO 8601. Defaults to None.
             today (datetime): Date to use for today. Defaults to now_utc().
 
         Returns:
             Dict: Dictionary of date information
         """
-        return DateHelper.get_date_info(
+        return DateHelper.get_reference_period_info(
             self.data.get("dataset_date"), date_format, today
         )
 
     def set_reference_period(
         self,
         startdate: Union[datetime, str],
         enddate: Union[datetime, str, None] = None,
@@ -1278,15 +1278,15 @@
             enddate (Union[datetime, str, None]): Dataset end date. Defaults to None.
             ongoing (bool): True if ongoing, False if not. Defaults to False.
             ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
 
         Returns:
             None
         """
-        self.data["dataset_date"] = DateHelper.get_hdx_date(
+        self.data["dataset_date"] = DateHelper.get_hdx_reference_period(
             startdate, enddate, ongoing, ignore_timeinfo
         )
 
     def set_reference_period_year_range(
         self,
         dataset_year: Union[str, int, Iterable],
         dataset_end_year: Optional[Union[str, int]] = None,
@@ -1296,15 +1296,18 @@
         Args:
             dataset_year (Union[str, int, Iterable]): Dataset year given as string or int or range in an iterable
             dataset_end_year (Optional[Union[str, int]]): Dataset end year given as string or int
 
         Returns:
             List[int]: The start and end year if supplied or sorted list of years
         """
-        self.data["dataset_date"], retval = DateHelper.get_hdx_date_from_years(
+        (
+            self.data["dataset_date"],
+            retval,
+        ) = DateHelper.get_hdx_reference_period_from_years(
             dataset_year, dataset_end_year
         )
         return retval
 
     @classmethod
     def list_valid_update_frequencies(cls) -> List[str]:
         """List of valid update frequency values
```

### Comparing `hdx_python_api-6.0.5/src/hdx/data/dataset_title_helper.py` & `hdx_python_api-6.0.6/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/date_helper.py` & `hdx_python_api-6.0.6/src/hdx/data/date_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,38 +5,82 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 from hdx.utilities.dateparse import now_utc, parse_date
 
 
 class DateHelper:
     @staticmethod
-    def get_date_info(
-        hdx_date: Dict,
+    def get_hdx_date(
+        date: Union[datetime, str], ignore_timeinfo: bool, max=False
+    ):
+        """Get an HDX date as a string from a datetime.datetime object.
+
+        Args:
+            date (Union[datetime, str]): Date as datetime or string
+            ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
+
+        Returns:
+            str: HDX date as a string
+        """
+        if ignore_timeinfo:
+            timezone_handling = 0
+        else:
+            timezone_handling = 3
+
+        if isinstance(date, str):
+            date = parse_date(date, timezone_handling=timezone_handling)
+
+        if ignore_timeinfo:
+            if max:
+                date = date.replace(
+                    hour=23,
+                    minute=59,
+                    second=59,
+                    microsecond=0,
+                    tzinfo=None,
+                )
+            else:
+                date = date.replace(
+                    hour=0, minute=0, second=0, microsecond=0, tzinfo=None
+                )
+        else:
+            date = date.astimezone(timezone.utc).replace(
+                microsecond=0, tzinfo=None
+            )
+        return date.isoformat()
+
+    @staticmethod
+    def get_reference_period_info(
+        hdx_reference_period: Dict,
         date_format: Optional[str] = None,
         today: datetime = now_utc(),
     ) -> Dict:
-        """Get date as datetimes and strings in specified format. If no format is
-        supplied, the ISO 8601 format is used. Returns a dictionary containing keys
-        startdate (start date as datetime), enddate (end date as datetime),
-        startdate_str (start date as string), enddate_str (end date as string) and
-        ongoing (whether the end date is a rolls forward every day).
+        """Get reference period as datetimes and strings in specified format.
+        If no format is supplied, the ISO 8601 format is used. Returns a
+        dictionary containing keys startdate (start date as datetime), enddate
+        (end date as datetime), startdate_str (start date as string),
+        enddate_str (enddate as string) and ongoing (whether the end date rolls
+        forward every day).
 
         Args:
-            hdx_date (str): Input date
+            hdx_reference_period (str): Input reference period
             date_format (Optional[str]): Date format. None is taken to be ISO 8601. Defaults to None.
             today (datetime): Date to use for today. Defaults to now_utc().
 
         Returns:
             Dict: Dictionary of date information
         """
         result = dict()
-        if hdx_date:
-            if hdx_date[0] == "[" and hdx_date[-1] == "]":
-                hdx_date = hdx_date[1:-1]
-            dataset_dates = hdx_date.split(" TO ")
+        if hdx_reference_period:
+            if (
+                hdx_reference_period[0] == "["
+                and hdx_reference_period[-1] == "]"
+            ):
+                hdx_reference_period = hdx_reference_period[1:-1]
+            dataset_dates = hdx_reference_period.split(" TO ")
             startdate = parse_date(dataset_dates[0])
             enddate = dataset_dates[1]
             if enddate == "*":
                 enddate = today.replace(
                     hour=23,
                     minute=59,
                     second=59,
@@ -55,90 +99,59 @@
                 startdate_str = startdate.strftime(date_format)
                 enddate_str = enddate.strftime(date_format)
             result["startdate_str"] = startdate_str
             result["enddate_str"] = enddate_str
             result["ongoing"] = ongoing
         return result
 
-    @staticmethod
-    def get_hdx_date(
+    @classmethod
+    def get_hdx_reference_period(
+        cls,
         startdate: Union[datetime, str],
         enddate: Union[datetime, str, None] = None,
         ongoing: bool = False,
         ignore_timeinfo: bool = True,
     ) -> str:
-        """Get an HDX date from either datetime.datetime objects or strings with option
-        to set ongoing.
+        """Get an HDX reference period from either datetime.datetime objects or
+        strings with option to set ongoing.
 
         Args:
             startdate (Union[datetime, str]): Dataset start date
             enddate (Union[datetime, str, None]): Dataset end date. Defaults to None.
             ongoing (bool): True if ongoing, False if not. Defaults to False.
             ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
 
         Returns:
-            str: HDX date
+            str: HDX reference period
         """
-        if ignore_timeinfo:
-            timezone_handling = 0
-        else:
-            timezone_handling = 3
-
-        def get_date_str(dt, max=False):
-            if ignore_timeinfo:
-                if max:
-                    dt = dt.replace(
-                        hour=23,
-                        minute=59,
-                        second=59,
-                        microsecond=0,
-                        tzinfo=None,
-                    )
-                else:
-                    dt = dt.replace(
-                        hour=0, minute=0, second=0, microsecond=0, tzinfo=None
-                    )
-            else:
-                dt = dt.astimezone(timezone.utc).replace(
-                    microsecond=0, tzinfo=None
-                )
-            return dt.isoformat()
-
-        if isinstance(startdate, str):
-            startdate = parse_date(
-                startdate, timezone_handling=timezone_handling
-            )
-        startdate = get_date_str(startdate)
+        startdate = cls.get_hdx_date(startdate, ignore_timeinfo)
         if ongoing:
             enddate = "*"
         else:
             if not enddate:
                 enddate = startdate
             else:
-                if isinstance(enddate, str):
-                    enddate = parse_date(
-                        enddate, timezone_handling=timezone_handling
-                    )
-                enddate = get_date_str(enddate, max=True)
+                enddate = cls.get_hdx_date(enddate, ignore_timeinfo, max=True)
         return f"[{startdate} TO {enddate}]"
 
     @classmethod
-    def get_hdx_date_from_years(
+    def get_hdx_reference_period_from_years(
         cls,
         startyear: Union[str, int, Iterable],
         endyear: Union[str, int, None] = None,
     ) -> Tuple[str, List[int]]:
-        """Get an HDX date from an iterable of years or a start and end year.
+        """Get an HDX reference period from an iterable of years or a start and
+        end year.
 
         Args:
             startyear (Union[str, int, Iterable]): Start year given as string or int or range in an iterable
             endyear (Union[str, int, None]): End year given as string or int
 
         Returns:
-            Tuple[str,List[int]]: (HDX date, the start and end year if supplied or sorted list of years)
+            Tuple[str,List[int]]: (HDX reference period, the start and end year if supplied or sorted list of years)
         """
         retval = list()
         if isinstance(startyear, str):
             startyear = int(startyear)
         if not isinstance(startyear, Iterable):
             retval.append(startyear)
             if endyear is not None:
@@ -148,10 +161,12 @@
         else:
             retval = sorted(int(x) for x in list(startyear))
         startyear = retval[0]
         endyear = retval[-1]
         startdate = datetime(startyear, 1, 1, tzinfo=timezone.utc)
         enddate = datetime(endyear, 12, 31, 23, 59, 59, tzinfo=timezone.utc)
         return (
-            cls.get_hdx_date(startdate, enddate, ignore_timeinfo=False),
+            cls.get_hdx_reference_period(
+                startdate, enddate, ignore_timeinfo=False
+            ),
             retval,
         )
```

### Comparing `hdx_python_api-6.0.5/src/hdx/data/filestore_helper.py` & `hdx_python_api-6.0.6/src/hdx/data/filestore_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         Returns:
             None
         """
         file_to_upload = updated_resource.get_file_to_upload()
         if file_to_upload:
             resource.set_file_to_upload(file_to_upload)
             filestore_resources[resource_index] = file_to_upload
-        data_updated = updated_resource.is_data_updated()
+        data_updated = updated_resource.is_marked_data_updated()
         merge_two_dictionaries(resource, updated_resource)
         cls.resource_check_required_fields(
             resource, check_upload=True, **kwargs
         )
         if resource.get_file_to_upload():
             resource["url"] = cls.temporary_url
         if data_updated:
```

### Comparing `hdx_python_api-6.0.5/src/hdx/data/hdxobject.py` & `hdx_python_api-6.0.6/src/hdx/data/hdxobject.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/indicator_resource_view_template.yaml` & `hdx_python_api-6.0.6/src/hdx/data/indicator_resource_view_template.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/organization.py` & `hdx_python_api-6.0.6/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/resource.py` & `hdx_python_api-6.0.6/src/hdx/data/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import hdx.data.dataset
 import hdx.data.filestore_helper as filestore_helper
 from hdx.api.configuration import Configuration
 from hdx.data.date_helper import DateHelper
 from hdx.data.hdxobject import HDXError, HDXObject
 from hdx.data.resource_view import ResourceView
-from hdx.utilities.dateparse import now_utc
+from hdx.utilities.dateparse import now_utc, parse_date
 from hdx.utilities.downloader import Download
 from hdx.utilities.typehint import ListTuple
 from hdx.utilities.uuid import is_valid_uuid
 
 logger = logging.getLogger(__name__)
 
 
@@ -118,15 +118,15 @@
         Args:
             date_format (Optional[str]): Date format. None is taken to be ISO 8601. Defaults to None.
             today (datetime): Date to use for today. Defaults to now_utc().
 
         Returns:
             Dict: Dictionary of date information
         """
-        return DateHelper.get_date_info(
+        return DateHelper.get_reference_period_info(
             self.data.get("daterange_for_data"), date_format, today
         )
 
     def set_date_of_resource(
         self,
         startdate: Union[datetime, str],
         enddate: Union[datetime, str],
@@ -142,15 +142,15 @@
             startdate (Union[datetime, str]): Resource start date
             enddate (Union[datetime, str]): Resource end date
             ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
 
         Returns:
             None
         """
-        self.data["daterange_for_data"] = DateHelper.get_hdx_date(
+        self.data["daterange_for_data"] = DateHelper.get_hdx_reference_period(
             startdate, enddate, ignore_timeinfo=ignore_timeinfo
         )
 
     @classmethod
     def read_formats_mappings(
         cls,
         configuration: Optional[Configuration] = None,
@@ -385,14 +385,15 @@
         is used to supply a file, the resource last_modified field is set to
         now automatically regardless of the value of data_updated.
 
         Args:
             **kwargs: See below
             operation (string): Operation to perform eg. patch. Defaults to update.
             data_updated (bool): If True, set last_modified to now. Defaults to False.
+            date_data_updated (datetime): Date to use for last_modified. Default to None.
 
         Returns:
             None
         """
         self._check_load_existing_object("resource", "id")
         if self.file_to_upload and "url" in self.data:
             del self.data["url"]
@@ -406,14 +407,15 @@
         set_file_to_upload is used to supply a file, the resource last_modified
         field is set to now automatically regardless of the value of
         data_updated.
 
         Args:
             **kwargs: See below
             data_updated (bool): If True, set last_modified to now. Defaults to False.
+            date_data_updated (datetime): Date to use for last_modified. Default to None.
 
         Returns:
             None
         """
         if "ignore_check" not in kwargs:  # allow ignoring of field checks
             self.check_required_fields()
         id = self.data.get("id")
@@ -741,22 +743,46 @@
             skip_validation=True,
         )
         if success:
             self.data = result
         else:
             logger.debug(result)
 
-    def is_data_updated(self) -> bool:
-        """Return if the resource's data is updated
+    def is_marked_data_updated(self) -> bool:
+        """Return if the resource's data is marked to be updated
 
         Returns:
-            bool: Whether resource's data is updated
+            bool: Whether resource's data is marked to be updated
         """
         return self.data_updated
 
     def mark_data_updated(self) -> None:
         """Mark resource data as updated
 
         Returns:
             None
         """
         self.data_updated = True
+
+    def get_date_data_updated(self) -> datetime:
+        """Get date resource data was updated
+
+        Returns:
+            datetime: Date resource data was updated
+        """
+        return parse_date(self.data["last_modified"])
+
+    def set_date_data_updated(
+        self, date: Union[datetime, str], ignore_timeinfo: bool = True
+    ) -> None:
+        """Set date resource data was updated
+
+        Args:
+            date (Union[datetime, str]): Date resource data was updated
+            ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
+
+        Returns:
+            None
+        """
+        self.data["last_modified"] = DateHelper.get_hdx_date(
+            date, ignore_timeinfo
+        )
```

### Comparing `hdx_python_api-6.0.5/src/hdx/data/resource_matcher.py` & `hdx_python_api-6.0.6/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/resource_view.py` & `hdx_python_api-6.0.6/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/showcase.py` & `hdx_python_api-6.0.6/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/user.py` & `hdx_python_api-6.0.6/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/data/vocabulary.py` & `hdx_python_api-6.0.6/src/hdx/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/facades/infer_arguments.py` & `hdx_python_api-6.0.6/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/facades/keyword_arguments.py` & `hdx_python_api-6.0.6/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/src/hdx/facades/simple.py` & `hdx_python_api-6.0.6/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/Accepted_Tags.csv` & `hdx_python_api-6.0.6/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/Tag_Mapping.csv` & `hdx_python_api-6.0.6/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/dataset_search_results.yaml` & `hdx_python_api-6.0.6/tests/fixtures/dataset_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/organization_show_results.yaml` & `hdx_python_api-6.0.6/tests/fixtures/organization_show_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/resource_formats.json` & `hdx_python_api-6.0.6/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/showcase_all_search_results.yaml` & `hdx_python_api-6.0.6/tests/fixtures/showcase_all_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/test_data.csv` & `hdx_python_api-6.0.6/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/test_data.zip` & `hdx_python_api-6.0.6/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.json` & `hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.yaml` & `hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/config/hdx_datasource_topline.json` & `hdx_python_api-6.0.6/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_view_static.yaml` & `hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_view_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx_python_api-6.0.6/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx_python_api-6.0.6/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.6/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx_python_api-6.0.6/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources.yaml` & `hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources_new.yaml` & `hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources_new.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/conftest.py` & `hdx_python_api-6.0.6/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/api/test_configuration.py` & `hdx_python_api-6.0.6/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/api/test_locations.py` & `hdx_python_api-6.0.6/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/__init__.py` & `hdx_python_api-6.0.6/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_dataset_core.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_dataset_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,15 +709,15 @@
         resource = Resource(resourcesdata[0])
         resource.mark_data_updated()
         dataset.add_update_resources([resource, resource])
         dataset.create_in_hdx()
         assert dataset["state"] == "active"
         assert len(dataset.resources) == 3
         resource = dataset.get_resource()
-        assert resource.is_data_updated() is False
+        assert resource.is_marked_data_updated() is False
         match = date_pattern.search(resource["last_modified"])
         assert match
 
         dataset = Dataset(datasetdata)
         resourcesdata = copy.deepcopy(resources_data)
         resource = Resource(resourcesdata[0])
         dataset.add_update_resources([resource, resource])
```

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_dataset_noncore.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_dataset_noncore.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_dataset_title_helper.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_organization.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_resource.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pytest
 
 from . import MockResponse, dataset_resultdict
 from .test_resource_view import resource_view_list, resource_view_mocklist
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.resource import Resource
+from hdx.utilities.dateparse import parse_date
 from hdx.utilities.dictandlist import merge_two_dictionaries
 from hdx.utilities.downloader import DownloadError
 
 resultdict = {
     "cache_last_updated": None,
     "package_id": "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d",
     "webstore_last_updated": None,
@@ -841,17 +842,17 @@
 
         resource_data = copy.deepcopy(TestResource.resource_data)
         resource_data["name"] = "MyResource1"
         resource_data["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
         resource = Resource(resource_data)
         resource.mark_data_updated()
         assert resource.data_updated is True
-        assert resource.is_data_updated() is True
+        assert resource.is_marked_data_updated() is True
         resource.create_in_hdx()
-        assert resource.is_data_updated() is False
+        assert resource.is_marked_data_updated() is False
         assert resource["id"] == "74b74ae1-df0c-4716-829f-4f939a046811"
         assert resource.get_file_type() == "xlsx"
         assert resource["state"] == "active"
         match = date_pattern.search(resource["last_modified"])
         assert match
         resource["format"] = "Geoservice"
         resource.update_in_hdx()
@@ -1006,7 +1007,20 @@
             "74b74ae1-df0c-4716-829f-4f939a046811"
         )
         assert resource["id"] == "de6549d8-268b-4dfe-adaf-a4ae5c8510d5"
         assert resource["name"] == "MyResource1"
         assert resource["package_id"] == "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d"
         resource.mark_broken()
         assert resource.is_broken() is True
+
+    def test_date_data_updated(self, configuration, read):
+        resource = Resource.read_from_hdx(
+            "74b74ae1-df0c-4716-829f-4f939a046811"
+        )
+        assert resource["id"] == "de6549d8-268b-4dfe-adaf-a4ae5c8510d5"
+        assert resource["name"] == "MyResource1"
+        assert resource["package_id"] == "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d"
+        resource.set_date_data_updated("2020-03-02")
+        expected = "2020-03-02T00:00:00+00:00"
+        assert resource.get_date_data_updated().isoformat() == expected
+        resource.set_date_data_updated(parse_date("2020-03-02"))
+        assert resource.get_date_data_updated().isoformat() == expected
```

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_resource_view.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_showcase.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_update_dataset_resources.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_update_dataset_resources.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_update_logic.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_user.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/data/test_vocabulary.py` & `hdx_python_api-6.0.6/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/facades/__init__.py` & `hdx_python_api-6.0.6/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/facades/test_infer_arguments.py` & `hdx_python_api-6.0.6/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/facades/test_keyword_arguments.py` & `hdx_python_api-6.0.6/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/tests/hdx/facades/test_simple.py` & `hdx_python_api-6.0.6/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/workingexample/my_resource.xlsx` & `hdx_python_api-6.0.6/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/.gitignore` & `hdx_python_api-6.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/LICENSE` & `hdx_python_api-6.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/README.md` & `hdx_python_api-6.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/pyproject.toml` & `hdx_python_api-6.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.5/PKG-INFO` & `hdx_python_api-6.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 6.0.5
+Version: 6.0.6
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-api
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: API,CKAN,HDX,humanitarian data exchange
 Classifier: Development Status :: 5 - Production/Stable
```

