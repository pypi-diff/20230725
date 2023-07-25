# Comparing `tmp/pg-sui-0.2.4.tar.gz` & `tmp/pg-sui-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg-sui-0.2.4.tar", last modified: Sun Jul 23 21:41:00 2023, max compression
+gzip compressed data, was "pg-sui-0.3.tar", last modified: Tue Jul 25 19:10:33 2023, max compression
```

## Comparing `pg-sui-0.2.4.tar` & `pg-sui-0.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:59.602384 pg-sui-0.2.4/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35149 2023-07-16 18:34:37.000000 pg-sui-0.2.4/LICENSE
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      220 2023-07-23 06:06:57.000000 pg-sui-0.2.4/MANIFEST.in
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14102 2023-07-23 21:40:59.599382 pg-sui-0.2.4/PKG-INFO
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10444 2023-07-23 06:06:57.000000 pg-sui-0.2.4/README.md
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:56.314872 pg-sui-0.2.4/pg_sui.egg-info/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14102 2023-07-23 21:40:51.000000 pg-sui-0.2.4/pg_sui.egg-info/PKG-INFO
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2994 2023-07-23 21:40:53.000000 pg-sui-0.2.4/pg_sui.egg-info/SOURCES.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        1 2023-07-23 21:40:51.000000 pg-sui-0.2.4/pg_sui.egg-info/dependency_links.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      331 2023-07-23 21:40:51.000000 pg-sui-0.2.4/pg_sui.egg-info/requires.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       22 2023-07-23 21:40:51.000000 pg-sui-0.2.4/pg_sui.egg-info/top_level.txt
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:56.378344 pg-sui-0.2.4/pgsui/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1449 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/__init__.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:56.506344 pg-sui-0.2.4/pgsui/data_processing/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.2.4/pgsui/data_processing/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    43851 2023-07-23 21:38:52.000000 pg-sui-0.2.4/pgsui/data_processing/transformers.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:56.533342 pg-sui-0.2.4/pgsui/example_data/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.2.4/pgsui/example_data/__init__.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:56.894338 pg-sui-0.2.4/pgsui/example_data/phylip_files/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/phylip_files/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   238537 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/phylip_files/test.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2897 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n10.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13428 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n100.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1960 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n2.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    60228 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n500.phy
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:56.970336 pg-sui-0.2.4/pgsui/example_data/popmaps/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/popmaps/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1954 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/popmaps/test.popmap
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:57.425940 pg-sui-0.2.4/pgsui/example_data/structure_files/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6375 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.1row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50808 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.100sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7978 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    17512 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.30sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967410 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.allsites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6609 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.pops.1row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     8446 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.pops.2row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967878 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/structure_files/test.pops.2row.allsites.str
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:57.995612 pg-sui-0.2.4/pgsui/example_data/trees/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    25575 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test.iqtree
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      134 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test.qmat
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    46013 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4696 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test.tre
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      678 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test_n10.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2577 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test_n100.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11387 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test_n500.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16235 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test_siterates.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       80 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test_siterates_n10.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      804 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test_siterates_n100.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4008 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/trees/test_siterates_n500.txt
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:58.160139 pg-sui-0.2.4/pgsui/example_data/vcf_files/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   380243 2023-07-23 04:24:43.000000 pg-sui-0.2.4/pgsui/example_data/vcf_files/test.vcf
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    72705 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/example_data/vcf_files/test.vcf.gz
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2581 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/example_data/vcf_files/test.vcf.gz.tbi
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:58.305707 pg-sui-0.2.4/pgsui/impute/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.2.4/pgsui/impute/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   120473 2023-07-23 21:38:52.000000 pg-sui-0.2.4/pgsui/impute/estimators.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    51210 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/impute.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    53283 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/simple_imputers.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:58.403669 pg-sui-0.2.4/pgsui/impute/supervised/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.2.4/pgsui/impute/supervised/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35075 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/supervised/iterative_imputer_fixedparams.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    45443 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/supervised/iterative_imputer_gridsearch.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:58.644143 pg-sui-0.2.4/pgsui/impute/unsupervised/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     9682 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/callbacks.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    29483 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/keras_classifiers.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:58.889858 pg-sui-0.2.4/pgsui/impute/unsupervised/models/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/models/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    20161 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/models/autoencoder_model.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:58.988856 pg-sui-0.2.4/pgsui/impute/unsupervised/models/in_development/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/models/in_development/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15036 2023-07-23 04:24:45.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/models/in_development/cnn_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14501 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/models/nlpca_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    37879 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/models/ubp_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    22338 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/models/vae_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    52329 2023-07-23 21:38:52.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/neural_network_imputers.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50830 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/impute/unsupervised/neural_network_methods.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7471 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/pg_sui.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:59.231767 pg-sui-0.2.4/pgsui/utils/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.2.4/pgsui/utils/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15705 2023-07-23 04:24:45.000000 pg-sui-0.2.4/pgsui/utils/misc.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    33748 2023-07-23 06:06:59.000000 pg-sui-0.2.4/pgsui/utils/plotting.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    27088 2023-07-23 21:38:52.000000 pg-sui-0.2.4/pgsui/utils/scorers.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10143 2023-07-23 04:24:45.000000 pg-sui-0.2.4/pgsui/utils/sequence_tools.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       38 2023-07-23 21:40:59.617388 pg-sui-0.2.4/setup.cfg
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     3046 2023-07-23 21:38:52.000000 pg-sui-0.2.4/setup.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:59.358765 pg-sui-0.2.4/simulation/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.2.4/simulation/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11345 2023-07-23 04:24:46.000000 pg-sui-0.2.4/simulation/sim_benchmarks.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13793 2023-07-23 04:24:46.000000 pg-sui-0.2.4/simulation/sim_treeparams.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 21:40:59.568386 pg-sui-0.2.4/test/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:46.000000 pg-sui-0.2.4/test/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6024 2023-07-23 04:24:46.000000 pg-sui-0.2.4/test/pg_sui_simtest.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15871 2023-07-23 04:24:46.000000 pg-sui-0.2.4/test/pg_sui_testing.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6832 2023-07-23 21:38:52.000000 pg-sui-0.2.4/test/test.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14310 2023-07-23 04:24:46.000000 pg-sui-0.2.4/test/test_pgsui.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7041 2023-07-23 21:38:52.000000 pg-sui-0.2.4/test/test_tkc.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.207312 pg-sui-0.3/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35149 2023-07-16 18:34:37.000000 pg-sui-0.3/LICENSE
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      220 2023-07-23 06:06:57.000000 pg-sui-0.3/MANIFEST.in
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14121 2023-07-25 19:10:32.204312 pg-sui-0.3/PKG-INFO
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10444 2023-07-23 06:06:57.000000 pg-sui-0.3/README.md
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.174327 pg-sui-0.3/pg_sui.egg-info/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14121 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/PKG-INFO
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2994 2023-07-25 19:10:29.000000 pg-sui-0.3/pg_sui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        1 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      331 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/requires.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       22 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/top_level.txt
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.202329 pg-sui-0.3/pgsui/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1449 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/__init__.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.236326 pg-sui-0.3/pgsui/data_processing/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.3/pgsui/data_processing/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    42452 2023-07-24 01:34:13.000000 pg-sui-0.3/pgsui/data_processing/transformers.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.256330 pg-sui-0.3/pgsui/example_data/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.3/pgsui/example_data/__init__.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.401326 pg-sui-0.3/pgsui/example_data/phylip_files/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   238537 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2897 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n10.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13428 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n100.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1960 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n2.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    60228 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n500.phy
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.447326 pg-sui-0.3/pgsui/example_data/popmaps/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/popmaps/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1954 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/popmaps/test.popmap
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.775325 pg-sui-0.3/pgsui/example_data/structure_files/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6375 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.1row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50808 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.100sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7978 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    17512 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.30sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967410 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.allsites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6609 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.pops.1row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     8446 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967878 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.allsites.str
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.133322 pg-sui-0.3/pgsui/example_data/trees/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    25575 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.iqtree
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      134 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.qmat
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    46013 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4696 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.tre
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      678 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_n10.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2577 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_n100.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11387 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_n500.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16235 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       80 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates_n10.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      804 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates_n100.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4008 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates_n500.txt
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.225320 pg-sui-0.3/pgsui/example_data/vcf_files/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   380243 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    72705 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2581 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz.tbi
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.324319 pg-sui-0.3/pgsui/impute/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3/pgsui/impute/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    49767 2023-07-25 05:09:59.000000 pg-sui-0.3/pgsui/impute/estimators.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    51148 2023-07-24 06:54:52.000000 pg-sui-0.3/pgsui/impute/impute.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    53283 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/simple_imputers.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.417320 pg-sui-0.3/pgsui/impute/supervised/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3/pgsui/impute/supervised/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35075 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_fixedparams.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    45443 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_gridsearch.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.570317 pg-sui-0.3/pgsui/impute/unsupervised/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3/pgsui/impute/unsupervised/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     9682 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/unsupervised/callbacks.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    29626 2023-07-24 07:18:02.000000 pg-sui-0.3/pgsui/impute/unsupervised/keras_classifiers.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.809313 pg-sui-0.3/pgsui/impute/unsupervised/models/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    19704 2023-07-24 17:44:03.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/autoencoder_model.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.884314 pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15036 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/cnn_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16939 2023-07-24 18:00:06.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/nlpca_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    44658 2023-07-24 17:18:02.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/ubp_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    21805 2023-07-24 17:30:15.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/vae_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    51530 2023-07-24 21:25:03.000000 pg-sui-0.3/pgsui/impute/unsupervised/neural_network_imputers.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50820 2023-07-25 05:36:56.000000 pg-sui-0.3/pgsui/impute/unsupervised/neural_network_methods.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7471 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/pg_sui.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.026312 pg-sui-0.3/pgsui/utils/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/utils/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15705 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/utils/misc.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    32470 2023-07-24 08:43:44.000000 pg-sui-0.3/pgsui/utils/plotting.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    17472 2023-07-24 20:47:26.000000 pg-sui-0.3/pgsui/utils/scorers.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10143 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/utils/sequence_tools.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       38 2023-07-25 19:10:32.208311 pg-sui-0.3/setup.cfg
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     3087 2023-07-25 18:35:09.000000 pg-sui-0.3/setup.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.080312 pg-sui-0.3/simulation/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/simulation/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11345 2023-07-23 04:24:46.000000 pg-sui-0.3/simulation/sim_benchmarks.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13793 2023-07-23 04:24:46.000000 pg-sui-0.3/simulation/sim_treeparams.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.185312 pg-sui-0.3/test/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:46.000000 pg-sui-0.3/test/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6024 2023-07-23 04:24:46.000000 pg-sui-0.3/test/pg_sui_simtest.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15871 2023-07-23 04:24:46.000000 pg-sui-0.3/test/pg_sui_testing.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6773 2023-07-25 18:43:07.000000 pg-sui-0.3/test/test.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14310 2023-07-23 04:24:46.000000 pg-sui-0.3/test/test_pgsui.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     5867 2023-07-24 00:02:54.000000 pg-sui-0.3/test/test_tkc.py
```

### Comparing `pg-sui-0.2.4/LICENSE` & `pg-sui-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/PKG-INFO` & `pg-sui-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-sui
-Version: 0.2.4
+Version: 0.3
 Summary: Python machine and deep learning package to impute missing SNPs
 Home-page: https://github.com/btmartin721/PG-SUI
 Author: Bradley T. Martin and Tyler K. Chafin
 Author-email: evobio721@gmail.com
 Maintainer: Bradley T. Martin
 Maintainer-email: evobio721@gmail.com
 License: GNU General Public License v3 (GPLv3)
@@ -273,25 +273,25 @@
         
         <a name="3">3. </a>Hinton, G.E., & Salakhutdinov, R.R. (2006). Reducing the dimensionality of data with neural networks. Science, 313(5786), 504-507.
         
         <a name="4">4. </a>Scholz, M., Kaplan, F., Guy, C. L., Kopka, J., & Selbig, J. (2005). Non-linear PCA: a missing data approach. Bioinformatics, 21(20), 3887-3895.
             
         <a name="5">5. </a>Gashler, M. S., Smith, M. R., Morris, R., & Martinez, T. (2016). Missing value imputation with unsupervised backpropagation. Computational Intelligence, 32(2), 196-215.
         
-Keywords: python,impute,imputation,imputer,machine learning,neural network,api,IterativeImputer,vae,ubp,nlpca,autoencoder,deep learning,population genomics
+Keywords: impute,imputation,imputer,machine learning,neural network,deep learning,python,api,vae,autoencoder,ubp,nlpca,population genomics,unsupervised,supervised,IterativeImputer
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: intel
```

### Comparing `pg-sui-0.2.4/README.md` & `pg-sui-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pg_sui.egg-info/PKG-INFO` & `pg-sui-0.3/pg_sui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-sui
-Version: 0.2.4
+Version: 0.3
 Summary: Python machine and deep learning package to impute missing SNPs
 Home-page: https://github.com/btmartin721/PG-SUI
 Author: Bradley T. Martin and Tyler K. Chafin
 Author-email: evobio721@gmail.com
 Maintainer: Bradley T. Martin
 Maintainer-email: evobio721@gmail.com
 License: GNU General Public License v3 (GPLv3)
@@ -273,25 +273,25 @@
         
         <a name="3">3. </a>Hinton, G.E., & Salakhutdinov, R.R. (2006). Reducing the dimensionality of data with neural networks. Science, 313(5786), 504-507.
         
         <a name="4">4. </a>Scholz, M., Kaplan, F., Guy, C. L., Kopka, J., & Selbig, J. (2005). Non-linear PCA: a missing data approach. Bioinformatics, 21(20), 3887-3895.
             
         <a name="5">5. </a>Gashler, M. S., Smith, M. R., Morris, R., & Martinez, T. (2016). Missing value imputation with unsupervised backpropagation. Computational Intelligence, 32(2), 196-215.
         
-Keywords: python,impute,imputation,imputer,machine learning,neural network,api,IterativeImputer,vae,ubp,nlpca,autoencoder,deep learning,population genomics
+Keywords: impute,imputation,imputer,machine learning,neural network,deep learning,python,api,vae,autoencoder,ubp,nlpca,population genomics,unsupervised,supervised,IterativeImputer
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: intel
```

### Comparing `pg-sui-0.2.4/pg_sui.egg-info/SOURCES.txt` & `pg-sui-0.3/pg_sui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/__init__.py` & `pg-sui-0.3/pgsui/__init__.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/data_processing/transformers.py` & `pg-sui-0.3/pgsui/data_processing/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -968,15 +968,15 @@
 
     def random_weighted_missing_data(self, X, inv=False):
         """Choose values for which to simulate missing data by biasing towards the minority or majority alleles, depending on whether inv is True or False.
 
         Args:
             X (np.ndarray): True values.
 
-            inv (bool, optional): If True, then biases towards choosing majority alleles. If False, then generates a stratified random sample (class proportions ~= full dataset) Defaults to False.
+            inv (bool, optional): If True, then biases towards choosing majority alleles. If False, then biases towards choosing minority alleles. Defaults to False.
 
         Returns:
             np.ndarray: X with simulated missing values.
 
         """
         # Get unique classes and their counts
         classes, counts = np.unique(X, return_counts=True)
@@ -1108,48 +1108,14 @@
             raise ValueError(f"Invalid shape of input X: {X.shape}")
 
         Xt = X.copy()
         mask_boolean = self.mask_ != 0
         Xt[mask_boolean] = mask_val
         return Xt
 
-    def write_mask(self, filename_prefix):
-        """Write mask to file.
-
-        Args:
-            filename_prefix (str): Prefix for the filenames to write to.
-        """
-        np.save(filename_prefix + "_mask.npy", self.mask_)
-        np.save(filename_prefix + "_original_missing_mask.npy", self.original_missing_mask_)
-
-    def read_mask(self, filename_prefix):
-        """Read mask from file.
-
-        Args:
-            filename_prefix (str): Prefix for the filenames to read from.
-
-        Returns:
-            tuple of np.ndarray: The read masks.
-        """
-        # Check if files exist
-        if not os.path.isfile(filename_prefix + "_mask.npy"):
-            raise FileNotFoundError(filename_prefix + "_mask.npy" + " does not exist.")
-        if not os.path.isfile(filename_prefix + "_original_missing_mask.npy"):
-            raise FileNotFoundError(filename_prefix + "_original_missing_mask.npy" + " does not exist.")
-
-        # Load mask from file
-        self.mask_ = np.load(filename_prefix + "_mask.npy")
-        self.original_missing_mask_ = np.load(filename_prefix + "_original_missing_mask.npy")
-
-        # Recalculate all_missing_mask_ from mask_ and original_missing_mask_
-        self.all_missing_mask_ = np.logical_or(self.mask_, self.original_missing_mask_)
-
-        return self.mask_, self.original_missing_mask_, self.all_missing_mask_
-
-
     @property
     def missing_count(self) -> int:
         """Count of masked genotypes in SimGenotypeData.mask
 
         Returns:
             int: Integer count of masked alleles.
         """
```

### Comparing `pg-sui-0.2.4/pgsui/example_data/phylip_files/test.phy` & `pg-sui-0.3/pgsui/example_data/phylip_files/test.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n10.phy` & `pg-sui-0.3/pgsui/example_data/phylip_files/test_n10.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n100.phy` & `pg-sui-0.3/pgsui/example_data/phylip_files/test_n100.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n2.phy` & `pg-sui-0.3/pgsui/example_data/phylip_files/test_n2.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/phylip_files/test_n500.phy` & `pg-sui-0.3/pgsui/example_data/phylip_files/test_n500.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/popmaps/test.popmap` & `pg-sui-0.3/pgsui/example_data/popmaps/test.popmap`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.1row.10sites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.1row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.100sites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.100sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.10sites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.30sites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.30sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.nopops.2row.allsites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.allsites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.pops.1row.10sites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.pops.1row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.pops.2row.10sites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/structure_files/test.pops.2row.allsites.str` & `pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.allsites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test.iqtree` & `pg-sui-0.3/pgsui/example_data/trees/test.iqtree`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test.rate` & `pg-sui-0.3/pgsui/example_data/trees/test.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test.tre` & `pg-sui-0.3/pgsui/example_data/trees/test.tre`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test_n10.rate` & `pg-sui-0.3/pgsui/example_data/trees/test_n10.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test_n100.rate` & `pg-sui-0.3/pgsui/example_data/trees/test_n100.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test_n500.rate` & `pg-sui-0.3/pgsui/example_data/trees/test_n500.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test_siterates.txt` & `pg-sui-0.3/pgsui/example_data/trees/test_siterates.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test_siterates_n100.txt` & `pg-sui-0.3/pgsui/example_data/trees/test_siterates_n100.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/trees/test_siterates_n500.txt` & `pg-sui-0.3/pgsui/example_data/trees/test_siterates_n500.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/vcf_files/test.vcf` & `pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/vcf_files/test.vcf.gz` & `pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/example_data/vcf_files/test.vcf.gz.tbi` & `pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/impute/impute.py` & `pg-sui-0.3/pgsui/impute/impute.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,34 +364,34 @@
             genotype_data (GenotypeData): Original GenotypeData object to load attributes from.
 
         Returns:
             GenotypeData: GenotypeData object with imputed data.
         """
         imputed_gd = deepcopy(genotype_data)
 
-        if self.clf == VAE:
-            if len(imp012.shape) == 3:
-                if imp012.shape[-1] == 4:
-                    imputed_gd.genotypes_onehot = imp012
-                else:
-                    raise ValueError("Invalid shape for imputed output.")
-            elif len(imp012.shape) == 2:
-                if isinstance(imp012, pd.DataFrame):
-                    imp012 = imp012.to_numpy()
-                imp012 = imp012.astype(int)
-                if np.max(imp012) > 2:
-                    imputed_gd.genotypes_int = imp012
-                else:
-                    imputed_gd.genotypes_012 = imp012
+        # if self.clf == VAE:
+        if len(imp012.shape) == 3:
+            if imp012.shape[-1] == 4:
+                imputed_gd.genotypes_onehot = imp012
             else:
-                raise ValueError(
-                    f"Invalid shape for imputed output: {imp012.shape}"
-                )
+                raise ValueError("Invalid shape for imputed output.")
+        elif len(imp012.shape) == 2:
+            if isinstance(imp012, pd.DataFrame):
+                imp012 = imp012.to_numpy()
+            imp012 = imp012.astype(int)
+            if np.max(imp012) > 2:
+                imputed_gd.genotypes_int = imp012
+            else:
+                imputed_gd.genotypes_012 = imp012
         else:
-            imputed_gd.genotypes_012 = imp012
+            raise ValueError(
+                f"Invalid shape for imputed output: {imp012.shape}"
+            )
+        # else:
+        #     imputed_gd.genotypes_012 = imp012
 
         return imputed_gd
 
     def _subset_data_for_gridsearch(
         self,
         df: pd.DataFrame,
         columns_to_subset: Union[int, float],
```

### Comparing `pg-sui-0.2.4/pgsui/impute/simple_imputers.py` & `pg-sui-0.3/pgsui/impute/simple_imputers.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/impute/supervised/iterative_imputer_fixedparams.py` & `pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_fixedparams.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/impute/supervised/iterative_imputer_gridsearch.py` & `pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_gridsearch.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/callbacks.py` & `pg-sui-0.3/pgsui/impute/unsupervised/callbacks.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/keras_classifiers.py` & `pg-sui-0.3/pgsui/impute/unsupervised/keras_classifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
         hidden_activation="elu",
         l1_penalty=0.01,
         l2_penalty=0.01,
         dropout_rate=0.2,
         n_components=3,
         sample_weight=None,
         missing_mask=None,
-        num_classes=3,
-        activate="softmax",
+        num_classes=4,
+        activate="sigmoid",
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.y = y
         self.output_shape = output_shape
         self.weights_initializer = weights_initializer
@@ -485,14 +485,15 @@
         l1_penalty=0.01,
         l2_penalty=0.01,
         dropout_rate=0.2,
         num_classes=3,
         phase=None,
         sample_weight=None,
         n_components=3,
+        activate=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.V = V
         self.y_train = y_train
         self.ubp_weights = ubp_weights
         self.batch_size = batch_size
@@ -505,14 +506,15 @@
         self.l1_penalty = l1_penalty
         self.l2_penalty = l2_penalty
         self.dropout_rate = dropout_rate
         self.num_classes = num_classes
         self.phase = phase
         self.sample_weight = sample_weight
         self.n_components = n_components
+        self.activate = activate
 
     def _keras_build_fn(self, compile_kwargs):
         """Build model with custom parameters.
 
         Args:
             compile_kwargs (Dict[str, Any]): Dictionary with parameters: values. The parameters should be passed to the class constructor, but should be captured as kwargs. They should also have the routing prefix (e.g., optimizer__learning_rate=0.01). compile_kwargs will automatically be parsed from **kwargs by KerasClassifier and sent here.
 
@@ -656,15 +658,18 @@
     @property
     def target_encoder(self):
         """Handles target input and output, y_true and y_pred, both before and after training.
 
         Returns:
             NNOutputTransformer: NNOutputTransformer object that includes fit(), transform(), and inverse_transform() methods.
         """
-        return MLPTargetTransformer()
+        return AutoEncoderFeatureTransformer(
+            num_classes=self.num_classes,
+            activate=None,
+        )
 
     def predict(self, X, **kwargs):
         """Returns predictions for the given test data.
 
         Args:
             X (Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)): Training samples where n_samples is the number of samples and n_features is the number of features.
         kwargs (Dict[str, Any]): Extra arguments to route to ``Model.predict``\.
```

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/models/autoencoder_model.py` & `pg-sui-0.3/pgsui/impute/unsupervised/models/autoencoder_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from tensorflow.keras.layers import (
     Dropout,
     Dense,
     Reshape,
     Flatten,
     LeakyReLU,
     PReLU,
+    Activation,
 )
 
 from tensorflow.keras.regularizers import l1_l2
 from tensorflow.keras import backend as K
 
 # Custom Modules
 try:
@@ -307,22 +308,20 @@
         dropout_rate=0.2,
         sample_weight=None,
         missing_mask=None,
         num_classes=3,
     ):
         super(AutoEncoderModel, self).__init__()
 
-        self.nn_ = NeuralNetworkMethods()
-        self.categorical_accuracy = self.nn_.make_masked_categorical_accuracy()
-
-        self.total_loss_tracker = tf.keras.metrics.Mean(name="loss")
-        self.reconstruction_loss_tracker = tf.keras.metrics.Mean(
-            name="reconstruction_loss"
+        self.total_loss_tracker = tf.keras.metrics.Mean(name="total_loss")
+        self.binary_accuracy_tracker = tf.keras.metrics.Mean(
+            name="binary_accuracy"
         )
-        self.accuracy_tracker = tf.keras.metrics.Mean(name="accuracy")
+
+        self.nn_ = NeuralNetworkMethods()
 
         self._y = y
         self._batch_idx = 0
         self._batch_size = batch_size
         self._sample_weight = sample_weight
         self._missing_mask = missing_mask
 
@@ -399,18 +398,21 @@
             hidden_layer_sizes,
             self.dropout_rate,
             activation,
             kernel_initializer,
             kernel_regularizer,
         )
 
+        self.activation = Activation("sigmoid")
+
     def call(self, inputs, training=None):
         """Forward pass through model."""
         x = self.encoder(inputs)
-        return self.decoder(x)
+        x = self.decoder(x)
+        return self.activation(x)
 
     def model(self):
         """To allow model.summary().summar() to be called."""
         x = tf.keras.Input(shape=(self.n_features, self.num_classes))
         return tf.keras.Model(inputs=[x], outputs=self.call(x))
 
     def set_model_outputs(self):
@@ -419,16 +421,15 @@
         model = tf.keras.Model(inputs=[x], outputs=self.call(x))
         self.outputs = model.outputs
 
     @property
     def metrics(self):
         return [
             self.total_loss_tracker,
-            self.reconstruction_loss_tracker,
-            self.accuracy_tracker,
+            self.binary_accuracy_tracker,
         ]
 
     @tf.function
     def train_step(self, data):
         y = self._y
 
         (
@@ -475,32 +476,25 @@
 
             regularization_loss = sum(self.losses)
 
             total_loss = reconstruction_loss + regularization_loss
 
         grads = tape.gradient(total_loss, self.trainable_weights)
         self.optimizer.apply_gradients(zip(grads, self.trainable_weights))
-        self.total_loss_tracker.update_state(total_loss)
-        self.reconstruction_loss_tracker.update_state(reconstruction_loss)
 
         ### NOTE: If you get the error, "'tuple' object has no attribute
         ### 'rank', then convert y_true to a tensor object."
-        # self.compiled_metrics.update_state(
-        self.accuracy_tracker.update_state(
-            self.categorical_accuracy(
-                y_true_masked,
-                y_pred_masked,
-                sample_weight=sample_weight_masked,
-            )
+        self.total_loss_tracker.update_state(total_loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
         )
 
         return {
             "loss": self.total_loss_tracker.result(),
-            "reconstruction_loss": self.reconstruction_loss_tracker.result(),
-            "accuracy": self.accuracy_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
         }
 
     @tf.function
     def test_step(self, data):
         """Custom evaluation loop for one step (=batch) in a single epoch.
 
         This function will evaluate on a batch of samples (rows), which can be adjusted with the ``batch_size`` parameter from the estimator.
@@ -553,29 +547,24 @@
             sample_weight=sample_weight_masked,
         )
 
         regularization_loss = sum(self.losses)
 
         total_loss = reconstruction_loss + regularization_loss
 
-        self.accuracy_tracker.update_state(
-            self.categorical_accuracy(
-                y_true_masked,
-                y_pred_masked,
-                sample_weight=sample_weight_masked,
-            )
-        )
-
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank', then convert y_true to a tensor object."
         self.total_loss_tracker.update_state(total_loss)
-        self.reconstruction_loss_tracker.update_state(reconstruction_loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
 
         return {
             "loss": self.total_loss_tracker.result(),
-            "reconstruction_loss": self.reconstruction_loss_tracker.result(),
-            "accuracy": self.accuracy_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
         }
 
     @property
     def batch_size(self):
         """Batch (=step) size per epoch.
         :noindex:
         """
```

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/models/in_development/cnn_model.py` & `pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/cnn_model.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/models/nlpca_model.py` & `pg-sui-0.3/pgsui/impute/unsupervised/models/nlpca_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 from tensorflow.keras.layers import (
     Dropout,
     Dense,
     Reshape,
     LeakyReLU,
     PReLU,
+    Activation,
 )
 
 from tensorflow.keras.regularizers import l1_l2
 
 # Custom Modules
 try:
     from ..neural_network_methods import NeuralNetworkMethods
@@ -119,14 +120,19 @@
         dropout_rate=0.2,
         num_classes=3,
         phase=None,
         sample_weight=None,
     ):
         super(NLPCAModel, self).__init__()
 
+        self.total_loss_tracker = tf.keras.metrics.Mean(name="total_loss")
+        self.binary_accuracy_tracker = tf.keras.metrics.Mean(
+            name="binary_accuracy"
+        )
+
         nn = NeuralNetworkMethods()
         self.nn = nn
 
         if V is None:
             self._V = nn.init_weights(y.shape[0], n_components)
         elif isinstance(V, dict):
             self._V = V[n_components]
@@ -241,14 +247,16 @@
             kernel_regularizer=kernel_regularizer,
         )
 
         self.rshp = Reshape((output_shape, num_classes))
 
         self.dropout_layer = Dropout(rate=dropout_rate)
 
+        self.activation = Activation("sigmoid")
+
     def call(self, inputs, training=None):
         x = self.dense1(inputs)
         x = self.dropout_layer(x, training=training)
         if self.dense2 is not None:
             x = self.dense2(x)
             x = self.dropout_layer(x, training=training)
         if self.dense3 is not None:
@@ -258,25 +266,34 @@
             x = self.dense4(x)
             x = self.dropout_layer(x, training=training)
         if self.dense5 is not None:
             x = self.dense5(x)
             x = self.dropout_layer(x, training=training)
 
         x = self.output1(x)
-        return self.rshp(x)
+        x = self.rshp(x)
+        return self.activation(x)
 
     def model(self):
         x = tf.keras.Input(shape=(self.n_components,))
-        return tf.keras.Model(inputs=[x], outputs=self.call(x))
+        x = tf.keras.Model(inputs=[x], outputs=self.call(x))
 
     def set_model_outputs(self):
         x = tf.keras.Input(shape=(self.n_components,))
         model = tf.keras.Model(inputs=[x], outputs=self.call(x))
         self.outputs = model.outputs
 
+    @property
+    def metrics(self):
+        """Set metric trackers."""
+        return [
+            self.total_loss_tracker,
+            self.binary_accuracy_tracker,
+        ]
+
     def train_step(self, data):
         """Train step function. Parameters are set in UBPCallbacks callback."""
         y = self._y
 
         (
             v,
             y_true,
@@ -338,31 +355,92 @@
 
         # Apply separate gradients to v.
         vgrad = tape.gradient(loss, src)
         self.optimizer.apply_gradients(zip(vgrad, src))
 
         del tape
 
+        # NOTE: run_eagerly must be set to True in the compile() method for this
+        # to work. Otherwise it can't convert a Tensor object to a numpy array.
+        # There is really no other way to set v back to V_latent_ in graph
+        # mode as far as I know. eager execution is slower, so it would be nice
+        # to find a way to do this without converting to numpy.
+        self.V_latent_[batch_start:batch_end, :] = v.numpy()
+
         ### NOTE: If you get the error, "'tuple' object has no attribute
         ### 'rank', then convert y_true to a tensor object."
-        self.compiled_metrics.update_state(
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
+
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
+
+    def test_step(self, data):
+        """Test step function. Parameters are set in UBPCallbacks callback."""
+        y = self._y
+
+        (
+            v,
+            y_true,
+            sample_weight,
+            missing_mask,
+            batch_start,
+            batch_end,
+        ) = self.nn.prepare_training_batches(
+            self.V_latent_,
+            y,
+            self._batch_size,
+            self._batch_idx,
+            True,
+            self.n_components,
+            self._sample_weight,
+            self._missing_mask,
+        )
+
+        if sample_weight is not None:
+            sample_weight_masked = tf.convert_to_tensor(
+                sample_weight[~missing_mask], dtype=tf.float32
+            )
+        else:
+            sample_weight_masked = None
+
+        y_true_masked = tf.boolean_mask(
+            tf.convert_to_tensor(y_true, dtype=tf.float32),
+            tf.reduce_any(tf.not_equal(y_true, -1), axis=2),
+        )
+
+        y_pred = self(v, training=False)
+        y_pred_masked = tf.boolean_mask(
+            y_pred, tf.reduce_any(tf.not_equal(y_true, -1), axis=2)
+        )
+
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank'", then convert y_true to a tensor object."
+        loss = self.compiled_loss(
             y_true_masked,
             y_pred_masked,
             sample_weight=sample_weight_masked,
+            regularization_losses=self.losses,
         )
 
-        # NOTE: run_eagerly must be set to True in the compile() method for this
-        # to work. Otherwise it can't convert a Tensor object to a numpy array.
-        # There is really no other way to set v back to V_latent_ in graph
-        # mode as far as I know. eager execution is slower, so it would be nice
-        # to find a way to do this without converting to numpy.
-        self.V_latent_[batch_start:batch_end, :] = v.numpy()
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank', then convert y_true to a tensor object."
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
 
-        # history object that gets returned from fit().
-        return {m.name: m.result() for m in self.metrics}
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
 
     @property
     def V_latent(self):
         """Randomly initialized input that gets refined during training.
         :noindex:
         """
         return self.V_latent_
```

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/models/ubp_model.py` & `pg-sui-0.3/pgsui/impute/unsupervised/models/ubp_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 from tensorflow.keras.layers import (
     Dropout,
     Dense,
     Reshape,
     LeakyReLU,
     PReLU,
+    Activation,
 )
 
 from tensorflow.keras.regularizers import l1_l2
 
 # Custom Modules
 try:
     from ..neural_network_methods import NeuralNetworkMethods
@@ -122,14 +123,19 @@
         dropout_rate=0.2,
         num_classes=3,
         phase=1,
         sample_weight=None,
     ):
         super(UBPPhase1, self).__init__()
 
+        self.total_loss_tracker = tf.keras.metrics.Mean(name="total_loss")
+        self.binary_accuracy_tracker = tf.keras.metrics.Mean(
+            name="binary_accuracy"
+        )
+
         nn = NeuralNetworkMethods()
         self.nn = nn
 
         if V is None:
             self._V = nn.init_weights(y.shape[0], n_components)
         elif isinstance(V, dict):
             self._V = V[n_components]
@@ -193,14 +199,21 @@
         return tf.keras.Model(inputs=[x], outputs=self.call(x))
 
     def set_model_outputs(self):
         x = tf.keras.Input(shape=(self.n_components,))
         model = tf.keras.Model(inputs=[x], outputs=self.call(x))
         self.outputs = model.outputs
 
+    @property
+    def metrics(self):
+        return [
+            self.total_loss_tracker,
+            self.binary_accuracy_tracker,
+        ]
+
     def train_step(self, data):
         """Train step function. Parameters are set in the UBPCallbacks callback"""
         y = self._y
 
         (
             v,
             y_true,
@@ -246,15 +259,14 @@
             )
             ### NOTE: If you get the error, "'tuple' object has no attribute
             ### 'rank'", then convert y_true to a tensor object."
             loss = self.compiled_loss(
                 y_true_masked,
                 y_pred_masked,
                 sample_weight=sample_weight_masked,
-                regularization_losses=self.losses,
             )
 
         # Refine the watched variables with
         # gradient descent backpropagation
         gradients = tape.gradient(loss, self.trainable_variables)
         self.optimizer.apply_gradients(
             zip(gradients, self.trainable_variables)
@@ -262,31 +274,91 @@
 
         # Apply separate gradients to v.
         vgrad = tape.gradient(loss, src)
         self.optimizer.apply_gradients(zip(vgrad, src))
 
         del tape
 
-        ### NOTE: If you get the error, "'tuple' object has no attribute
-        ### 'rank', then convert y_true to a tensor object."
-        self.compiled_metrics.update_state(
-            y_true_masked,
-            y_pred_masked,
-            sample_weight=sample_weight_masked,
-        )
-
         # NOTE: run_eagerly must be set to True in the compile() method for this
         # to work. Otherwise it can't convert a Tensor object to a numpy array.
         # There is really no other way to set v back to V_latent_ in graph
         # mode as far as I know. eager execution is slower, so it would be nice
         # to find a way to do this without converting to numpy.
         self.V_latent_[batch_start:batch_end, :] = v.numpy()
 
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank', then convert y_true to a tensor object."
         # history object that gets returned from model.fit().
-        return {m.name: m.result() for m in self.metrics}
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
+
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
+
+    def test_step(self, data):
+        """Train step function. Parameters are set in the UBPCallbacks callback"""
+        y = self._y
+
+        (
+            v,
+            y_true,
+            sample_weight,
+            missing_mask,
+            batch_start,
+            batch_end,
+        ) = self.nn.prepare_training_batches(
+            self.V_latent_,
+            y,
+            self._batch_size,
+            self._batch_idx,
+            True,
+            self.n_components,
+            self._sample_weight,
+            self._missing_mask,
+        )
+
+        if sample_weight is not None:
+            sample_weight_masked = tf.convert_to_tensor(
+                sample_weight[~missing_mask], dtype=tf.float32
+            )
+        else:
+            sample_weight_masked = None
+
+        y_true_masked = tf.boolean_mask(
+            tf.convert_to_tensor(y_true, dtype=tf.float32),
+            tf.reduce_any(tf.not_equal(y_true, -1), axis=2),
+        )
+
+        y_pred = self(v, training=False)
+        y_pred_masked = tf.boolean_mask(
+            y_pred, tf.reduce_any(tf.not_equal(y_true, -1), axis=2)
+        )
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank'", then convert y_true to a tensor object."
+        loss = self.compiled_loss(
+            y_true_masked,
+            y_pred_masked,
+            sample_weight=sample_weight_masked,
+        )
+
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank', then convert y_true to a tensor object."
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
+
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
 
     @property
     def V_latent(self):
         """Randomly initialized input that gets refined during training.
         :noindex:
         """
         return self.V_latent_
@@ -438,14 +510,19 @@
         dropout_rate=0.2,
         num_classes=3,
         phase=2,
         sample_weight=None,
     ):
         super(UBPPhase2, self).__init__()
 
+        self.total_loss_tracker = tf.keras.metrics.Mean(name="total_loss")
+        self.binary_accuracy_tracker = tf.keras.metrics.Mean(
+            name="binary_accuracy"
+        )
+
         nn = NeuralNetworkMethods()
         self.nn = nn
 
         if V is None:
             self._V = nn.init_weights(y.shape[0], n_components)
         elif isinstance(V, dict):
             self._V = V[n_components]
@@ -588,14 +665,21 @@
         return tf.keras.Model(inputs=[x], outputs=self.call(x))
 
     def set_model_outputs(self):
         x = tf.keras.Input(shape=(self.n_components,))
         model = tf.keras.Model(inputs=[x], outputs=self.call(x))
         self.outputs = model.outputs
 
+    @property
+    def metrics(self):
+        return [
+            self.total_loss_tracker,
+            self.binary_accuracy_tracker,
+        ]
+
     def train_step(self, data):
         """Train step function. Parameters are set in the UBPCallbacks callback"""
         y = self._y
 
         (
             v,
             y_true,
@@ -638,33 +722,91 @@
             )
             ### NOTE: If you get the error, "'tuple' object has no attribute
             ### 'rank'", then convert y_true to a tensor object."
             loss = self.compiled_loss(
                 y_true_masked,
                 y_pred_masked,
                 sample_weight=sample_weight_masked,
-                regularization_losses=self.losses,
             )
 
         # Refine the watched variables with backpropagation
         gradients = tape.gradient(loss, self.trainable_variables)
         self.optimizer.apply_gradients(
             zip(gradients, self.trainable_variables)
         )
 
         ### NOTE: If you get the error, "'tuple' object has no attribute
         ### 'rank', then convert y_true to a tensor object."
-        self.compiled_metrics.update_state(
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
+
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
+
+    def test_step(self, data):
+        """Train step function. Parameters are set in the UBPCallbacks callback"""
+        y = self._y
+
+        (
+            v,
+            y_true,
+            sample_weight,
+            missing_mask,
+            _,
+            __,
+        ) = self.nn.prepare_training_batches(
+            self.V_latent_,
+            y,
+            self._batch_size,
+            self._batch_idx,
+            True,
+            self.n_components,
+            self._sample_weight,
+            self._missing_mask,
+        )
+
+        if sample_weight is not None:
+            sample_weight_masked = tf.convert_to_tensor(
+                sample_weight[~missing_mask], dtype=tf.float32
+            )
+        else:
+            sample_weight_masked = None
+
+        y_true_masked = tf.boolean_mask(
+            tf.convert_to_tensor(y_true, dtype=tf.float32),
+            tf.reduce_any(tf.not_equal(y_true, -1), axis=2),
+        )
+
+        y_pred = self(v, training=False)
+        y_pred_masked = tf.boolean_mask(
+            y_pred, tf.reduce_any(tf.not_equal(y_true, -1), axis=2)
+        )
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank'", then convert y_true to a tensor object."
+        loss = self.compiled_loss(
             y_true_masked,
             y_pred_masked,
             sample_weight=sample_weight_masked,
         )
 
-        # history object that gets returned from fit().
-        return {m.name: m.result() for m in self.metrics}
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank', then convert y_true to a tensor object."
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
+
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
 
     @property
     def V_latent(self):
         """Randomly initialized input variable that gets refined during training.
         :noindex:
         """
         return self.V_latent_
@@ -814,14 +956,19 @@
         dropout_rate=0.2,
         num_classes=3,
         phase=3,
         sample_weight=None,
     ):
         super(UBPPhase3, self).__init__()
 
+        self.total_loss_tracker = tf.keras.metrics.Mean(name="total_loss")
+        self.binary_accuracy_tracker = tf.keras.metrics.Mean(
+            name="binary_accuracy"
+        )
+
         nn = NeuralNetworkMethods()
         self.nn = nn
 
         if V is None:
             self._V = nn.init_weights(y.shape[0], n_components)
         elif isinstance(V, dict):
             self._V = V[n_components]
@@ -926,38 +1073,47 @@
             output_shape * num_classes,
             kernel_initializer=kernel_initializer,
         )
 
         self.rshp = Reshape((output_shape, num_classes))
 
         self.dropout_layer = Dropout(rate=dropout_rate)
+        self.activation = Activation("sigmoid")
 
     def call(self, inputs, training=None):
         x = self.dense1(inputs)
         if self.dense2 is not None:
             x = self.dense2(x)
         if self.dense3 is not None:
             x = self.dense3(x)
         if self.dense4 is not None:
             x = self.dense4(x)
         if self.dense5 is not None:
             x = self.dense5(x)
 
         x = self.output1(x)
-        return self.rshp(x)
+        x = self.rshp(x)
+        return self.activation(x)
 
     def model(self):
         x = tf.keras.Input(shape=(self.n_components,))
         return tf.keras.Model(inputs=[x], outputs=self.call(x))
 
     def set_model_outputs(self):
         x = tf.keras.Input(shape=(self.n_components,))
         model = tf.keras.Model(inputs=[x], outputs=self.call(x))
         self.outputs = model.outputs
 
+    @property
+    def metrics(self):
+        return [
+            self.total_loss_tracker,
+            self.binary_accuracy_tracker,
+        ]
+
     def train_step(self, data):
         """Train step function. Parameters are set in the UBPCallbacks callback"""
         y = self._y
 
         (
             v,
             y_true,
@@ -1003,15 +1159,14 @@
             )
             ### NOTE: If you get the error, "'tuple' object has no attribute
             ### 'rank'", then convert y_true to a tensor object."
             loss = self.compiled_loss(
                 y_true_masked,
                 y_pred_masked,
                 sample_weight=sample_weight_masked,
-                regularization_losses=self.losses,
             )
 
         # Refine the watched variables with
         # gradient descent backpropagation
         gradients = tape.gradient(loss, self.trainable_variables)
         self.optimizer.apply_gradients(
             zip(gradients, self.trainable_variables)
@@ -1019,31 +1174,90 @@
 
         # Apply separate gradients to v.
         vgrad = tape.gradient(loss, src)
         self.optimizer.apply_gradients(zip(vgrad, src))
 
         del tape
 
+        # NOTE: run_eagerly must be set to True in the compile() method for this
+        # to work. Otherwise it can't convert a Tensor object to a numpy array.
+        # There is really no other way to set v back to V_latent_ in graph
+        # mode as far as I know. eager execution is slower, so it would be nice
+        # to find a way to do this without converting to numpy.
+        self.V_latent_[batch_start:batch_end, :] = v.numpy()
+
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
+
         ### NOTE: If you get the error, "'tuple' object has no attribute
         ### 'rank', then convert y_true to a tensor object."
-        self.compiled_metrics.update_state(
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
+
+    def test_step(self, data):
+        """Train step function. Parameters are set in the UBPCallbacks callback"""
+        y = self._y
+
+        (
+            v,
+            y_true,
+            sample_weight,
+            missing_mask,
+            batch_start,
+            batch_end,
+        ) = self.nn.prepare_training_batches(
+            self.V_latent_,
+            y,
+            self._batch_size,
+            self._batch_idx,
+            True,
+            self.n_components,
+            self._sample_weight,
+            self._missing_mask,
+        )
+
+        if sample_weight is not None:
+            sample_weight_masked = tf.convert_to_tensor(
+                sample_weight[~missing_mask], dtype=tf.float32
+            )
+        else:
+            sample_weight_masked = None
+
+        y_true_masked = tf.boolean_mask(
+            tf.convert_to_tensor(y_true, dtype=tf.float32),
+            tf.reduce_any(tf.not_equal(y_true, -1), axis=2),
+        )
+
+        y_pred = self(v, training=False)
+        y_pred_masked = tf.boolean_mask(
+            y_pred, tf.reduce_any(tf.not_equal(y_true, -1), axis=2)
+        )
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank'", then convert y_true to a tensor object."
+        loss = self.compiled_loss(
             y_true_masked,
             y_pred_masked,
             sample_weight=sample_weight_masked,
         )
 
-        # NOTE: run_eagerly must be set to True in the compile() method for this
-        # to work. Otherwise it can't convert a Tensor object to a numpy array.
-        # There is really no other way to set v back to V_latent_ in graph
-        # mode as far as I know. eager execution is slower, so it would be nice
-        # to find a way to do this without converting to numpy.
-        self.V_latent_[batch_start:batch_end, :] = v.numpy()
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank', then convert y_true to a tensor object."
+        self.total_loss_tracker.update_state(loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
 
-        # history object that gets returned from fit().
-        return {m.name: m.result() for m in self.metrics}
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
 
     @property
     def V_latent(self):
         """Randomly initialized input variable that gets refined during training.
         :noindex:
         """
         return self.V_latent_
```

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/models/vae_model.py` & `pg-sui-0.3/pgsui/impute/unsupervised/models/vae_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -399,14 +399,19 @@
         missing_mask=None,
         batch_size=32,
         final_activation=None,
         y=None,
     ):
         super(VAEModel, self).__init__()
 
+        self.total_loss_tracker = tf.keras.metrics.Mean(name="total_loss")
+        self.binary_accuracy_tracker = tf.keras.metrics.Mean(
+            name="binary_accuracy"
+        )
+
         self.kl_beta = K.variable(0.0)
         self.kl_beta._trainable = False
 
         self._sample_weight = sample_weight
         self._missing_mask = missing_mask
         self._batch_idx = 0
         self._batch_size = batch_size
@@ -416,21 +421,14 @@
         if num_classes == 10 or num_classes == 3:
             self.acc_func = tf.keras.metrics.categorical_accuracy
         elif num_classes == 4:
             self.acc_func = tf.keras.metrics.binary_accuracy
 
         self.nn_ = NeuralNetworkMethods()
 
-        self.total_loss_tracker = tf.keras.metrics.Mean(name="loss")
-        self.reconstruction_loss_tracker = tf.keras.metrics.Mean(
-            name="reconstruction_loss"
-        )
-        # self.kl_loss_tracker = tf.keras.metrics.Mean(name="kl_loss")
-        self.accuracy_tracker = tf.keras.metrics.Mean(name="accuracy")
-
         # y_train[1] dimension.
         self.n_features = output_shape
 
         self.n_components = n_components
         self.weights_initializer = weights_initializer
         self.hidden_layer_sizes = hidden_layer_sizes
         self.num_hidden_layers = num_hidden_layers
@@ -499,24 +497,21 @@
             hidden_layer_sizes,
             self.dropout_rate,
             activation,
             kernel_initializer,
             kernel_regularizer,
         )
 
-        if final_activation is not None:
-            self.act = Activation(final_activation)
+        self.activation = Activation("sigmoid")
 
     def call(self, inputs, training=None):
         """Forward pass for model."""
         z_mean, z_log_var, z = self.encoder(inputs)
         reconstruction = self.decoder(z)
-        if self._final_activation is not None:
-            reconstruction = self.act(reconstruction)
-        return reconstruction
+        return self.activation(reconstruction)
 
     def model(self):
         """Here so that mymodel.model().summary() can be called for debugging.
         :noindex:
         """
         x = tf.keras.Input(shape=(self.n_features, self.num_classes))
         return tf.keras.Model(inputs=[x], outputs=self.call(x))
@@ -527,20 +522,17 @@
         """
         x = tf.keras.Input(shape=(self.n_features, self.num_classes))
         model = tf.keras.Model(inputs=[x], outputs=self.call(x))
         self.outputs = model.outputs
 
     @property
     def metrics(self):
-        """Set metric trackers."""
         return [
             self.total_loss_tracker,
-            self.reconstruction_loss_tracker,
-            # self.kl_loss_tracker,
-            self.accuracy_tracker,
+            self.binary_accuracy_tracker,
         ]
 
     @tf.function
     def train_step(self, data):
         y = self._y
 
         (
@@ -580,93 +572,98 @@
             )
 
             # Returns binary crossentropy loss.
             reconstruction_loss = self.compiled_loss(
                 y_true_masked,
                 y_pred_masked,
                 sample_weight=sample_weight_masked,
+                regularization_losses=self.losses,
             )
 
             # Doesn't include KL Divergence Loss.
             regularization_loss = sum(self.losses)
 
             total_loss = reconstruction_loss + regularization_loss
 
         grads = tape.gradient(total_loss, self.trainable_variables)
         self.optimizer.apply_gradients(zip(grads, self.trainable_variables))
 
-        ### NOTE: If you get the error, "'tuple' object has no attribute
-        ### 'rank', then convert y_true to a tensor object."
-        # self.compiled_metrics.update_state(
-        self.accuracy_tracker.update_state(
-            self.acc_func(
-                y_true_masked,
-                y_pred_masked,
+        self.total_loss_tracker.update_state(total_loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
+
+        return {
+            "loss": self.total_loss_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
+        }
+
+    @tf.function
+    def test_step(self, data):
+        y = self._y
+
+        (
+            y_true,
+            sample_weight,
+            missing_mask,
+        ) = self.nn_.prepare_training_batches(
+            y,
+            y,
+            self._batch_size,
+            self._batch_idx,
+            True,
+            self.n_components,
+            self._sample_weight,
+            self._missing_mask,
+            ubp=False,
+        )
+
+        if sample_weight is not None:
+            sample_weight_masked = tf.convert_to_tensor(
+                sample_weight[~missing_mask], dtype=tf.float32
             )
+        else:
+            sample_weight_masked = None
+
+        y_true_masked = tf.boolean_mask(
+            tf.convert_to_tensor(y_true, dtype=tf.float32),
+            tf.reduce_any(tf.not_equal(y_true, -1), axis=-1),
+        )
+
+        reconstruction = self(y_true, training=False)
+
+        y_pred_masked = tf.boolean_mask(
+            reconstruction,
+            tf.reduce_any(tf.not_equal(y_true, -1), axis=-1),
+        )
+
+        reconstruction_loss = self.compiled_loss(
+            y_true_masked,
+            y_pred_masked,
+            sample_weight=sample_weight_masked,
+            regularization_losses=self.losses,
         )
 
+        # Doesn't include KL Divergence Loss.
+        regularization_loss = sum(self.losses)
+
+        total_loss = reconstruction_loss + regularization_loss
+
+        ### NOTE: If you get the error, "'tuple' object has no attribute
+        ### 'rank', then convert y_true to a tensor object."
         self.total_loss_tracker.update_state(total_loss)
-        self.reconstruction_loss_tracker.update_state(reconstruction_loss)
+        self.binary_accuracy_tracker.update_state(
+            tf.keras.metrics.binary_accuracy(y_true_masked, y_pred_masked)
+        )
 
         return {
             "loss": self.total_loss_tracker.result(),
-            "reconstruction_loss": self.reconstruction_loss_tracker.result(),
-            "accuracy": self.accuracy_tracker.result(),
+            "binary_accuracy": self.binary_accuracy_tracker.result(),
         }
 
-    # @tf.function
-    # def test_step(self, data):
-    #     if isinstance(data, tuple):
-    #         if len(data) == 2:
-    #             x, y = data
-    #             sample_weight = None
-    #         else:
-    #             x, y, sample_weight = data
-    #     else:
-    #         raise TypeError("Target y must be supplied to fit in this model.")
-
-    #     if sample_weight is not None:
-    #         sample_weight_masked = tf.boolean_mask(
-    #             tf.convert_to_tensor(sample_weight),
-    #             tf.reduce_any(tf.not_equal(y, -1), axis=2),
-    #         )
-    #     else:
-    #         sample_weight_masked = None
-
-    #     reconstruction, z_mean, z_log_var, z = self(x, training=False)
-    #     reconstruction_loss = self.compiled_loss(
-    #         y,
-    #         reconstruction,
-    #         sample_weight=sample_weight_masked,
-    #     )
-
-    #     # Includes KL Divergence Loss.
-    #     regularization_loss = sum(self.losses)
-
-    #     total_loss = reconstruction_loss + regularization_loss
-
-    #     self.accuracy_tracker.update_state(
-    #         self.cateogrical_accuracy(
-    #             y,
-    #             reconstruction,
-    #             sample_weight=sample_weight_masked,
-    #         )
-    #     )
-
-    #     self.total_loss_tracker.update_state(total_loss)
-    #     self.reconstruction_loss_tracker.update_state(reconstruction_loss)
-    #     self.kl_loss_tracker.update_state(regularization_loss)
-
-    #     return {
-    #         "loss": self.total_loss_tracker.result(),
-    #         "reconstruction_loss": self.reconstruction_loss_tracker.result(),
-    #         "kl_loss": self.kl_loss_tracker.result(),
-    #         "accuracy": self.accuracy_tracker.result(),
-    #     }
-
     @property
     def batch_size(self):
         """Batch (=step) size per epoch."""
         return self._batch_size
 
     @property
     def batch_idx(self):
```

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/neural_network_imputers.py` & `pg-sui-0.3/pgsui/impute/unsupervised/neural_network_imputers.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         ga_kwargs=None,
         scoring_metric="auc_macro",
         sim_strategy="random",
         sim_prop_missing=0.2,
         n_jobs=1,
         verbose=0,
         kl_beta=tf.Variable(1.0, trainable=False),
-        validation_split=0.0,
+        validation_split=0.2,
         nlpca=False,
         testing=False,
     ):
         self.activate = activate
         self.act_func_ = act_func
         self.num_classes = num_classes
         self.testing = testing
@@ -311,20 +311,23 @@
         self.all_missing_ = self.sim.all_missing_mask_
 
         # Just y_original with missing values encoded as -1.
         y_train = self.tt_.fit_transform(self.y_original_)
 
         if self.gridparams is not None:
             self.scoring_metrics_ = [
-                "precision_recall_macro",
-                "precision_recall_micro",
-                "f1_score",
-                "f1_score_weighted",
-                "auc_macro",
-                "auc_micro",
+                "average_precision_macro",
+                "average_precision_micro",
+                "average_precision_weighted",
+                "f1_micro",
+                "f1_macro",
+                "f1_weighted",
+                "roc_auc_macro",
+                "roc_auc_micro",
+                "roc_auc_weighted",
                 "accuracy",
                 "hamming",
             ]
 
         (
             logfile,
             callbacks,
@@ -498,15 +501,14 @@
         y_train,
         y_true,
         model_params,
         compile_params,
         fit_params,
         ubp_weights=None,
         phase=None,
-        scoring=None,
         testing=False,
         **kwargs,
     ):
         """Run KerasClassifier with neural network model and grid search.
 
         Args:
             y_train (numpy.ndarray): Onehot-encoded training input data of shape (n_samples, n_features, num_classes).
@@ -515,16 +517,14 @@
 
             model_params (Dict[str, Any]): Dictionary with model parameters to be passed to KerasClassifier model.
 
             compile_params (Dict[str, Any]): Dictionary with params to be passed to Keras model.compile() in KerasClassifier.
 
             fit_params (Dict[str, Any]): Dictionary with parameters to be passed to fit in KerasClassifier.
 
-            scoring (Dict[str, Callable], optional): Multimetric scorer made using sklearn.metrics.make_scorer. To be used with grid search.
-
         Returns:
             List[tf.keras.Model]: List of keras model objects. One for each phase (len=1 if NLPCA, len=3 if UBP).
 
             List[Dict[str, float]]: List of dictionaries with best neural network model history.
 
             Dict[str, Any] or None: Best parameters found during a grid search, or None if a grid search was not run.
 
@@ -606,27 +606,35 @@
                 loss=compile_params["loss"],
                 metrics=compile_params["metrics"],
                 epochs=fit_params["epochs"],
                 phase=phase,
                 callbacks=fit_params["callbacks"],
                 validation_split=fit_params["validation_split"],
                 verbose=0,
+                activate=self.act_func_,
                 score__missing_mask=self.sim_missing_mask_,
                 score__scoring_metric=self.scoring_metric,
             )
 
         if self.run_gridsearch_:
             # Cannot do CV because there is no way to use test splits
             # given that the input gets refined. If using a test split,
             # then it would just be the randomly initialized values and
             # would not accurately represent the model.
             # Thus, we disable cross-validation for the grid searches.
             cross_val = DisabledCV()
             verbose = False if self.verbose == 0 else True
 
+            scorers = Scorers()
+            scoring = scorers.make_multimetric_scorer(
+                self.scoring_metrics_,
+                self.sim_missing_mask_,
+                num_classes=self.num_classes,
+            )
+
             if self.ga_:
                 # Stop searching if GA sees no improvement.
                 callback = [
                     ConsecutiveStopping(
                         generations=self.early_stop_gen, metric="fitness"
                     )
                 ]
@@ -831,17 +839,14 @@
         if not self.disable_progressbar and not search_mode:
             callbacks.append(
                 TqdmCallback(epochs=self.epochs, verbose=0, desc="Epoch: ")
             )
 
         if self.nn_method_ in ["UBP", "NLPCA"]:
             vinput = self._initV(y_train, search_mode)
-            compile_params = self.nn_.set_compile_params(self.optimizer)
-        else:
-            vae = True if self.nn_method_ in ["VAE", "SAE"] else False
 
         if self.sample_weights == "auto" or self.sample_weights == "logsmooth":
             # Get class weights for each column.
             sample_weights = self.nn_.get_class_weights(
                 self.y_original_,
                 self.original_missing_mask_,
                 return_1d=False,
@@ -857,21 +862,19 @@
             sample_weights = self.nn_.get_class_weights(
                 self.y_original_, user_weights=self.sample_weights
             )
 
         else:
             sample_weights = None
 
-        vae = True if self.nn_method_ == "VAE" else False
-
         compile_params = self.nn_.set_compile_params(
             self.optimizer,
             sample_weights,
-            vae=vae,
-            act_func=self.act_func_,
+            vae=False,
+            act_func="sigmoid",
         )
 
         compile_params["learning_rate"] = self.learning_rate
 
         if self.nn_method_ in ["VAE", "SAE"]:
             model_params = {
                 "y": y_train,
@@ -913,27 +916,24 @@
 
         fit_verbose = 1 if self.verbose == 2 else 0
 
         fit_params = {
             "batch_size": self.batch_size,
             "epochs": self.epochs,
             "callbacks": callbacks,
-            "shuffle": True,
             "verbose": fit_verbose,
             "sample_weight": sample_weights,
         }
 
         if self.nn_method_ in ["VAE", "SAE"]:
-            shuffle = True
             fit_params["validation_split"] = self.validation_split
         else:
-            shuffle = False
-            fit_params["validation_split"] = 0.0
+            fit_params["validation_split"] = self.validation_split
 
-        fit_params["shuffle"] = shuffle
+        fit_params["shuffle"] = False
 
         if self.run_gridsearch_ and "learning_rate" in self.gridparams:
             self.gridparams["optimizer__learning_rate"] = self.gridparams[
                 "learning_rate"
             ]
 
             self.gridparams.pop("learning_rate")
@@ -962,20 +962,15 @@
         self.nn_method_ = "VAE"
         self.num_classes = 4
         self.activate = None
         self.is_multiclass_ = True if self.num_classes != 4 else False
         self.testing = kwargs.get("testing", False)
         self.do_act_in_model_ = True if self.activate is None else False
 
-        if self.do_act_in_model_ and self.is_multiclass_:
-            self.act_func_ = "softmax"
-        elif self.do_act_in_model_ and not self.is_multiclass_:
-            self.act_func_ = "sigmoid"
-        else:
-            self.act_func_ = None
+        self.act_func_ = None
 
         super().__init__(
             self.activate,
             self.nn_method_,
             self.num_classes,
             self.act_func_,
             **kwargs,
@@ -1021,36 +1016,28 @@
         """
         scorers = Scorers()
         scoring = None
 
         histories = list()
         models = list()
 
-        if self.run_gridsearch_:
-            scoring = scorers.make_multimetric_scorer(
-                self.scoring_metrics_,
-                self.sim_missing_mask_,
-                num_classes=self.num_classes,
-            )
-
         (
             model,
             best_history,
             best_params,
             best_score,
             best_clf,
             search,
             metrics,
         ) = self.run_clf(
             y_train,
             y_true,
             model_params,
             compile_params,
             fit_params,
-            scoring=scoring,
         )
 
         histories.append(best_history)
         models.append(model)
         del model
 
         return (
@@ -1065,18 +1052,19 @@
 
 
 class SAE(BaseNNImputer):
     def __init__(
         self,
         **kwargs,
     ):
-        self.num_classes = 3
-        self.activate = "softmax"
+        self.num_classes = 4
+        self.is_multiclass_ = True if self.num_classes != 4 else False
+        self.activate = None
         self.nn_method_ = "SAE"
-        self.act_func_ = "softmax"
+        self.act_func_ = None
         self.testing = kwargs.get("testing", False)
 
         super().__init__(
             self.activate,
             self.nn_method_,
             self.num_classes,
             self.act_func_,
@@ -1121,34 +1109,28 @@
         """
         scorers = Scorers()
         scoring = None
 
         histories = list()
         models = list()
 
-        if self.run_gridsearch_:
-            scoring = scorers.make_multimetric_scorer(
-                self.scoring_metrics_, self.sim_missing_mask_
-            )
-
         (
             model,
             best_history,
             best_params,
             best_score,
             best_clf,
             search,
             metrics,
         ) = self.run_clf(
             y_train,
             y_true,
             model_params,
             compile_params,
             fit_params,
-            scoring=scoring,
             testing=False,
         )
 
         histories.append(best_history)
         models.append(model)
         del model
 
@@ -1170,18 +1152,19 @@
         nlpca=False,
         **kwargs,
     ):
         # TODO: Make estimators compatible with variable number of classes.
         # E.g., with morphological data.
         self.nlpca = nlpca
         self.nn_method_ = "NLPCA" if self.nlpca else "UBP"
-        self.num_classes = 3
+        self.num_classes = 4
+        self.is_multiclass_ = True if self.num_classes != 4 else False
         self.testing = kwargs.get("testing", False)
         self.activate = None
-        self.act_func_ = "softmax"
+        self.act_func_ = None
 
         super().__init__(
             self.activate,
             self.nn_method_,
             self.num_classes,
             self.act_func_,
             **kwargs,
@@ -1227,20 +1210,14 @@
         scorers = Scorers()
 
         histories = list()
         models = list()
         y_train = model_params.pop("y_train")
         ubp_weights = None
         phase = None
-        scoring = None
-
-        if self.run_gridsearch_:
-            scoring = scorers.make_multimetric_scorer(
-                self.scoring_metrics_, self.sim_missing_mask_
-            )
 
         (
             V,
             model,
             best_history,
             best_params,
             best_score,
@@ -1251,15 +1228,14 @@
             y_train,
             y_true,
             model_params,
             compile_params,
             fit_params,
             ubp_weights=ubp_weights,
             phase=phase,
-            scoring=scoring,
             testing=False,
         )
 
         histories.append(best_history)
         models.append(model)
         del model
 
@@ -1320,15 +1296,17 @@
         if self.run_gridsearch_:
             # Cannot do CV because there is no way to use test splits
             # given that the input gets refined. If using a test split,
             # then it would just be the randomly initialized values and
             # would not accurately represent the model.
             # Thus, we disable cross-validation for the grid searches.
             scoring = scorers.make_multimetric_scorer(
-                self.scoring_metrics_, self.sim_missing_mask_
+                self.scoring_metrics_,
+                self.sim_missing_mask_,
+                num_classes=self.num_classes,
             )
 
             if "n_components" in self.gridparams:
                 search_n_components = True
                 n_components_searched = self.n_components
         else:
             scoring = None
@@ -1349,15 +1327,14 @@
                 y_train,
                 y_true,
                 model_params,
                 compile_params,
                 fit_params,
                 ubp_weights=ubp_weights,
                 phase=phase,
-                scoring=scoring,
                 testing=False,
             )
 
             if phase == 1:
                 # Cannot have V input with different n_components
                 # in other phases than are in phase 1.
                 # So the n_components search has to happen in phase 1.
```

### Comparing `pg-sui-0.2.4/pgsui/impute/unsupervised/neural_network_methods.py` & `pg-sui-0.3/pgsui/impute/unsupervised/neural_network_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         y_true_bin,
         y_pred_proba,
         is_multiclass=True,
         return_proba=False,
         return_multilab=False,
         return_int=True,
         predict_still_missing=True,
-        threshold_increment=0.01,
+        threshold_increment=0.1,
         multilabel_averaging="macro",
         missing_mask=None,
     ):
         """Evaluate model predictions by decoding from one-hot encoding to integer-encoded format.
 
         Gets the index of the highest predicted value to obtain the integer encodings or integer encodings.
 
@@ -859,16 +859,16 @@
                 )
 
             loss = loss_func()
             metrics = None
 
         else:
             # Doing grid search. Params are callables.
-            loss = tf.keras.losses.CategoricalCrossentropy(from_logits=True)
-            metrics = [tf.keras.metrics.CategoricalAccuracy()]
+            loss = tf.keras.losses.BinaryCrossentropy(from_logits=False)
+            metrics = [tf.keras.metrics.BinaryAccuracy()]
 
         return {
             "optimizer": opt,
             "loss": loss,
             "metrics": metrics,
             "run_eagerly": False,
         }
```

### Comparing `pg-sui-0.2.4/pgsui/pg_sui.py` & `pg-sui-0.3/pgsui/pg_sui.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/utils/misc.py` & `pg-sui-0.3/pgsui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/pgsui/utils/plotting.py` & `pg-sui-0.3/pgsui/utils/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -712,85 +712,46 @@
                 f"{prefix}_output",
                 "plots",
                 "Unsupervised",
                 nn_method,
                 "histplot.pdf",
             )
 
-            if nn_method == "VAE":
-                fig, axes = plt.subplots(2, 2)
-                ax1 = axes[0, 0]
-                ax2 = axes[0, 1]
-                # ax3 = axes[1, 0]
-                # ax4 = axes[1, 1]
-            else:
-                fig, (ax1, ax2) = plt.subplots(1, 2)
+            # if nn_method == "VAE":
+            fig, axes = plt.subplots(1, 2)
+            ax1 = axes[0]
+            ax2 = axes[1]
+
             fig.suptitle(title)
             fig.tight_layout(h_pad=3.0, w_pad=3.0)
             history = lod[0]
 
-            acctrain = (
-                "categorical_accuracy" if nn_method == "NLPCA" else "accuracy"
-            )
-
-            # if nn_method == "VAE":
-            #     accval = "val_accuracy"
-            #     # recon_loss = "reconstruction_loss"
-            #     # kl_loss = "kl_loss"
-            #     # val_recon_loss = "val_reconstruction_loss"
-            #     # val_kl_loss = "val_kl_loss"
-            #     lossval = "val_loss"
-
-            if nn_method == "SAE":
-                accval = "val_accuracy"
-                lossval = "val_loss"
+            acctrain = "binary_accuracy"
+            accval = "val_binary_accuracy"
+            lossval = "val_loss"
 
             # Plot train accuracy
             ax1.plot(history[acctrain])
             ax1.set_title("Model Accuracy")
             ax1.set_ylabel("Accuracy")
             ax1.set_xlabel("Epoch")
             ax1.set_ylim(bottom=0.0, top=1.0)
             ax1.set_yticks([0.0, 0.25, 0.5, 0.75, 1.0])
 
             labels = ["Train"]
-            if nn_method == "SAE":
-                # Plot validation accuracy
-                ax1.plot(history[accval])
-                labels.append("Validation")
 
-            ax1.legend(labels, loc="best")
+            # Plot validation accuracy
+            ax1.plot(history[accval])
+            labels.append("Validation")
 
-            # Plot model loss
-            # if nn_method == "VAE":
-            #     # Reconstruction loss only.
-            #     ax2.plot(history["loss"])
-            # ax2.plot(history[val_recon_loss])
-
-            # # KL Loss
-            # ax3.plot(history[kl_loss])
-            # ax3.plot(history[val_kl_loss])
-            # ax3.set_title("KL Divergence Loss")
-            # ax3.set_ylabel("Loss")
-            # ax3.set_xlabel("Epoch")
-            # ax3.legend(labels, loc="best")
-
-            # Total Loss (Reconstruction Loss + KL Loss)
-            # ax4.plot(history["loss"])
-            # ax4.plot(history[lossval])
-            # ax4.set_title("Total Loss (Recon. + KL)")
-            # ax4.set_ylabel("Loss")
-            # ax4.set_xlabel("Epoch")
-            # ax4.legend(labels, loc="best")
+            ax1.legend(labels, loc="best")
 
             # else:
             ax2.plot(history["loss"])
-
-            if nn_method == "SAE":
-                ax2.plot(history[lossval])
+            ax2.plot(history[lossval])
 
             ax2.set_title("Total Loss")
             ax2.set_ylabel("Loss")
             ax2.set_xlabel("Epoch")
             ax2.legend(labels, loc="best")
 
             fig.savefig(fn, bbox_inches="tight", facecolor="white")
@@ -813,29 +774,35 @@
             idx = 1
             for i, history in enumerate(lod, start=1):
                 plt.subplot(3, 2, idx)
                 title = f"Phase {i}"
 
                 # Plot model accuracy
                 ax = plt.gca()
-                ax.plot(history["categorical_accuracy"])
+                ax.plot(history["binary_accuracy"])
                 ax.set_title(f"{title} Accuracy")
                 ax.set_ylabel("Accuracy")
                 ax.set_xlabel("Epoch")
                 ax.set_yticks([0.0, 0.25, 0.5, 0.75, 1.0])
-                ax.legend(["Training"], loc="best")
+
+                # Plot validation accuracy
+                ax.plot(history["val_binary_accuracy"])
+                ax.legend(["Train", "Validation"], loc="best")
 
                 # Plot model loss
                 plt.subplot(3, 2, idx + 1)
                 ax = plt.gca()
                 ax.plot(history["loss"])
                 ax.set_title(f"{title} Loss")
                 ax.set_ylabel("Loss (MSE)")
                 ax.set_xlabel("Epoch")
-                ax.legend(["Train"], loc="best")
+
+                # Plot validation loss
+                ax.plot(history["val_loss"])
+                ax.legend(["Train", "Validation"], loc="best")
 
                 idx += 2
 
             plt.savefig(fn, bbox_inches="tight", facecolor="white")
 
             plt.close()
             plt.clf()
```

### Comparing `pg-sui-0.2.4/pgsui/utils/sequence_tools.py` & `pg-sui-0.3/pgsui/utils/sequence_tools.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/setup.py` & `pg-sui-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 NAME = "pg-sui"
-VERSION = "0.2.4"
+VERSION = "0.3"
 AUTHORS = "Bradley T. Martin and Tyler K. Chafin"
 AUTHOR_EMAIL = "evobio721@gmail.com"
 MAINTAINER = "Bradley T. Martin"
 DESCRIPTION = "Python machine and deep learning package to impute missing SNPs"
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
@@ -28,28 +28,30 @@
     project_urls={
         "Homepage": "https://github.com/btmartin721/PG-SUI",
         "Documentation": "https://pg-sui.readthedocs.io/en/latest/",
         "Source": "https://github.com/btmartin721/PG-SUI.git",
         "Bug Tracker": "https://github.com/btmartin721/PG-SUI/issues",
     },
     keywords=[
-        "python",
         "impute",
         "imputation",
         "imputer",
         "machine learning",
         "neural network",
+        "deep learning",
+        "python",
         "api",
-        "IterativeImputer",
         "vae",
+        "autoencoder",
         "ubp",
         "nlpca",
-        "autoencoder",
-        "deep learning",
         "population genomics",
+        "unsupervised",
+        "supervised",
+        "IterativeImputer",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
@@ -59,15 +61,15 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Operating System :: OS Independent",
         "Natural Language :: English",
     ],
     license="GNU General Public License v3 (GPLv3)",
     packages=find_packages(),
-    python_requires=">=3.8,<4",
+    python_requires=">=3.8",
     install_requires=[
         "matplotlib",
         "seaborn",
         "jupyterlab",
         "scikit-learn>=1.0",
         "tqdm",
         "pandas",
```

### Comparing `pg-sui-0.2.4/simulation/sim_benchmarks.py` & `pg-sui-0.3/simulation/sim_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/simulation/sim_treeparams.py` & `pg-sui-0.3/simulation/sim_treeparams.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/test/pg_sui_simtest.py` & `pg-sui-0.3/test/pg_sui_simtest.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/test/pg_sui_testing.py` & `pg-sui-0.3/test/pg_sui_testing.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/test/test.py` & `pg-sui-0.3/test/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from sklearn.metrics import (
     balanced_accuracy_score,
     roc_auc_score,
     precision_recall_fscore_support,
     f1_score,
     average_precision_score,
+    accuracy_score,
 )
 
 from sklearn.preprocessing import label_binarize
 
 from sklearn.utils.class_weight import compute_class_weight
 
 
@@ -66,35 +67,36 @@
                 param_grid = {"n_neighbors": [5, 8]}
         else:
             param_grid = None
 
         instance = class_instance(
             self.simulated_data,
             gridparams=param_grid,
+            sample_weights=None,
         )
-        imputed_data = instance.imputed.genotypes_012(fmt="numpy")
+        imputed_data = instance.imputed.genotypes_int
 
         # Test that the imputed values are close to the original values
         # accuracy = self.transformer.accuracy(
         #     self.genotype_data.genotypes_012(fmt="numpy"), imputed_data
         # )
 
         (
             accuracy,
             auc_roc_scores,
             precision_scores,
             recall_scores,
             avg_precision_scores,
             f1,
         ) = self._scoring_metrics(
-            self.genotype_data.genotypes_012(fmt="numpy"), imputed_data
+            self.genotype_data.genotypes_int, imputed_data
         )
 
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
-            f"BALANCED ACCURACY: {accuracy}"
+            f"ACCURACY: {accuracy}"
         )
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
             f"AUC-ROC: {auc_roc_scores}"
         )
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
             f"PRECISION: {precision_scores}"
         )
@@ -105,67 +107,67 @@
             f"AVERAGE PRECISION: {avg_precision_scores}"
         )
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
             f"F1 SCORE: {f1}"
         )
         print("\n")
 
-    # def test_ImputeKNN(self):
-    #     self._test_class(ImputeKNN)
+    def test_ImputeKNN(self):
+        self._test_class(ImputeKNN)
 
-    # def test_ImputeRandomForest(self):
-    #     self._test_class(ImputeRandomForest)
+    def test_ImputeRandomForest(self):
+        self._test_class(ImputeRandomForest)
 
-    # def test_ImputeXGBoost(self):
-    #     self._test_class(ImputeXGBoost)
+    def test_ImputeXGBoost(self):
+        self._test_class(ImputeXGBoost)
 
-    # def test_ImputeVAE(self):
-    #     self._test_class(ImputeVAE)
+    def test_ImputeVAE(self):
+        self._test_class(ImputeVAE)
 
-    # def test_ImputeStandardAutoEncoder(self):
-    #     self._test_class(ImputeStandardAutoEncoder)
+    def test_ImputeStandardAutoEncoder(self):
+        self._test_class(ImputeStandardAutoEncoder)
 
-    # def test_ImputeUBP(self):
-    #     self._test_class(ImputeUBP)
+    def test_ImputeUBP(self):
+        self._test_class(ImputeUBP)
 
-    # def test_ImputeNLPCA(self):
-    #     self._test_class(ImputeNLPCA)
+    def test_ImputeNLPCA(self):
+        self._test_class(ImputeNLPCA)
 
-    # def test_ImputeKNN_grid(self):
-    #     self._test_class(ImputeKNN, do_gridsearch=True)
+    def test_ImputeKNN_grid(self):
+        self._test_class(ImputeKNN, do_gridsearch=True)
 
-    # def test_ImputeRandomForest_grid(self):
-    #     self._test_class(ImputeRandomForest, do_gridsearch=True)
+    def test_ImputeRandomForest_grid(self):
+        self._test_class(ImputeRandomForest, do_gridsearch=True)
 
-    # def test_ImputeXGBoost_grid(self):
-    #     self._test_class(ImputeXGBoost, do_gridsearch=True)
+    def test_ImputeXGBoost_grid(self):
+        self._test_class(ImputeXGBoost, do_gridsearch=True)
 
     def test_ImputeVAE_grid(self):
         self._test_class(ImputeVAE, do_gridsearch=True)
 
-    # def test_ImputeStandardAutoEncoder_grid(self):
-    #     self._test_class(ImputeStandardAutoEncoder, do_gridsearch=True)
+    def test_ImputeStandardAutoEncoder_grid(self):
+        self._test_class(ImputeStandardAutoEncoder, do_gridsearch=True)
 
-    # def test_ImputeUBP_grid(self):
-    #     self._test_class(ImputeUBP, do_gridsearch=True)
+    def test_ImputeUBP_grid(self):
+        self._test_class(ImputeUBP, do_gridsearch=True)
 
-    # def test_ImputeNLPCA_grid(self):
-    #     self._test_class(ImputeNLPCA, do_gridsearch=True)
+    def test_ImputeNLPCA_grid(self):
+        self._test_class(ImputeNLPCA, do_gridsearch=True)
 
-    # def test_ImputePhylo(self):
-    #     self._test_class(ImputePhylo)
+    def test_ImputePhylo(self):
+        self._test_class(ImputePhylo)
 
-    # def test_ImputeAlleleFreq(self):
-    #     self._test_class(ImputeAlleleFreq)
+    def test_ImputeAlleleFreq(self):
+        self._test_class(ImputeAlleleFreq)
 
-    # def test_ImputeMF(self):
-    #     self._test_class(ImputeMF)
+    def test_ImputeMF(self):
+        self._test_class(ImputeMF)
 
-    # def test_ImputeRefAllele(self):
-    #     self._test_class(ImputeRefAllele)
+    def test_ImputeRefAllele(self):
+        self._test_class(ImputeRefAllele)
 
     def _scoring_metrics(self, y_true, y_pred):
         """Calcuate AUC-ROC, Precision-Recall, and Average Precision (AP).
 
         Args:
             X_true (np.ndarray): True values.
 
@@ -181,15 +183,15 @@
         y_true = y_true[self.transformer.sim_missing_mask_]
         y_pred = y_pred[self.transformer.sim_missing_mask_]
 
         # Binarize the output
         y_true_bin = label_binarize(y_true, classes=[0, 1, 2])
         y_pred_bin = label_binarize(y_pred, classes=[0, 1, 2])
 
-        accuracy = balanced_accuracy_score(y_true, y_pred)
+        accuracy = accuracy_score(y_true, y_pred)
 
         # AUC-ROC score
         auc_roc = roc_auc_score(y_true_bin, y_pred_bin, average="weighted")
 
         # Precision-recall score
         precision, recall, _, _ = precision_recall_fscore_support(
             y_true_bin, y_pred_bin, average="weighted"
```

### Comparing `pg-sui-0.2.4/test/test_pgsui.py` & `pg-sui-0.3/test/test_pgsui.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.2.4/test/test_tkc.py` & `pg-sui-0.3/test/test_tkc.py`

 * *Files 26% similar despite different names*

```diff
@@ -86,17 +86,14 @@
         }
 
         instance = class_instance(
             self.simulated_data, 
             gridparams=param_grid, 
             **kwargs)
 
-        # Write the masks
-        self.transformer.write_mask(filename_prefix="mask_test")
-
         imputed_data = instance.imputed.genotypes_012(fmt="numpy")
 
         # Test that the imputed values are close to the original values
         accuracy = self.transformer.accuracy(
             self.genotype_data.genotypes_012(fmt="numpy"), imputed_data
         )
 
@@ -120,59 +117,33 @@
         )
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
             f"RECALL PER CLASS: {dict(zip(range(3), recall_scores))}"
         )
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
             f"AVERAGE PRECISION PER CLASS: {dict(zip(range(3), avg_precision_scores))}"
         )
-
-        # Read masks from file
-        self.transformer.read_mask(filename_prefix="mask_test")
-
-        # Recalculate accuracy after reading in the mask
-        accuracy_after_read = self.transformer.accuracy(
-            self.genotype_data.genotypes_012(fmt="numpy"), imputed_data
-        )
-
-        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
-            f"OVERALL ACCURACY AFTER READ: {accuracy_after_read}"
-        )
-        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
-            f"AUC-ROC PER CLASS AFTER READ: {dict(zip(range(3), auc_roc_scores))}"
-        )
-        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
-            f"PRECISION PER CLASS AFTER READ: {dict(zip(range(3), precision_scores))}"
-        )
-        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
-            f"RECALL PER CLASS AFTER READ: {dict(zip(range(3), recall_scores))}"
-        )
-        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
-            f"AVERAGE PRECISION PER CLASS AFTER READ: {dict(zip(range(3), avg_precision_scores))}"
-        )
-
-
         print("\n")
 
     # def test_ImputeKNN(self):
     #     self._test_class(ImputeKNN)
 
     # def test_ImputeRandomForest(self):
     #     self._test_class(ImputeRandomForest)
 
     # def test_ImputeXGBoost(self):
     #     self._test_class(ImputeXGBoost)
 
-    def test_ImputeVAE(self):
-        self._test_class(ImputeVAE)
+    # def test_ImputeVAE(self):
+    #     self._test_class(ImputeVAE)
 
     # def test_ImputeStandardAutoEncoder(self):
     #     self._test_class(ImputeStandardAutoEncoder)
 
-    # def test_ImputeUBP(self):
-    #     self._test_class(ImputeUBP)
+    def test_ImputeUBP(self):
+        self._test_class(ImputeUBP)
 
     # def test_ImputeNLPCA(self):
     #     self._test_class(ImputeNLPCA)
 
     # def test_ImputeKNN_grid(self):
     #     self._test_class(ImputeKNN, do_gridsearch=True)
```

