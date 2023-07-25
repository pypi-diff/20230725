# Comparing `tmp/holobench-0.0.6.tar.gz` & `tmp/holobench-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holobench-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "holobench-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `holobench-0.0.6.tar` & `holobench-0.0.8.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0      338 2023-07-22 13:39:33.630996 holobench-0.0.6/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1482 2023-07-24 17:38:19.734638 holobench-0.0.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.6/.github/dependabot.yml
--rw-r--r--   0        0        0     1264 2023-07-16 12:36:45.474978 holobench-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.6/.gitignore
--rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.6/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.6/.pylintrc
--rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0      895 2023-07-24 17:38:19.734638 holobench-0.0.6/.vscode/tasks.json
--rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.6/LICENSE
--rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.6/README.md
--rw-r--r--   0        0        0      789 2023-07-22 12:02:54.862576 holobench-0.0.6/bencher/__init__.py
--rw-r--r--   0        0        0    26273 2023-07-24 17:38:19.734638 holobench-0.0.6/bencher/bench_cfg.py
--rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.6/bencher/bench_plot_server.py
--rw-r--r--   0        0        0    24828 2023-07-22 09:13:13.899071 holobench-0.0.6/bencher/bench_vars.py
--rw-r--r--   0        0        0    27768 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/bencher.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.6/bencher/example/__init__.py
--rw-r--r--   0        0        0     4168 2023-07-22 13:39:33.630996 holobench-0.0.6/bencher/example/benchmark_data.py
--rw-r--r--   0        0        0      923 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/example/example_bokeh_plotly.py
--rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_categorical.py
--rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_custom_sweep.py
--rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float2D_scatter.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float3D.py
--rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float3D_cone.py
--rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float_cat.py
--rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_floats.py
--rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_floats2D.py
--rw-r--r--   0        0        0     5136 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/example/example_holosweep.py
--rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/example_hvplot_explorer.py
--rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/example_interactive.py
--rw-r--r--   0        0        0     2416 2023-07-22 12:02:54.862576 holobench-0.0.6/bencher/example/example_kwargs.py
--rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_pareto.py
--rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_persistent.py
--rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/example/example_plot_library.py
--rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_sample_cache.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_sample_cache_context.py
--rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_simple.py
--rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/example_simple_bool.py
--rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_simple_cat.py
--rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_simple_float.py
--rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/example/example_template.py
--rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_time_event.py
--rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.6/bencher/example/example_vector.py
--rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_workflow.py
--rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/hv_bool_bug.py
--rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/optuna_conversions.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/__init__.py
--rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/plotting/plot_collection.py
--rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plot_filter.py
--rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plot_library.py
--rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plot_types.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/catplot.py
--rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/plotting/plots/heatmap.py
--rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/hv_interactive.py
--rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/lineplot.py
--rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.6/bencher/plotting/plots/plot_base.py
--rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/scatterplot.py
--rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/surface.py
--rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/tables.py
--rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/volume.py
--rw-r--r--   0        0        0    11572 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/plotting_functions.py
--rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plt_cfg.py
--rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/utils.py
--rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.6/dependencies.yaml
--rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.6/package.xml
--rw-r--r--   0        0        0     1473 2023-07-24 17:39:14.150854 holobench-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.6/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/resource/bencher
--rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.6/setup.cfg
--rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.6/setup.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/test/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/__init__.py
--rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/test_catplot.py
--rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/test_plots_common.py
--rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/test_tables.py
--rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.6/test/test_bench_examples.py
--rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_bencher.py
--rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_combinations.py
--rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_plot_collection.py
--rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_plot_filter.py
--rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_plot_library.py
--rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_sample_cache.py
--rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_sweep_vars.py
--rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_utils.py
--rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_vars.py
--rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 holobench-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      338 2023-07-22 13:39:33.630996 holobench-0.0.8/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1497 2023-07-25 17:13:34.222057 holobench-0.0.8/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     1266 2023-07-25 17:13:34.222057 holobench-0.0.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      658 2023-07-25 17:13:34.222057 holobench-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.8/.gitignore
+-rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.8/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.8/.pylintrc
+-rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0      895 2023-07-25 17:13:34.222057 holobench-0.0.8/.vscode/tasks.json
+-rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.8/README.md
+-rw-r--r--   0        0        0      789 2023-07-22 12:02:54.862576 holobench-0.0.8/bencher/__init__.py
+-rw-r--r--   0        0        0    26370 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/bench_cfg.py
+-rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.8/bencher/bench_plot_server.py
+-rw-r--r--   0        0        0    26094 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/bench_vars.py
+-rw-r--r--   0        0        0    27790 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/bencher.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.8/bencher/example/__init__.py
+-rw-r--r--   0        0        0     4168 2023-07-22 13:39:33.630996 holobench-0.0.8/bencher/example/benchmark_data.py
+-rw-r--r--   0        0        0      846 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/example/example_bokeh_plotly.py
+-rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_categorical.py
+-rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_custom_sweep.py
+-rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float2D_scatter.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float3D.py
+-rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float3D_cone.py
+-rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float_cat.py
+-rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_floats.py
+-rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_floats2D.py
+-rw-r--r--   0        0        0     5225 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/example/example_holosweep.py
+-rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/example_hvplot_explorer.py
+-rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/example_interactive.py
+-rw-r--r--   0        0        0     2416 2023-07-22 12:02:54.862576 holobench-0.0.8/bencher/example/example_kwargs.py
+-rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_pareto.py
+-rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_persistent.py
+-rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/example/example_plot_library.py
+-rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_sample_cache.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_sample_cache_context.py
+-rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_simple.py
+-rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/example_simple_bool.py
+-rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_simple_cat.py
+-rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_simple_float.py
+-rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/example/example_template.py
+-rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_time_event.py
+-rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.8/bencher/example/example_vector.py
+-rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_workflow.py
+-rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/hv_bool_bug.py
+-rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/optuna_conversions.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/__init__.py
+-rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/plotting/plot_collection.py
+-rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plot_filter.py
+-rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plot_library.py
+-rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plot_types.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/catplot.py
+-rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/plotting/plots/heatmap.py
+-rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/hv_interactive.py
+-rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/lineplot.py
+-rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.8/bencher/plotting/plots/plot_base.py
+-rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/scatterplot.py
+-rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/surface.py
+-rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/tables.py
+-rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/volume.py
+-rw-r--r--   0        0        0    11034 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/plotting_functions.py
+-rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plt_cfg.py
+-rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/utils.py
+-rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.8/dependencies.yaml
+-rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.8/package.xml
+-rw-r--r--   0        0        0     1452 2023-07-25 17:13:34.222057 holobench-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.8/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/resource/bencher
+-rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.8/setup.cfg
+-rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.8/setup.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/test_catplot.py
+-rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/test_plots_common.py
+-rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/test_tables.py
+-rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.8/test/test_bench_examples.py
+-rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_bencher.py
+-rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_combinations.py
+-rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_plot_collection.py
+-rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_plot_filter.py
+-rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_plot_library.py
+-rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_sample_cache.py
+-rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_sweep_vars.py
+-rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_utils.py
+-rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_vars.py
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 holobench-0.0.8/PKG-INFO
```

### Comparing `holobench-0.0.6/.devcontainer/devcontainer.json` & `holobench-0.0.8/.devcontainer/devcontainer.json`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 // }
 {
 	"name": "Python Environment",
 	"build": {
 		"dockerfile": "Dockerfile",
 		"context": ".."
 	},
-	"postCreateCommand": "flit install",
+	"postCreateCommand": "flit install --symlink",
 	"customizations": {
 		"vscode": {
 			"extensions": [
 				"ms-python.python",
 				"ms-python.vscode-pylance",
 				"ms-python.pylint",
 				"njpwerner.autodocstring",
 				"charliermarsh.ruff",
 				"mhutchie.git-graph",
-				"bungcip.better-toml",
-				"eamodio.gitlens"
+				"eamodio.gitlens",
+				"tamasfe.even-better-toml"
 			]
 		}
 	},
 	// "onCreateCommand": "pre-commit install-hooks"
 }
```

### Comparing `holobench-0.0.6/.github/workflows/ci.yml` & `holobench-0.0.8/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 name: CI
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
-    branches: [ "main" ]
+    branches: [ "main" ]  
 
 permissions:
   contents: read
 
 jobs:
 
   black:
```

### Comparing `holobench-0.0.6/.gitignore` & `holobench-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/.vscode/tasks.json` & `holobench-0.0.8/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/LICENSE` & `holobench-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/README.md` & `holobench-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/__init__.py` & `holobench-0.0.8/bencher/__init__.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/bench_cfg.py` & `holobench-0.0.8/bencher/bench_cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,14 +543,17 @@
     def to_bar(self, reduce=None) -> hv.Bars:
         ds = self.get_hv_dataset(reduce)
         pt = ds.to(hv.Bars)
         if reduce:
             pt *= ds.to(hv.ErrorBars)
         return pt
 
+    def to_heatmap(self, reduce=None) -> hv.HeatMap:
+        return self.to(hv.HeatMap, reduce)
+
     def to_nd_layout(self) -> hv.NdLayout:
         return hv.NdLayout(self.hmap, kdims=self.hmap_kdims).opts(
             shared_axes=False, shared_datasource=False
         )
 
     def to_holomap(self) -> hv.HoloMap:
         # return hv.HoloMap(self.hmap, self.hmap_kdims)
```

### Comparing `holobench-0.0.6/bencher/bench_plot_server.py` & `holobench-0.0.8/bencher/bench_plot_server.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/bench_vars.py` & `holobench-0.0.8/bencher/bench_vars.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,16 +164,51 @@
         """Return a list of input parameters
 
         Returns:
             List[param.Parameter]: A list of input parameters
         """
         return list(self.get_input_and_results().inputs.values())
 
-    def get_inputs_as_dims(self, compute_values=False):
-        return [iv.as_dim(compute_values) for iv in self.get_inputs_only()]
+    def get_inputs_as_dims(
+        self, compute_values=False, remove_dims: str | List[str] = None
+    ) -> List[hv.Dimension]:
+        inputs = self.get_inputs_only()
+
+        if remove_dims is not None:
+            if type(remove_dims) == str:
+                remove_dims = [remove_dims]
+            filtered_inputs = [i for i in inputs if i.name not in remove_dims]
+            inputs = filtered_inputs
+
+        return [iv.as_dim(compute_values) for iv in inputs]
+
+    def to_dynamic_map(
+        self,
+        callback,
+        remove_dims: str | List[str] = None,
+    ) -> hv.DynamicMap:
+        def callback_wrapper(**kwargs):
+            return callback(**kwargs)["hmap"]
+
+        return hv.DynamicMap(
+            callback=callback_wrapper,
+            kdims=self.get_inputs_as_dims(compute_values=False, remove_dims=remove_dims),
+        ).opts(shared_axes=False)
+
+    def to_holomap(self, callback, remove_dims: str | List[str] = None) -> hv.DynamicMap:
+        return hv.HoloMap(
+            hv.DynamicMap(
+                callback=callback,
+                kdims=self.get_inputs_as_dims(compute_values=True, remove_dims=remove_dims),
+            )
+        )
+        # return hv.HoloMap(self.to_dynamic_map(callback=callback, remove_dims=remove_dims))
+        # return hv.DynamicMap(
+        #     kdims=self.get_inputs_as_dims(compute_values=True, remove_dims=remove_dims)
+        # )
 
 
 # slots that are shared across all Sweep classes
 # param does not work with multiple inheritance so define here
 shared_slots = ["units", "samples", "samples_debug"]
```

### Comparing `holobench-0.0.6/bencher/bencher.py` & `holobench-0.0.8/bencher/bencher.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             plot_lib: (PlotCollection):  A dictionary of plot names:method pairs that are selected for plotting based on the type of data they can plot.
         """
         self.bench_name = bench_name
         self.worker = None
         self.worker_input_cfg = None
         self.set_worker(worker, worker_input_cfg)
 
-        self.plots_instance = pn.Tabs(tabs_location="left", name=self.bench_name)
+        self.pane = pn.Tabs(tabs_location="left", name=self.bench_name)
         # The number of times the wrapped worker was called
         self.worker_wrapper_call_count = 0
         self.worker_fn_call_count = 0  # The number of times the raw worker was called
         # The number of times the cache was used instead of the raw worker
         self.worker_cache_call_count = 0
         self.bench_cfg_hashes = []  # a list of hashes that point to benchmark results
         self.last_run_cfg = None  # cached run_cfg used to pass to the plotting function
@@ -260,15 +260,15 @@
                 bench_cfg.ds = self.load_history_cache(
                     bench_cfg.ds, bench_cfg_hash, run_cfg.clear_history
                 )
 
             self.report_results(bench_cfg, run_cfg.print_xarray, run_cfg.print_pandas)
             self.cache_results(bench_cfg, bench_cfg_hash)
 
-        self.plots_instance = BenchPlotter.plot(bench_cfg, self.plots_instance)
+        self.pane = BenchPlotter.plot(bench_cfg, self.pane)
         return bench_cfg
 
     def check_var_is_a_param(self, variable: param.Parameter, var_type: str):
         """check that a variable is a subclass of param
 
         Args:
             variable (param.Parameter): the varible to check
@@ -328,15 +328,15 @@
 
         Args:
             run_cfg (BenchRunCfg, optional): Options for the webserve such as the port. Defaults to None.
 
         """
         if run_cfg is None:
             run_cfg = self.last_run_cfg
-        BenchPlotServer().plot_server(self.bench_name, run_cfg, self.plots_instance)
+        BenchPlotServer().plot_server(self.bench_name, run_cfg, self.pane)
 
     def load_history_cache(
         self, ds: xr.Dataset, bench_cfg_hash: int, clear_history: bool
     ) -> xr.Dataset:
         """Load historical data from a cache if over_time=true
 
         Args:
@@ -649,20 +649,23 @@
         Args:
             main_plot (bool, optional): return the last added page. Defaults to True.
 
         Returns:
             pn.pane: results panel
         """
         if main_plot:
-            return self.plots_instance[-1][0]
-        return self.plots_instance[-1]
+            return self.pane[-1][0]
+        return self.pane[-1]
 
-    def append(self, pane: pn.panel):
+    def append(self, pane: pn.panel) -> None:
         self.get_panel().append(pane)
 
+    def append_tab(self, pane: pn.panel):
+        self.pane.append(pane)
+
     def get_best_params(self, bench_cfg: BenchCfg) -> dict:
         """Get a dictionary of the best found parameters found during the sweep
 
         Args:
             bench_cfg (BenchCfg): Results
 
         Returns:
```

### Comparing `holobench-0.0.6/bencher/example/benchmark_data.py` & `holobench-0.0.8/bencher/example/benchmark_data.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_bokeh_plotly.py` & `holobench-0.0.8/bencher/example/example_bokeh_plotly.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import holoviews as hv
 import numpy as np
 import panel as pn
-from holoviews import opts
-import matplotlib.pyplot as plt
-import matplotlib
 
 # hv.extension("bokeh", "plotly")
 backend1 = "plotly"
 # backend1 = "matplotlib"
 backend2 = "bokeh"
 
 # matplotlib.use("agg")
```

### Comparing `holobench-0.0.6/bencher/example/example_categorical.py` & `holobench-0.0.8/bencher/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_custom_sweep.py` & `holobench-0.0.8/bencher/example/example_custom_sweep.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_float2D_scatter.py` & `holobench-0.0.8/bencher/example/example_float2D_scatter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_float3D.py` & `holobench-0.0.8/bencher/example/example_float3D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_float3D_cone.py` & `holobench-0.0.8/bencher/example/example_float3D_cone.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_float_cat.py` & `holobench-0.0.8/bencher/example/example_float_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_floats.py` & `holobench-0.0.8/bencher/example/example_floats.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_floats2D.py` & `holobench-0.0.8/bencher/example/example_floats2D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_holosweep.py` & `holobench-0.0.8/bencher/example/example_holosweep.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # pylint: disable=duplicate-code,unused-argument
 
 
 import bencher as bch
 import math
 import random
 import numpy as np
-from holoviews import opts
 import panel as pn
 import holoviews as hv
 
 
 from strenum import StrEnum
 from enum import auto
 
@@ -32,33 +31,38 @@
         default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=10
     )
 
     compute_fn = bch.EnumSweep(Function)
 
     noisy = bch.BoolSweep(default=True)
 
-    out_sin = bch.ResultVar(units="v", doc="sin of theta with some noise")
+    fn_output = bch.ResultVar(units="v", doc="sin of theta with some noise")
     # out_cos = bch.ResultVar(units="v", doc="cos of theta with some noise")
 
     out_sum = bch.ResultVar(units="v", doc="The sum")
 
-    def calc(self, phase=0.0, freq=1.0, theta=0.0, noisy=True) -> dict:
+    def calc(
+        self, phase=0.0, freq=1.0, theta=0.0, noisy=True, compute_fn: Function = Function.fn_sin
+    ) -> dict:
         if noisy:
             noise = 1.0
         else:
             noise = 0.0
 
-        self.out_sin = np.sin(phase + freq * theta) + random.uniform(0, noise)
-        self.out_cos = np.cos(phase + freq * theta) + random.uniform(0, noise)
+        match compute_fn:
+            case Function.fn_sin:
+                self.fn_output = np.sin(phase + freq * theta)
+            case Function.fn_cos:
+                self.fn_output = np.cos(phase + freq * theta)
 
-        # self.image = hv.Text
+        self.fn_output += random.uniform(0, noise)
 
         pt = hv.Text(0, 0, f"{phase}\n{freq}\n {theta}")
         pt *= hv.Ellipse(0, 0, 1)
-        pt = hv.Points([theta, self.out_sin])
+        pt = hv.Points([theta, self.fn_output])
 
         return self.get_results_values_as_dict(holomap=pt)
 
     def calc_vec(
         self, phase=0.0, freq=1.0, noisy=True, compute_fn: Function = Function.fn_sin
     ) -> dict:
         if noisy:
@@ -71,75 +75,74 @@
         match compute_fn:
             case Function.fn_sin:
                 dat = np.sin(phase + freq * theta) + random.uniform(0, noise)
             case Function.fn_cos:
                 dat = np.cos(phase + freq * theta) + random.uniform(0, noise)
 
         self.out_sum = sum(dat)
-        hmap = hv.Curve((theta, dat), "theta", "voltage")
+        hv.Curve((theta, dat), "theta", "voltage")
 
         pt = hv.Text(0, 0, f"{compute_fn}\n{phase}\n{freq}")
         pt *= hv.Ellipse(0, 0, 1)
 
-        # pt = hv.Image(np.ones([100, 100]) * freq * phase * 100)
-        # pt = hv.Points([theta, self.out_sin])
-
         return self.get_results_values_as_dict(holomap=pt)
 
 
 if __name__ == "__main__":
     # opts.defaults(
     #     # opts.NdLayout(shared_axes=False, shared_datasource=False, width=500),
     #     opts.Overlay(width=500, legend_position="right"),
     # )
     wv = Waves()
 
-    # hv.extension("plotly", "bokeh")
-
     bch_wv = bch.Bench("waves", wv.calc, plot_lib=None)
 
-    # res = bch_wv.plot_sweep(
-    #     "phase",
-    #     # input_vars=[wv.param.theta, wv.param.freq, wv.param.phase, wv.param.noisy],
-    #     input_vars=[wv.param.theta, wv.param.freq, wv.param.phase],
-    #     result_vars=[wv.param.out_sin],
-    #     run_cfg=bch.BenchRunCfg(repeats=3),
-    # )
-
-    # bch_wv.append(res.to_curve().layout("freq"))
+    res = bch_wv.plot_sweep(
+        "phase",
+        input_vars=[wv.param.theta, wv.param.freq, wv.param.phase],
+        result_vars=[wv.param.fn_output],
+        run_cfg=bch.BenchRunCfg(repeats=3),
+    )
+    bch_wv.append_tab(wv.to_dynamic_map(wv.calc))
 
     bch_wv.worker = wv.calc_vec
     res = bch_wv.plot_sweep(
         "holo",
         input_vars=[wv.param.freq, wv.param.phase, wv.param.compute_fn],
         result_vars=[wv.param.out_sum],
         run_cfg=bch.BenchRunCfg(repeats=3, auto_plot=False),
     )
 
-    # hv.extension("bokeh")
+    # bch_wv.append(res.to_heatmap())
+    # bch_wv.append(res.to_holomap())
+    # bch_wv.append_tab(res.to_nd_layout())  # doesn't work on the same page yet.. TODO
+
+    bch_wv.append(res.to_grid())
+
+    bch_wv.append_tab(wv.to_dynamic_map(wv.calc_vec, "theta"))
 
-    # bch_wv.append(res.to_holomap().opts(backend="bokeh"))
+    # bch_wv.append_tab(wv.to_holomap(wv.calc_vec, "theta"))
 
     # bch_wv.append(hv.HoloMap(res.hmap, res.hmap_kdims).opts(backend="bokeh"))
     # bch_wv.plots_instance.append(res.to_grid().opts(backend="bokeh"))
     # bch_wv.append(res.to_holomap().layout().)
 
     # bch_wv.append(res.to_holomap())
-    bch_wv.append(res.to_grid())
+    # bch_wv.append(res.to_grid())
 
     # bch_wv.append(ndlay.grid("freq"))
     bch_wv.plot()
 
     # bch_wv.append(res.to_curve().layout())
 
     # res = bch_wv.plot_sweep(
     #     "phase",
     #     input_vars=[wv.param.theta, wv.param.freq, wv.param.phase, wv.param.noisy],
     #     # input_vars=[wv.param.theta, wv.param.freq, wv.param.phase],
-    #     result_vars=[wv.param.out_sin],
+    #     result_vars=[wv.param.fn_output],
     #     run_cfg=bch.BenchRunCfg(repeats=5),
     # )
 
     # bch_wv.plots_instance.append(res.to_curve())
     # bch_wv.plots_instance.append(res.to_curve().overlay("phase"))
     # bch_wv.plots_instance.append(res.to_curve().overlay("freq"))
     # bch_wv.plots_instance.append(res.to_curve().overlay("phase").layout())
```

### Comparing `holobench-0.0.6/bencher/example/example_hvplot_explorer.py` & `holobench-0.0.8/bencher/example/example_hvplot_explorer.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_interactive.py` & `holobench-0.0.8/bencher/example/example_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_kwargs.py` & `holobench-0.0.8/bencher/example/example_kwargs.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_pareto.py` & `holobench-0.0.8/bencher/example/example_pareto.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_persistent.py` & `holobench-0.0.8/bencher/example/example_persistent.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_plot_library.py` & `holobench-0.0.8/bencher/example/example_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_sample_cache.py` & `holobench-0.0.8/bencher/example/example_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_sample_cache_context.py` & `holobench-0.0.8/bencher/example/example_sample_cache_context.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_simple.py` & `holobench-0.0.8/bencher/example/example_simple.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_simple_bool.py` & `holobench-0.0.8/bencher/example/example_simple_bool.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_simple_cat.py` & `holobench-0.0.8/bencher/example/example_simple_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_simple_float.py` & `holobench-0.0.8/bencher/example/example_simple_float.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_template.py` & `holobench-0.0.8/bencher/example/example_template.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_time_event.py` & `holobench-0.0.8/bencher/example/example_time_event.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_vector.py` & `holobench-0.0.8/bencher/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/example_workflow.py` & `holobench-0.0.8/bencher/example/example_workflow.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/example/hv_bool_bug.py` & `holobench-0.0.8/bencher/example/hv_bool_bug.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/optuna_conversions.py` & `holobench-0.0.8/bencher/optuna_conversions.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plot_collection.py` & `holobench-0.0.8/bencher/plotting/plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plot_filter.py` & `holobench-0.0.8/bencher/plotting/plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plot_library.py` & `holobench-0.0.8/bencher/plotting/plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plot_types.py` & `holobench-0.0.8/bencher/plotting/plot_types.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/catplot.py` & `holobench-0.0.8/bencher/plotting/plots/catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/heatmap.py` & `holobench-0.0.8/bencher/plotting/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/hv_interactive.py` & `holobench-0.0.8/bencher/plotting/plots/hv_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/lineplot.py` & `holobench-0.0.8/bencher/plotting/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/plot_base.py` & `holobench-0.0.8/bencher/plotting/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/scatterplot.py` & `holobench-0.0.8/bencher/plotting/plots/scatterplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/surface.py` & `holobench-0.0.8/bencher/plotting/plots/surface.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/tables.py` & `holobench-0.0.8/bencher/plotting/plots/tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting/plots/volume.py` & `holobench-0.0.8/bencher/plotting/plots/volume.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/plotting_functions.py` & `holobench-0.0.8/bencher/plotting_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from holoviews import opts
 
 from bencher.bench_cfg import BenchCfg, PltCfgBase
 from bencher.bench_vars import ParametrizedSweep, ResultList, ResultVar, ResultVec
 import plotly.graph_objs as go
 
 
-# hv.extension("plotly")
-
-
 hv.extension("bokeh", "plotly")
+# hv.extension("plotly", "bokeh")
+
+# hv.extension("plotly")
 
 
 def wrap_long_time_labels(bench_cfg: BenchCfg) -> BenchCfg:
     """Takes a benchCfg and wraps any index labels that are too long to be plotted easily
 
     Args:
         bench_cfg (BenchCfg):
@@ -317,55 +317,39 @@
 
     bench_cfg = wrap_long_time_labels(bench_cfg)
 
     alpha = 0.3
 
     da = bench_cfg.ds[rv.name]
 
+    # hv.extension("plotly")
+    # hv.extension("bokeh", "plotly")
+
     mean = da.mean("repeat")
 
-    # opts.defaults(
-    #     opts.Surface(
-    #         backend=bke
-    #         # colorbar=True,
-    #         # width=800,
-    #         # height=800,
-    #         # zlabel=xr_cfg.zlabel,
-    #         # title=xr_cfg.title,
-    #         # image_rtol=0.002,
-    #     )
-    # )
     # TODO a warning suggests setting this parameter, but it does not seem to help as expected, leaving here to fix in the future
     # hv.config.image_rtol = 1.0
 
     ds = hv.Dataset(mean)
-    # return hv.output(ds.to(hv.Surface).opts(backend=bke), backend=bke)
     surface = ds.to(hv.Surface)
 
-    # if bench_cfg.repeats > 1:
-    #     std_dev = da.std("repeat")
-    #     upper = hv.Dataset(mean + std_dev).to(hv.Surface).opts(alpha=alpha, colorbar=False)
-    #     lower = hv.Dataset(mean - std_dev).to(hv.Surface).opts(alpha=alpha, colorbar=False)
-    #     return surface * upper * lower
-    # return surface
-
     if bench_cfg.repeats > 1:
         std_dev = da.std("repeat")
         surface *= (
             hv.Dataset(mean + std_dev)
             .to(hv.Surface)
             .opts(alpha=alpha, colorbar=False, backend="plotly")
         )
         surface *= (
             hv.Dataset(mean - std_dev)
             .to(hv.Surface)
             .opts(alpha=alpha, colorbar=False, backend="plotly")
         )
     return pn.Column(
-        # surface
+        # using render disabled the holoviews sliders :(
         hv.render(
             surface.opts(
                 width=800, height=800, zlabel=xr_cfg.zlabel, title=xr_cfg.title, backend="plotly"
             ),
             backend="plotly",
         )
     )
```

### Comparing `holobench-0.0.6/bencher/plt_cfg.py` & `holobench-0.0.8/bencher/plt_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/bencher/utils.py` & `holobench-0.0.8/bencher/utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/package.xml` & `holobench-0.0.8/package.xml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/pyproject.toml` & `holobench-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [project]
-name =  "holobench"
-version = "0.0.6"
+name = "holobench"
+version = "0.0.8"
 
-authors = [
-    {name = "Austin Gregg-Smith", email = "blooop@gmail.com"},
-]
+authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
 description = "A package for benchmarking the performance of arbitrary functions"
 readme = "README.md"
 
 requires-python = ">=3.10"
 
 dependencies = [
   "holoviews[reccomended]",
@@ -18,29 +16,29 @@
   "xarray",
   "plotly",
   "sortedcontainers",
   "pandas",
   "strenum",
   "seaborn",
   "scikit-learn",
-  "str2bool"
+  "str2bool",
 ]
 
 [project.optional-dependencies]
 test = [
-    "black==23.3.0",
-    "check-manifest",
-    "pre-commit",
-    "pylint",
-    "pytest-cov",
-    "pytest-mock<3.10.2",
-    "pytest-runner",
-    "pytest",
-    "hypothesis",
-    "ruff"
+  "black==23.3.0",
+  "check-manifest",
+  "pre-commit",
+  "pylint",
+  "pytest-cov",
+  "pytest-mock<3.10.2",
+  "pytest-runner",
+  "pytest",
+  "hypothesis",
+  "ruff",
 ]
 
 [project.urls]
 Source = "https://github.com/blooop/bencher"
 Home = "https://github.com/blooop/bencher"
 
 
@@ -58,22 +56,22 @@
 
 [tool.black]
 line-length = 100
 
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
-ignore = ["E501","E902"]
+ignore = ["E501", "E902"]
 
 
 # Same as Black.
 line-length = 100
 
 target-version = "py310"
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 # Ignore `E402` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
 [tool.ruff.per-file-ignores]
-"__init__.py" = ["E402","F401"]
-"path/to/file.py" = ["E402"]
+"__init__.py" = ["E402", "F401"]
+"path/to/file.py" = ["E402"]
```

### Comparing `holobench-0.0.6/setup.py` & `holobench-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/plots/test_catplot.py` & `holobench-0.0.8/test/plots/test_catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/plots/test_plots_common.py` & `holobench-0.0.8/test/plots/test_plots_common.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/plots/test_tables.py` & `holobench-0.0.8/test/plots/test_tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_bench_examples.py` & `holobench-0.0.8/test/test_bench_examples.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_bencher.py` & `holobench-0.0.8/test/test_bencher.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_combinations.py` & `holobench-0.0.8/test/test_combinations.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_plot_collection.py` & `holobench-0.0.8/test/test_plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_plot_filter.py` & `holobench-0.0.8/test/test_plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_plot_library.py` & `holobench-0.0.8/test/test_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_sample_cache.py` & `holobench-0.0.8/test/test_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_sweep_vars.py` & `holobench-0.0.8/test/test_sweep_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_utils.py` & `holobench-0.0.8/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/test/test_vars.py` & `holobench-0.0.8/test/test_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.6/PKG-INFO` & `holobench-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holobench
-Version: 0.0.6
+Version: 0.0.8
 Summary: A package for benchmarking the performance of arbitrary functions
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: holoviews[reccomended]
 Requires-Dist: hvplot==0.8.4
 Requires-Dist: diskcache
```

