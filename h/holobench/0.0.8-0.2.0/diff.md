# Comparing `tmp/holobench-0.0.8.tar.gz` & `tmp/holobench-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holobench-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "holobench-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `holobench-0.0.8.tar` & `holobench-0.2.0.tar`

### file list

```diff
@@ -1,89 +1,105 @@
--rw-r--r--   0        0        0      338 2023-07-22 13:39:33.630996 holobench-0.0.8/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1497 2023-07-25 17:13:34.222057 holobench-0.0.8/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0     1266 2023-07-25 17:13:34.222057 holobench-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      658 2023-07-25 17:13:34.222057 holobench-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.8/.gitignore
--rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.8/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.8/.pylintrc
--rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0      895 2023-07-25 17:13:34.222057 holobench-0.0.8/.vscode/tasks.json
--rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.8/LICENSE
--rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.8/README.md
--rw-r--r--   0        0        0      789 2023-07-22 12:02:54.862576 holobench-0.0.8/bencher/__init__.py
--rw-r--r--   0        0        0    26370 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/bench_cfg.py
--rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.8/bencher/bench_plot_server.py
--rw-r--r--   0        0        0    26094 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/bench_vars.py
--rw-r--r--   0        0        0    27790 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/bencher.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.8/bencher/example/__init__.py
--rw-r--r--   0        0        0     4168 2023-07-22 13:39:33.630996 holobench-0.0.8/bencher/example/benchmark_data.py
--rw-r--r--   0        0        0      846 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/example/example_bokeh_plotly.py
--rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_categorical.py
--rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_custom_sweep.py
--rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float2D_scatter.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float3D.py
--rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float3D_cone.py
--rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_float_cat.py
--rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_floats.py
--rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_floats2D.py
--rw-r--r--   0        0        0     5225 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/example/example_holosweep.py
--rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/example_hvplot_explorer.py
--rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/example_interactive.py
--rw-r--r--   0        0        0     2416 2023-07-22 12:02:54.862576 holobench-0.0.8/bencher/example/example_kwargs.py
--rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_pareto.py
--rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_persistent.py
--rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/example/example_plot_library.py
--rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_sample_cache.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_sample_cache_context.py
--rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_simple.py
--rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/example_simple_bool.py
--rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_simple_cat.py
--rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_simple_float.py
--rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/example/example_template.py
--rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_time_event.py
--rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.8/bencher/example/example_vector.py
--rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/example/example_workflow.py
--rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/example/hv_bool_bug.py
--rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/optuna_conversions.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/__init__.py
--rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/plotting/plot_collection.py
--rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plot_filter.py
--rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plot_library.py
--rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plot_types.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/catplot.py
--rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.8/bencher/plotting/plots/heatmap.py
--rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/hv_interactive.py
--rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/lineplot.py
--rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.8/bencher/plotting/plots/plot_base.py
--rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/scatterplot.py
--rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/surface.py
--rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/plotting/plots/tables.py
--rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plotting/plots/volume.py
--rw-r--r--   0        0        0    11034 2023-07-25 17:13:34.222057 holobench-0.0.8/bencher/plotting_functions.py
--rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.8/bencher/plt_cfg.py
--rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.8/bencher/utils.py
--rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.8/dependencies.yaml
--rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.8/package.xml
--rw-r--r--   0        0        0     1452 2023-07-25 17:13:34.222057 holobench-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.8/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/resource/bencher
--rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.8/setup.cfg
--rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.8/setup.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/test/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/__init__.py
--rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/test_catplot.py
--rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/test_plots_common.py
--rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.8/test/plots/test_tables.py
--rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.8/test/test_bench_examples.py
--rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_bencher.py
--rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_combinations.py
--rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_plot_collection.py
--rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_plot_filter.py
--rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_plot_library.py
--rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_sample_cache.py
--rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_sweep_vars.py
--rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_utils.py
--rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.8/test/test_vars.py
--rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 holobench-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      338 2023-08-03 08:51:40.821127 holobench-0.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1518 2023-08-03 12:33:34.699796 holobench-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      311 2023-08-04 08:53:49.179620 holobench-0.2.0/.github/ISSUE_TEMPLATE/sweep-bugfix.yml
+-rw-r--r--   0        0        0      373 2023-08-04 08:53:49.179620 holobench-0.2.0/.github/ISSUE_TEMPLATE/sweep-feature.yml
+-rw-r--r--   0        0        0      347 2023-08-04 08:53:49.179620 holobench-0.2.0/.github/ISSUE_TEMPLATE/sweep-refactor.yml
+-rw-r--r--   0        0        0      502 2023-06-12 11:29:17.697385 holobench-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1230 2023-08-03 13:36:05.592564 holobench-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      594 2023-08-03 10:06:54.411399 holobench-0.2.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      658 2023-08-03 08:51:40.821127 holobench-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3219 2023-08-03 12:33:34.699796 holobench-0.2.0/.gitignore
+-rw-r--r--   0        0        0      381 2023-06-21 11:57:49.059788 holobench-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      209 2023-06-21 11:57:49.059788 holobench-0.2.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      376 2023-08-04 12:12:12.979096 holobench-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1499 2023-08-07 10:00:25.774350 holobench-0.2.0/.vscode/tasks.json
+-rw-r--r--   0        0        0     1065 2023-06-06 14:46:44.492489 holobench-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2934 2023-08-07 10:06:00.323293 holobench-0.2.0/README.md
+-rw-r--r--   0        0        0      747 2023-08-07 10:00:25.774350 holobench-0.2.0/bencher/__init__.py
+-rw-r--r--   0        0        0    28553 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/bench_cfg.py
+-rw-r--r--   0        0        0     3887 2023-08-03 13:53:55.016296 holobench-0.2.0/bencher/bench_plot_server.py
+-rw-r--r--   0        0        0    27981 2023-08-07 10:01:24.930513 holobench-0.2.0/bencher/bencher.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:46:44.492489 holobench-0.2.0/bencher/example/__init__.py
+-rw-r--r--   0        0        0     4224 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/example/benchmark_data.py
+-rw-r--r--   0        0        0     3740 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_categorical.py
+-rw-r--r--   0        0        0     1901 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_custom_sweep.py
+-rw-r--r--   0        0        0     3197 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_float2D_scatter.py
+-rw-r--r--   0        0        0     3716 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_float3D.py
+-rw-r--r--   0        0        0     2817 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_float3D_cone.py
+-rw-r--r--   0        0        0     3366 2023-08-07 10:00:16.262324 holobench-0.2.0/bencher/example/example_float_cat.py
+-rw-r--r--   0        0        0     4318 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_floats.py
+-rw-r--r--   0        0        0     3949 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_floats2D.py
+-rw-r--r--   0        0        0     3469 2023-08-04 08:53:49.183620 holobench-0.2.0/bencher/example/example_holosweep_tap.py
+-rw-r--r--   0        0        0     2360 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_kwargs.py
+-rw-r--r--   0        0        0     2342 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_pareto.py
+-rw-r--r--   0        0        0     2494 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_plot_library.py
+-rw-r--r--   0        0        0     4027 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_sample_cache.py
+-rw-r--r--   0        0        0     3716 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_sample_cache_context.py
+-rw-r--r--   0        0        0    11658 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_simple.py
+-rw-r--r--   0        0        0     1525 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_simple_bool.py
+-rw-r--r--   0        0        0     1473 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_simple_cat.py
+-rw-r--r--   0        0        0     1393 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_simple_float.py
+-rw-r--r--   0        0        0     1996 2023-08-07 10:00:10.682308 holobench-0.2.0/bencher/example/example_time_event.py
+-rw-r--r--   0        0        0     6718 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/example_workflow.py
+-rw-r--r--   0        0        0      846 2023-08-03 15:55:05.360291 holobench-0.2.0/bencher/example/experimental/example_bokeh_plotly.py
+-rw-r--r--   0        0        0     1815 2023-08-03 15:55:05.360291 holobench-0.2.0/bencher/example/experimental/example_hvplot_explorer.py
+-rw-r--r--   0        0        0     2619 2023-08-03 15:55:05.360291 holobench-0.2.0/bencher/example/experimental/example_interactive.py
+-rw-r--r--   0        0        0     1030 2023-08-03 12:33:34.699796 holobench-0.2.0/bencher/example/experimental/example_streams.py
+-rw-r--r--   0        0        0     1172 2023-08-03 15:55:05.360291 holobench-0.2.0/bencher/example/experimental/example_template.py
+-rw-r--r--   0        0        0     3118 2023-08-04 14:29:32.550734 holobench-0.2.0/bencher/example/experimental/example_vector.py
+-rw-r--r--   0        0        0     1052 2023-08-03 12:33:34.699796 holobench-0.2.0/bencher/example/experimental/hover_ex.py
+-rw-r--r--   0        0        0     2261 2023-08-03 15:55:05.360291 holobench-0.2.0/bencher/example/experimental/hv_bool_bug.py
+-rw-r--r--   0        0        0     1414 2023-08-03 12:33:34.703796 holobench-0.2.0/bencher/example/experimental/streamnd.py
+-rw-r--r--   0        0        0     1835 2023-08-03 12:33:34.703796 holobench-0.2.0/bencher/example/experimental/updates.py
+-rw-r--r--   0        0        0     1880 2023-08-03 15:05:36.669832 holobench-0.2.0/bencher/example/mortgage/example_investment.py
+-rw-r--r--   0        0        0     2275 2023-08-03 15:05:36.669832 holobench-0.2.0/bencher/example/mortgage/example_mortgage.py
+-rw-r--r--   0        0        0     8657 2023-08-07 09:59:23.806181 holobench-0.2.0/bencher/example/mortgage/example_mortgage_simulator.py
+-rw-r--r--   0        0        0     3168 2023-08-03 15:05:36.673832 holobench-0.2.0/bencher/example/mortgage/example_personal_finance.py
+-rw-r--r--   0        0        0     2142 2023-08-07 10:00:25.774350 holobench-0.2.0/bencher/example/optuna/example_optuna.py
+-rw-r--r--   0        0        0    12472 2023-08-07 10:00:25.774350 holobench-0.2.0/bencher/optuna_conversions.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/__init__.py
+-rw-r--r--   0        0        0     5454 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/plotting/plot_collection.py
+-rw-r--r--   0        0        0     4723 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/plotting/plot_filter.py
+-rw-r--r--   0        0        0     3579 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/plot_library.py
+-rw-r--r--   0        0        0     1197 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/plot_types.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/plots/__init__.py
+-rw-r--r--   0        0        0     2539 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/plots/catplot.py
+-rw-r--r--   0        0        0     3772 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/plotting/plots/heatmap.py
+-rw-r--r--   0        0        0     3821 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/plots/hv_interactive.py
+-rw-r--r--   0        0        0     6359 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/plots/lineplot.py
+-rw-r--r--   0        0        0      270 2023-08-07 07:29:13.111656 holobench-0.2.0/bencher/plotting/plots/plot_base.py
+-rw-r--r--   0        0        0     2698 2023-08-04 12:12:12.979096 holobench-0.2.0/bencher/plotting/plots/scatterplot.py
+-rw-r--r--   0        0        0     5992 2023-08-07 07:29:13.111656 holobench-0.2.0/bencher/plotting/plots/surface.py
+-rw-r--r--   0        0        0     1194 2023-08-03 08:51:40.829127 holobench-0.2.0/bencher/plotting/plots/tables.py
+-rw-r--r--   0        0        0     5990 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/plotting/plots/volume.py
+-rw-r--r--   0        0        0     5742 2023-08-07 07:29:13.111656 holobench-0.2.0/bencher/plotting_functions.py
+-rw-r--r--   0        0        0    13743 2023-08-07 07:29:13.111656 holobench-0.2.0/bencher/plt_cfg.py
+-rw-r--r--   0        0        0     2528 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/utils.py
+-rw-r--r--   0        0        0     6480 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/variables/inputs.py
+-rw-r--r--   0        0        0     5447 2023-08-07 10:00:25.774350 holobench-0.2.0/bencher/variables/parametrised_sweep.py
+-rw-r--r--   0        0        0     5201 2023-08-07 10:00:25.774350 holobench-0.2.0/bencher/variables/results.py
+-rw-r--r--   0        0        0     4324 2023-08-07 10:00:25.774350 holobench-0.2.0/bencher/variables/sweep_base.py
+-rw-r--r--   0        0        0     2840 2023-08-04 11:10:26.639259 holobench-0.2.0/bencher/variables/time.py
+-rw-r--r--   0        0        0      442 2023-08-03 10:06:54.411399 holobench-0.2.0/dependencies.yaml
+-rw-r--r--   0        0        0     1045 2023-06-06 14:46:44.492489 holobench-0.2.0/package.xml
+-rw-r--r--   0        0        0     2428 2023-08-07 10:02:02.722619 holobench-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 14:46:44.492489 holobench-0.2.0/resource/bencher
+-rw-r--r--   0        0        0       83 2023-06-06 14:46:44.496489 holobench-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      628 2023-06-06 14:46:44.496489 holobench-0.2.0/setup.py
+-rw-r--r--   0        0        0      821 2023-08-04 08:53:49.183620 holobench-0.2.0/sweep.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 14:46:44.496489 holobench-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:51:40.829127 holobench-0.2.0/test/plots/__init__.py
+-rw-r--r--   0        0        0      973 2023-08-03 08:51:40.829127 holobench-0.2.0/test/plots/test_catplot.py
+-rw-r--r--   0        0        0     1330 2023-08-03 15:05:36.673832 holobench-0.2.0/test/plots/test_plots_common.py
+-rw-r--r--   0        0        0     1089 2023-08-03 08:51:40.829127 holobench-0.2.0/test/plots/test_tables.py
+-rw-r--r--   0        0        0     3713 2023-08-07 10:00:25.774350 holobench-0.2.0/test/test_bench_examples.py
+-rw-r--r--   0        0        0    16047 2023-08-03 15:05:36.673832 holobench-0.2.0/test/test_bencher.py
+-rw-r--r--   0        0        0     6150 2023-08-03 15:05:36.673832 holobench-0.2.0/test/test_combinations.py
+-rw-r--r--   0        0        0     2140 2023-08-07 10:00:25.774350 holobench-0.2.0/test/test_parametrized_sweep.py
+-rw-r--r--   0        0        0     3534 2023-08-03 08:51:40.833127 holobench-0.2.0/test/test_plot_collection.py
+-rw-r--r--   0        0        0     2772 2023-08-03 08:51:40.833127 holobench-0.2.0/test/test_plot_filter.py
+-rw-r--r--   0        0        0     1788 2023-08-03 08:51:40.833127 holobench-0.2.0/test/test_plot_library.py
+-rw-r--r--   0        0        0     5671 2023-08-03 15:05:36.673832 holobench-0.2.0/test/test_sample_cache.py
+-rw-r--r--   0        0        0     1978 2023-08-04 11:10:26.639259 holobench-0.2.0/test/test_sweep_vars.py
+-rw-r--r--   0        0        0     2487 2023-08-03 14:59:11.292279 holobench-0.2.0/test/test_utils.py
+-rw-r--r--   0        0        0     2439 2023-08-03 08:51:40.833127 holobench-0.2.0/test/test_vars.py
+-rw-r--r--   0        0        0     4345 1970-01-01 00:00:00.000000 holobench-0.2.0/PKG-INFO
```

### Comparing `holobench-0.0.8/.devcontainer/devcontainer.json` & `holobench-0.2.0/.devcontainer/devcontainer.json`

 * *Files 5% similar despite different names*

```diff
@@ -32,13 +32,14 @@
 				"ms-python.python",
 				"ms-python.vscode-pylance",
 				"ms-python.pylint",
 				"njpwerner.autodocstring",
 				"charliermarsh.ruff",
 				"mhutchie.git-graph",
 				"eamodio.gitlens",
-				"tamasfe.even-better-toml"
+				"tamasfe.even-better-toml",
+				"Codium.codium"
 			]
 		}
 	},
 	// "onCreateCommand": "pre-commit install-hooks"
 }
```

### Comparing `holobench-0.0.8/.github/workflows/publish.yml` & `holobench-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/.gitignore` & `holobench-0.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -161,8 +161,8 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 hashed_vars_comparison_tmp
-.vscode/cfg/
+.vscode/active_file.cfg
```

### Comparing `holobench-0.0.8/.vscode/tasks.json` & `holobench-0.2.0/.vscode/tasks.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8833333333333333%*

 * *Differences: {"'tasks'": "{7: {'command': 'echo ${file} > ${workspaceFolder}/.vscode/active_file.cfg; echo "*

 * *            "Setting the current file: ${file} as the active file.'}, 8: {'command': "*

 * *            "'RUNFILE=$(cat ${workspaceFolder}/.vscode/active_file.cfg); echo Running file: "*

 * *            "$RUNFILE; python3 $RUNFILE'}, insert: [(1, OrderedDict([('label', 'pylint'), ('type', "*

 * *            '\'shell\'), (\'command\', "pylint $(git ls-files \'*.py\') ")])), (2, '*

 * *            "OrderedDict([('label', 'code coverag […]*

```diff
@@ -2,35 +2,65 @@
     "tasks": [
         {
             "command": "ruff . --fix && black .",
             "label": "autoformat",
             "type": "shell"
         },
         {
+            "command": "pylint $(git ls-files '*.py') ",
+            "label": "pylint",
+            "type": "shell"
+        },
+        {
+            "command": "coverage run -m pytest ; coverage report",
+            "label": "code coverage",
+            "type": "shell"
+        },
+        {
+            "command": "pytest --durations=0",
+            "label": "pytest duration",
+            "type": "shell"
+        },
+        {
+            "dependsOn": [
+                "autoformat",
+                "pylint",
+                "code coverage"
+            ],
+            "dependsOrder": "sequence",
+            "detail": "Runs the basic formatting and linting checks performed by CI",
+            "label": "check CI",
+            "presentation": {
+                "panel": "dedicated",
+                "reveal": "always"
+            },
+            "type": "shell"
+        },
+        {
             "command": "flit install --symlink",
             "label": "flit install",
             "type": "shell"
         },
         {
             "command": "flit publish",
             "label": "flit publish",
             "type": "shell"
         },
         {
-            "command": "mkdir ${workspaceFolder}/.vscode/cfg/;echo ${file} > $_/active_file.cfg; echo Setting the current file: ${file} as the active file.",
+            "command": "echo ${file} > ${workspaceFolder}/.vscode/active_file.cfg; echo Setting the current file: ${file} as the active file.",
             "group": {
                 "isDefault": "True",
                 "kind": "test"
             },
             "label": "sa: Set Active File",
             "problemMatcher": [],
             "type": "shell"
         },
         {
-            "command": "RUNFILE=$(cat ${workspaceFolder}/.vscode/cfg/active_file.cfg); echo Running file: $RUNFILE; python3 $RUNFILE",
+            "command": "RUNFILE=$(cat ${workspaceFolder}/.vscode/active_file.cfg); echo Running file: $RUNFILE; python3 $RUNFILE",
             "group": {
                 "isDefault": "True",
                 "kind": "build"
             },
             "label": "ra: Run Active File",
             "problemMatcher": [],
             "type": "shell"
```

### Comparing `holobench-0.0.8/LICENSE` & `holobench-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/README.md` & `holobench-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Bencher
 
 ## Continuous Integration Status
 
 [![Ci](https://github.com/dyson-ai/bencher/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/dyson-ai/bencher/actions/workflows/ci.yml?query=branch%3Amain)
-[![Code Coverage](https://codecov.io/gh/dyson-ai/bencher/branch/main/graph/badge.svg?token=W7uHKcY0ly)](https://codecov.io/gh/dyson-ai/bencher)
+[![Codecov](https://codecov.io/gh/blooop/bencher/branch/main/graph/badge.svg?token=AVFC5D5Z43)](https://codecov.io/gh/blooop/bencher)
+![PyPI](https://img.shields.io/pypi/v/holobench)
+![License](https://img.shields.io/pypi/l/bencher)
+[![Python](https://img.shields.io/badge/python-3.10%20%7C%203.11-blue)](https://www.python.org/downloads/release/python-310/)
+
 
 ## Intro
 
 Bencher is a tool to make it easy to benchmark the interactions between the input parameters to your algorithm and its resulting performance on a set of metrics.
 
 Parameters for bencher are defined using the param library https://param.holoviz.org/ as a config class with extra metadata that describes the bounds of the search space you want to measure.  You must define a benchmarking function that accepts an instance of the config class and return a dictionary with string metric names and float values.
 
@@ -30,9 +34,8 @@
         look up previous results for that hash
         if it exists:
             load historical data
             combine latest data with historical data
         
         store the results using the input hash as a key
     deduce the type of plot based on the input types
-    return data and plot
- 
+    return data and plot
```

### Comparing `holobench-0.0.8/bencher/bench_cfg.py` & `holobench-0.2.0/bencher/bench_cfg.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,27 @@
 import xarray as xr
 from pandas import DataFrame
 from str2bool import str2bool
 import holoviews as hv
 import numpy as np
 
 import bencher as bch
-from bencher.bench_vars import OptDir, TimeEvent, TimeSnapshot, describe_variable, hash_sha1
+from bencher.variables.sweep_base import hash_sha1, describe_variable
+from bencher.variables.time import TimeSnapshot, TimeEvent
+from bencher.variables.results import OptDir
+from bencher.utils import hmap_canonical_input
+
+from enum import Enum, auto
+
+
+class ReduceType(Enum):
+    AUTO = auto()
+    SQUEEZE = auto()
+    REDUCE = auto()
+    NONE = auto()
 
 
 def to_filename(
     param_cfg: param.Parameterized, param_list: list[str] = None, exclude_params: list[str] = None
 ) -> str:
     """given a parametrized class, generate a filename based on some of the parameter properties
 
@@ -129,14 +141,18 @@
     cat_cnt = param.Integer(0, doc="The number of cat variables")
     vector_len = param.Integer(1, doc="The vector length of the return variable , scalars = len 1")
     result_vars = param.Integer(1, doc="The number result variables to plot")
 
 
 class BenchPlotSrvCfg(param.Parameterized):
     port: int = param.Integer(None, doc="The port to launch panel with")
+    allow_ws_origin = param.Boolean(
+        False,
+        doc="Add the port to the whilelist, (warning will disable remote access if set to true)",
+    )
 
 
 class BenchRunCfg(BenchPlotSrvCfg):
     """A Class to store options for how to run a benchmark parameter sweep"""
 
     repeats: bool = param.Integer(1, doc="The number of times to sample the inputs")
 
@@ -223,14 +239,19 @@
     time_event: str = param.String(
         None,
         doc="A string representation of a sequence over time, i.e. datetime, pull request number, or run number",
     )
 
     headless: bool = param.Boolean(False, doc="Run the benchmarks headlessly")
 
+    render_plotly = param.Boolean(
+        True,
+        doc="Plotly and Bokeh don't play nicely together, so by default pre-render plotly figures to a non dynamic version so that bokeh plots correctly.  If you want interactive 3D graphs, set this to true but be aware that your 2D interactive graphs will probalby stop working.",
+    )
+
     @staticmethod
     def from_cmd_line() -> BenchRunCfg:
         """create a BenchRunCfg by parsing command line arguments
 
         Returns:
             parsed args: parsed args
         """
@@ -358,14 +379,15 @@
     def __init__(self, **params):
         super().__init__(**params)
         self.studies = []
         self.ds = xr.Dataset()
         self.plot_lib = None
         self.hmap = {}
         self.hmap_kdims = None
+        self.iv_repeat = None
 
     def hash_persistent(self, include_repeats) -> str:
         """override the default hash function becuase the default hash function does not return the same value for the same inputs.  It references internal variables that are unique per instance of BenchCfg
 
         Args:
             include_repeats (bool) : by default include repeats as part of the hash execpt with using the sample cache
         """
@@ -494,75 +516,92 @@
 
     def get_best_trial_params(self):
         return self.studies[0].best_trials[0].params
 
     def get_pareto_front_params(self):
         return [p.params for p in self.studies[0].trials]
 
-    def get_hv_dataset(self, reduce=None):
+    def get_hv_dataset(self, reduce: ReduceType = ReduceType.AUTO) -> hv.Dataset:
+        """Generate a holoviews dataset from the xarray dataset.
+
+        Args:
+            reduce (ReduceType, optional): Optionally perform reduce options on the dataset.  By default the returned dataset will calculate the mean and standard devation over the "repeat" dimension so that the dataset plays nicely with most of the holoviews plot types.  Reduce.Sqeeze is used if there is only 1 repeat and you want the "reduce" variable removed from the dataset. ReduceType.None returns an unaltered dataset. Defaults to ReduceType.AUTO.
+
+        Returns:
+            hv.Dataset: results in the form of a holoviews dataset
+        """
         ds = convert_dataset_bool_dims_to_str(self.ds)
-        if reduce is None:
-            reduce = self.repeats > 1
-        if reduce:
-            return hv.Dataset(ds).reduce(["repeat"], np.mean, np.std)
-            # return hv.Dataset(self.ds).reduce(["repeat"], np.mean, np.std, "nearest")
 
-        if self.repeats == 1:
-            return hv.Dataset(ds.squeeze("repeat", drop=True))
-        return hv.Dataset(ds)
+        if reduce == ReduceType.AUTO:
+            reduce = ReduceType.REDUCE if self.repeats > 1 else ReduceType.SQUEEZE
+
+        result_vars_str = [r.name for r in self.result_vars]
+        hvds = hv.Dataset(ds, vdims=result_vars_str)
+        if reduce == ReduceType.REDUCE:
+            return hvds.reduce(["repeat"], np.mean, np.std)
+        if reduce == ReduceType.SQUEEZE:
+            return hv.Dataset(ds.squeeze("repeat", drop=True), vdims=result_vars_str)
+        return hvds
 
-    def to(self, hv_type: hv.Chart, reduce=True) -> hv.Chart:
-        return self.get_hv_dataset(reduce).to(hv_type)
+    def to(self, hv_type: hv.Chart, reduce: ReduceType = ReduceType.AUTO, **kwargs) -> hv.Chart:
+        return self.get_hv_dataset(reduce).to(hv_type, **kwargs)
 
-    def to_curve(self, reduce=None) -> hv.Curve:
+    def to_curve(self, reduce: ReduceType = ReduceType.AUTO) -> hv.Curve:
         ds = self.get_hv_dataset(reduce)
         pt = ds.to(hv.Curve)
         if self.repeats > 1:
             pt *= ds.to(hv.Spread).opts(alpha=0.2)
         return pt
 
     def to_error_bar(self) -> hv.Bars:
-        return self.get_hv_dataset(True).to(hv.ErrorBars)
+        return self.get_hv_dataset(ReduceType.REDUCE).to(hv.ErrorBars)
 
-    def to_points(self, reduce=None) -> hv.Points:
+    def to_points(self, reduce: ReduceType = ReduceType.AUTO) -> hv.Points:
         ds = self.get_hv_dataset(reduce)
         pt = ds.to(hv.Points)
         if reduce:
             pt *= ds.to(hv.ErrorBars)
         return pt
 
     def to_scatter(self) -> hv.Scatter:
-        ds = self.get_hv_dataset(False)
+        ds = self.get_hv_dataset(ReduceType.NONE)
         pt = ds.to(hv.Scatter).opts(jitter=0.1).overlay("repeat").opts(show_legend=False)
         return pt
-        # ds = self.get_hv_dataset(reduce)
-        # pt = ds.to(hv.Points)
-        # if reduce:
-        # pt *= ds.to(hv.ErrorBars)
-        # return pt
 
-    def to_bar(self, reduce=None) -> hv.Bars:
+    def to_bar(self, reduce: ReduceType = ReduceType.AUTO) -> hv.Bars:
         ds = self.get_hv_dataset(reduce)
         pt = ds.to(hv.Bars)
         if reduce:
             pt *= ds.to(hv.ErrorBars)
         return pt
 
-    def to_heatmap(self, reduce=None) -> hv.HeatMap:
-        return self.to(hv.HeatMap, reduce)
+    def to_heatmap(self, reduce: ReduceType = ReduceType.AUTO, **kwargs) -> hv.HeatMap:
+        return self.to(hv.HeatMap, reduce, **kwargs)
 
     def to_nd_layout(self) -> hv.NdLayout:
         return hv.NdLayout(self.hmap, kdims=self.hmap_kdims).opts(
             shared_axes=False, shared_datasource=False
         )
 
     def to_holomap(self) -> hv.HoloMap:
         # return hv.HoloMap(self.hmap, self.hmap_kdims)
         return hv.HoloMap(self.to_nd_layout()).opts(shared_axes=False)
 
+    def to_dynamic_map(self) -> hv.DynamicMap:
+        """use the values stored in the holomap dictionary to populate a dynamic map. Note that this is much faster than passing the holomap to a holomap object as the values are calculated on the fly"""
+
+        def cb(**kwargs):
+            return self.hmap[hmap_canonical_input(kwargs)].opts(framewise=True, shared_axes=False)
+
+        kdims = []
+        for i in self.input_vars + [self.iv_repeat]:
+            kdims.append(i.as_dim(compute_values=True, debug=self.debug))
+
+        return hv.DynamicMap(cb, kdims=kdims)
+
     def to_grid(self):
         inputs = self.inputs_as_str()
         if len(inputs) > 2:
             inputs = inputs[:2]
         return self.to_holomap().grid(inputs)
 
     def inputs_as_str(self) -> List[str]:
```

### Comparing `holobench-0.0.8/bencher/bench_plot_server.py` & `holobench-0.2.0/bencher/bench_plot_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             plot_cfg (BenchPlotSrvCfg, optional): Options for the plot server. Defaults to BenchPlotSrvCfg().
 
         Raises:
             FileNotFoundError: No data found was found in the database to plot
         """
         if plots_instance is None:
             plots_instance = self.load_data_from_cache(bench_name)
-        if plot_cfg.port is not None:
+        if plot_cfg.port is not None and plot_cfg.allow_ws_origin:
             os.environ["BOKEH_ALLOW_WS_ORIGIN"] = f"localhost:{plot_cfg.port}"
 
         self.serve(bench_name, plots_instance, port=plot_cfg.port)
 
     def load_data_from_cache(self, bench_name: str) -> Tuple[BenchCfg, List[pn.panel]] | None:
         """Load previously calculated benchmark data from the database and start a plot server to display it
```

### Comparing `holobench-0.0.8/bencher/bencher.py` & `holobench-0.2.0/bencher/bencher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import logging
 from datetime import datetime
 from itertools import product
 from typing import Callable, List
+import warnings
 
 import numpy as np
 import panel as pn
 import param
 import xarray as xr
 from diskcache import Cache
 from sortedcontainers import SortedDict
 
 from bencher.bench_cfg import BenchCfg, BenchRunCfg, DimsCfg
 from bencher.bench_plot_server import BenchPlotServer
-from bencher.bench_vars import (
-    IntSweep,
-    ParametrizedSweep,
-    ResultList,
-    ResultVar,
-    ResultVec,
-    TimeEvent,
-    TimeSnapshot,
-    hash_sha1,
-)
+
+
+from bencher.variables.sweep_base import hash_sha1
+from bencher.variables.inputs import IntSweep
+from bencher.variables.time import TimeSnapshot, TimeEvent
+from bencher.variables.results import ResultVar, ResultVec
+
+from bencher.variables.parametrised_sweep import ParametrizedSweep
+
 from bencher.plotting.plot_collection import PlotCollection
 from bencher.plt_cfg import BenchPlotter
 from bencher.plotting.plot_library import PlotLibrary  # noqa pylint: disable=unused-import
+from bencher.utils import hmap_canonical_input
 
 # Customize the formatter
 formatter = logging.Formatter("%(levelname)s: %(message)s")
 logging.basicConfig(level=logging.INFO, format="%(levelname)s %(message)s")
 
 for handler in logging.root.handlers:
     handler.setFormatter(formatter)
@@ -122,14 +123,15 @@
         # The number of times the cache was used instead of the raw worker
         self.worker_cache_call_count = 0
         self.bench_cfg_hashes = []  # a list of hashes that point to benchmark results
         self.last_run_cfg = None  # cached run_cfg used to pass to the plotting function
         self.sample_cache = None  # store the results of each benchmark function call in a cache
         self.ds_dynamic = {}  # A dictionary to store unstructured vector datasets
         self.plot_lib = plot_lib
+        self.cache_size = int(100e9)  # default to 100gb
 
     def set_worker(self, worker: Callable, worker_input_cfg: ParametrizedSweep = None) -> None:
         """Set the benchmark worker function and optionally the type the worker expects
 
         Args:
             worker (Callable): The benchmark worker function
             worker_input_cfg (ParametrizedSweep, optional): The input type the worker expects. Defaults to None.
@@ -219,20 +221,23 @@
         bench_cfg_hash = bench_cfg.hash_persistent(True)
         bench_cfg.hash_value = bench_cfg_hash
 
         # does not include repeats in hash as sample_hash already includes repeat as part of the per sample hash
         bench_cfg_sample_hash = bench_cfg.hash_persistent(False)
 
         if bench_cfg.use_sample_cache:
-            self.sample_cache = Cache("cachedir/sample_cache", tag_index=True)
+            # default to 20Gb cache
+            self.sample_cache = Cache(
+                "cachedir/sample_cache", tag_index=True, size_limit=self.cache_size
+            )
             if bench_cfg.clear_sample_cache:
                 self.clear_tag_from_cache(bench_cfg.tag)
 
         calculate_results = True
-        with Cache("cachedir/benchmark_inputs") as c:
+        with Cache("cachedir/benchmark_inputs", size_limit=self.cache_size) as c:
             if run_cfg.clear_cache:
                 c.delete(bench_cfg_hash)
                 logging.info("cleared cache")
             elif run_cfg.use_cache:
                 logging.info(
                     f"checking for previously calculated results with key: {bench_cfg_hash}"
                 )
@@ -260,14 +265,19 @@
                 bench_cfg.ds = self.load_history_cache(
                     bench_cfg.ds, bench_cfg_hash, run_cfg.clear_history
                 )
 
             self.report_results(bench_cfg, run_cfg.print_xarray, run_cfg.print_pandas)
             self.cache_results(bench_cfg, bench_cfg_hash)
 
+        if self.sample_cache is not None:
+            logging.info(
+                f"cache size :{int(self.sample_cache.volume() / 1000000)}MB / {int(self.cache_size/1000000)}MB"
+            )
+
         self.pane = BenchPlotter.plot(bench_cfg, self.pane)
         return bench_cfg
 
     def check_var_is_a_param(self, variable: param.Parameter, var_type: str):
         """check that a variable is a subclass of param
 
         Args:
@@ -279,15 +289,15 @@
         """
         if not isinstance(variable, param.Parameter):
             raise TypeError(
                 f"You need to use {var_type}_vars =[{self.worker_input_cfg}.param.your_variable], instead of {var_type}_vars =[{self.worker_input_cfg}.your_variable]"
             )
 
     def cache_results(self, bench_cfg: BenchCfg, bench_cfg_hash: int) -> None:
-        with Cache("cachedir/benchmark_inputs") as c:
+        with Cache("cachedir/benchmark_inputs", size_limit=self.cache_size) as c:
             logging.info(f"saving results with key: {bench_cfg_hash}")
             self.bench_cfg_hashes.append(bench_cfg_hash)
             c[bench_cfg_hash] = bench_cfg
             logging.info(f"saving benchmark: {self.bench_name}")
             c[self.bench_name] = self.bench_cfg_hashes
 
     def calculate_benchmark_results(
@@ -301,15 +311,16 @@
 
         Returns:
             bench_cfg (BenchCfg): description of the benchmark parameters
         """
         bench_cfg, func_inputs, dims_name = self.setup_dataset(bench_cfg, time_src)
         constant_inputs = self.define_const_inputs(bench_cfg.const_vars)
         callcount = 1
-        bench_cfg.hmap_kdims = dims_name
+        bench_cfg.hmap_kdims = sorted(dims_name)
+
         for idx_tuple, function_input_vars in func_inputs:
             logging.info(f"{bench_cfg.title}:call {callcount}/{len(func_inputs)}")
             self.call_worker_and_store_results(
                 bench_cfg,
                 idx_tuple,
                 function_input_vars,
                 dims_name,
@@ -319,23 +330,27 @@
             )
             callcount += 1
 
         for inp in bench_cfg.all_vars:
             self.add_metadata_to_dataset(bench_cfg, inp)
         return bench_cfg
 
-    def plot(self, run_cfg: BenchRunCfg = None) -> None:
+    def show(self, run_cfg: BenchRunCfg = None) -> None:
         """Launches a webserver with plots of the benchmark results, blocking
 
         Args:
             run_cfg (BenchRunCfg, optional): Options for the webserve such as the port. Defaults to None.
 
         """
         if run_cfg is None:
-            run_cfg = self.last_run_cfg
+            if self.last_run_cfg is not None:
+                run_cfg = self.last_run_cfg
+            else:
+                run_cfg = BenchRunCfg()
+
         BenchPlotServer().plot_server(self.bench_name, run_cfg, self.pane)
 
     def load_history_cache(
         self, ds: xr.Dataset, bench_cfg_hash: int, clear_history: bool
     ) -> xr.Dataset:
         """Load historical data from a cache if over_time=true
 
@@ -343,15 +358,15 @@
             ds (xr.Dataset): Freshly calcuated data
             bench_cfg_hash (int): Hash of the input variables used to generate the data
             clear_history (bool): Optionally clear the history
 
         Returns:
             xr.Dataset: historical data as an xr dataset
         """
-        with Cache("cachedir/history") as c:
+        with Cache("cachedir/history", size_limit=self.cache_size) as c:
             if clear_history:
                 logging.info("clearing history")
             else:
                 logging.info(f"checking historical key: {bench_cfg_hash}")
                 if bench_cfg_hash in c:
                     logging.info("loading historical data from cache")
                     ds_old = c[bench_cfg_hash]
@@ -485,17 +500,17 @@
             bench_cfg (BenchCfg): description of the benchmark parameters
             index_tuple (tuple): tuple of n-d array indices
             function_input_vars (List): list of function inputs as dicts
             dims_name (List[str]): names of the n-d dimension
             constant_inputs (dict): input values to keep constant
         """
         self.worker_wrapper_call_count += 1
-        function_input = dict(zip(dims_name, function_input_vars))
+        function_input = SortedDict(zip(dims_name, function_input_vars))
 
-        fn_inp_with_rep = tuple(function_input.values())
+        canonical_input = hmap_canonical_input(function_input)
 
         if constant_inputs is not None:
             function_input |= constant_inputs
 
         if bench_cfg.print_bench_inputs:
             logging.info("Bench Inputs:")
             for k, v in function_input.items():
@@ -506,45 +521,52 @@
             # the signature is the hash of the inputs to to the function + meta variables such as repeat and time + the hash of the benchmark sweep as a whole (without the repeats hash)
             fn_inputs_sorted = list(SortedDict(function_input).items())
             function_input_signature_pure = hash_sha1((fn_inputs_sorted, bench_cfg.tag))
 
             function_input_signature_benchmark_context = hash_sha1(
                 (function_input_signature_pure, bench_cfg_sample_hash)
             )
-            print("inputs", fn_inputs_sorted)
-            print("pure", function_input_signature_pure)
+            # logging.info(f"inputs: {fn_inputs_sorted}")
+            # logging.info(f"pure: {function_input_signature_pure}")
             if function_input_signature_benchmark_context in self.sample_cache:
                 logging.info(
-                    f"Found a previously calculated value in the sample cache with the benchmark: {bench_cfg.title}, hash: {bench_cfg_sample_hash}"
+                    f"Hash: {function_input_signature_benchmark_context} was found in context cache, loading..."
                 )
                 result = self.sample_cache[function_input_signature_benchmark_context]
                 self.worker_cache_call_count += 1
-            elif bench_run_cfg.only_hash_tag and function_input_signature_pure in self.sample_cache:
+            elif bench_run_cfg.only_hash_tag and (
+                function_input_signature_pure in self.sample_cache
+            ):
                 logging.info(
-                    f"A value including the benchmark context was not found: {bench_cfg.title} hash: {bench_cfg_sample_hash}, but was found with tag:{bench_cfg.tag} so loading those values from the cache.  Beware that depending on how you have run the benchmarks, the data in this cache could be invalid"
+                    f"Hash: {function_input_signature_benchmark_context} not found in context cache"
                 )
+                logging.info(
+                    f"Hash: {function_input_signature_pure} was found in the function cache, loading..."
+                )
+
                 result = self.sample_cache[function_input_signature_pure]
                 self.worker_cache_call_count += 1
             else:
-                logging.info(
-                    "Sample cache values Not Found for either pure function inputs or inputs within a benchmark context, calling benchmark function"
-                )
+                logging.info(f"Context not in cache: {function_input_signature_benchmark_context}")
+                logging.info(f"Function inputs not cache: {function_input_signature_pure}")
+                logging.info("Calling benchmark function")
+
                 result = self.worker_wrapper(bench_cfg, function_input)
                 self.sample_cache.set(
                     function_input_signature_benchmark_context, result, tag=bench_cfg.tag
                 )
                 self.sample_cache.set(function_input_signature_pure, result, tag=bench_cfg.tag)
         else:
             result = self.worker_wrapper(bench_cfg, function_input)
 
         # construct a dict for a holomap
         if type(result) == dict:  # todo holomaps with named types
             if "hmap" in result:
                 # print(isinstance(result["hmap"], hv.element.Element))
-                bench_cfg.hmap[fn_inp_with_rep] = result["hmap"]
+                bench_cfg.hmap[canonical_input] = result["hmap"]
 
         logging.debug(f"input_index {index_tuple}")
         logging.debug(f"input {function_input_vars}")
         logging.debug(f"result {result}")
         for rv in bench_cfg.result_vars:
             if type(result) == dict:
                 result_value = result[rv.name]
@@ -559,42 +581,27 @@
             elif type(rv) == ResultVec:
                 if isinstance(result_value, (list, np.ndarray)):
                     if len(result_value) == rv.size:
                         for i in range(rv.size):
                             set_xarray_multidim(
                                 bench_cfg.ds[rv.index_name(i)], index_tuple, result_value[i]
                             )
-            elif type(rv) == ResultList:
-                # TODO generalise this for arbirary dimensions, only works for 1 input dim so far.
-                dimname = bench_cfg.input_vars[0].name
-                input_value = function_input[dimname]
-
-                new_dataarray = xr.DataArray(
-                    [result_value.values],
-                    name=rv.name,
-                    coords={dimname: [input_value], rv.dim_name: result_value.index},
-                )
 
-                dataset_key = (bench_cfg.hash_value, rv.name)
-                if dataset_key in self.ds_dynamic:
-                    self.ds_dynamic[dataset_key] = xr.concat(
-                        [self.ds_dynamic[dataset_key], new_dataarray], dimname
-                    )
-                else:
-                    self.ds_dynamic[dataset_key] = new_dataarray
             else:
                 raise RuntimeError("Unsupported result type")
 
     def clear_tag_from_cache(self, tag: str):
         """Clear all samples from the cache that match a tag
         Args:
             tag(str): clear samples with this tag
         """
         if self.sample_cache is None:
-            self.sample_cache = Cache("cachedir/sample_cache", tag_index=True)
+            self.sample_cache = Cache(
+                "cachedir/sample_cache", tag_index=True, size_limit=self.cache_size
+            )
         logging.info(f"clearing the sample cache for tag: {tag}")
         removed_vals = self.sample_cache.evict(tag)
         logging.info(f"removed: {removed_vals} items from the cache")
 
     def add_metadata_to_dataset(self, bench_cfg: BenchCfg, input_var: ParametrizedSweep) -> None:
         """Adds variable metadata to the xrarry so that it can be used to automatically plot the dimension units etc.
 
@@ -649,15 +656,17 @@
         Args:
             main_plot (bool, optional): return the last added page. Defaults to True.
 
         Returns:
             pn.pane: results panel
         """
         if main_plot:
-            return self.pane[-1][0]
+            if len(self.pane) > 0:
+                return self.pane[-1][0]
+            return self.pane
         return self.pane[-1]
 
     def append(self, pane: pn.panel) -> None:
         self.get_panel().append(pane)
 
     def append_tab(self, pane: pn.panel):
         self.pane.append(pane)
@@ -668,7 +677,12 @@
         Args:
             bench_cfg (BenchCfg): Results
 
         Returns:
             dict: dictionary of best params
         """
         return bench_cfg.studies[0].best_trials[0].params
+
+
+def to_bench(param_class: ParametrizedSweep) -> Bench:
+    instance = param_class()
+    return Bench(param_class.name, instance.call)
```

### Comparing `holobench-0.0.8/bencher/example/benchmark_data.py` & `holobench-0.2.0/bencher/example/benchmark_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 
 import math
 import random
 from enum import auto
 
 from strenum import StrEnum
 
-from bencher.bench_vars import (
-    BoolSweep,
-    EnumSweep,
-    FloatSweep,
-    IntSweep,
-    OptDir,
-    ParametrizedSweep,
-    ResultVar,
-    StringSweep,
-)
+
+from bencher.variables.inputs import IntSweep, FloatSweep, StringSweep, EnumSweep, BoolSweep
+from bencher.variables.results import ResultVar, OptDir
+
+from bencher.variables.parametrised_sweep import ParametrizedSweep
 
 
 class PostprocessFn(StrEnum):
     """Apply a postprocessing step to the data"""
 
     absolute = auto()  # return the abs of the output data
     negate = auto()  # return the negative of the output data
```

### Comparing `holobench-0.0.8/bencher/example/example_bokeh_plotly.py` & `holobench-0.2.0/bencher/example/experimental/example_bokeh_plotly.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/example/example_categorical.py` & `holobench-0.2.0/bencher/example/example_categorical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pylint: disable=duplicate-code
 
 import pathlib
 
-from bencher.bencher import Bench, BenchRunCfg
+import bencher as bch
 
 # All the examples will be using the data structures and benchmark function defined in this file
 from bencher.example.benchmark_data import ExampleBenchCfgIn, ExampleBenchCfgOut, bench_function
 
-bench = Bench("Bencher_Example_Categorical", bench_function, ExampleBenchCfgIn)
+bench = bch.Bench("Bencher_Example_Categorical", bench_function, ExampleBenchCfgIn)
 
 
-def example_categorical(run_cfg: BenchRunCfg) -> Bench:
+def example_categorical(run_cfg: bch.BenchRunCfg) -> bch.Bench:
     """Example of how to perform a categorical parameter sweep
 
     Args:
         run_cfg (BenchRunCfg): configuration of how to perform the param sweep
 
     Returns:
         Bench: results of the parameter sweep
@@ -76,18 +76,18 @@
             ExampleBenchCfgIn.param.noise_distribution,
             ExampleBenchCfgIn.param.postprocess_fn,
         ],
         title="Categorical 3D Example Over Time",
         result_vars=[ExampleBenchCfgOut.param.out_sin],
         description="""Lastly, what if you want to track these distributions over time? Set over_time=True and bencher will cache and display historical resuts alongside the latest result.  Use clear_history=True to clear that cache.""",
         post_description="The output shows faceted line plot with confidence intervals for the mean value over time.",
-        run_cfg=BenchRunCfg(repeats=20, over_time=True),
+        run_cfg=bch.BenchRunCfg(repeats=20, over_time=True),
     )
 
     return bench
 
 
 if __name__ == "__main__":
-    ex_run_cfg = BenchRunCfg(repeats=10)
+    ex_run_cfg = bch.BenchRunCfg(repeats=10)
     ex_run_cfg.over_time = True
 
-    example_categorical(ex_run_cfg).plot()
+    example_categorical(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_custom_sweep.py` & `holobench-0.2.0/bencher/example/example_custom_sweep.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,8 +56,8 @@
     )
     return bencher
 
 
 if __name__ == "__main__":
     ex_run_cfg = bch.BenchRunCfg()
     # ex_run_cfg.debug = True
-    example_custom_sweep(ex_run_cfg).plot()
+    example_custom_sweep(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_float2D_scatter.py` & `holobench-0.2.0/bencher/example/example_float2D_scatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,8 +102,8 @@
 
 
 if __name__ == "__main__":
     ex_run_cfg = bch.BenchRunCfg()
     ex_run_cfg.repeats = 50
     ex_run_cfg.over_time = True
     # ex_run_cfg.clear_history = True
-    example_floats2D_scatter(ex_run_cfg).plot()
+    example_floats2D_scatter(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_float3D.py` & `holobench-0.2.0/bencher/example/example_float3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,8 @@
     )
 
     return bench
 
 
 if __name__ == "__main__":
     ex_run_cfg = bch.BenchRunCfg()
-    example_floats3D(ex_run_cfg).plot()
+    example_floats3D(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_float3D_cone.py` & `holobench-0.2.0/bencher/example/example_float3D_cone.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,8 +89,8 @@
 
     return bench
 
 
 if __name__ == "__main__":
     ex_run_cfg = bch.BenchRunCfg()
     ex_run_cfg.use_cache = True
-    example_cone(ex_run_cfg).plot()
+    example_cone(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_float_cat.py` & `holobench-0.2.0/bencher/example/example_float_cat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Example of how to perform a parameter sweep for categorical variables"""
-from bencher import Bench, BenchRunCfg
+import bencher as bch
+
 
 # All the examples will be using the data structures and benchmark function defined in this file
 from bencher.example.benchmark_data import ExampleBenchCfgIn, ExampleBenchCfgOut, bench_function
 
 
-def example_cat_float(run_cfg: BenchRunCfg) -> Bench:
+def example_float_cat(run_cfg: bch.BenchRunCfg) -> bch.Bench:
     """Example of how to perform a parameter sweep for categorical variables
 
     Args:
         run_cfg (BenchRunCfg): configuration of how to perform the param sweep
 
     Returns:
         Bench: results of the parameter sweep
     """
-    bench = Bench("Bencher_Example_Float_Cat", bench_function, ExampleBenchCfgIn)
+    bench = bch.Bench("Bencher_Example_Float_Cat", bench_function, ExampleBenchCfgIn)
 
     ExampleBenchCfgIn.param.theta.samples = 3
 
     bench.plot_sweep(
         input_vars=[
             ExampleBenchCfgIn.param.theta,
             ExampleBenchCfgIn.param.offset,
@@ -38,50 +39,43 @@
         const_vars=[(ExampleBenchCfgIn.param.noisy, True)],
         title="Float 1D Cat 1D  Example",
         description="""Following from the previous example lets add another input parameter to see how that affects the output.  We pass the boolean  'noisy' and keep the other parameters the same""",
         post_description="Now the plot has two lines, one for each of the boolean values where noisy=true and noisy=false.",
         run_cfg=run_cfg,
     )
 
-    # this does not work yet because it tries to find min and max of categorical values
+    # # this does not work yet because it tries to find min and max of categorical values
     # bench.plot_sweep(
     #     input_vars=[ExampleBenchCfgIn.param.theta, ExampleBenchCfgIn.param.postprocess_fn],
     #     result_vars=[ExampleBenchCfgOut.param.out_sin],
     #     const_vars=[(ExampleBenchCfgIn.param.noisy, True)],
     #     title="Float 1D Cat 1D  Example",
     #     description="""Following from the previous example lets add another input parameter to see how that affects the output.  We pass the boolean  'noisy' and keep the other parameters the same""",
     #     post_description="Now the plot has two lines, one for each of the boolean values where noisy=true and noisy=false.",
     #     run_cfg=run_cfg,
     # )
 
     return bench
 
 
-if __name__ == "__main__":
-    import time
-
-    ex_run_cfg = BenchRunCfg()
+def run_example_float_cat(ex_run_cfg=bch.BenchRunCfg()) -> None:
     ex_run_cfg.repeats = 2
     ex_run_cfg.over_time = True
-    # ex_run_cfg.debug = True
-    # ex_run_cfg.print_pandas = True
     ex_run_cfg.clear_cache = True
     ex_run_cfg.clear_history = True
     ex_run_cfg.time_event = "run 1"
     ex_run_cfg.use_optuna = True
-    # ex_run_cfg.time_src = str(datetime.now())
-
-    example_cat_float(ex_run_cfg)
 
-    time.sleep(1)
+    example_float_cat(ex_run_cfg)
 
     ex_run_cfg.clear_cache = False
     ex_run_cfg.clear_history = False
     ex_run_cfg.time_event = "run 2"
-    # ex_run_cfg.time_src = str(datetime.now())
 
-    example_cat_float(ex_run_cfg)
-    time.sleep(1)
+    example_float_cat(ex_run_cfg)
 
     ex_run_cfg.time_event = "run 3"
-    # ex_run_cfg.time_src = str(datetime.now())
-    example_cat_float(ex_run_cfg).plot()
+    return example_float_cat(ex_run_cfg)
+
+
+if __name__ == "__main__":
+    run_example_float_cat().show()
```

### Comparing `holobench-0.0.8/bencher/example/example_floats.py` & `holobench-0.2.0/bencher/example/example_floats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # pylint: disable=duplicate-code
 
 import pathlib
 
-from bencher import Bench, BenchRunCfg
+import bencher as bch
 
 # All the examples will be using the data structures and benchmark function defined in this file
 from bencher.example.benchmark_data import ExampleBenchCfgIn, ExampleBenchCfgOut, bench_function
 
 
-def example_floats(run_cfg: BenchRunCfg) -> Bench:
+def example_floats(run_cfg: bch.BenchRunCfg) -> bch.Bench:
     """Example of how to perform a parameter sweep for floating point variables
 
     Args:
         run_cfg (BenchRunCfg): configuration of how to perform the param sweep
 
     Returns:
         Bench: results of the parameter sweep
     """
-    bench = Bench("Bencher_Example_Floats", bench_function, ExampleBenchCfgIn)
+    bench = bch.Bench("Bencher_Example_Floats", bench_function, ExampleBenchCfgIn)
 
     rdmepath = pathlib.Path(__file__).parent.parent.parent / "README.md"
     with open(rdmepath, "r", encoding="utf-8") as file:
         readme = file.read()
 
     bench.plot_sweep(title="Intro", description=readme)
 
@@ -84,10 +84,8 @@
         run_cfg=run_cfg,
     )
 
     return bench
 
 
 if __name__ == "__main__":
-    ex_run_cfg = BenchRunCfg(repeats=10)
-
-    example_floats(ex_run_cfg).plot()
+    example_floats(bch.BenchRunCfg(repeats=10)).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_floats2D.py` & `holobench-0.2.0/bencher/example/example_floats2D.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # pylint: disable=duplicate-code
 import bencher as bch
-from bencher import Bench, BenchRunCfg
 
 # All the examples will be using the data structures and benchmark function defined in this file
 from bencher.example.benchmark_data import (
     ExampleBenchCfgIn,
     ExampleBenchCfgOut,
     NoiseDistribution,
     bench_function,
 )
 
 
-def example_floats2D(run_cfg: BenchRunCfg) -> Bench:
+def example_floats2D(run_cfg: bch.BenchRunCfg) -> bch.Bench:
     """Example of how to perform a 2D floating point parameter sweep
 
     Args:
         run_cfg (BenchRunCfg): configuration of how to perform the param sweep
 
     Returns:
         Bench: results of the parameter sweep
     """
-    bench = Bench(
+    bench = bch.Bench(
         "Bencher_Example_Floats",
         bench_function,
         ExampleBenchCfgIn,
         plot_lib=bch.PlotLibrary.default(),
     )
 
     cfg = ExampleBenchCfgIn()
@@ -97,10 +96,8 @@
         run_cfg=run_cfg,
     )
 
     return bench
 
 
 if __name__ == "__main__":
-    ex_run_cfg = BenchRunCfg()
-    ex_run_cfg.repeats = 1
-    example_floats2D(ex_run_cfg).plot()
+    example_floats2D(bch.BenchRunCfg(repeats=2)).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_hvplot_explorer.py` & `holobench-0.2.0/bencher/example/experimental/example_hvplot_explorer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # THIS IS NOT A WORKING EXAMPLE YET
 # pylint: disable=duplicate-code
-from bencher import Bench, BenchRunCfg, ExampleBenchCfgIn, ExampleBenchCfgOut, bench_function
 import hvplot
+import bencher as bch
+from bencher import ExampleBenchCfgIn, ExampleBenchCfgOut, bench_function
 
-bench = Bench("Bencher_Example_Simple", bench_function, ExampleBenchCfgIn)
+bench = bch.Bench("Bencher_Example_Simple", bench_function, ExampleBenchCfgIn)
 
 
 if __name__ == "__main__":
     bench_out = bench.plot_sweep(
         input_vars=[ExampleBenchCfgIn.param.theta, ExampleBenchCfgIn.param.offset],
         result_vars=[ExampleBenchCfgOut.param.out_sin],
         title="Float 1D Example",
@@ -23,15 +24,15 @@
             postprocess_fn = abs if cfg.postprocess_fn == PostprocessFn.absolute else negate_fn
 
             out.out_sin = postprocess_fn(offset + math.sin(cfg.theta) + noise)
             out.out_cos = postprocess_fn(offset + math.cos(cfg.theta) + noise)
             return out
         """,
         post_description="Here you can see the output plot of sin theta between 0 and pi.  In the tabs at the top you can also view 3 tabular representations of the data",
-        run_cfg=BenchRunCfg(
+        run_cfg=bch.BenchRunCfg(
             auto_plot=True,
             use_cache=False,
             repeats=2,
         ),
     )
 
     hvexplorer = hvplot.explorer(bench_out.get_dataframe())
```

### Comparing `holobench-0.0.8/bencher/example/example_interactive.py` & `holobench-0.2.0/bencher/example/experimental/example_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/example/example_kwargs.py` & `holobench-0.2.0/bencher/example/example_kwargs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 import math
 
-from bencher import (
-    Bench,
-    FloatSweep,
-    ParametrizedSweep,
-    ResultVar,
-    StringSweep,
-)
+import bencher as bch
 
 
 def bench_function(
     theta: float = 0,
     offset: float = 0,
     scale: float = 1.0,
     trig_func: str = "sin",
@@ -23,47 +17,47 @@
         output["voltage"] = offset + math.sin(theta) * scale
     elif trig_func == "cos":
         output["voltage"] = offset + math.cos(theta) * scale
 
     return output
 
 
-class InputCfg(ParametrizedSweep):
+class InputCfg(bch.ParametrizedSweep):
     """This class is used to define the default values and bounds of the variables to benchmark."""
 
-    theta = FloatSweep(
+    theta = bch.FloatSweep(
         default=0.0,
         bounds=[0.0, 6.0],
         doc="Input angle to the trig function",
         units="rad",
         samples=10,
     )
 
-    offset = FloatSweep(
+    offset = bch.FloatSweep(
         default=0.0,
         bounds=[0.0, 3.0],
         doc="Add an offset voltage to the result of the trig function",
         units="v",
         samples=5,
     )
 
-    trig_func = StringSweep(["sin", "cos"], doc="Select what trigonometric function use")
+    trig_func = bch.StringSweep(["sin", "cos"], doc="Select what trigonometric function use")
 
 
-class OutputVoltage(ParametrizedSweep):
-    voltage = ResultVar(units="v", doc="Output voltage")
+class OutputVoltage(bch.ParametrizedSweep):
+    voltage = bch.ResultVar(units="v", doc="Output voltage")
 
 
 if __name__ == "__main__":
     # pass the objective function you have defined to bencher.  The other examples pass the InputCfg type, but this benchmark function accepts a kwargs dictionary so you don't need to pass the inputCfg type.
-    bench = Bench("Bencher_Example_Categorical", bench_function)
+    bench = bch.Bench("Bencher_Example_Categorical", bench_function)
 
     # Bencher needs to know the metadata of the variable in order to automatically sweep and plot it, so it is passed by using param's metadata syntax.  InputCfg.param.* is how to access the metadata defined in the class description.
     bench.plot_sweep(
         input_vars=[InputCfg.param.theta, InputCfg.param.offset],
         result_vars=[OutputVoltage.param.voltage],
         title="Example with kwarg inputs and dict output",
         description=bench_function.__doc__,
     )
 
     # launch web server and view
-    bench.plot()
+    bench.show()
```

### Comparing `holobench-0.0.8/bencher/example/example_pareto.py` & `holobench-0.2.0/bencher/example/example_pareto.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,12 +31,8 @@
 This is a slightly unusual way of doing pareto optimisation as we are not using a typical multi-objective optimisation algorithm [TODO, add example].  Instead we are performing a grid search and looking at the resulting pareto plot.  The reason for doing a grid search instead of standard pareto optimisation is that we can produce more isolated plots of how an input affects an output which can help understanding of the parameter space.  Future examples will show how to use grid search to bootstrap further optimisation with a multi objective optimiser""",
         run_cfg=run_cfg,
     )
     return bench
 
 
 if __name__ == "__main__":
-    ex_run_cfg = BenchRunCfg()
-    ex_run_cfg.repeats = 1
-    ex_run_cfg.print_pandas = True
-    ex_run_cfg.over_time = True
-    example_pareto(ex_run_cfg).plot()
+    example_pareto(BenchRunCfg(over_time=True, print_pandas=True)).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_plot_library.py` & `holobench-0.2.0/bencher/example/example_plot_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,10 +60,8 @@
         plot_lib=plot_lib,
     )
 
     return bencher
 
 
 if __name__ == "__main__":
-    ex_run_cfg = bch.BenchRunCfg()
-    ex_run_cfg.repeats = 5
-    example_plot_library(ex_run_cfg).plot()
+    example_plot_library(bch.BenchRunCfg(repeats=5)).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_sample_cache.py` & `holobench-0.2.0/bencher/example/example_sample_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,10 +71,10 @@
         "Running the same benchmark but without checking the limit.  The benchmarking should load the previously calculated values and continue to finish calculating the values that were missed due to the crash"
     )
     ex_run_cfg.clear_sample_cache = False
     example_sample_cache(ex_run_cfg, trigger_crash=False)
 
     ex_run_cfg.repeats = 2
 
-    example_sample_cache(ex_run_cfg, trigger_crash=False).plot()
+    example_sample_cache(ex_run_cfg, trigger_crash=False).show()
 
     # see the test_sample_cache for a more detailed explanation of the mechanisms of the cache
```

### Comparing `holobench-0.0.8/bencher/example/example_sample_cache_context.py` & `holobench-0.2.0/bencher/example/example_sample_cache_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,8 @@
     # Both calls are calcuated becuase the tag is different so they don't hit the cache
     assert_call_counts(bencher, run_cfg, wrapper_calls=2, fn_calls=2, cache_calls=0)
 
     return bencher
 
 
 if __name__ == "__main__":
-    example_cache_context().plot()
+    example_cache_context().show()
```

### Comparing `holobench-0.0.8/bencher/example/example_simple.py` & `holobench-0.2.0/bencher/example/example_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,26 @@
 import random
 import time
 from datetime import datetime
 from enum import auto
 
 from strenum import StrEnum
 
-from bencher import (
-    Bench,
-    BenchRunCfg,
-    EnumSweep,
-    FloatSweep,
-    OptDir,
-    ParametrizedSweep,
-    ResultVar,
-)
+import bencher as bch
 
 
 # define a class with the output variables you want to benchmark. It must inherit from ParametrizedSweep (which inherits from param.Parametrized). Param is a python library that allows you to track metadata about parameters.  I would recommend reading at least the intro: https://param.holoviz.org/.  I have extended param with some extra metadata such is the units of the variable so that it can automaticaly be plotted.
-class OutputCfg(ParametrizedSweep):
+class OutputCfg(bch.ParametrizedSweep):
     """A class for defining what variables the benchmark function returns and metadata on those variables"""
 
     # Documenting the variable here with enables automatic summaries of what has been benchmarked.
     # This made up example uses accuracy as an example, but the variable defined here can be any metric that is important for the performance of a system.  You can also define the direction of the optimisation i.e. to minimise or maximise the metric.
-    accuracy = ResultVar(units="%", direction=OptDir.maximize, doc="The accuracy of the algorithm.")
+    accuracy = bch.ResultVar(
+        units="%", direction=bch.OptDir.maximize, doc="The accuracy of the algorithm."
+    )
 
 
 # Define categorical variables with enums that inherit from StrEnum.  In this example, its just an arbitrary set of categories that have an unknown influence on the metric you want to understand. In a real world case these would be a set of conditions or settings you are benchmarking
 class AlgoSetting(StrEnum):
     """Use enums to describe categorical input.  In this example they are given names that describe how they affect the function output, but in a real world example these will be some settings to an algorithm that you want to understand how they affect the metric you are trying to optimise."""
 
     # add some random noise to the output.  When your algorithm has noisy output it often is an indication that something is not quite right.  The graphs should show that you want to avoid the "noisy" setting in your algorithm
@@ -39,23 +33,23 @@
     # This is the setting with the best performance, and characterising that that is is the goal of the benchmarking
     optimum = auto()
 
     poor = auto()  # this setting results in poor performance
 
 
 # define a class with the input variables you want to benchmark.  It must inherit from ParametrizeSweep. This class defines a struct that is passed to the benchmark function.  The function must be pure and so we define it as a staticmethod that takes an InputCfg class and returns an OutputCfg class. By accepting and returning parametrized classes the metadata about what the relationship between the input and output are easy to track.
-class InputCfg(ParametrizedSweep):
+class InputCfg(bch.ParametrizedSweep):
     # The variables must be defined as one of the Sweep types, i.e, FloatSweep, IntSweep, EnumSweep from bencher.bench_vars
     # theta = FloatSweep(default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=30)
 
     # Define sweep variables by passing in an enum class name. The first element of the enum is the default by convention, but you can overrride the default in the constructor
-    algo_setting_enum = EnumSweep(AlgoSetting, default=AlgoSetting.poor)
+    algo_setting_enum = bch.EnumSweep(AlgoSetting, default=AlgoSetting.poor)
 
     # In this case there are no units so its marked as unitless or ul. You can define how many evenly distributed samples to sample the parameter with
-    algo_setting_float = FloatSweep(
+    algo_setting_float = bch.FloatSweep(
         default=0.0,
         bounds=[0.0, 6.0],
         doc="This represents a continuous input value to your function that affects the desired output in a way you want to characterise.",
         units="ul",
         samples=10,
     )
 
@@ -79,62 +73,62 @@
             case AlgoSetting.poor:
                 output.accuracy -= 20  # this setting results in poor performance
         return output
 
 
 if __name__ == "__main__":
     # pass the objective function you have defined to bencher.  This benchmark function can be reused for multiple sweeps.  You also need to pass the inputCfg to the bencher so that it can process the metadata about the input configuration.
-    bench = Bench("Bencher_Example_Categorical", InputCfg.bench_function, InputCfg)
+    bench = bch.Bench("Bencher_Example_Categorical", InputCfg.bench_function, InputCfg)
 
     # Bencher needs to know the metadata of the variable in order to automatically sweep and plot it, so it is passed by using param's metadata syntax.  InputCfg.param.* is how to access the metadata defined in the class description.  Unfortunately vscode autocomplete doesn't work with params metaclass machinery so you will need to look at the class definition to get a list of possible settings. Define what parameter you want to sweep over and the result variable you want to plot.  If you pass 1 input, it will perform a 1D sweep over that dimension and plot a line or a bar graph of the result (depending on if that variable on continuous or discrete).  In this example we are going to sweep the enum variable and record the accuracy.
     bench.plot_sweep(
         input_vars=[InputCfg.param.algo_setting_enum],
         result_vars=[OutputCfg.param.accuracy],
         title="Simple example 1D enum sweep",
         description="""Sample all the values in enum setting and record the resulting accuracy.  The algo_setting_float is not mentioned in the inputs and so it takes the default value that was set in the InputCfg class.  Repeats=10 so the benchmark function is called 10 times serially.  This is why the function must be pure, if a past call to the function affects the future call to the function (through global side effects) any statistics you calculate will not be correct. 
         """,
         post_description="Here you can see the affect of each setting on the output and the optimum is clearly the best.",
-        run_cfg=BenchRunCfg(repeats=10),
+        run_cfg=bch.BenchRunCfg(repeats=10),
     )
 
     # There is also a floating point input setting that affects the performance of the algorithm.  By passing only the float setting, the InputCfg class will use the default setting of the categorical value so you can understand the float setting in isolation
     bench.plot_sweep(
         input_vars=[InputCfg.param.algo_setting_float],
         result_vars=[OutputCfg.param.accuracy],
         title="Simple example 1D float sweep",
         description="""Perform a 1D sweep over the continuous variable algo_setting_float taking sweep the bounds and number of samples from the InputCfg class definition.  The algo_setting_enum is not mentioned in the inputs and so it takes the default value that was set in the InputCfg class.  Repeats=10 so the benchmark function is called 10 times serially.  
         """,
         post_description="The plot shows the output is affected by the float input in a continuous way with a peak around 1.5",
-        run_cfg=BenchRunCfg(repeats=10),
+        run_cfg=bch.BenchRunCfg(repeats=10),
     )
 
     # This sweep is a combination of the previous two sweeps
     bench.plot_sweep(
         input_vars=[
             InputCfg.param.algo_setting_enum,
             InputCfg.param.algo_setting_float,
         ],
         result_vars=[OutputCfg.param.accuracy],
         title="Simple example 2D sweep",
         description="""Perform a 2D sweep over the enum and continuous variable to see how they act together.  Here the setting use_optuna=True so additional graphs a plotted at the end. 
         """,
         post_description="In this example function the two input settings combine in a linear and predictable way, so the best combination of settings is enum = AlgoSetting.optimum and float = 1.33.  Setting use_optuna=True adds a plot of how much each input parameter affects the metric and a printout of the best parameter values found during the sweep.  If the value for repeat is high it is an indication there is something wrong with your benchmark function. The repeat should have no affect on the value of the function if calls to the function are independent.  This can be useful to detect undesired side effects in your code",
-        run_cfg=BenchRunCfg(repeats=10, use_optuna=True),
+        run_cfg=bch.BenchRunCfg(repeats=10, use_optuna=True),
     )
 
     # In the last example we track the value of the categorical values over time.
     # run this code in a loop twice to simulate calling the benchmarking function at different times.  The most common use case for tracking over time would be run once a day during nightly benchmarking
     bench.plot_sweep(
         input_vars=[InputCfg.param.algo_setting_enum],
         result_vars=[OutputCfg.param.accuracy],
         const_vars=[(InputCfg.param.algo_setting_float, 1.33)],
         title="Simple example 1D sweep over time",
         description="""Once you have found the optimal settings for your algorithm you want to make sure that the performance is not lost over time.  You can set variables to a constant value and in this case the float value is set to its optimum value.  The first time this function is run only the results from sweeping the categorical value is plotted (the same as example 1), but the second time it is run a graph the values over time is shown. [Run the code again if you don't see a graph over time]. If the graphs over time shows long term changes (not just noise), it indicate there is another external factor that is affecting your performace over time, i.e. dependencies changing, physical degradation of equipment, an unnoticed bug from a pull request etc...
 
         This shows the basic features of bencher.  These examples are purposefully simplified to demonstrate its features in isolation and don't reeally show the real advantages of bencher.  If you only have a few inputs and outputs its not that complicated to throw together some plots of performance.  The power of bencher is that when you have a system with many moving parts that all interact with eachother, teasing apart those influences becomes much harder because the parameter spaces combine quite quickly into a high dimensional mess. Bencher makes it easier to experiment with different combination of inputs to gain an intuition of the system performance. Bencher can plot up to 6D input natively and you can add custom plots if you have exotic data types or state spaces [WIP]. 
         """,
         post_description="",
-        run_cfg=BenchRunCfg(repeats=10, over_time=True, clear_history=False),
+        run_cfg=bch.BenchRunCfg(repeats=10, over_time=True, clear_history=False),
     )
 
     # launch web server and view
-    bench.plot()
+    bench.show()
```

### Comparing `holobench-0.0.8/bencher/example/example_simple_bool.py` & `holobench-0.2.0/bencher/example/example_simple_bool.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 
 if __name__ == "__main__":
     ex_run_cfg = bch.BenchRunCfg()
     ex_run_cfg.repeats = 3
     ex_run_cfg.print_pandas = True
     ex_run_cfg.over_time = False
 
-    example_1D_bool(ex_run_cfg).plot()
+    example_1D_bool(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_simple_cat.py` & `holobench-0.2.0/bencher/example/example_simple_cat.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
 if __name__ == "__main__":
     ex_run_cfg = bch.BenchRunCfg()
     ex_run_cfg.repeats = 10
     ex_run_cfg.print_pandas = True
     ex_run_cfg.over_time = True
 
-    example_1D_cat(ex_run_cfg).plot()
+    example_1D_cat(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_simple_float.py` & `holobench-0.2.0/bencher/example/example_simple_float.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 if __name__ == "__main__":
     ex_run_cfg = BenchRunCfg()
     ex_run_cfg.repeats = 5
     ex_run_cfg.print_pandas = True
     ex_run_cfg.over_time = True
 
-    example_1D_float(ex_run_cfg).plot()
+    example_1D_float(ex_run_cfg).show()
```

### Comparing `holobench-0.0.8/bencher/example/example_template.py` & `holobench-0.2.0/bencher/example/experimental/example_template.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/example/example_time_event.py` & `holobench-0.2.0/bencher/example/example_time_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,15 @@
         result_vars=[ExampleBenchCfgOut.param.out_cos],
         description=example_time_event.__doc__,
         run_cfg=run_cfg,
     )
     return bencher
 
 
-if __name__ == "__main__":
-    ex_run_cfg = BenchRunCfg()
+def run_example_time_event(ex_run_cfg):
     ex_run_cfg.repeats = 1
     ex_run_cfg.print_pandas = True
     ex_run_cfg.over_time = True
 
     ex_run_cfg.clear_cache = True
     ex_run_cfg.clear_history = True
 
@@ -45,8 +44,12 @@
     ex_run_cfg.clear_history = False
     ex_run_cfg.time_event = "_second_event"
     example_time_event(ex_run_cfg)
 
     ex_run_cfg.time_event = (
         "*third_event has a very very long label to demonstrate automatic text wrapping"
     )
-    example_time_event(ex_run_cfg).plot()
+    return example_time_event(ex_run_cfg)
+
+
+if __name__ == "__main__":
+    run_example_time_event.show()
```

### Comparing `holobench-0.0.8/bencher/example/example_vector.py` & `holobench-0.2.0/bencher/example/experimental/example_vector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""Example on how to sweep over function with vector outputs"""
+# """Example on how to sweep over function with vector outputs"""
 
-from math import cos, sin
+# from math import cos, sin
 
-import numpy as np
+# import numpy as np
 
-import bencher as bch
+# import bencher as bch
 
 
-class OffsetCfg(bch.ParametrizedSweep):
-    """A class for describing which parameters to sweep"""
-
-    dc_offset = bch.FloatSweep(
-        default=0,
-        bounds=[0.0, 2.0],
-        samples=4,
-        units="v",
-        doc="DC offset to add to the result of the signal",
-    )
-    phase_offset = bch.FloatSweep(
-        default=0,
-        bounds=[0.0, 3.14],
-        samples=4,
-        units="rad",
-        doc="phase offset that is added to the input before passing to the trig function",
-    )
-
-
-class SweepResult(bch.ParametrizedSweep):
-    """A class to describe the vector outputs of the benchmark function"""
-
-    sin_sweep = bch.ResultList(
-        index_name="time", index_units="s", units="v", doc="A list of values from a sin function"
-    )
-    cos_sweep = bch.ResultList(
-        index_name="time", index_units="s", units="v", doc="A list of values from a cos function"
-    )
-
-
-def sin_sweep(cfg: OffsetCfg) -> SweepResult:
-    """A function that returns vector outputs of the sin and cos functions
-
-    Args:
-        cfg (OffsetCfg): Options for phase and dc offset
-
-    Returns:
-        SweepResult: vectors with sin and cos results
-    """
-    res = SweepResult()
-    print(type(res.sin_sweep))
-    for i in np.arange(0, 6.28, 0.02):
-        res.sin_sweep.append(sin(i + cfg.phase_offset) + cfg.dc_offset, i)
-        # res.sin_sweep.indices.append(i)
-    for i in np.arange(0, 3.28, 0.02):
-        res.cos_sweep.append(cos(i + cfg.phase_offset) + cfg.dc_offset, i)
-        # res.cos_sweep.indices.append(i)
-    return res
-
-
-def example_vector() -> bch.Bench:
-    """Example on how to sweep over function with vector outputs"""
-    bencher = bch.Bench("vector output example", sin_sweep, OffsetCfg)
-
-    bencher.plot_sweep(
-        title="Sweep DC offset",
-        input_vars=[OffsetCfg.param.dc_offset],
-        result_vars=[SweepResult.param.sin_sweep, SweepResult.param.cos_sweep],
-        description="""This is an example of how to sample function that return a vector of unknown or varying size. In this example it returns the output of the sin and cos function for varying angles and a range of dc offsets""",
-        post_description="""The output shows stack of sin and cos functions as the dc offset increases""",
-    )
-
-    bencher.plot_sweep(
-        title="Sweep phase offset",
-        input_vars=[OffsetCfg.param.phase_offset],
-        result_vars=[SweepResult.param.sin_sweep, SweepResult.param.cos_sweep],
-        description="""This is an example of how to sample function that return a vector of unknown or varying size. In this example it returns the output of the sin and cos function for varying angles and a range of phase offsets""",
-        post_description="""The output shows different phases of the sin and cos functions""",
-    )
+# class OffsetCfg(bch.ParametrizedSweep):
+#     """A class for describing which parameters to sweep"""
+
+#     dc_offset = bch.FloatSweep(
+#         default=0,
+#         bounds=[0.0, 2.0],
+#         samples=4,
+#         units="v",
+#         doc="DC offset to add to the result of the signal",
+#     )
+#     phase_offset = bch.FloatSweep(
+#         default=0,
+#         bounds=[0.0, 3.14],
+#         samples=4,
+#         units="rad",
+#         doc="phase offset that is added to the input before passing to the trig function",
+#     )
+
+
+# class SweepResult(bch.ParametrizedSweep):
+#     """A class to describe the vector outputs of the benchmark function"""
+
+#     sin_sweep = bch.ResultList(
+#         index_name="time", index_units="s", units="v", doc="A list of values from a sin function"
+#     )
+#     cos_sweep = bch.ResultList(
+#         index_name="time", index_units="s", units="v", doc="A list of values from a cos function"
+#     )
+
+
+# def sin_sweep(cfg: OffsetCfg) -> SweepResult:
+#     """A function that returns vector outputs of the sin and cos functions
+
+#     Args:
+#         cfg (OffsetCfg): Options for phase and dc offset
+
+#     Returns:
+#         SweepResult: vectors with sin and cos results
+#     """
+#     res = SweepResult()
+#     print(type(res.sin_sweep))
+#     for i in np.arange(0, 6.28, 0.02):
+#         res.sin_sweep.append(sin(i + cfg.phase_offset) + cfg.dc_offset, i)
+#         # res.sin_sweep.indices.append(i)
+#     for i in np.arange(0, 3.28, 0.02):
+#         res.cos_sweep.append(cos(i + cfg.phase_offset) + cfg.dc_offset, i)
+#         # res.cos_sweep.indices.append(i)
+#     return res
+
+
+# def example_vector() -> bch.Bench:
+#     """Example on how to sweep over function with vector outputs"""
+#     bencher = bch.Bench("vector output example", sin_sweep, OffsetCfg)
+
+#     bencher.plot_sweep(
+#         title="Sweep DC offset",
+#         input_vars=[OffsetCfg.param.dc_offset],
+#         result_vars=[SweepResult.param.sin_sweep, SweepResult.param.cos_sweep],
+#         description="""This is an example of how to sample function that return a vector of unknown or varying size. In this example it returns the output of the sin and cos function for varying angles and a range of dc offsets""",
+#         post_description="""The output shows stack of sin and cos functions as the dc offset increases""",
+#     )
+
+#     bencher.plot_sweep(
+#         title="Sweep phase offset",
+#         input_vars=[OffsetCfg.param.phase_offset],
+#         result_vars=[SweepResult.param.sin_sweep, SweepResult.param.cos_sweep],
+#         description="""This is an example of how to sample function that return a vector of unknown or varying size. In this example it returns the output of the sin and cos function for varying angles and a range of phase offsets""",
+#         post_description="""The output shows different phases of the sin and cos functions""",
+#     )
 
-    return bencher
+#     return bencher
 
 
-if __name__ == "__main__":
-    example_vector().plot()
+# if __name__ == "__main__":
+#     example_vector().plot()
```

### Comparing `holobench-0.0.8/bencher/example/example_workflow.py` & `holobench-0.2.0/bencher/example/example_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,8 +182,8 @@
 
 if __name__ == "__main__":
     ex_run_cfg = bch.BenchRunCfg()
 
     bench_ex = example_floats2D_workflow(ex_run_cfg)
     example_floats3D_workflow(ex_run_cfg, bench_ex)
 
-    bench_ex.plot()
+    bench_ex.show()
```

### Comparing `holobench-0.0.8/bencher/example/hv_bool_bug.py` & `holobench-0.2.0/bencher/example/experimental/hv_bool_bug.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/optuna_conversions.py` & `holobench-0.2.0/bencher/optuna_conversions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import List
 
 import numpy as np
 import optuna
 import panel as pn
 import param
-from optuna.visualization import plot_param_importances, plot_pareto_front
+from optuna.visualization import (
+    plot_param_importances,
+    plot_pareto_front,
+    plot_optimization_history,
+)
 
 from bencher.bench_cfg import BenchCfg
-from bencher.bench_vars import (
-    BoolSweep,
-    EnumSweep,
-    FloatSweep,
-    IntSweep,
-    OptDir,
-    ParametrizedSweep,
-    StringSweep,
-    TimeEvent,
-    TimeSnapshot,
-)
+
+
+from bencher.variables.inputs import IntSweep, FloatSweep, StringSweep, EnumSweep, BoolSweep
+from bencher.variables.time import TimeSnapshot, TimeEvent
+from bencher.variables.results import OptDir
+
+from bencher.variables.parametrised_sweep import ParametrizedSweep
 
 
 def optuna_grid_search(bench_cfg: BenchCfg) -> optuna.Study:
     """use optuna to perform a grid search
 
     Args:
         bench_cfg (BenchCfg): setting for grid search
@@ -41,14 +41,40 @@
         sampler=optuna.samplers.GridSampler(search_space),
         directions=directions,
         study_name=bench_cfg.title,
     )
     return study
 
 
+def to_optuna(worker, bench_cfg: BenchCfg, n_trials=100, sampler=optuna.samplers.TPESampler()):
+    directions = []
+    for rv in bench_cfg.result_vars:
+        if rv.direction != OptDir.none:
+            directions.append(rv.direction)
+
+    study = optuna.create_study(sampler=sampler, directions=directions, study_name=bench_cfg.title)
+
+    study.add_trials(
+        bench_results_to_optuna_trials(bench_cfg, True)
+    )  # add already calculated results
+
+    def wrapped(trial):
+        kwargs = {}
+        for iv in bench_cfg.input_vars:
+            kwargs[iv.name] = sweep_var_to_suggest(iv, trial)
+        result = worker(**kwargs)
+        output = []
+        for rv in bench_cfg.result_vars:
+            output.append(result[rv.name])
+        return tuple(output)
+
+    study.optimize(wrapped, n_trials=n_trials)
+    return study
+
+
 def extract_study_to_dataset(study: optuna.Study, bench_cfg: BenchCfg) -> BenchCfg:
     """Extract an optuna study into an xarray dataset for easy plotting
 
     Args:
         study (optuna.Study): The result of a gridsearch
         bench_cfg (BenchCfg): Options for the grid search
 
@@ -223,17 +249,15 @@
 
     if iv_type == IntSweep:
         return trial.suggest_int(iv.name, iv.bounds[0], iv.bounds[1])
     if iv_type == FloatSweep:
         return trial.suggest_float(iv.name, iv.bounds[0], iv.bounds[1])
     if iv_type in (EnumSweep, StringSweep):
         return trial.suggest_categorical(iv.name, iv.objects)
-    if iv_type == TimeSnapshot:
-        pass  # optuna does not like time
-    if iv_type == TimeEvent:
+    if iv_type in (TimeSnapshot, TimeEvent):
         pass  # optuna does not like time
     if iv_type == BoolSweep:
         return trial.suggest_categorical(iv.name, [True, False])
     raise ValueError(f"This input type {iv_type} is not supported")
 
 
 def cfg_from_optuna_trial(
@@ -243,15 +267,15 @@
     for iv in bench_cfg.input_vars:
         cfg.param.set_param(iv.name, sweep_var_to_suggest(iv, trial))
     for mv in bench_cfg.meta_vars:
         sweep_var_to_suggest(mv, trial)
     return cfg
 
 
-def bench_cfg_to_study(bench_cfg: BenchCfg, include_meta: bool) -> optuna.Study:
+def bench_results_to_optuna_trials(bench_cfg: BenchCfg, include_meta: bool = True) -> optuna.Study:
     """Convert an xarray dataset to an optuna study so optuna can further optimise or plot the statespace
 
     Args:
         bench_cfg (BenchCfg): benchmark config to convert
 
     Returns:
         optuna.Study: optuna description of the study
@@ -293,19 +317,39 @@
         trials.append(
             optuna.trial.create_trial(
                 params=params,
                 distributions=distributions,
                 values=values,
             )
         )
+    return trials
+
 
+def bench_cfg_to_study(bench_cfg: BenchCfg, include_meta: bool) -> optuna.Study:
+    trials = bench_results_to_optuna_trials(bench_cfg, include_meta)
     study = optuna_grid_search(bench_cfg)
     optuna.logging.set_verbosity(optuna.logging.CRITICAL)
     import warnings
 
     # /usr/local/lib/python3.10/dist-packages/optuna/samplers/_grid.py:224: UserWarning: over_time contains a value with the type of <class 'pandas._libs.tslibs.timestamps.Timestamp'>, which is not supported by `GridSampler`. Please make sure a value is `str`, `int`, `float`, `bool` or `None` for persistent storage.
 
     # this is not disabling the warning
     warnings.filterwarnings(action="ignore", category=UserWarning)
     # remove optuna gridsearch warning as we are not using their gridsearch because it has the most inexplicably terrible performance I have ever seen in my life. How can a for loop of 400 iterations start out with 100ms per loop and increase to greater than a 1000ms after 250ish iterations!?!?!??!!??!
     study.add_trials(trials)
     return study
+
+
+def summarise_study(study: optuna.study.Study) -> None:
+    row = pn.Column(name="Optimisation Results")
+    row.append(plot_optimization_history(study))
+    row.append(plot_param_importances(study))
+    try:
+        row.append(plot_pareto_front(study))
+    except Exception:
+        pass
+
+    row.append(
+        pn.pane.Markdown(f"```\nBest value: {study.best_value}\nParams: {study.best_params}```")
+    )
+
+    return row
```

### Comparing `holobench-0.0.8/bencher/plotting/plot_collection.py` & `holobench-0.2.0/bencher/plotting/plot_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import inspect
 import logging
 from typing import Callable, List
 
 import panel as pn
 
 from bencher.bench_cfg import BenchCfg, PltCntCfg
-from bencher.bench_vars import ParametrizedSweep
 from bencher.plotting.plot_filter import PlotInput, PlotProvider
+from bencher.variables.parametrised_sweep import ParametrizedSweep
 
 
 class PlotCollection:
     """A set of plot providers with filters that determine if they are able to plot the type of data in the results.  The plot collection can be customised with user defined plots or ones already defined by bencher. You can also take predefine PlotCollections defined in PlotLibrary and add or remove specific plots that you want to override.  The add and remove function accept strings, or StrEnums (which are equivalent to strings)"""
 
     def __init__(self) -> None:
         """A PlotCollection has a dictionary of function_name:function_pointer which are all the available types of plot. The plotters variable contains an ordered dictionary of the active plotting functions"""
```

### Comparing `holobench-0.0.8/bencher/plotting/plot_filter.py` & `holobench-0.2.0/bencher/plotting/plot_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 from bencher.bench_cfg import BenchCfg, PltCntCfg
-from bencher.bench_vars import ParametrizedSweep
+from bencher.variables.parametrised_sweep import ParametrizedSweep
 
 
 class VarRange:
     def __init__(self, lower_bound: int = 0, upper_bound: int = -1) -> None:
         """A VarRange represents the bounded and unbounded ranges of integers.  This class is used to define filters for various variable types.  For example by defining cat_var = VarRange(0,0), calling matches(0) will return true, but any other integer will not match.  You can also have unbounded ranges for example VarRange(2,None) will match to 2,3,4... up to infinity. for By default the lower and upper bounds are set to -1 so so that no matter what value is passsed to matches() will return false.  Matches only takes 0 and positive integers.
 
         Args:
```

### Comparing `holobench-0.0.8/bencher/plotting/plot_library.py` & `holobench-0.2.0/bencher/plotting/plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/plotting/plot_types.py` & `holobench-0.2.0/bencher/plotting/plot_types.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/plotting/plots/catplot.py` & `holobench-0.2.0/bencher/plotting/plots/catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/plotting/plots/heatmap.py` & `holobench-0.2.0/bencher/plotting/plots/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import panel as pn
 import plotly.express as px
 import xarray as xr
 
 import hvplot.xarray  # noqa pylint: disable=unused-import
 
 
-from bencher.bench_vars import ParametrizedSweep
 from bencher.plotting.plot_filter import PlotFilter, PlotInput, VarRange
 from bencher.plotting.plot_types import PlotTypes
+from bencher.variables.parametrised_sweep import ParametrizedSweep
 
 
 class Heatmap:
     # shared plot filter for 2d plots
     plot_filter = PlotFilter(
         float_range=VarRange(2, 2),
         cat_range=VarRange(0, 0),
```

### Comparing `holobench-0.0.8/bencher/plotting/plots/hv_interactive.py` & `holobench-0.2.0/bencher/plotting/plots/hv_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/plotting/plots/lineplot.py` & `holobench-0.2.0/bencher/plotting/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/plotting/plots/scatterplot.py` & `holobench-0.2.0/bencher/plotting/plots/scatterplot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Optional
 import matplotlib.pyplot as plt
 import panel as pn
 import seaborn as sns
-from typing import Optional
+import plotly.express as px
 
 from bencher.plotting.plot_filter import PlotFilter, PlotInput, VarRange
 from bencher.plotting.plot_types import PlotTypes
 from bencher.plotting_functions import wrap_long_time_labels
 
 
 class Scatter:
@@ -41,7 +42,40 @@
             else:
                 h = sns.jointplot(df, x=names[0], y=names[1])
 
             h.set_axis_labels(f"{names[0]} [{pl_in.rv.units}]", f"{names[1]} [{pl_in.rv.units}]")
             plt.tight_layout()
             return pn.panel(h.fig, name=PlotTypes.scatter2D_sns)
         return None
+
+    def plot_scatter3D_px(self, pl_in: PlotInput) -> pn.pane.Plotly:
+        """Given a benchCfg generate a 3D scatter plot with plotly express
+
+        Args:
+            bench_cfg (BenchCfg): description of benchmark
+            rv (ParametrizedSweep): result variable to plot
+
+        Returns:
+            pn.pane.Plotly: A 3d scatter plot as a holoview in a pane
+        """
+
+        bench_cfg = pl_in.bench_cfg
+        rv = pl_in.rv
+
+        bench_cfg = wrap_long_time_labels(bench_cfg)
+
+        df = bench_cfg.get_dataframe()
+
+        names = rv.index_names()  # get the column names of the vector result
+
+        if bench_cfg.input_vars:
+            color = bench_cfg.input_vars[0].name
+        else:
+            color = None
+
+        if bench_cfg.over_time:
+            if len(names) < 3:  # only a 2d vector result so use the time axis as the third point
+                names.insert(0, bench_cfg.iv_time[0].name)
+
+        return px.scatter_3d(
+            df, x=names[0], y=names[1], z=names[2], color=color, symbol=color, size_max=2
+        )
```

### Comparing `holobench-0.0.8/bencher/plotting/plots/tables.py` & `holobench-0.2.0/bencher/plotting/plots/tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/bencher/plotting/plots/volume.py` & `holobench-0.2.0/bencher/plotting/plots/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import panel as pn
 import plotly.graph_objs as go
 import logging
 import xarray as xr
 
 from bencher.bench_cfg import BenchCfg
-from bencher.bench_vars import ParametrizedSweep
+from bencher.variables.parametrised_sweep import ParametrizedSweep
+
 from bencher.plotting.plot_filter import PlotFilter, PlotInput, VarRange, PltCntCfg
 from bencher.plt_cfg import PltCfgBase
 from bencher.plotting.plot_types import PlotTypes
 
 from bencher.plotting_functions import wrap_long_time_labels
```

### Comparing `holobench-0.0.8/bencher/plt_cfg.py` & `holobench-0.2.0/bencher/plt_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 from copy import deepcopy
 
 import panel as pn
 import seaborn as sns
 
 import bencher.plotting_functions as plt_func
 from bencher.bench_cfg import BenchCfg, PltCfgBase, PltCntCfg, describe_benchmark
-from bencher.bench_vars import ParametrizedSweep, ResultVec, ResultVar
 from bencher.optuna_conversions import collect_optuna_plots
+from bencher.variables.parametrised_sweep import ParametrizedSweep
+
+from bencher.variables.results import ResultVar, ResultVec
+
 import xarray as xr
 
 
 class BenchPlotter:
     @staticmethod
     def plot(bench_cfg: BenchCfg, main_tab=None, append_cols=None) -> pn.pane:
         """Given the dataset result of a benchmark run, automatically dedeuce how to plot the data based on the types of variables that were sampled
@@ -21,97 +24,96 @@
 
         Returns:
             pn.pane: A panel containing plot results
         """
 
         if main_tab is None:
             main_tab = pn.Tabs(tabs_location="left")
+        if bench_cfg.auto_plot:
+            if len(bench_cfg.result_vars) == 0:
+                tabs = pn.Column(name=bench_cfg.title)
+                tabs.append(pn.pane.Markdown(f"{bench_cfg.description}"))
 
-        if len(bench_cfg.result_vars) == 0:
-            tabs = pn.Column(name=bench_cfg.title)
-            tabs.append(pn.pane.Markdown(f"{bench_cfg.description}"))
-
-        else:
-            plot_cols = pn.Column(name="Plots View")
-            plot_cols.append(pn.pane.Markdown(f"# {bench_cfg.title}\n{bench_cfg.description}"))
-            benmark_str = describe_benchmark(bench_cfg)
-            plot_cols.append(pn.pane.Markdown(f"{benmark_str}"))
-            if bench_cfg.over_time:
-                if len(bench_cfg.ds.coords["over_time"]) > 1:
-                    plot_cols.append(pn.pane.Markdown("## Results Over Time"))
-                    plot_cols.append(BenchPlotter.plot_results_row(bench_cfg))
-                else:
-                    plot_cols.append(
-                        pn.pane.Markdown(
-                            "Results over time needs at least 2 time snapshots to plot"
+            else:
+                plot_cols = pn.Column(name="Plots View")
+                plot_cols.append(pn.pane.Markdown(f"# {bench_cfg.title}\n{bench_cfg.description}"))
+                benmark_str = describe_benchmark(bench_cfg)
+                plot_cols.append(pn.pane.Markdown(f"{benmark_str}"))
+                if bench_cfg.over_time:
+                    if len(bench_cfg.ds.coords["over_time"]) > 1:
+                        plot_cols.append(pn.pane.Markdown("## Results Over Time"))
+                        plot_cols.append(BenchPlotter.plot_results_row(bench_cfg))
+                    else:
+                        plot_cols.append(
+                            pn.pane.Markdown(
+                                "Results over time needs at least 2 time snapshots to plot"
+                            )
                         )
-                    )
 
-            plot_cols.append(pn.pane.Markdown("## Most Recent Results"))
-            if bench_cfg.over_time:
-                bench_deep = deepcopy(bench_cfg)  # TODO do this in the future without copying
-                bench_deep.over_time = False
-                bench_deep.iv_time = []
-                last_time = bench_deep.ds.coords["over_time"][-1]
-                try:
-                    bench_deep.ds = bench_deep.ds.sel(over_time=last_time)
-                    plot_cols.append(BenchPlotter.plot_results_row(bench_deep))
-                except ValueError as e:
-                    warning = f"failed to load historical data: {e}"
-                    plot_cols.append(pn.pane.Markdown(warning))
-                    logging.warning(warning)
+                plot_cols.append(pn.pane.Markdown("## Most Recent Results"))
+                if bench_cfg.over_time:
+                    bench_deep = deepcopy(bench_cfg)  # TODO do this in the future without copying
+                    bench_deep.over_time = False
+                    bench_deep.iv_time = []
+                    last_time = bench_deep.ds.coords["over_time"][-1]
+                    try:
+                        bench_deep.ds = bench_deep.ds.sel(over_time=last_time)
+                        plot_cols.append(BenchPlotter.plot_results_row(bench_deep))
+                    except ValueError as e:
+                        warning = f"failed to load historical data: {e}"
+                        plot_cols.append(pn.pane.Markdown(warning))
+                        logging.warning(warning)
 
-            else:
-                plot_cols.append(BenchPlotter.plot_results_row(bench_cfg))
+                else:
+                    plot_cols.append(BenchPlotter.plot_results_row(bench_cfg))
+
+                if bench_cfg.use_optuna:
+                    plot_cols.extend(collect_optuna_plots(bench_cfg))
 
-            if bench_cfg.use_optuna:
-                plot_cols.extend(collect_optuna_plots(bench_cfg))
+                if append_cols is not None:
+                    plot_cols.extend(append_cols)
+                # plot_cols.append(pn.Column(pn.Row()))#attempt to add spacer to stop overlapping but does not work todo
 
-            if append_cols is not None:
-                plot_cols.extend(append_cols)
-            # plot_cols.append(pn.Column(pn.Row()))#attempt to add spacer to stop overlapping but does not work todo
-
-            plot_cols.append(pn.pane.Markdown(f"{bench_cfg.post_description}"))
-
-            tabs = pn.Tabs(plot_cols, name=bench_cfg.title)
-
-            if bench_cfg.serve_xarray:
-                tabs.append(
-                    pn.Column(
-                        pn.pane.Markdown(
-                            """This page shows the with the inputs of the parameter sweep and the results in its native N-D xarray dataset format."""
-                        ),
-                        bench_cfg.ds,
-                        name="Xarray Dataset View",
+                plot_cols.append(pn.pane.Markdown(f"{bench_cfg.post_description}"))
+
+                tabs = pn.Tabs(plot_cols, name=bench_cfg.title)
+
+                if bench_cfg.serve_xarray:
+                    tabs.append(
+                        pn.Column(
+                            pn.pane.Markdown(
+                                """This page shows the with the inputs of the parameter sweep and the results in its native N-D xarray dataset format."""
+                            ),
+                            bench_cfg.ds,
+                            name="Xarray Dataset View",
+                        )
                     )
-                )
-            if bench_cfg.serve_pandas:
-                tabs.append(
-                    pn.Column(
-                        pn.pane.Markdown(
-                            """This page shows the with the inputs of the parameter sweep and the results as a pandas multiindex."""
-                        ),
-                        bench_cfg.ds.to_dataframe(),
-                        name="Pandas Dataframe MultiIndex View",
+                if bench_cfg.serve_pandas:
+                    tabs.append(
+                        pn.Column(
+                            pn.pane.Markdown(
+                                """This page shows the with the inputs of the parameter sweep and the results as a pandas multiindex."""
+                            ),
+                            bench_cfg.ds.to_dataframe(),
+                            name="Pandas Dataframe MultiIndex View",
+                        )
                     )
-                )
 
-                tabs.append(
-                    pn.Column(
-                        pn.pane.Markdown(
-                            """This page shows the with the inputs of the parameter sweep and the results as a flattened padas dataframe."""
-                        ),
-                        bench_cfg.get_dataframe(),
-                        name="Pandas Dataframe Flattened View",
+                    tabs.append(
+                        pn.Column(
+                            pn.pane.Markdown(
+                                """This page shows the with the inputs of the parameter sweep and the results as a flattened padas dataframe."""
+                            ),
+                            bench_cfg.get_dataframe(),
+                            name="Pandas Dataframe Flattened View",
+                        )
                     )
-                )
 
-        main_tab.append(tabs)
+            main_tab.append(tabs)
         main_tab.servable()
-
         return main_tab
 
     @staticmethod
     def plot_results_row(bench_cfg: BenchCfg) -> pn.Row:
         """Given a BenchCfg, plot each result variable and add to a panel row
 
         Args:
@@ -210,28 +212,15 @@
                 sns_cfg.marker = "."
             if plt_cnt_cfg.float_cnt == 0:
                 sns_cfg = BenchPlotter.plot_float_cnt_0(sns_cfg, plt_cnt_cfg)
             elif plt_cnt_cfg.float_cnt == 1:
                 sns_cfg = BenchPlotter.plot_float_cnt_1(sns_cfg, plt_cnt_cfg)
             sns_cfg = BenchPlotter.get_axes_and_title(rv, sns_cfg, plt_cnt_cfg)
             surf_col.append(plt_func.plot_sns(bench_cfg, rv, sns_cfg))
-        else:
-            if plt_cnt_cfg.float_cnt == 2:
-                xr_cfg = BenchPlotter.plot_float_cnt_2(plt_cnt_cfg, rv, bench_cfg.debug)
-                if plt_cnt_cfg.cat_cnt == 0:
-                    surf_col.append(plt_func.plot_surface_plotly(bench_cfg, rv, xr_cfg))
-                else:
-                    try:
-                        surf_col.append(plt_func.plot_surface_holo(bench_cfg, rv, xr_cfg))
-                    except (TypeError, KeyError) as e:
-                        surf_col.append(
-                            pn.pane.Markdown(
-                                f"3D (cat,float,cat) inputs -> (float) output plots are not supported yet, error:{e}"
-                            )
-                        )
+
         return surf_col
 
     @staticmethod
     def axis_mapping(cat_axis_order, sns_cfg: PltCfgBase, plt_cnt_cfg: PltCntCfg) -> PltCfgBase:
         """A function for determining the plot settings if there are 0 float variable and updates the PltCfgBase
 
         Args:
```

### Comparing `holobench-0.0.8/package.xml` & `holobench-0.2.0/package.xml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/setup.py` & `holobench-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/plots/test_catplot.py` & `holobench-0.2.0/test/plots/test_catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/plots/test_plots_common.py` & `holobench-0.2.0/test/plots/test_plots_common.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/plots/test_tables.py` & `holobench-0.2.0/test/plots/test_tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/test_bench_examples.py` & `holobench-0.2.0/test/test_bench_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import unittest
-import pytest
-from bencher import BenchRunCfg
+import bencher as bch
 from bencher.example.example_categorical import example_categorical
 from bencher.example.example_floats import example_floats
 from bencher.example.example_floats2D import example_floats2D
 from bencher.example.example_pareto import example_pareto
 from bencher.example.example_simple_cat import example_1D_cat
 from bencher.example.example_simple_float import example_1D_float
-from bencher.example.example_persistent import example_persistent
-from bencher.example.example_float_cat import example_cat_float
-from bencher.example.example_time_event import example_time_event
+from bencher.example.example_float_cat import run_example_float_cat
+from bencher.example.example_time_event import run_example_time_event
 from bencher.example.example_float3D import example_floats3D
 from bencher.example.example_float3D_cone import example_cone
 from bencher.example.example_custom_sweep import example_custom_sweep
 from bencher.example.example_workflow import example_floats2D_workflow, example_floats3D_workflow
-from bencher.example.example_vector import example_vector
 from bencher.example.example_plot_library import example_plot_library
+from bencher.example.example_holosweep_tap import example_holosweep_tap
+from bencher.example.example_float2D_scatter import example_floats2D_scatter
+from bencher.example.optuna.example_optuna import optuna_rastrigin
 
 
 class TestBenchExamples(unittest.TestCase):
     """The purpose of this test class is to run the example problems to make sure they don't crash.  The bencher logic is tested in the other test files test_bencher.py and test_vars.py"""
 
-    def create_run_cfg(self) -> BenchRunCfg:
-        cfg = BenchRunCfg()
+    def create_run_cfg(self) -> bch.BenchRunCfg:
+        cfg = bch.BenchRunCfg()
         cfg.repeats = 2  # low number of repeats to reduce test time, but also test averaging and variance code
         cfg.debug = True  # reduce size of param sweep so tests are faster
         cfg.clear_cache = True
         return cfg
 
     def test_example_categorical(self) -> None:
         self.assertIsNotNone(example_categorical(self.create_run_cfg()))
@@ -42,22 +42,19 @@
 
     def test_example_simple_cat(self) -> None:
         self.assertIsNotNone(example_1D_cat(self.create_run_cfg()))
 
     def test_example_simple_float(self) -> None:
         self.assertIsNotNone(example_1D_float(self.create_run_cfg()))
 
-    def test_example_persistent(self) -> None:
-        self.assertIsNotNone(example_persistent(self.create_run_cfg()))
-
-    def test_example_cat_float(self) -> None:
-        self.assertIsNotNone(example_cat_float(self.create_run_cfg()))
+    def test_example_float_cat(self) -> None:
+        self.assertIsNotNone(run_example_float_cat(self.create_run_cfg()))
 
     def test_example_time_event(self) -> None:
-        self.assertIsNotNone(example_time_event(self.create_run_cfg()))
+        self.assertIsNotNone(run_example_time_event(self.create_run_cfg()))
 
     def test_example_float3D(self) -> None:
         self.assertIsNotNone(example_floats3D(self.create_run_cfg()))
 
     def test_example_cone(self) -> None:
         self.assertIsNotNone(example_cone(self.create_run_cfg()))
 
@@ -66,13 +63,18 @@
 
     def test_example_floats2D_workflow(self) -> None:
         self.assertIsNotNone(example_floats2D_workflow(self.create_run_cfg()))
 
     def test_example_floats3D_workflow(self) -> None:
         self.assertIsNotNone(example_floats3D_workflow(self.create_run_cfg()))
 
-    @pytest.mark.skip
-    def test_example_vector(self) -> None:
-        self.assertIsNotNone(example_vector())
-
     def test_plot_library(self) -> None:
         self.assertIsNotNone(example_plot_library(self.create_run_cfg()))
+
+    def test_holosweep_tap(self) -> None:
+        self.assertIsNotNone(example_holosweep_tap(self.create_run_cfg()))
+
+    def test_float2D_scatter(self) -> None:
+        self.assertIsNotNone(example_floats2D_scatter(self.create_run_cfg()))
+
+    def test_optuna_rastrigin(self) -> None:
+        self.assertIsNotNone(optuna_rastrigin(self.create_run_cfg()))
```

### Comparing `holobench-0.0.8/test/test_bencher.py` & `holobench-0.2.0/test/test_bencher.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         )
 
     def test_bench_cfg_hash_isolated(self):
         """hash values only seem to not match if run in a separate process, so run the hash test in separate processes"""
         self.assertEqual(get_hash_isolated_process(), get_hash_isolated_process())
 
     # @pytest.mark.skip
-    @settings(deadline=15000)
+    @settings(deadline=30000)
     @given(
         input_vars=st.sampled_from(input_var_cat_permutations),
         result_vars=st.sampled_from([[ExampleBenchCfgOut.param.out_sin]]),
     )
     def test_combinations_over_time(self, input_vars, result_vars) -> None:
         """check that up to 3 categorical values over time can be plotted"""
         # needed her instead of init because hypothesis calls this function multiple times after init() and the randomly generated data need to be the same each time to produce identical results to match the hand check plot iamges
```

### Comparing `holobench-0.0.8/test/test_combinations.py` & `holobench-0.2.0/test/test_combinations.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/test_plot_collection.py` & `holobench-0.2.0/test/test_plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/test_plot_filter.py` & `holobench-0.2.0/test/test_plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/test_plot_library.py` & `holobench-0.2.0/test/test_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/test_sample_cache.py` & `holobench-0.2.0/test/test_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/test/test_sweep_vars.py` & `holobench-0.2.0/test/test_sweep_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from hypothesis import given, strategies as st  # pylint: disable=unused-import
 import pytest
-from bencher.bench_vars import IntSweep
+from bencher.variables.inputs import IntSweep
 
 
 class TestVarSweeps(unittest.TestCase):
     def test_int_sweep_01(self):
         int_sweep = IntSweep(bounds=[0, 1])
         self.assertEqual(int_sweep.default, 0)
         self.assertEqual(int_sweep.values(False), [0, 1])
```

### Comparing `holobench-0.0.8/test/test_vars.py` & `holobench-0.2.0/test/test_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.8/PKG-INFO` & `holobench-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 Metadata-Version: 2.1
 Name: holobench
-Version: 0.0.8
+Version: 0.2.0
 Summary: A package for benchmarking the performance of arbitrary functions
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: holoviews[reccomended]
-Requires-Dist: hvplot==0.8.4
-Requires-Dist: diskcache
-Requires-Dist: optuna
-Requires-Dist: xarray
-Requires-Dist: plotly
-Requires-Dist: sortedcontainers
-Requires-Dist: pandas
-Requires-Dist: strenum
-Requires-Dist: seaborn
-Requires-Dist: scikit-learn
-Requires-Dist: str2bool
-Requires-Dist: black==23.3.0 ; extra == "test"
-Requires-Dist: check-manifest ; extra == "test"
-Requires-Dist: pre-commit ; extra == "test"
-Requires-Dist: pylint ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: pytest-mock<3.10.2 ; extra == "test"
-Requires-Dist: pytest-runner ; extra == "test"
-Requires-Dist: pytest ; extra == "test"
-Requires-Dist: hypothesis ; extra == "test"
-Requires-Dist: ruff ; extra == "test"
+Requires-Dist: holoviews>=1.15,<=1.17
+Requires-Dist: hvplot>=0.8,<=0.8.4
+Requires-Dist: diskcache>=5.6
+Requires-Dist: optuna>=3.2,<=3.2
+Requires-Dist: xarray>=2023.7,<=2023.7
+Requires-Dist: plotly>=5.15,<=5.15
+Requires-Dist: sortedcontainers>=2.4,<=2.4
+Requires-Dist: pandas>=2.0,<=2.0.1
+Requires-Dist: strenum>0.4
+Requires-Dist: seaborn>0.1.2
+Requires-Dist: scikit-learn>=1.3
+Requires-Dist: str2bool>=1.1
+Requires-Dist: mortgage
+Requires-Dist: black>=23,<=23.3 ; extra == "test"
+Requires-Dist: check-manifest>=0.49 ; extra == "test"
+Requires-Dist: pre-commit>=3.3.3 ; extra == "test"
+Requires-Dist: pylint>=2.17 ; extra == "test"
+Requires-Dist: pytest-cov>=4.1 ; extra == "test"
+Requires-Dist: pytest-mock>=3.10,<=3.11.1 ; extra == "test"
+Requires-Dist: pytest-runner>=6.0 ; extra == "test"
+Requires-Dist: pytest>=7.4 ; extra == "test"
+Requires-Dist: hypothesis>6 ; extra == "test"
+Requires-Dist: ruff>=0.0.28 ; extra == "test"
+Requires-Dist: mypy>=1.4,<1.4.1 ; extra == "test"
+Requires-Dist: coverage<=7.2.7,>=7.2.7 ; extra == "test"
 Project-URL: Home, https://github.com/blooop/bencher
 Project-URL: Source, https://github.com/blooop/bencher
 Provides-Extra: test
 
 # Bencher
 
 ## Continuous Integration Status
 
 [![Ci](https://github.com/dyson-ai/bencher/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/dyson-ai/bencher/actions/workflows/ci.yml?query=branch%3Amain)
-[![Code Coverage](https://codecov.io/gh/dyson-ai/bencher/branch/main/graph/badge.svg?token=W7uHKcY0ly)](https://codecov.io/gh/dyson-ai/bencher)
+[![Codecov](https://codecov.io/gh/blooop/bencher/branch/main/graph/badge.svg?token=AVFC5D5Z43)](https://codecov.io/gh/blooop/bencher)
+![PyPI](https://img.shields.io/pypi/v/holobench)
+![License](https://img.shields.io/pypi/l/bencher)
+[![Python](https://img.shields.io/badge/python-3.10%20%7C%203.11-blue)](https://www.python.org/downloads/release/python-310/)
+
 
 ## Intro
 
 Bencher is a tool to make it easy to benchmark the interactions between the input parameters to your algorithm and its resulting performance on a set of metrics.
 
 Parameters for bencher are defined using the param library https://param.holoviz.org/ as a config class with extra metadata that describes the bounds of the search space you want to measure.  You must define a benchmarking function that accepts an instance of the config class and return a dictionary with string metric names and float values.
 
@@ -64,8 +71,7 @@
         if it exists:
             load historical data
             combine latest data with historical data
         
         store the results using the input hash as a key
     deduce the type of plot based on the input types
     return data and plot
-
```

