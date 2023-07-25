# Comparing `tmp/PyBADS-1.0.1.tar.gz` & `tmp/PyBADS-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBADS-1.0.1.tar", last modified: Thu Jul 13 15:52:54 2023, max compression
+gzip compressed data, was "PyBADS-1.0.2.tar", last modified: Tue Jul 25 10:32:15 2023, max compression
```

## Comparing `PyBADS-1.0.1.tar` & `PyBADS-1.0.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.097682 PyBADS-1.0.1/.github/
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.100682 PyBADS-1.0.1/.github/workflows/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      504 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1297 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2223 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/merge-tests.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1054 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2258 2023-06-10 16:10:47.000000 PyBADS-1.0.1/.gitignore
--rw-r--r--   0 jeet      (1000) jeet      (1000)      619 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1517 2022-12-31 10:58:21.000000 PyBADS-1.0.1/LICENSE
--rw-r--r--   0 jeet      (1000) jeet      (1000)       12 2023-06-10 16:10:47.000000 PyBADS-1.0.1/MANIFEST.in
--rw-r--r--   0 jeet      (1000) jeet      (1000)    12476 2023-07-13 15:52:54.112682 PyBADS-1.0.1/PKG-INFO
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.100682 PyBADS-1.0.1/PyBADS.egg-info/
--rw-r--r--   0 jeet      (1000) jeet      (1000)    12476 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/PKG-INFO
--rw-r--r--   0 jeet      (1000) jeet      (1000)     3456 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/SOURCES.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)        1 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/dependency_links.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)      313 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/requires.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)        7 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/top_level.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10509 2023-07-07 08:40:58.000000 PyBADS-1.0.1/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)      137 2022-12-31 10:58:21.000000 PyBADS-1.0.1/environment.yml
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.101682 PyBADS-1.0.1/examples/
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10228 2023-07-07 08:40:58.000000 PyBADS-1.0.1/examples/pybads_example_1_basic_usage.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9736 2023-07-07 08:40:58.000000 PyBADS-1.0.1/examples/pybads_example_2_nonbox_constraints.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    14356 2023-07-07 08:40:58.000000 PyBADS-1.0.1/examples/pybads_example_3_noisy_objective.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    17944 2023-07-07 08:30:17.000000 PyBADS-1.0.1/examples/pybads_example_4_user_provided_noise.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10359 2023-07-07 08:30:17.000000 PyBADS-1.0.1/examples/pybads_example_5_extended_usage.ipynb
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.102682 PyBADS-1.0.1/examples/scripts/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      981 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_1_basic_usage.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1179 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_2_nonbox_constraints.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1307 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_3_noisy_objective.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1637 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_4_user_provided_noise.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1629 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_5_extended_usage.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.103682 PyBADS-1.0.1/pybads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      556 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      635 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/__main__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      160 2023-07-13 15:52:53.000000 PyBADS-1.0.1/pybads/_version.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.103682 PyBADS-1.0.1/pybads/acquisition_functions/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       37 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/acquisition_functions/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1418 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/acquisition_functions/acq_fcn_lcb.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.104682 PyBADS-1.0.1/pybads/bads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      255 2023-06-10 07:26:33.000000 PyBADS-1.0.1/pybads/bads/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)      388 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)   103341 2023-06-10 18:40:03.000000 PyBADS-1.0.1/pybads/bads/bads.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2249 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/bads_dump.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    38330 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/gaussian_process_train.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5870 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/optimize_result.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.105682 PyBADS-1.0.1/pybads/bads/option_configs/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       53 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    15922 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/advanced_bads_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)      805 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/basic_bads_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/options_confs.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/option_configs/test_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)      108 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/option_configs/test_options2.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)     7371 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/bads/options.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.105682 PyBADS-1.0.1/pybads/decorators/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      573 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/decorators/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)       51 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/decorators/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2175 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/decorators/handle_0D_1D_input.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1779 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/function_examples.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.106682 PyBADS-1.0.1/pybads/function_logger/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      106 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/function_logger/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1731 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/function_logger/constraints_check.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    16376 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/function_logger/function_logger.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.106682 PyBADS-1.0.1/pybads/init_functions/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       35 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/init_functions/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1256 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/init_functions/init_sobol.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.106682 PyBADS-1.0.1/pybads/poll/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/poll/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1403 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/poll/poll_mads_2n.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.107682 PyBADS-1.0.1/pybads/search/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      177 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/search/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10448 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/search/es_search.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1659 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/search/grid_functions.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5383 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/search/search_hedge.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.107682 PyBADS-1.0.1/pybads/stats/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      110 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/stats/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)       87 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/stats/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1197 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/stats/get_hpd.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     8723 2023-06-10 07:27:45.000000 PyBADS-1.0.1/pybads/stats/kde1d.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1435 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/stats/kldiv_mvn.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.108682 PyBADS-1.0.1/pybads/testing/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/__init__.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.109682 PyBADS-1.0.1/pybads/testing/bads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      349 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/X.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      202 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/dF.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)      211 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/dF_gplogjoint.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1286 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/hyp.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)       89 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/mu.dat
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.109682 PyBADS-1.0.1/pybads/testing/bads/poll/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/poll/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      551 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/poll/test_poll_mads.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.110682 PyBADS-1.0.1/pybads/testing/bads/scripts/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      747 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/ackley_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2631 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1874 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/bads_rosenbrock_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      908 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/non_bound_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      780 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/rastrigin_example.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.110682 PyBADS-1.0.1/pybads/testing/bads/search/
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5583 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/testing/bads/search/test_search.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     3953 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/testing/bads/test_bads_optimization.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     6697 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/test_gaussian_process_train.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      132 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/test_init_conf.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4933 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/test_iteration_history.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      192 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/y.dat
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.110682 PyBADS-1.0.1/pybads/testing/decorators/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/decorators/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4746 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.111682 PyBADS-1.0.1/pybads/testing/function_logger/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/function_logger/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9336 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/function_logger/test_function_logger.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      240 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/run_tests.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.111682 PyBADS-1.0.1/pybads/testing/variable_transformer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/variable_transformer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5524 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/variable_transformer/test_variable_transformer.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/pybads/utils/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      119 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4359 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/iteration_history.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      117 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/period_check.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/pybads/utils/timer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/utils/timer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1544 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/timer/timer.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/pybads/variable_transformer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       55 2023-06-27 15:19:01.000000 PyBADS-1.0.1/pybads/variable_transformer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10171 2023-06-10 18:40:03.000000 PyBADS-1.0.1/pybads/variable_transformer/variables_transformer.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1477 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pyproject.toml
--rw-r--r--   0 jeet      (1000) jeet      (1000)       38 2023-07-13 15:52:54.113682 PyBADS-1.0.1/setup.cfg
--rw-r--r--   0 jeet      (1000) jeet      (1000)      169 2023-04-23 21:57:13.000000 PyBADS-1.0.1/setup.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.549604 PyBADS-1.0.2/
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.533604 PyBADS-1.0.2/.github/
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.537604 PyBADS-1.0.2/.github/workflows/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      504 2023-04-23 21:57:13.000000 PyBADS-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1297 2023-04-23 21:57:13.000000 PyBADS-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2223 2023-04-23 21:57:13.000000 PyBADS-1.0.2/.github/workflows/merge-tests.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1054 2023-04-23 21:57:13.000000 PyBADS-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2258 2023-06-10 16:10:47.000000 PyBADS-1.0.2/.gitignore
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      619 2023-04-23 21:57:13.000000 PyBADS-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1517 2022-12-31 10:58:21.000000 PyBADS-1.0.2/LICENSE
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       12 2023-06-10 16:10:47.000000 PyBADS-1.0.2/MANIFEST.in
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    12476 2023-07-25 10:32:15.549604 PyBADS-1.0.2/PKG-INFO
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.537604 PyBADS-1.0.2/PyBADS.egg-info/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    12476 2023-07-25 10:32:15.000000 PyBADS-1.0.2/PyBADS.egg-info/PKG-INFO
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     3456 2023-07-25 10:32:15.000000 PyBADS-1.0.2/PyBADS.egg-info/SOURCES.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        1 2023-07-25 10:32:15.000000 PyBADS-1.0.2/PyBADS.egg-info/dependency_links.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      298 2023-07-25 10:32:15.000000 PyBADS-1.0.2/PyBADS.egg-info/requires.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        7 2023-07-25 10:32:15.000000 PyBADS-1.0.2/PyBADS.egg-info/top_level.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10509 2023-07-07 08:40:58.000000 PyBADS-1.0.2/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      137 2022-12-31 10:58:21.000000 PyBADS-1.0.2/environment.yml
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.539604 PyBADS-1.0.2/examples/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10228 2023-07-07 08:40:58.000000 PyBADS-1.0.2/examples/pybads_example_1_basic_usage.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     9736 2023-07-07 08:40:58.000000 PyBADS-1.0.2/examples/pybads_example_2_nonbox_constraints.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    14356 2023-07-07 08:40:58.000000 PyBADS-1.0.2/examples/pybads_example_3_noisy_objective.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    17944 2023-07-07 08:30:17.000000 PyBADS-1.0.2/examples/pybads_example_4_user_provided_noise.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10359 2023-07-07 08:30:17.000000 PyBADS-1.0.2/examples/pybads_example_5_extended_usage.ipynb
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.539604 PyBADS-1.0.2/examples/scripts/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      981 2023-06-10 16:10:47.000000 PyBADS-1.0.2/examples/scripts/pybads_example_1_basic_usage.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1179 2023-06-10 16:10:47.000000 PyBADS-1.0.2/examples/scripts/pybads_example_2_nonbox_constraints.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1307 2023-06-10 16:10:47.000000 PyBADS-1.0.2/examples/scripts/pybads_example_3_noisy_objective.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1637 2023-07-19 08:54:22.000000 PyBADS-1.0.2/examples/scripts/pybads_example_4_user_provided_noise.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1629 2023-06-10 16:10:47.000000 PyBADS-1.0.2/examples/scripts/pybads_example_5_extended_usage.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.540604 PyBADS-1.0.2/pybads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      556 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      635 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/__main__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      160 2023-07-25 10:32:15.000000 PyBADS-1.0.2/pybads/_version.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.540604 PyBADS-1.0.2/pybads/acquisition_functions/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       37 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/acquisition_functions/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1418 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/acquisition_functions/acq_fcn_lcb.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.541604 PyBADS-1.0.2/pybads/bads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      255 2023-06-10 07:26:33.000000 PyBADS-1.0.2/pybads/bads/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      388 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/bads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)   103463 2023-07-24 12:29:06.000000 PyBADS-1.0.2/pybads/bads/bads.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2249 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/bads/bads_dump.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    38535 2023-07-24 12:29:06.000000 PyBADS-1.0.2/pybads/bads/gaussian_process_train.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5870 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/bads/optimize_result.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.542604 PyBADS-1.0.2/pybads/bads/option_configs/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       53 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/bads/option_configs/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    15922 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/bads/option_configs/advanced_bads_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      805 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/bads/option_configs/basic_bads_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/bads/option_configs/options_confs.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/bads/option_configs/test_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      108 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/bads/option_configs/test_options2.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     7371 2022-12-31 10:58:21.000000 PyBADS-1.0.2/pybads/bads/options.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.542604 PyBADS-1.0.2/pybads/decorators/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      573 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/decorators/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       51 2022-12-31 10:58:21.000000 PyBADS-1.0.2/pybads/decorators/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2175 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/decorators/handle_0D_1D_input.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1779 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/function_examples.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.543604 PyBADS-1.0.2/pybads/function_logger/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      106 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/function_logger/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1731 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/function_logger/constraints_check.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    16376 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/function_logger/function_logger.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.543604 PyBADS-1.0.2/pybads/init_functions/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       35 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/init_functions/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1256 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/init_functions/init_sobol.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.543604 PyBADS-1.0.2/pybads/poll/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/poll/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1403 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/poll/poll_mads_2n.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.544604 PyBADS-1.0.2/pybads/search/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      177 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/search/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10448 2023-07-07 08:40:58.000000 PyBADS-1.0.2/pybads/search/es_search.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1659 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/search/grid_functions.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5383 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/search/search_hedge.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.545604 PyBADS-1.0.2/pybads/stats/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      110 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/stats/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       87 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/stats/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1197 2022-12-31 10:58:21.000000 PyBADS-1.0.2/pybads/stats/get_hpd.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     8723 2023-06-10 07:27:45.000000 PyBADS-1.0.2/pybads/stats/kde1d.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1435 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/stats/kldiv_mvn.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.545604 PyBADS-1.0.2/pybads/testing/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/__init__.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.546604 PyBADS-1.0.2/pybads/testing/bads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      349 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/X.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      202 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/dF.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      211 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/dF_gplogjoint.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1286 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/hyp.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       89 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/mu.dat
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.547604 PyBADS-1.0.2/pybads/testing/bads/poll/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/poll/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      551 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/poll/test_poll_mads.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.547604 PyBADS-1.0.2/pybads/testing/bads/scripts/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      747 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/scripts/ackley_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2631 2023-07-24 12:29:06.000000 PyBADS-1.0.2/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1874 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/scripts/bads_rosenbrock_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      908 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/scripts/non_bound_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      780 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/scripts/rastrigin_example.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.547604 PyBADS-1.0.2/pybads/testing/bads/search/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5583 2023-07-07 08:40:58.000000 PyBADS-1.0.2/pybads/testing/bads/search/test_search.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4199 2023-07-24 12:29:06.000000 PyBADS-1.0.2/pybads/testing/bads/test_bads_optimization.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     6697 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/test_gaussian_process_train.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      132 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/test_init_conf.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4933 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/test_iteration_history.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      192 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/bads/y.dat
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.547604 PyBADS-1.0.2/pybads/testing/decorators/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/decorators/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4746 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.548604 PyBADS-1.0.2/pybads/testing/function_logger/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/function_logger/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     9336 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/function_logger/test_function_logger.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      240 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/run_tests.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.548604 PyBADS-1.0.2/pybads/testing/variable_transformer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/variable_transformer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5524 2023-06-10 16:10:47.000000 PyBADS-1.0.2/pybads/testing/variable_transformer/test_variable_transformer.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.548604 PyBADS-1.0.2/pybads/utils/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      119 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/utils/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4359 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/utils/iteration_history.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      117 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/utils/period_check.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.549604 PyBADS-1.0.2/pybads/utils/timer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2022-12-31 10:58:21.000000 PyBADS-1.0.2/pybads/utils/timer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1544 2023-04-23 21:57:13.000000 PyBADS-1.0.2/pybads/utils/timer/timer.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-25 10:32:15.549604 PyBADS-1.0.2/pybads/variable_transformer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       55 2023-06-27 15:19:01.000000 PyBADS-1.0.2/pybads/variable_transformer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10233 2023-07-24 12:29:06.000000 PyBADS-1.0.2/pybads/variable_transformer/variables_transformer.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1453 2023-07-24 12:29:06.000000 PyBADS-1.0.2/pyproject.toml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       38 2023-07-25 10:32:15.549604 PyBADS-1.0.2/setup.cfg
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      169 2023-04-23 21:57:13.000000 PyBADS-1.0.2/setup.py
```

### Comparing `PyBADS-1.0.1/.github/workflows/docs.yml` & `PyBADS-1.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/.github/workflows/merge-tests.yml` & `PyBADS-1.0.2/.github/workflows/merge-tests.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/.github/workflows/tests.yml` & `PyBADS-1.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/.gitignore` & `PyBADS-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/.pre-commit-config.yaml` & `PyBADS-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/LICENSE` & `PyBADS-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/PKG-INFO` & `PyBADS-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBADS
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bayesian Adaptive Direct Search in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2022, acerbilab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `PyBADS-1.0.1/PyBADS.egg-info/PKG-INFO` & `PyBADS-1.0.2/PyBADS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBADS
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bayesian Adaptive Direct Search in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2022, acerbilab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `PyBADS-1.0.1/PyBADS.egg-info/SOURCES.txt` & `PyBADS-1.0.2/PyBADS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/README.md` & `PyBADS-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/pybads_example_1_basic_usage.ipynb` & `PyBADS-1.0.2/examples/pybads_example_1_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/pybads_example_2_nonbox_constraints.ipynb` & `PyBADS-1.0.2/examples/pybads_example_2_nonbox_constraints.ipynb`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/pybads_example_3_noisy_objective.ipynb` & `PyBADS-1.0.2/examples/pybads_example_3_noisy_objective.ipynb`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/pybads_example_4_user_provided_noise.ipynb` & `PyBADS-1.0.2/examples/pybads_example_4_user_provided_noise.ipynb`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/pybads_example_5_extended_usage.ipynb` & `PyBADS-1.0.2/examples/pybads_example_5_extended_usage.ipynb`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/scripts/pybads_example_1_basic_usage.py` & `PyBADS-1.0.2/examples/scripts/pybads_example_1_basic_usage.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/scripts/pybads_example_2_nonbox_constraints.py` & `PyBADS-1.0.2/examples/scripts/pybads_example_2_nonbox_constraints.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/scripts/pybads_example_3_noisy_objective.py` & `PyBADS-1.0.2/examples/scripts/pybads_example_3_noisy_objective.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/scripts/pybads_example_4_user_provided_noise.py` & `PyBADS-1.0.2/examples/scripts/pybads_example_4_user_provided_noise.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/examples/scripts/pybads_example_5_extended_usage.py` & `PyBADS-1.0.2/examples/scripts/pybads_example_5_extended_usage.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/__init__.py` & `PyBADS-1.0.2/pybads/__init__.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/__main__.py` & `PyBADS-1.0.2/pybads/__main__.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/acquisition_functions/acq_fcn_lcb.py` & `PyBADS-1.0.2/pybads/acquisition_functions/acq_fcn_lcb.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/bads/bads.py` & `PyBADS-1.0.2/pybads/bads/bads.py`

 * *Files 1% similar despite different names*

```diff
@@ -1636,15 +1636,16 @@
             if self.options["search_optimize"]:
                 pass
 
             y_search, f_sd_search, idx = self.function_logger(u_search)
 
             if z.size > 0:
                 # Save statistics of gp prediction,
-                self._save_gp_stats_(y_search, f_mu[index_acq], fs[index_acq])
+                self._save_gp_stats_(y_search, f_mu[index_acq].item(),
+                                    fs[index_acq].item())
 
             # Add search point to training setMeshSize
             if (
                 u_search.size
                 > 0 & self.search_es_hedge.count
                 < self.options["search_n_try"]
             ):
@@ -2068,15 +2069,16 @@
             u_new = u_poll[index_acq]
             y_poll, y_sd_poll, f_idx_new = self.function_logger(u_new)
 
             # Remove polled vector from set.
             u_poll = np.delete(u_poll, index_acq, axis=0)
 
             # Save statistics of gp prediction
-            self._save_gp_stats_(y_poll, f_mu[index_acq], fs[index_acq])
+            self._save_gp_stats_(y_poll, f_mu[index_acq].item(),
+                                fs[index_acq].item())
 
             if self.optim_state["uncertainty_handling_level"] > 0:
                 # Update posterior with the new polled point
                 gp = add_and_update_gp(
                     self.function_logger,
                     gp,
                     u_new,
@@ -2299,20 +2301,22 @@
                 .astype("float")
             )
             yvals = (
                 self.gp_stats.get("ymu")[: gp_iter_idx + 1]
                 .flatten()
                 .astype("float")
             )
+            
             zscore = f_vals - yvals
             gp_ys = (
                 self.gp_stats.get("ys")[: gp_iter_idx + 1]
                 .flatten()
                 .astype("float")
             )
+            
             # Avoid division by zero, sometimes the GP variance is zero (e.g at end of the optimization of a deterministic)
             idx_zero_gp_ys = np.where(np.isclose(0., gp_ys))[0]
             gp_ys[idx_zero_gp_ys] = 1e-6
             
             zscore = zscore / gp_ys
 
             if np.any(np.isnan(zscore)):
```

### Comparing `PyBADS-1.0.1/pybads/bads/bads_dump.py` & `PyBADS-1.0.2/pybads/bads/bads_dump.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/bads/gaussian_process_train.py` & `PyBADS-1.0.2/pybads/bads/gaussian_process_train.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,17 @@
         if options["use_effective_radius"]:
             if isinstance(
                 gp.covariance,
                 gpr.gpyreg.covariance_functions.RationalQuadraticARD,
             ):
                 alpha = np.zeros((hyp_n_samples))
                 for i in range(hyp_n_samples):
-                    alpha[i] = np.exp(dic_hyp_gp[i]["covariance_log_shape"])
+                    # Casting to a scalar suppress deprecation warnings in pytest runs.
+                    # "Conversion of an array with ndim > 0 to a scalar is deprecated, and will error in future."
+                    alpha[i] = np.exp(dic_hyp_gp[i]["covariance_log_shape"])[0]
 
                 gp.temporary_data["effective_radius"] = np.sqrt(
                     alpha * (np.exp(1 / alpha) - 1)
                 )
     else:
         hyp_gp = old_hyp_gp
```

### Comparing `PyBADS-1.0.1/pybads/bads/optimize_result.py` & `PyBADS-1.0.2/pybads/bads/optimize_result.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/bads/option_configs/advanced_bads_options.ini` & `PyBADS-1.0.2/pybads/bads/option_configs/advanced_bads_options.ini`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/bads/option_configs/basic_bads_options.ini` & `PyBADS-1.0.2/pybads/bads/option_configs/basic_bads_options.ini`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/bads/options.py` & `PyBADS-1.0.2/pybads/bads/options.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/decorators/README.md` & `PyBADS-1.0.2/pybads/decorators/README.md`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/decorators/handle_0D_1D_input.py` & `PyBADS-1.0.2/pybads/decorators/handle_0D_1D_input.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/function_examples.py` & `PyBADS-1.0.2/pybads/function_examples.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/function_logger/constraints_check.py` & `PyBADS-1.0.2/pybads/function_logger/constraints_check.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/function_logger/function_logger.py` & `PyBADS-1.0.2/pybads/function_logger/function_logger.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/init_functions/init_sobol.py` & `PyBADS-1.0.2/pybads/init_functions/init_sobol.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/poll/poll_mads_2n.py` & `PyBADS-1.0.2/pybads/poll/poll_mads_2n.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/search/es_search.py` & `PyBADS-1.0.2/pybads/search/es_search.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/search/grid_functions.py` & `PyBADS-1.0.2/pybads/search/grid_functions.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/search/search_hedge.py` & `PyBADS-1.0.2/pybads/search/search_hedge.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/stats/get_hpd.py` & `PyBADS-1.0.2/pybads/stats/get_hpd.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/stats/kde1d.py` & `PyBADS-1.0.2/pybads/stats/kde1d.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/stats/kldiv_mvn.py` & `PyBADS-1.0.2/pybads/stats/kldiv_mvn.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/hyp.dat` & `PyBADS-1.0.2/pybads/testing/bads/hyp.dat`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/poll/test_poll_mads.py` & `PyBADS-1.0.2/pybads/testing/bads/poll/test_poll_mads.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/scripts/ackley_example.py` & `PyBADS-1.0.2/pybads/testing/bads/scripts/ackley_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py` & `PyBADS-1.0.2/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from pybads import BADS
 from pybads.bads import BADSDump
 from pybads.function_examples import quadratic_unknown_noisy_fcn, extra_noisy_quadratic_fcn, quadratic_hetsk_noisy_fcn, rosebrocks_hetsk_noisy_fcn
 
-D = 3
+D = 2
 x0 = np.ones((1, D)) * -3      # Starting point
 lb = np.ones((1, D)) * -7      # Lower bounds
 ub = np.ones((1, D)) * 7       # Upper bounds
 plb = np.ones((1, D)) * -3     # Plausible lower bounds
 pub = np.ones((1, D)) * 3     # Plausible upper bounds
 
 title = 'Noise objective function'
```

### Comparing `PyBADS-1.0.1/pybads/testing/bads/scripts/bads_rosenbrock_example.py` & `PyBADS-1.0.2/pybads/testing/bads/scripts/bads_rosenbrock_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/scripts/non_bound_example.py` & `PyBADS-1.0.2/pybads/testing/bads/scripts/non_bound_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/scripts/rastrigin_example.py` & `PyBADS-1.0.2/pybads/testing/bads/scripts/rastrigin_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/search/test_search.py` & `PyBADS-1.0.2/pybads/testing/bads/search/test_search.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/test_bads_optimization.py` & `PyBADS-1.0.2/pybads/testing/bads/test_bads_optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,19 @@
     return optimize_result, err
     
 def test_ellipsoid_opt():
     D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf()
     fun = lambda x: np.sum((np.atleast_2d(x) / np.arange(1, len(x) + 1) ** 2) ** 2)
     run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min=0.0, assert_flag=True)
 
+def test_1D_opt():
+    D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf(D=1)
+    fun = lambda x: np.sum((np.atleast_2d(x) / np.arange(1, len(x) + 1) ** 2) ** 2)
+    run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min=0.0, assert_flag=True)
+
 def test_high_dim_opt():
     D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf(D=60)
     fun = lambda x: np.sum((np.atleast_2d(x) / np.arange(1, len(x) + 1) ** 2) ** 2)
     run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min=0.0, assert_flag=False, max_fun_evals=200)
 
 def test_sphere_opt():
     D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf()
```

### Comparing `PyBADS-1.0.1/pybads/testing/bads/test_gaussian_process_train.py` & `PyBADS-1.0.2/pybads/testing/bads/test_gaussian_process_train.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/bads/test_iteration_history.py` & `PyBADS-1.0.2/pybads/testing/bads/test_iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py` & `PyBADS-1.0.2/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/function_logger/test_function_logger.py` & `PyBADS-1.0.2/pybads/testing/function_logger/test_function_logger.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/testing/variable_transformer/test_variable_transformer.py` & `PyBADS-1.0.2/pybads/testing/variable_transformer/test_variable_transformer.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/utils/iteration_history.py` & `PyBADS-1.0.2/pybads/utils/iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/utils/timer/timer.py` & `PyBADS-1.0.2/pybads/utils/timer/timer.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.1/pybads/variable_transformer/variables_transformer.py` & `PyBADS-1.0.2/pybads/variable_transformer/variables_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,16 @@
             and np.all(self.plb < self.pub)\
             and np.all(self.pub <= self.ub)):
                 raise ValueError("Interval bounds needs to respect the order lower_bound <= plausible_lower_bounds < plausible_upper_bounds <= upper_bound for all coordinates.")
          
 
         # A variable is converted to log scale if all bounds are positive and
         # the plausible range spans at least one order of magnitude
-        for i in np.argwhere(np.isnan(self.apply_log_t.squeeze())):
+        check_idx_log_t = np.argwhere(np.isnan(self.apply_log_t.flatten()))
+        for i in check_idx_log_t:
             self.apply_log_t[:, i] = (
                 np.all(
                     np.concatenate(
                         [
                             self.lb[:, i],
                             self.ub[:, i],
                             self.plb[:, i],
@@ -208,16 +209,16 @@
             np.logical_and((~np.isfinite(self.orig_ub)), self.apply_log_t)
         ] = 1e6
 
         numeps = 1e-6  # accepted numerical error
         tests = np.zeros(4)
         tests[0] = np.all(np.abs(ginv(g(lbtest)) - lbtest) < numeps)
         tests[1] = np.all(np.abs(ginv(g(ubtest)) - ubtest) < numeps)
-        tests[2] = np.all(np.abs(ginv(g(self.plb)) - self.plb) < numeps)
-        tests[3] = np.all(np.abs(ginv(g(self.pub)) - self.pub) < numeps)
+        tests[2] = np.all(np.abs(ginv(g(self.orig_plb)) - self.orig_plb) < numeps)
+        tests[3] = np.all(np.abs(ginv(g(self.orig_pub)) - self.orig_pub) < numeps)
         if not np.all(tests):
             raise ValueError("Cannot invert the transform to obtain the identity at the provided boundaries.")
 
         return (
             g(self.orig_lb),
             g(self.orig_ub),
             g(self.orig_plb),
```

### Comparing `PyBADS-1.0.1/pyproject.toml` & `PyBADS-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 name = "PyBADS"
 dynamic = ["version"]  # use git tags for version, via setuptools_scm
 description = "Bayesian Adaptive Direct Search in Python."
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
     "cma >= 3.1.0",
-    "corner >= 2.2.1",
-    "dill >= 0.3.5.1",
     "gpyreg >= 0.1.0",
-    "imageio >= 2.13.5",
     "matplotlib >= 3.5.1",
     "numpy >= 1.22.1",
-    "plotly >= 5.11.0",
     "pytest >= 6.2.5",
     "pytest-mock >= 3.6.1",
     "pytest-rerunfailures >= 10.2",
     "scipy >= 1.7.3",
 ]
 requires-python = ">=3.9"
 
@@ -30,14 +26,17 @@
 
 [tool.setuptools.package-data]
 # Make sure to include example Notebooks:
 "pybads.examples" = ["*.ipynb"]
 
 [project.optional-dependencies]
 dev = [
+    "imageio >= 2.13.5",
+    "corner >= 2.2.1",
+    "dill >= 0.3.5.1",
     "myst_nb >= 0.13.1",
     "numpydoc >= 1.2.1",
     "pylint >= 2.15.5",
     "pytest-cov >= 4.0.0",
     "sphinx >= 4.3.2",
     "sphinx-book-theme>=0.2.0",
     "build >= 0.9.0",
```

