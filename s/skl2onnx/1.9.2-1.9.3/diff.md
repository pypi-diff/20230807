# Comparing `tmp/skl2onnx-1.9.2.tar.gz` & `tmp/skl2onnx-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skl2onnx-1.9.2.tar", last modified: Tue Aug 17 12:30:07 2021, max compression
+gzip compressed data, was "skl2onnx-1.9.3.tar", last modified: Mon Sep 20 23:13:02 2021, max compression
```

## Comparing `skl2onnx-1.9.2.tar` & `skl2onnx-1.9.3.tar`

### file list

```diff
@@ -1,344 +1,372 @@
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:06.981960 skl2onnx-1.9.2/
--rw-rw-rw-   0        0        0    11358 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/LICENSE
--rw-rw-rw-   0        0        0      410 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0      180 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/NOTICE
--rw-rw-rw-   0        0        0     2086 2021-08-17 12:30:06.982959 skl2onnx-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1655 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:00.411500 skl2onnx-1.9.2/docs/
--rw-rw-rw-   0        0        0     2526 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/api_summary.rst
--rw-rw-rw-   0        0        0     6255 2021-08-02 12:52:05.000000 skl2onnx-1.9.2/docs/conf.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:00.841999 skl2onnx-1.9.2/docs/examples/
--rw-rw-rw-   0        0        0    66698 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/Au-Salon-de-l-agriculture-la-campagne-recrute.jpg
--rw-rw-rw-   0        0        0       71 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/README.txt
--rw-rw-rw-   0        0        0   112576 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/daisy_wikipedia.jpg
--rw-rw-rw-   0        0        0     1956 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_backend.py
--rw-rw-rw-   0        0        0     3396 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_benchmark_cdist.py
--rw-rw-rw-   0        0        0     4282 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_benchmark_pipeline.py
--rw-rw-rw-   0        0        0     4364 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_black_op.py
--rw-rw-rw-   0        0        0     5029 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_cast_transformer.py
--rw-rw-rw-   0        0        0     8655 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_complex_pipeline.py
--rw-rw-rw-   0        0        0     2367 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_convert_decision_function.py
--rw-rw-rw-   0        0        0     2556 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_convert_model.py
--rw-rw-rw-   0        0        0     5790 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_convert_syntax.py
--rw-rw-rw-   0        0        0     4024 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_convert_zipmap.py
--rw-rw-rw-   0        0        0    14723 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_custom_model.py
--rw-rw-rw-   0        0        0     9023 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_custom_parser.py
--rw-rw-rw-   0        0        0     8723 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_custom_parser_alternative.py
--rw-rw-rw-   0        0        0     4665 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_errors_onnxruntime.py
--rw-rw-rw-   0        0        0     6887 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_gpr.py
--rw-rw-rw-   0        0        0     9370 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_intermediate_outputs.py
--rw-rw-rw-   0        0        0     3873 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_investigate_pipeline.py
--rw-rw-rw-   0        0        0     1647 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_metadata.py
--rw-rw-rw-   0        0        0     4601 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_nmf.py
--rw-rw-rw-   0        0        0     5923 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_onnx_operators.py
--rw-rw-rw-   0        0        0     2232 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_pipeline.py
--rw-rw-rw-   0        0        0     4516 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_pipeline_lightgbm.py
--rw-rw-rw-   0        0        0     4845 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_pipeline_xgboost.py
--rw-rw-rw-   0        0        0     6645 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/examples/plot_tfidfvectorizer.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:00.867903 skl2onnx-1.9.2/docs/exts/
--rw-rw-rw-   0        0        0     2832 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/exts/github_link.py
--rw-rw-rw-   0        0        0     8593 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/exts/sphinx_skl2onnx_extension.py
--rw-rw-rw-   0        0        0     4300 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/index.rst
--rw-rw-rw-   0        0        0     1103 2021-08-02 12:52:05.000000 skl2onnx-1.9.2/docs/index_tutorial.rst
--rw-rw-rw-   0        0        0     4441 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/introduction.rst
--rw-rw-rw-   0        0        0    14733 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/logo_main.png
--rw-rw-rw-   0        0        0     4247 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/parameterized.rst
--rw-rw-rw-   0        0        0   229347 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/pipeline.png
--rw-rw-rw-   0        0        0    13747 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/pipeline.rst
--rw-rw-rw-   0        0        0      365 2021-08-02 12:52:05.000000 skl2onnx-1.9.2/docs/requirements.txt
--rw-rw-rw-   0        0        0     1940 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/supported.rst
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:00.954393 skl2onnx-1.9.2/docs/tests/
--rw-rw-rw-   0        0        0     3639 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tests/test_documentation_examples.py
--rw-rw-rw-   0        0        0     3662 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tests/test_documentation_tutorial.py
--rw-rw-rw-   0        0        0      774 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tests/test_utils_benchmark.py
--rw-rw-rw-   0        0        0      381 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tests/test_utils_classes.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:01.434746 skl2onnx-1.9.2/docs/tutorial/
--rw-rw-rw-   0        0        0       18 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/README.txt
--rw-rw-rw-   0        0        0     3511 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_abegin_convert_pipeline.py
--rw-rw-rw-   0        0        0     4173 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_bbegin_measure_time.py
--rw-rw-rw-   0        0        0     3860 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_cbegin_opset.py
--rw-rw-rw-   0        0        0     8425 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_dbegin_options.py
--rw-rw-rw-   0        0        0     3445 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_dbegin_options_list.py
--rw-rw-rw-   0        0        0    10456 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_ebegin_float_double.py
--rw-rw-rw-   0        0        0     3872 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_fbegin_investigate.py
--rw-rw-rw-   0        0        0     4585 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_gbegin_dataframe.py
--rw-rw-rw-   0        0        0     7248 2021-08-17 12:27:08.000000 skl2onnx-1.9.2/docs/tutorial/plot_gbegin_transfer_learning.py
--rw-rw-rw-   0        0        0     3244 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_gexternal_lightgbm.py
--rw-rw-rw-   0        0        0     6070 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_gexternal_xgboost.py
--rw-rw-rw-   0        0        0     6796 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_icustom_converter.py
--rw-rw-rw-   0        0        0     5319 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_jcustom_syntax.py
--rw-rw-rw-   0        0        0     5574 2021-07-27 10:51:18.000000 skl2onnx-1.9.2/docs/tutorial/plot_kcustom_converter_wrapper.py
--rw-rw-rw-   0        0        0     5410 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_lcustom_options.py
--rw-rw-rw-   0        0        0     5388 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_mcustom_parser.py
--rw-rw-rw-   0        0        0    12335 2021-07-26 15:09:32.000000 skl2onnx-1.9.2/docs/tutorial/plot_pextend_python_runtime.py
--rw-rw-rw-   0        0        0      663 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_qextend_onnxruntime.py
--rw-rw-rw-   0        0        0     8825 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial/plot_usparse_xgboost.py
--rw-rw-rw-   0        0        0     5853 2021-08-17 08:59:01.000000 skl2onnx-1.9.2/docs/tutorial/plot_wext_pyod_forest.py
--rw-rw-rw-   0        0        0      519 2021-08-02 12:52:05.000000 skl2onnx-1.9.2/docs/tutorial_1-5_external.rst
--rw-rw-rw-   0        0        0      885 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial_1_simple.rst
--rw-rw-rw-   0        0        0      606 2021-08-02 12:52:05.000000 skl2onnx-1.9.2/docs/tutorial_2-5_extlib.rst
--rw-rw-rw-   0        0        0     1085 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial_2_new_converter.rst
--rw-rw-rw-   0        0        0      922 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial_3_new_operator.rst
--rw-rw-rw-   0        0        0      246 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/docs/tutorial_4_advanced.rst
--rw-rw-rw-   0        0        0       91 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/requirements.txt
--rw-rw-rw-   0        0        0       92 2021-08-17 12:30:06.989727 skl2onnx-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1911 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:01.508461 skl2onnx-1.9.2/skl2onnx/
--rw-rw-rw-   0        0        0     1627 2021-08-17 09:01:20.000000 skl2onnx-1.9.2/skl2onnx/__init__.py
--rw-rw-rw-   0        0        0    29733 2021-08-17 11:18:44.000000 skl2onnx-1.9.2/skl2onnx/_parse.py
--rw-rw-rw-   0        0        0    15118 2021-07-30 14:55:02.000000 skl2onnx-1.9.2/skl2onnx/_supported_operators.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:01.835791 skl2onnx-1.9.2/skl2onnx/algebra/
--rw-rw-rw-   0        0        0       88 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/__init__.py
--rw-rw-rw-   0        0        0     9442 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/automation.py
--rw-rw-rw-   0        0        0     7263 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/complex_functions.py
--rw-rw-rw-   0        0        0     1997 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/custom_ops.py
--rw-rw-rw-   0        0        0    22725 2021-08-02 17:42:02.000000 skl2onnx-1.9.2/skl2onnx/algebra/graph_state.py
--rw-rw-rw-   0        0        0    38753 2021-07-27 15:59:09.000000 skl2onnx-1.9.2/skl2onnx/algebra/onnx_operator.py
--rw-rw-rw-   0        0        0     7610 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/onnx_operator_mixin.py
--rw-rw-rw-   0        0        0    13031 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/onnx_ops.py
--rw-rw-rw-   0        0        0      216 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/onnx_subgraph_operator_mixin.py
--rw-rw-rw-   0        0        0     4317 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/sklearn_ops.py
--rw-rw-rw-   0        0        0     2871 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/algebra/type_helper.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:02.171494 skl2onnx-1.9.2/skl2onnx/common/
--rw-rw-rw-   0        0        0      184 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/__init__.py
--rw-rw-rw-   0        0        0     2615 2021-07-27 10:51:18.000000 skl2onnx-1.9.2/skl2onnx/common/_apply_operation.py
--rw-rw-rw-   0        0        0    29886 2021-08-17 12:27:08.000000 skl2onnx-1.9.2/skl2onnx/common/_container.py
--rw-rw-rw-   0        0        0     8001 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/_onnx_optimisation_common.py
--rw-rw-rw-   0        0        0     4208 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/_registration.py
--rw-rw-rw-   0        0        0    56217 2021-08-17 12:27:08.000000 skl2onnx-1.9.2/skl2onnx/common/_topology.py
--rw-rw-rw-   0        0        0    14384 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/data_types.py
--rw-rw-rw-   0        0        0     1274 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/exceptions.py
--rw-rw-rw-   0        0        0     2752 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/interface.py
--rw-rw-rw-   0        0        0     4297 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/onnx_optimisation_identity.py
--rw-rw-rw-   0        0        0     4901 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/shape_calculator.py
--rw-rw-rw-   0        0        0     7967 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/tree_ensemble.py
--rw-rw-rw-   0        0        0     4891 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/utils.py
--rw-rw-rw-   0        0        0     1393 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/utils_checking.py
--rw-rw-rw-   0        0        0     3412 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/utils_classifier.py
--rw-rw-rw-   0        0        0     5081 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/common/utils_sklearn.py
--rw-rw-rw-   0        0        0    11139 2021-08-17 12:27:08.000000 skl2onnx-1.9.2/skl2onnx/convert.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:02.251045 skl2onnx-1.9.2/skl2onnx/helpers/
--rw-rw-rw-   0        0        0      176 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/helpers/__init__.py
--rw-rw-rw-   0        0        0    12640 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/helpers/investigate.py
--rw-rw-rw-   0        0        0    10572 2021-08-11 08:36:57.000000 skl2onnx-1.9.2/skl2onnx/helpers/onnx_helper.py
--rw-rw-rw-   0        0        0     2839 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/helpers/onnx_rare_helper.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:03.422035 skl2onnx-1.9.2/skl2onnx/operator_converters/
--rw-rw-rw-   0        0        0     2678 2021-07-30 14:55:02.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/__init__.py
--rw-rw-rw-   0        0        0    15707 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/_gp_kernels.py
--rw-rw-rw-   0        0        0    28070 2021-08-12 11:18:31.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/ada_boost.py
--rw-rw-rw-   0        0        0     1666 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/array_feature_extractor.py
--rw-rw-rw-   0        0        0    10206 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/bagging.py
--rw-rw-rw-   0        0        0     1789 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/binariser.py
--rw-rw-rw-   0        0        0    21948 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/calibrated_classifier_cv.py
--rw-rw-rw-   0        0        0     1606 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/cast_op.py
--rw-rw-rw-   0        0        0     2448 2021-08-02 17:42:02.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/common.py
--rw-rw-rw-   0        0        0      994 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/concat_op.py
--rw-rw-rw-   0        0        0     1461 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/cross_decomposition.py
--rw-rw-rw-   0        0        0    18722 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/decision_tree.py
--rw-rw-rw-   0        0        0     3848 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/decomposition.py
--rw-rw-rw-   0        0        0     2271 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/dict_vectoriser.py
--rw-rw-rw-   0        0        0     2242 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/feature_selection.py
--rw-rw-rw-   0        0        0      602 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/flatten_op.py
--rw-rw-rw-   0        0        0     1166 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/function_transformer.py
--rw-rw-rw-   0        0        0    11558 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/gaussian_mixture.py
--rw-rw-rw-   0        0        0    13885 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/gaussian_process.py
--rw-rw-rw-   0        0        0     6759 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/gradient_boosting.py
--rw-rw-rw-   0        0        0     1681 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/grid_search_cv.py
--rw-rw-rw-   0        0        0      629 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/id_op.py
--rw-rw-rw-   0        0        0     4870 2021-08-02 17:42:02.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/imputer_op.py
--rw-rw-rw-   0        0        0     9845 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/isolation_forest.py
--rw-rw-rw-   0        0        0     4880 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/k_bins_discretiser.py
--rw-rw-rw-   0        0        0     4364 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/k_means.py
--rw-rw-rw-   0        0        0     4480 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/label_binariser.py
--rw-rw-rw-   0        0        0     1323 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/label_encoder.py
--rw-rw-rw-   0        0        0    10583 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/linear_classifier.py
--rw-rw-rw-   0        0        0     6022 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/linear_regressor.py
--rw-rw-rw-   0        0        0     7968 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/multilayer_perceptron.py
--rw-rw-rw-   0        0        0      796 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/multiply_op.py
--rw-rw-rw-   0        0        0    24587 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/naive_bayes.py
--rw-rw-rw-   0        0        0    31603 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/nearest_neighbours.py
--rw-rw-rw-   0        0        0     1450 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/normaliser.py
--rw-rw-rw-   0        0        0     6920 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/one_hot_encoder.py
--rw-rw-rw-   0        0        0     7704 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/one_vs_rest_classifier.py
--rw-rw-rw-   0        0        0     4071 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/ordinal_encoder.py
--rw-rw-rw-   0        0        0     3361 2021-08-17 08:59:01.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/polynomial_features.py
--rw-rw-rw-   0        0        0     6109 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/power_transformer.py
--rw-rw-rw-   0        0        0    21335 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/random_forest.py
--rw-rw-rw-   0        0        0      963 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/random_projection.py
--rw-rw-rw-   0        0        0     1047 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/ransac_regressor.py
--rw-rw-rw-   0        0        0     1372 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/replace_op.py
--rw-rw-rw-   0        0        0     5932 2021-08-02 17:42:02.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/scaler_op.py
--rw-rw-rw-   0        0        0    11861 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/sgd_classifier.py
--rw-rw-rw-   0        0        0     7201 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/stacking.py
--rw-rw-rw-   0        0        0    15609 2021-08-02 12:52:05.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/support_vector_machines.py
--rw-rw-rw-   0        0        0    15985 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/text_vectoriser.py
--rw-rw-rw-   0        0        0     3949 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/tfidf_transformer.py
--rw-rw-rw-   0        0        0     2248 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/tfidf_vectoriser.py
--rw-rw-rw-   0        0        0     5933 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/voting_classifier.py
--rw-rw-rw-   0        0        0     2463 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/voting_regressor.py
--rw-rw-rw-   0        0        0     2447 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/operator_converters/zip_map.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:03.465628 skl2onnx-1.9.2/skl2onnx/proto/
--rw-rw-rw-   0        0        0     2494 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/proto/__init__.py
--rw-rw-rw-   0        0        0     8018 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/proto/onnx_helper_modified.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:04.227362 skl2onnx-1.9.2/skl2onnx/shape_calculators/
--rw-rw-rw-   0        0        0     1911 2021-07-30 14:55:02.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/__init__.py
--rw-rw-rw-   0        0        0      566 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/array_feature_extractor.py
--rw-rw-rw-   0        0        0      996 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/cast_op.py
--rw-rw-rw-   0        0        0     3781 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/concat.py
--rw-rw-rw-   0        0        0     1037 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/cross_decomposition.py
--rw-rw-rw-   0        0        0      721 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/dict_vectorizer.py
--rw-rw-rw-   0        0        0     3592 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/ensemble_shapes.py
--rw-rw-rw-   0        0        0      907 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/flatten.py
--rw-rw-rw-   0        0        0     1119 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/function_transformer.py
--rw-rw-rw-   0        0        0     1490 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/gaussian_process.py
--rw-rw-rw-   0        0        0      756 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/grid_search_cv.py
--rw-rw-rw-   0        0        0      456 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/identity.py
--rw-rw-rw-   0        0        0     1857 2021-08-02 17:42:02.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/imputer.py
--rw-rw-rw-   0        0        0      455 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/isolation_forest.py
--rw-rw-rw-   0        0        0      890 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/k_bins_discretiser.py
--rw-rw-rw-   0        0        0     1157 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/k_means.py
--rw-rw-rw-   0        0        0      820 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/label_binariser.py
--rw-rw-rw-   0        0        0     1068 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/label_encoder.py
--rw-rw-rw-   0        0        0     1746 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/linear_classifier.py
--rw-rw-rw-   0        0        0     2529 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/linear_regressor.py
--rw-rw-rw-   0        0        0     1249 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/mixture.py
--rw-rw-rw-   0        0        0     4173 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/nearest_neighbours.py
--rw-rw-rw-   0        0        0      987 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/one_hot_encoder.py
--rw-rw-rw-   0        0        0      307 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/one_vs_rest_classifier.py
--rw-rw-rw-   0        0        0      799 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/ordinal_encoder.py
--rw-rw-rw-   0        0        0      919 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/polynomial_features.py
--rw-rw-rw-   0        0        0      508 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/power_transformer.py
--rw-rw-rw-   0        0        0      502 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/random_projection.py
--rw-rw-rw-   0        0        0      467 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/replace_op.py
--rw-rw-rw-   0        0        0     2148 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/scaler.py
--rw-rw-rw-   0        0        0     2949 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/support_vector_machines.py
--rw-rw-rw-   0        0        0     1661 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/svd.py
--rw-rw-rw-   0        0        0      860 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/text_vectorizer.py
--rw-rw-rw-   0        0        0      566 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/tfidf_transformer.py
--rw-rw-rw-   0        0        0      304 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/voting_classifier.py
--rw-rw-rw-   0        0        0      302 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/voting_regressor.py
--rw-rw-rw-   0        0        0      828 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/shape_calculators/zip_map.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:04.317409 skl2onnx-1.9.2/skl2onnx/sklapi/
--rw-rw-rw-   0        0        0      204 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/sklapi/__init__.py
--rw-rw-rw-   0        0        0     1936 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/sklapi/cast_regressor.py
--rw-rw-rw-   0        0        0     1593 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/sklapi/cast_transformer.py
--rw-rw-rw-   0        0        0     1472 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/sklapi/replace_transformer.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:04.382447 skl2onnx-1.9.2/skl2onnx/tutorial/
--rw-rw-rw-   0        0        0      117 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/tutorial/__init__.py
--rw-rw-rw-   0        0        0     1411 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/tutorial/benchmark.py
--rw-rw-rw-   0        0        0    33995 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/skl2onnx/tutorial/imagenet_classes.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:01.583308 skl2onnx-1.9.2/skl2onnx.egg-info/
--rw-rw-rw-   0        0        0     2086 2021-08-17 12:29:58.000000 skl2onnx-1.9.2/skl2onnx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12579 2021-08-17 12:29:59.000000 skl2onnx-1.9.2/skl2onnx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-17 12:29:58.000000 skl2onnx-1.9.2/skl2onnx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2021-08-17 12:29:58.000000 skl2onnx-1.9.2/skl2onnx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-08-17 12:29:58.000000 skl2onnx-1.9.2/skl2onnx.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:06.610452 skl2onnx-1.9.2/tests/
--rw-rw-rw-   0        0        0     2801 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/benchmark.py
--rw-rw-rw-   0        0        0      185 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/bug.onnx
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:06.632926 skl2onnx-1.9.2/tests/datasets/
--rw-rw-rw-   0        0        0     3567 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/datasets/small_titanic.csv
--rw-rw-rw-   0        0        0    10571 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_cascade.py
--rw-rw-rw-   0        0        0     2038 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_complex.py
--rw-rw-rw-   0        0        0     4240 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_converters.py
--rw-rw-rw-   0        0        0     5072 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_custom_model.py
--rw-rw-rw-   0        0        0     3591 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_deprecation.py
--rw-rw-rw-   0        0        0     1435 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_double.py
--rw-rw-rw-   0        0        0     2307 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_doc.py
--rw-rw-rw-   0        0        0     9927 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_operator_mixin_syntax.py
--rw-rw-rw-   0        0        0    16707 2021-08-02 17:42:03.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_operators.py
--rw-rw-rw-   0        0        0     1326 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_operators_opset.py
--rw-rw-rw-   0        0        0    17718 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_operators_scan.py
--rw-rw-rw-   0        0        0     2965 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_operators_sparse.py
--rw-rw-rw-   0        0        0    10316 2021-08-02 17:42:03.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_operators_sub_estimator.py
--rw-rw-rw-   0        0        0     5709 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_onnx_operators_wrapped.py
--rw-rw-rw-   0        0        0     8703 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_symbolic.py
--rw-rw-rw-   0        0        0     6000 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_algebra_test_helper.py
--rw-rw-rw-   0        0        0    10427 2021-08-02 17:42:03.000000 skl2onnx-1.9.2/tests/test_algebra_to_onnx.py
--rw-rw-rw-   0        0        0      421 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_applied_functions.py
--rw-rw-rw-   0        0        0     5079 2021-08-11 08:36:59.000000 skl2onnx-1.9.2/tests/test_convert.py
--rw-rw-rw-   0        0        0     7372 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_custom_transformer.py
--rw-rw-rw-   0        0        0     9678 2021-08-17 12:27:08.000000 skl2onnx-1.9.2/tests/test_investigate.py
--rw-rw-rw-   0        0        0     4584 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_onnx_helper.py
--rw-rw-rw-   0        0        0     1722 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_onnx_rare_helper.py
--rw-rw-rw-   0        0        0     3884 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_op10.py
--rw-rw-rw-   0        0        0     3996 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_opset13.py
--rw-rw-rw-   0        0        0     4398 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_other_converter_library_pipelines.py
--rw-rw-rw-   0        0        0     4163 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_parsing_options.py
--rw-rw-rw-   0        0        0     1791 2021-08-13 16:43:38.000000 skl2onnx-1.9.2/tests/test_raw_name.py
--rw-rw-rw-   0        0        0     1611 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_scikit_pandas.py
--rw-rw-rw-   0        0        0     3455 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_shapes.py
--rw-rw-rw-   0        0        0    14830 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_adaboost_converter.py
--rw-rw-rw-   0        0        0     2746 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_array_feature_extractor.py
--rw-rw-rw-   0        0        0    13850 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_bagging_converter.py
--rw-rw-rw-   0        0        0      974 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_binarizer_converter.py
--rw-rw-rw-   0        0        0     9279 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_calibrated_classifier_cv_converter.py
--rw-rw-rw-   0        0        0     4631 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_cast_regressor.py
--rw-rw-rw-   0        0        0     5603 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_cast_transformer.py
--rw-rw-rw-   0        0        0     4771 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_concat.py
--rw-rw-rw-   0        0        0     5636 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_count_vectorizer_converter.py
--rw-rw-rw-   0        0        0     2794 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_count_vectorizer_converter_bug.py
--rw-rw-rw-   0        0        0     3306 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_custom_nmf.py
--rw-rw-rw-   0        0        0    18089 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_decision_tree_converters.py
--rw-rw-rw-   0        0        0     2995 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_dict_vectorizer_converter.py
--rw-rw-rw-   0        0        0     5958 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_documentation.py
--rw-rw-rw-   0        0        0    14035 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_double_tensor_type_cls.py
--rw-rw-rw-   0        0        0     6794 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_double_tensor_type_reg.py
--rw-rw-rw-   0        0        0    20245 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_double_tensor_type_tr.py
--rw-rw-rw-   0        0        0    17930 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_feature_selection_converters.py
--rw-rw-rw-   0        0        0     4587 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_feature_union.py
--rw-rw-rw-   0        0        0     6589 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_function_transformer_converter.py
--rw-rw-rw-   0        0        0    13697 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_gaussian_mixture_converter.py
--rw-rw-rw-   0        0        0     4686 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_gaussian_process_classifier.py
--rw-rw-rw-   0        0        0    45019 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_gaussian_process_regressor.py
--rw-rw-rw-   0        0        0    36600 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_glm_classifier_converter.py
--rw-rw-rw-   0        0        0    32214 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_glm_regressor_converter.py
--rw-rw-rw-   0        0        0    14701 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_gradient_boosting_converters.py
--rw-rw-rw-   0        0        0     9626 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_grid_search_cv_converter.py
--rw-rw-rw-   0        0        0     5883 2021-08-17 08:59:01.000000 skl2onnx-1.9.2/tests/test_sklearn_imputer_converter.py
--rw-rw-rw-   0        0        0     2652 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_isolation_forest.py
--rw-rw-rw-   0        0        0    13608 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_k_bins_discretiser_converter.py
--rw-rw-rw-   0        0        0     6422 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_k_means_converter.py
--rw-rw-rw-   0        0        0     4461 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_label_binariser_converter.py
--rw-rw-rw-   0        0        0     3776 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_label_encoder_converter.py
--rw-rw-rw-   0        0        0    14181 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_mlp_converter.py
--rw-rw-rw-   0        0        0    21072 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_naive_bayes_converter.py
--rw-rw-rw-   0        0        0    41750 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_nearest_neighbour_converter.py
--rw-rw-rw-   0        0        0     3220 2021-07-27 10:51:18.000000 skl2onnx-1.9.2/tests/test_sklearn_normalizer_converter.py
--rw-rw-rw-   0        0        0    13295 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_one_hot_encoder_converter.py
--rw-rw-rw-   0        0        0    24113 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_one_vs_rest_classifier_converter.py
--rw-rw-rw-   0        0        0     5752 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_ordinal_encoder.py
--rw-rw-rw-   0        0        0     4450 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_passive_aggressive_classifier_converter.py
--rw-rw-rw-   0        0        0     4137 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_pca_converter.py
--rw-rw-rw-   0        0        0     4303 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_perceptron_converter.py
--rw-rw-rw-   0        0        0    21423 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_pipeline.py
--rw-rw-rw-   0        0        0    10904 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_pipeline_within_pipeline.py
--rw-rw-rw-   0        0        0     3438 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_pls_regression.py
--rw-rw-rw-   0        0        0     5875 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_polynomial_features_converter.py
--rw-rw-rw-   0        0        0     6937 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_power_transformer.py
--rw-rw-rw-   0        0        0    35574 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_random_forest_converters.py
--rw-rw-rw-   0        0        0     1770 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_random_projection.py
--rw-rw-rw-   0        0        0     1568 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_replace_transformer.py
--rw-rw-rw-   0        0        0     8461 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_scaler_converter.py
--rw-rw-rw-   0        0        0    21459 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_sgd_classifier_converter.py
--rw-rw-rw-   0        0        0     3554 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_stacking.py
--rw-rw-rw-   0        0        0    19692 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_svm_converters.py
--rw-rw-rw-   0        0        0     2737 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_tfidf_transformer_converter.py
--rw-rw-rw-   0        0        0     2348 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_tfidf_transformer_converter_sparse.py
--rw-rw-rw-   0        0        0    23485 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter.py
--rw-rw-rw-   0        0        0     8414 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_char.py
--rw-rw-rw-   0        0        0     2308 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_dataset.py
--rw-rw-rw-   0        0        0     4960 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_pipeline.py
--rw-rw-rw-   0        0        0    16122 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_regex.py
--rw-rw-rw-   0        0        0     2336 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_truncated_svd.py
--rw-rw-rw-   0        0        0    11150 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_voting_classifier_converter.py
--rw-rw-rw-   0        0        0     2950 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_sklearn_voting_regressor_converter.py
--rw-rw-rw-   0        0        0     2659 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_supported_converters.py
--rw-rw-rw-   0        0        0     2200 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_topology_prune.py
-drwxrwxrwx   0        0        0        0 2021-08-17 12:30:06.972053 skl2onnx-1.9.2/tests/test_utils/
--rw-rw-rw-   0        0        0     2206 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_utils/__init__.py
--rw-rw-rw-   0        0        0     2453 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_utils/main.py
--rw-rw-rw-   0        0        0    36439 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_utils/tests_helper.py
--rw-rw-rw-   0        0        0    12215 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_utils/utils_backend.py
--rw-rw-rw-   0        0        0    23634 2021-07-26 07:31:25.000000 skl2onnx-1.9.2/tests/test_utils/utils_backend_onnxruntime.py
--rw-rw-rw-   0        0        0     9181 2021-08-17 08:59:01.000000 skl2onnx-1.9.2/tests/test_utils_sklearn.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:02.080469 skl2onnx-1.9.3/
+-rw-rw-rw-   0        0        0    11358 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/LICENSE
+-rw-rw-rw-   0        0        0      410 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      180 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/NOTICE
+-rw-rw-rw-   0        0        0     2086 2021-09-20 23:13:02.080922 skl2onnx-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1655 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/README.md
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:00.848351 skl2onnx-1.9.3/docs/
+-rw-rw-rw-   0        0        0     3114 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/docs/api_summary.rst
+-rw-rw-rw-   0        0        0     6237 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/docs/conf.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.025122 skl2onnx-1.9.3/docs/examples/
+-rw-rw-rw-   0        0        0    66698 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/Au-Salon-de-l-agriculture-la-campagne-recrute.jpg
+-rw-rw-rw-   0        0        0       71 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/README.txt
+-rw-rw-rw-   0        0        0   112576 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/daisy_wikipedia.jpg
+-rw-rw-rw-   0        0        0     2351 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/docs/examples/plot_backend.py
+-rw-rw-rw-   0        0        0     3396 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_benchmark_cdist.py
+-rw-rw-rw-   0        0        0     4282 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_benchmark_pipeline.py
+-rw-rw-rw-   0        0        0     4364 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_black_op.py
+-rw-rw-rw-   0        0        0     5029 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_cast_transformer.py
+-rw-rw-rw-   0        0        0     8655 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_complex_pipeline.py
+-rw-rw-rw-   0        0        0     2367 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_convert_decision_function.py
+-rw-rw-rw-   0        0        0     2556 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_convert_model.py
+-rw-rw-rw-   0        0        0     5920 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/docs/examples/plot_convert_syntax.py
+-rw-rw-rw-   0        0        0     4024 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_convert_zipmap.py
+-rw-rw-rw-   0        0        0    14723 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_custom_model.py
+-rw-rw-rw-   0        0        0     9023 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_custom_parser.py
+-rw-rw-rw-   0        0        0     8723 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_custom_parser_alternative.py
+-rw-rw-rw-   0        0        0     4665 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_errors_onnxruntime.py
+-rw-rw-rw-   0        0        0     6887 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_gpr.py
+-rw-rw-rw-   0        0        0     9370 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_intermediate_outputs.py
+-rw-rw-rw-   0        0        0     3873 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_investigate_pipeline.py
+-rw-rw-rw-   0        0        0     2836 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/docs/examples/plot_logging.py
+-rw-rw-rw-   0        0        0     1647 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_metadata.py
+-rw-rw-rw-   0        0        0     4601 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_nmf.py
+-rw-rw-rw-   0        0        0     5923 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_onnx_operators.py
+-rw-rw-rw-   0        0        0     2232 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_pipeline.py
+-rw-rw-rw-   0        0        0     4516 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_pipeline_lightgbm.py
+-rw-rw-rw-   0        0        0     4845 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_pipeline_xgboost.py
+-rw-rw-rw-   0        0        0     6645 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/examples/plot_tfidfvectorizer.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.038993 skl2onnx-1.9.3/docs/exts/
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.053334 skl2onnx-1.9.3/docs/exts/__pycache__/
+-rw-rw-rw-   0        0        0     2580 2021-08-30 17:15:38.000000 skl2onnx-1.9.3/docs/exts/__pycache__/github_link.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7088 2021-09-06 17:05:23.000000 skl2onnx-1.9.3/docs/exts/__pycache__/sphinx_skl2onnx_extension.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2832 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/exts/github_link.py
+-rw-rw-rw-   0        0        0     8593 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/exts/sphinx_skl2onnx_extension.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.060172 skl2onnx-1.9.3/docs/images/
+-rw-rw-rw-   0        0        0    46458 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/images/woe.png
+-rw-rw-rw-   0        0        0     4300 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1103 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/index_tutorial.rst
+-rw-rw-rw-   0        0        0     4441 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/introduction.rst
+-rw-rw-rw-   0        0        0    14733 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/logo_main.png
+-rw-rw-rw-   0        0        0     4247 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/parameterized.rst
+-rw-rw-rw-   0        0        0   229347 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/pipeline.png
+-rw-rw-rw-   0        0        0    13747 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/pipeline.rst
+-rw-rw-rw-   0        0        0      383 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1940 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/supported.rst
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.079705 skl2onnx-1.9.3/docs/tests/
+-rw-rw-rw-   0        0        0     3639 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tests/test_documentation_examples.py
+-rw-rw-rw-   0        0        0     3662 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tests/test_documentation_tutorial.py
+-rw-rw-rw-   0        0        0      774 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tests/test_utils_benchmark.py
+-rw-rw-rw-   0        0        0      381 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tests/test_utils_classes.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.170329 skl2onnx-1.9.3/docs/tutorial/
+-rw-rw-rw-   0        0        0       18 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/README.txt
+-rw-rw-rw-   0        0        0     3511 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_abegin_convert_pipeline.py
+-rw-rw-rw-   0        0        0     4173 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_bbegin_measure_time.py
+-rw-rw-rw-   0        0        0     7513 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/tutorial/plot_catwoe_transformer.py
+-rw-rw-rw-   0        0        0     3860 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_cbegin_opset.py
+-rw-rw-rw-   0        0        0     8425 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_dbegin_options.py
+-rw-rw-rw-   0        0        0     3445 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_dbegin_options_list.py
+-rw-rw-rw-   0        0        0    10587 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/tutorial/plot_ebegin_float_double.py
+-rw-rw-rw-   0        0        0     3872 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_fbegin_investigate.py
+-rw-rw-rw-   0        0        0     3222 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/docs/tutorial/plot_gbegin_cst.py
+-rw-rw-rw-   0        0        0     4585 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_gbegin_dataframe.py
+-rw-rw-rw-   0        0        0     7248 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_gbegin_transfer_learning.py
+-rw-rw-rw-   0        0        0     3254 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/docs/tutorial/plot_gexternal_lightgbm.py
+-rw-rw-rw-   0        0        0     5957 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/docs/tutorial/plot_gexternal_lightgbm_reg.py
+-rw-rw-rw-   0        0        0     6070 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_gexternal_xgboost.py
+-rw-rw-rw-   0        0        0     6983 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/tutorial/plot_icustom_converter.py
+-rw-rw-rw-   0        0        0     5506 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/tutorial/plot_jcustom_syntax.py
+-rw-rw-rw-   0        0        0     5574 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_kcustom_converter_wrapper.py
+-rw-rw-rw-   0        0        0     5410 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_lcustom_options.py
+-rw-rw-rw-   0        0        0     5388 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_mcustom_parser.py
+-rw-rw-rw-   0        0        0    12335 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_pextend_python_runtime.py
+-rw-rw-rw-   0        0        0      663 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_qextend_onnxruntime.py
+-rw-rw-rw-   0        0        0     8825 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial/plot_usparse_xgboost.py
+-rw-rw-rw-   0        0        0     5853 2021-09-20 15:34:38.000000 skl2onnx-1.9.3/docs/tutorial/plot_wext_pyod_forest.py
+-rw-rw-rw-   0        0        0     3284 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/tutorial/plot_woe_transformer.py
+-rw-rw-rw-   0        0        0      565 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/docs/tutorial_1-5_external.rst
+-rw-rw-rw-   0        0        0      919 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/docs/tutorial_1_simple.rst
+-rw-rw-rw-   0        0        0      606 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial_2-5_extlib.rst
+-rw-rw-rw-   0        0        0     1085 2021-09-20 23:09:34.000000 skl2onnx-1.9.3/docs/tutorial_2_new_converter.rst
+-rw-rw-rw-   0        0        0      922 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/docs/tutorial_3_new_operator.rst
+-rw-rw-rw-   0        0        0      285 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/docs/tutorial_4_advanced.rst
+-rw-rw-rw-   0        0        0       91 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/requirements.txt
+-rw-rw-rw-   0        0        0       92 2021-09-20 23:13:02.083302 skl2onnx-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.183780 skl2onnx-1.9.3/skl2onnx/
+-rw-rw-rw-   0        0        0     1627 2021-09-20 23:09:41.000000 skl2onnx-1.9.3/skl2onnx/__init__.py
+-rw-rw-rw-   0        0        0    31806 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/_parse.py
+-rw-rw-rw-   0        0        0    15716 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/_supported_operators.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.232289 skl2onnx-1.9.3/skl2onnx/algebra/
+-rw-rw-rw-   0        0        0       88 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/algebra/__init__.py
+-rw-rw-rw-   0        0        0     9442 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/algebra/automation.py
+-rw-rw-rw-   0        0        0     7243 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/algebra/complex_functions.py
+-rw-rw-rw-   0        0        0     1997 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/algebra/custom_ops.py
+-rw-rw-rw-   0        0        0    27627 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/algebra/graph_state.py
+-rw-rw-rw-   0        0        0    45463 2021-09-18 08:33:37.000000 skl2onnx-1.9.3/skl2onnx/algebra/onnx_operator.py
+-rw-rw-rw-   0        0        0     9228 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/algebra/onnx_operator_mixin.py
+-rw-rw-rw-   0        0        0    13076 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/algebra/onnx_ops.py
+-rw-rw-rw-   0        0        0      216 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/algebra/onnx_subgraph_operator_mixin.py
+-rw-rw-rw-   0        0        0     4362 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/algebra/sklearn_ops.py
+-rw-rw-rw-   0        0        0     3544 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/skl2onnx/algebra/type_helper.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.279123 skl2onnx-1.9.3/skl2onnx/common/
+-rw-rw-rw-   0        0        0      184 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/__init__.py
+-rw-rw-rw-   0        0        0     2615 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/_apply_operation.py
+-rw-rw-rw-   0        0        0    32819 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/common/_container.py
+-rw-rw-rw-   0        0        0     8001 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/_onnx_optimisation_common.py
+-rw-rw-rw-   0        0        0     4471 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/common/_registration.py
+-rw-rw-rw-   0        0        0    58076 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/common/_topology.py
+-rw-rw-rw-   0        0        0    14405 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/common/data_types.py
+-rw-rw-rw-   0        0        0     1274 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/exceptions.py
+-rw-rw-rw-   0        0        0     4297 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/onnx_optimisation_identity.py
+-rw-rw-rw-   0        0        0     5181 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/common/shape_calculator.py
+-rw-rw-rw-   0        0        0     7967 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/tree_ensemble.py
+-rw-rw-rw-   0        0        0     6306 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/common/utils.py
+-rw-rw-rw-   0        0        0     1393 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/utils_checking.py
+-rw-rw-rw-   0        0        0     3412 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/utils_classifier.py
+-rw-rw-rw-   0        0        0     5081 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/common/utils_sklearn.py
+-rw-rw-rw-   0        0        0    11774 2021-09-20 23:09:34.000000 skl2onnx-1.9.3/skl2onnx/convert.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.291122 skl2onnx-1.9.3/skl2onnx/helpers/
+-rw-rw-rw-   0        0        0      176 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/helpers/__init__.py
+-rw-rw-rw-   0        0        0    12638 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/helpers/investigate.py
+-rw-rw-rw-   0        0        0    14524 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/helpers/onnx_helper.py
+-rw-rw-rw-   0        0        0     2839 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/helpers/onnx_rare_helper.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.475726 skl2onnx-1.9.3/skl2onnx/operator_converters/
+-rw-rw-rw-   0        0        0     2862 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/__init__.py
+-rw-rw-rw-   0        0        0    15707 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/_gp_kernels.py
+-rw-rw-rw-   0        0        0    28123 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/ada_boost.py
+-rw-rw-rw-   0        0        0     1666 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/array_feature_extractor.py
+-rw-rw-rw-   0        0        0    10449 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/bagging.py
+-rw-rw-rw-   0        0        0     1789 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/binariser.py
+-rw-rw-rw-   0        0        0    21724 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/calibrated_classifier_cv.py
+-rw-rw-rw-   0        0        0     1606 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/cast_op.py
+-rw-rw-rw-   0        0        0     2448 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/common.py
+-rw-rw-rw-   0        0        0      994 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/concat_op.py
+-rw-rw-rw-   0        0        0     1461 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/cross_decomposition.py
+-rw-rw-rw-   0        0        0    18722 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/decision_tree.py
+-rw-rw-rw-   0        0        0     3848 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/decomposition.py
+-rw-rw-rw-   0        0        0     2271 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/dict_vectoriser.py
+-rw-rw-rw-   0        0        0     2242 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/feature_selection.py
+-rw-rw-rw-   0        0        0      602 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/flatten_op.py
+-rw-rw-rw-   0        0        0     1166 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/function_transformer.py
+-rw-rw-rw-   0        0        0    11835 2021-09-17 17:19:51.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/gaussian_mixture.py
+-rw-rw-rw-   0        0        0    13885 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/gaussian_process.py
+-rw-rw-rw-   0        0        0     6759 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/gradient_boosting.py
+-rw-rw-rw-   0        0        0     1329 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/grid_search_cv.py
+-rw-rw-rw-   0        0        0      629 2021-08-25 17:58:52.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/id_op.py
+-rw-rw-rw-   0        0        0     4870 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/imputer_op.py
+-rw-rw-rw-   0        0        0    10184 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/isolation_forest.py
+-rw-rw-rw-   0        0        0     4880 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/k_bins_discretiser.py
+-rw-rw-rw-   0        0        0     4315 2021-09-20 23:09:34.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/k_means.py
+-rw-rw-rw-   0        0        0     6127 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/kernel_pca.py
+-rw-rw-rw-   0        0        0     4480 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/label_binariser.py
+-rw-rw-rw-   0        0        0     1323 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/label_encoder.py
+-rw-rw-rw-   0        0        0    10583 2021-08-25 10:50:25.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/linear_classifier.py
+-rw-rw-rw-   0        0        0     5806 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/linear_regressor.py
+-rw-rw-rw-   0        0        0     4753 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/local_outlier_factor.py
+-rw-rw-rw-   0        0        0     7968 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/multilayer_perceptron.py
+-rw-rw-rw-   0        0        0     2908 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/multioutput.py
+-rw-rw-rw-   0        0        0      796 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/multiply_op.py
+-rw-rw-rw-   0        0        0    24587 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/naive_bayes.py
+-rw-rw-rw-   0        0        0    31756 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/nearest_neighbours.py
+-rw-rw-rw-   0        0        0     1450 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/normaliser.py
+-rw-rw-rw-   0        0        0     6920 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/one_hot_encoder.py
+-rw-rw-rw-   0        0        0     7859 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/one_vs_rest_classifier.py
+-rw-rw-rw-   0        0        0     4249 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/ordinal_encoder.py
+-rw-rw-rw-   0        0        0     1971 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/pipelines.py
+-rw-rw-rw-   0        0        0     3361 2021-09-20 15:34:38.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/polynomial_features.py
+-rw-rw-rw-   0        0        0     6109 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/power_transformer.py
+-rw-rw-rw-   0        0        0    21335 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/random_forest.py
+-rw-rw-rw-   0        0        0      963 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/random_projection.py
+-rw-rw-rw-   0        0        0     1093 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/ransac_regressor.py
+-rw-rw-rw-   0        0        0     1372 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/replace_op.py
+-rw-rw-rw-   0        0        0     7800 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/scaler_op.py
+-rw-rw-rw-   0        0        0    11861 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/sgd_classifier.py
+-rw-rw-rw-   0        0        0     7377 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/stacking.py
+-rw-rw-rw-   0        0        0    16351 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/support_vector_machines.py
+-rw-rw-rw-   0        0        0    15985 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/text_vectoriser.py
+-rw-rw-rw-   0        0        0     3949 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/tfidf_transformer.py
+-rw-rw-rw-   0        0        0     2239 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/tfidf_vectoriser.py
+-rw-rw-rw-   0        0        0     5989 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/voting_classifier.py
+-rw-rw-rw-   0        0        0     2463 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/voting_regressor.py
+-rw-rw-rw-   0        0        0     2447 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/operator_converters/zip_map.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.483850 skl2onnx-1.9.3/skl2onnx/proto/
+-rw-rw-rw-   0        0        0     2494 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/proto/__init__.py
+-rw-rw-rw-   0        0        0     8043 2021-09-18 10:02:53.000000 skl2onnx-1.9.3/skl2onnx/proto/onnx_helper_modified.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.613010 skl2onnx-1.9.3/skl2onnx/shape_calculators/
+-rw-rw-rw-   0        0        0     2095 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/__init__.py
+-rw-rw-rw-   0        0        0      566 2021-08-24 17:59:08.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/array_feature_extractor.py
+-rw-rw-rw-   0        0        0      996 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/cast_op.py
+-rw-rw-rw-   0        0        0     3781 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/concat.py
+-rw-rw-rw-   0        0        0     1037 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/cross_decomposition.py
+-rw-rw-rw-   0        0        0      721 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/dict_vectorizer.py
+-rw-rw-rw-   0        0        0     3874 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/ensemble_shapes.py
+-rw-rw-rw-   0        0        0      907 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/flatten.py
+-rw-rw-rw-   0        0        0     1119 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/function_transformer.py
+-rw-rw-rw-   0        0        0     1490 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/gaussian_process.py
+-rw-rw-rw-   0        0        0      908 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/grid_search_cv.py
+-rw-rw-rw-   0        0        0      456 2021-08-25 17:59:12.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/identity.py
+-rw-rw-rw-   0        0        0     1857 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/imputer.py
+-rw-rw-rw-   0        0        0      455 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/isolation_forest.py
+-rw-rw-rw-   0        0        0      890 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/k_bins_discretiser.py
+-rw-rw-rw-   0        0        0     1157 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/k_means.py
+-rw-rw-rw-   0        0        0     1459 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/kernel_pca.py
+-rw-rw-rw-   0        0        0      820 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/label_binariser.py
+-rw-rw-rw-   0        0        0     1068 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/label_encoder.py
+-rw-rw-rw-   0        0        0     1746 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/linear_classifier.py
+-rw-rw-rw-   0        0        0     2529 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/linear_regressor.py
+-rw-rw-rw-   0        0        0      466 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/local_outlier_factor.py
+-rw-rw-rw-   0        0        0     1249 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/mixture.py
+-rw-rw-rw-   0        0        0     1413 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/multioutput.py
+-rw-rw-rw-   0        0        0     4173 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/nearest_neighbours.py
+-rw-rw-rw-   0        0        0      987 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/one_hot_encoder.py
+-rw-rw-rw-   0        0        0      307 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/one_vs_rest_classifier.py
+-rw-rw-rw-   0        0        0      799 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/ordinal_encoder.py
+-rw-rw-rw-   0        0        0      532 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/pipelines.py
+-rw-rw-rw-   0        0        0      919 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/polynomial_features.py
+-rw-rw-rw-   0        0        0      508 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/power_transformer.py
+-rw-rw-rw-   0        0        0      502 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/random_projection.py
+-rw-rw-rw-   0        0        0      467 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/replace_op.py
+-rw-rw-rw-   0        0        0     2134 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/scaler.py
+-rw-rw-rw-   0        0        0     2951 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/support_vector_machines.py
+-rw-rw-rw-   0        0        0     1661 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/svd.py
+-rw-rw-rw-   0        0        0      860 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/text_vectorizer.py
+-rw-rw-rw-   0        0        0      566 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/tfidf_transformer.py
+-rw-rw-rw-   0        0        0      437 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/voting_classifier.py
+-rw-rw-rw-   0        0        0      426 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/voting_regressor.py
+-rw-rw-rw-   0        0        0      828 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/shape_calculators/zip_map.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.631711 skl2onnx-1.9.3/skl2onnx/sklapi/
+-rw-rw-rw-   0        0        0      256 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/sklapi/__init__.py
+-rw-rw-rw-   0        0        0     1936 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/sklapi/cast_regressor.py
+-rw-rw-rw-   0        0        0     1593 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/sklapi/cast_transformer.py
+-rw-rw-rw-   0        0        0      115 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/sklapi/register.py
+-rw-rw-rw-   0        0        0     1472 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/sklapi/replace_transformer.py
+-rw-rw-rw-   0        0        0     7945 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/skl2onnx/sklapi/woe_transformer.py
+-rw-rw-rw-   0        0        0    21676 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/skl2onnx/sklapi/woe_transformer_onnx.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.639781 skl2onnx-1.9.3/skl2onnx/tutorial/
+-rw-rw-rw-   0        0        0      117 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/tutorial/__init__.py
+-rw-rw-rw-   0        0        0     1411 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/tutorial/benchmark.py
+-rw-rw-rw-   0        0        0    33995 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/skl2onnx/tutorial/imagenet_classes.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.202238 skl2onnx-1.9.3/skl2onnx.egg-info/
+-rw-rw-rw-   0        0        0     2086 2021-09-20 23:12:56.000000 skl2onnx-1.9.3/skl2onnx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13632 2021-09-20 23:12:57.000000 skl2onnx-1.9.3/skl2onnx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-20 23:12:57.000000 skl2onnx-1.9.3/skl2onnx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2021-09-20 23:12:57.000000 skl2onnx-1.9.3/skl2onnx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2021-09-20 23:12:57.000000 skl2onnx-1.9.3/skl2onnx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.955202 skl2onnx-1.9.3/tests/
+-rw-rw-rw-   0        0        0     2801 2021-09-02 10:35:28.000000 skl2onnx-1.9.3/tests/benchmark.py
+-rw-rw-rw-   0        0        0      185 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/bug.onnx
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:01.958736 skl2onnx-1.9.3/tests/datasets/
+-rw-rw-rw-   0        0        0     3567 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/datasets/small_titanic.csv
+-rw-rw-rw-   0        0        0    10571 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_cascade.py
+-rw-rw-rw-   0        0        0     2161 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_algebra_complex.py
+-rw-rw-rw-   0        0        0     4240 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_converters.py
+-rw-rw-rw-   0        0        0     5156 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/tests/test_algebra_custom_model.py
+-rw-rw-rw-   0        0        0    18017 2021-09-13 14:39:20.000000 skl2onnx-1.9.3/tests/test_algebra_custom_model_sub_estimator.py
+-rw-rw-rw-   0        0        0     3591 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_deprecation.py
+-rw-rw-rw-   0        0        0     1435 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_double.py
+-rw-rw-rw-   0        0        0     2307 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_doc.py
+-rw-rw-rw-   0        0        0    10499 2021-09-08 12:34:04.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_operator_mixin_syntax.py
+-rw-rw-rw-   0        0        0    18916 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_operators.py
+-rw-rw-rw-   0        0        0     1326 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_operators_opset.py
+-rw-rw-rw-   0        0        0    17718 2021-09-09 10:04:45.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_operators_scan.py
+-rw-rw-rw-   0        0        0     2970 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_operators_sparse.py
+-rw-rw-rw-   0        0        0    10316 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_operators_sub_estimator.py
+-rw-rw-rw-   0        0        0     5722 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_algebra_onnx_operators_wrapped.py
+-rw-rw-rw-   0        0        0     8703 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_symbolic.py
+-rw-rw-rw-   0        0        0     6000 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_algebra_test_helper.py
+-rw-rw-rw-   0        0        0    11014 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_algebra_to_onnx.py
+-rw-rw-rw-   0        0        0      421 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_applied_functions.py
+-rw-rw-rw-   0        0        0     5079 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_convert.py
+-rw-rw-rw-   0        0        0     4512 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_custom_transformer_ordwoe.py
+-rw-rw-rw-   0        0        0     7376 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_custom_transformer_tsne.py
+-rw-rw-rw-   0        0        0     9634 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/tests/test_investigate.py
+-rw-rw-rw-   0        0        0     6801 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/tests/test_onnx_helper.py
+-rw-rw-rw-   0        0        0     1722 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_onnx_rare_helper.py
+-rw-rw-rw-   0        0        0     3884 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_op10.py
+-rw-rw-rw-   0        0        0     3996 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_opset13.py
+-rw-rw-rw-   0        0        0     7648 2021-09-10 13:56:02.000000 skl2onnx-1.9.3/tests/test_options.py
+-rw-rw-rw-   0        0        0     4398 2021-09-06 15:57:24.000000 skl2onnx-1.9.3/tests/test_other_converter_library_pipelines.py
+-rw-rw-rw-   0        0        0     4163 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_parsing_options.py
+-rw-rw-rw-   0        0        0     1791 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_raw_name.py
+-rw-rw-rw-   0        0        0     1611 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_scikit_pandas.py
+-rw-rw-rw-   0        0        0     3455 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_shapes.py
+-rw-rw-rw-   0        0        0    14830 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_adaboost_converter.py
+-rw-rw-rw-   0        0        0     2746 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_array_feature_extractor.py
+-rw-rw-rw-   0        0        0    14691 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/tests/test_sklearn_bagging_converter.py
+-rw-rw-rw-   0        0        0      974 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_binarizer_converter.py
+-rw-rw-rw-   0        0        0    13401 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/tests/test_sklearn_calibrated_classifier_cv_converter.py
+-rw-rw-rw-   0        0        0     4631 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_cast_regressor.py
+-rw-rw-rw-   0        0        0     5603 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_cast_transformer.py
+-rw-rw-rw-   0        0        0     4771 2021-09-01 00:02:54.000000 skl2onnx-1.9.3/tests/test_sklearn_concat.py
+-rw-rw-rw-   0        0        0     5636 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_count_vectorizer_converter.py
+-rw-rw-rw-   0        0        0     2794 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_count_vectorizer_converter_bug.py
+-rw-rw-rw-   0        0        0     3306 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_custom_nmf.py
+-rw-rw-rw-   0        0        0    18089 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_decision_tree_converters.py
+-rw-rw-rw-   0        0        0     2995 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_dict_vectorizer_converter.py
+-rw-rw-rw-   0        0        0     5958 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_documentation.py
+-rw-rw-rw-   0        0        0    14035 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_double_tensor_type_cls.py
+-rw-rw-rw-   0        0        0     6794 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_double_tensor_type_reg.py
+-rw-rw-rw-   0        0        0    20245 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_double_tensor_type_tr.py
+-rw-rw-rw-   0        0        0    17930 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_feature_selection_converters.py
+-rw-rw-rw-   0        0        0     4587 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_feature_union.py
+-rw-rw-rw-   0        0        0     6589 2021-08-31 23:47:15.000000 skl2onnx-1.9.3/tests/test_sklearn_function_transformer_converter.py
+-rw-rw-rw-   0        0        0    14357 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_sklearn_gaussian_mixture_converter.py
+-rw-rw-rw-   0        0        0     4686 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_gaussian_process_classifier.py
+-rw-rw-rw-   0        0        0    45019 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_gaussian_process_regressor.py
+-rw-rw-rw-   0        0        0    36600 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_glm_classifier_converter.py
+-rw-rw-rw-   0        0        0    32214 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_glm_regressor_converter.py
+-rw-rw-rw-   0        0        0    14585 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_sklearn_gradient_boosting_converters.py
+-rw-rw-rw-   0        0        0    10386 2021-09-08 13:37:25.000000 skl2onnx-1.9.3/tests/test_sklearn_grid_search_cv_converter.py
+-rw-rw-rw-   0        0        0     5883 2021-09-20 15:34:38.000000 skl2onnx-1.9.3/tests/test_sklearn_imputer_converter.py
+-rw-rw-rw-   0        0        0     3933 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/tests/test_sklearn_isolation_forest.py
+-rw-rw-rw-   0        0        0    13608 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_k_bins_discretiser_converter.py
+-rw-rw-rw-   0        0        0     6422 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_k_means_converter.py
+-rw-rw-rw-   0        0        0     4821 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/tests/test_sklearn_kernel_pca_converter.py
+-rw-rw-rw-   0        0        0     4461 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_label_binariser_converter.py
+-rw-rw-rw-   0        0        0     3776 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_label_encoder_converter.py
+-rw-rw-rw-   0        0        0    11060 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/tests/test_sklearn_local_outlier_factor.py
+-rw-rw-rw-   0        0        0    14181 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_mlp_converter.py
+-rw-rw-rw-   0        0        0     3280 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/tests/test_sklearn_multi_output.py
+-rw-rw-rw-   0        0        0    21072 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_naive_bayes_converter.py
+-rw-rw-rw-   0        0        0    42901 2021-09-16 14:58:17.000000 skl2onnx-1.9.3/tests/test_sklearn_nearest_neighbour_converter.py
+-rw-rw-rw-   0        0        0     3220 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_normalizer_converter.py
+-rw-rw-rw-   0        0        0    13295 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_one_hot_encoder_converter.py
+-rw-rw-rw-   0        0        0    24113 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_one_vs_rest_classifier_converter.py
+-rw-rw-rw-   0        0        0     5752 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_ordinal_encoder.py
+-rw-rw-rw-   0        0        0     4450 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_passive_aggressive_classifier_converter.py
+-rw-rw-rw-   0        0        0     4137 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_pca_converter.py
+-rw-rw-rw-   0        0        0     4303 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_perceptron_converter.py
+-rw-rw-rw-   0        0        0    34242 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/tests/test_sklearn_pipeline.py
+-rw-rw-rw-   0        0        0    12842 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_sklearn_pipeline_within_pipeline.py
+-rw-rw-rw-   0        0        0     3438 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_pls_regression.py
+-rw-rw-rw-   0        0        0     5875 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_polynomial_features_converter.py
+-rw-rw-rw-   0        0        0     6937 2021-09-08 21:32:09.000000 skl2onnx-1.9.3/tests/test_sklearn_power_transformer.py
+-rw-rw-rw-   0        0        0    35574 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_random_forest_converters.py
+-rw-rw-rw-   0        0        0     1770 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_random_projection.py
+-rw-rw-rw-   0        0        0     1568 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_replace_transformer.py
+-rw-rw-rw-   0        0        0     8461 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_scaler_converter.py
+-rw-rw-rw-   0        0        0    21459 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_sgd_classifier_converter.py
+-rw-rw-rw-   0        0        0     3554 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_stacking.py
+-rw-rw-rw-   0        0        0    25597 2021-09-20 15:43:06.000000 skl2onnx-1.9.3/tests/test_sklearn_svm_converters.py
+-rw-rw-rw-   0        0        0     2737 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_tfidf_transformer_converter.py
+-rw-rw-rw-   0        0        0     2348 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_tfidf_transformer_converter_sparse.py
+-rw-rw-rw-   0        0        0    23485 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter.py
+-rw-rw-rw-   0        0        0     8414 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_char.py
+-rw-rw-rw-   0        0        0     2308 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_dataset.py
+-rw-rw-rw-   0        0        0     4960 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_pipeline.py
+-rw-rw-rw-   0        0        0    16122 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_regex.py
+-rw-rw-rw-   0        0        0     2336 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_truncated_svd.py
+-rw-rw-rw-   0        0        0    11150 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_voting_classifier_converter.py
+-rw-rw-rw-   0        0        0     2950 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_sklearn_voting_regressor_converter.py
+-rw-rw-rw-   0        0        0    10095 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_sklearn_woe_transformer.py
+-rw-rw-rw-   0        0        0     2659 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_supported_converters.py
+-rw-rw-rw-   0        0        0     4296 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_topology_prune.py
+drwxrwxrwx   0        0        0        0 2021-09-20 23:13:02.078459 skl2onnx-1.9.3/tests/test_utils/
+-rw-rw-rw-   0        0        0     2232 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_utils/__init__.py
+-rw-rw-rw-   0        0        0     2453 2021-08-20 10:29:21.000000 skl2onnx-1.9.3/tests/test_utils/main.py
+-rw-rw-rw-   0        0        0    37390 2021-09-06 15:47:54.000000 skl2onnx-1.9.3/tests/test_utils/tests_helper.py
+-rw-rw-rw-   0        0        0    12280 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_utils/utils_backend.py
+-rw-rw-rw-   0        0        0    23500 2021-09-02 16:07:15.000000 skl2onnx-1.9.3/tests/test_utils/utils_backend_onnxruntime.py
+-rw-rw-rw-   0        0        0     9181 2021-09-20 15:34:38.000000 skl2onnx-1.9.3/tests/test_utils_sklearn.py
+-rw-rw-rw-   0        0        0     3691 2021-09-10 15:48:43.000000 skl2onnx-1.9.3/tests/test_variable_names.py
```

### Comparing `skl2onnx-1.9.2/LICENSE` & `skl2onnx-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/PKG-INFO` & `skl2onnx-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skl2onnx
-Version: 1.9.2
+Version: 1.9.3
 Summary: Convert scikit-learn models to ONNX
 Home-page: https://github.com/onnx/sklearn-onnx
 Author: Microsoft Corporation
 Author-email: onnx@microsoft.com
 License: Apache License v2.0
 Description: ## Introduction
         *sklearn-onnx* converts [scikit-learn](https://scikit-learn.org/stable/) models to [ONNX](https://github.com/onnx/onnx). Once in the ONNX format, you can use tools like [ONNX Runtime](https://github.com/Microsoft/onnxruntime) for high performance scoring.
```

### Comparing `skl2onnx-1.9.2/README.md` & `skl2onnx-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/api_summary.rst` & `skl2onnx-1.9.3/docs/api_summary.rst`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,33 @@
 registered, whether it is imported from another package
 or created from scratch.
 
 .. autofunction:: skl2onnx.convert_sklearn
 
 .. autofunction:: skl2onnx.to_onnx
 
+Logging
+=======
+
+.. index:: logging
+
+The conversion of a pipeline fails if it contains an object without any
+associated converter. It may also fails if one of the object is mapped
+by a custom converter. If the error message is not explicit enough,
+it is possible to enable logging:
+
+::
+
+    import logging
+    logger = logging.getLogger('skl2onnx')
+    logger.setLevel(logging.DEBUG)
+    logging.basicConfig(level=logging.DEBUG)
+
+Example :ref:`l-example-logging` illustrates what it looks like.
+
 Register a new converter
 ========================
 
 If a model has no converter
 implemented in this package, a new converter has then to be
 registered, whether it is imported from another package
 or created from scratch. Section :ref:`l-converter-list`
@@ -101,9 +120,10 @@
 .. autoclass:: skl2onnx.common._topology.Scope
     :members: get_unique_variable_name, get_unique_operator_name
 
 Topology
 --------
 
 .. autoclass:: skl2onnx.common._topology.Topology
-    :members: compile
+    :members: compile, topological_operator_iterator
 
+.. autofunction:: skl2onnx.common._topology.convert_topology
```

### Comparing `skl2onnx-1.9.2/docs/conf.py` & `skl2onnx-1.9.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,19 +118,19 @@
 sphinx_gallery_conf = {
     'examples_dirs': ['examples', 'tutorial'],
     'gallery_dirs': ['auto_examples', 'auto_tutorial'],
     'capture_repr': ('_repr_html_', '__repr__'),
     'ignore_repr_types': r'matplotlib.text|matplotlib.axes',
     'binder': {
         'org': 'onnx',
-        'repo': 'sklearn-onnx',
+        'repo': 'onnx.ai/sklearn-onnx/',
+        'notebooks_dir': 'auto_examples',
         'binderhub_url': 'https://mybinder.org',
         'branch': 'master',
-        'dependencies': os.path.abspath(
-            os.path.join(os.path.dirname(__file__), 'requirements.txt'))
+        'dependencies': './requirements.txt'
     },
 }
 
 epkg_dictionary = {
     'C': 'https://en.wikipedia.org/wiki/C_(programming_language)',
     'C++': 'https://en.wikipedia.org/wiki/C%2B%2B',
     'cython': 'https://cython.org/',
```

### Comparing `skl2onnx-1.9.2/docs/examples/Au-Salon-de-l-agriculture-la-campagne-recrute.jpg` & `skl2onnx-1.9.3/docs/examples/Au-Salon-de-l-agriculture-la-campagne-recrute.jpg`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/daisy_wikipedia.jpg` & `skl2onnx-1.9.3/docs/examples/daisy_wikipedia.jpg`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_backend.py` & `skl2onnx-1.9.3/docs/examples/plot_backend.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,24 +17,37 @@
 Let's use the API to compute the prediction
 of a simple logistic regression model.
 """
 import skl2onnx
 import onnxruntime
 import onnx
 import sklearn
+from sklearn.datasets import load_iris
+from sklearn.linear_model import LogisticRegression
 import numpy
 from onnxruntime import get_device
 import numpy as np
-from onnxruntime import datasets
 import onnxruntime.backend as backend
-from onnx import load
 
-name = datasets.get_example("logreg_iris.onnx")
-model = load(name)
 
+#######################################
+# Let's create an ONNX graph first.
+
+data = load_iris()
+X, Y = data.data, data.target
+logreg = LogisticRegression(C=1e5).fit(X, Y)
+model = skl2onnx.to_onnx(logreg, X.astype(np.float32))
+name = "logreg_iris.onnx"
+with open(name, "wb") as f:
+    f.write(model.SerializeToString())
+
+#######################################
+# Let's use ONNX backend API to test it.
+
+model = onnx.load(name)
 rep = backend.prepare(model, 'CPU')
 x = np.array([[-1.0, -2.0, 5.0, 6.0],
               [-1.0, -2.0, -3.0, -4.0],
               [-1.0, -2.0, 7.0, 8.0]],
              dtype=np.float32)
 label, proba = rep.run(x)
 print("label={}".format(label))
```

### Comparing `skl2onnx-1.9.2/docs/examples/plot_benchmark_cdist.py` & `skl2onnx-1.9.3/docs/examples/plot_benchmark_cdist.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_benchmark_pipeline.py` & `skl2onnx-1.9.3/docs/examples/plot_benchmark_pipeline.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_black_op.py` & `skl2onnx-1.9.3/docs/examples/plot_black_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_cast_transformer.py` & `skl2onnx-1.9.3/docs/examples/plot_cast_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_complex_pipeline.py` & `skl2onnx-1.9.3/docs/examples/plot_complex_pipeline.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_convert_decision_function.py` & `skl2onnx-1.9.3/docs/examples/plot_convert_decision_function.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_convert_model.py` & `skl2onnx-1.9.3/docs/examples/plot_convert_model.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_convert_syntax.py` & `skl2onnx-1.9.3/docs/examples/plot_convert_syntax.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,38 +102,41 @@
 
 class CustomOpTransformer(BaseEstimator, TransformerMixin,
                           OnnxOperatorMixin):
 
     def __init__(self):
         BaseEstimator.__init__(self)
         TransformerMixin.__init__(self)
+        self.op_version = 12
 
     def fit(self, X, y=None):
         self.W_ = np.mean(X, axis=0)
         self.S_ = np.std(X, axis=0)
         return self
 
     def transform(self, X):
         return (X - self.W_) / self.S_
 
     def onnx_shape_calculator(self):
         def shape_calculator(operator):
             operator.outputs[0].type = operator.inputs[0].type
         return shape_calculator
 
-    def to_onnx_operator(self, inputs=None, outputs=('Y', )):
+    def to_onnx_operator(self, inputs=None, outputs=('Y', ),
+                         target_opset=None, **kwargs):
         if inputs is None:
             raise RuntimeError("Parameter inputs should contain at least "
                                "one name.")
+        opv = target_opset or self.op_version
         i0 = self.get_inputs(inputs, 0)
         W = self.W_.astype(np.float32)
         S = self.S_.astype(np.float32)
         return OnnxDiv(OnnxSub(i0, W, op_version=12), S,
                        output_names=outputs,
-                       op_version=12)
+                       op_version=opv)
 
 #############################
 # Way 1
 
 
 X = np.arange(20).reshape(10, 2)
 tr = make_pipeline(CustomOpTransformer(), KMeans(n_clusters=2))
```

### Comparing `skl2onnx-1.9.2/docs/examples/plot_convert_zipmap.py` & `skl2onnx-1.9.3/docs/examples/plot_convert_zipmap.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_custom_model.py` & `skl2onnx-1.9.3/docs/examples/plot_custom_model.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_custom_parser.py` & `skl2onnx-1.9.3/docs/examples/plot_custom_parser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_custom_parser_alternative.py` & `skl2onnx-1.9.3/docs/examples/plot_custom_parser_alternative.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_errors_onnxruntime.py` & `skl2onnx-1.9.3/docs/examples/plot_errors_onnxruntime.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_gpr.py` & `skl2onnx-1.9.3/docs/examples/plot_gpr.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_intermediate_outputs.py` & `skl2onnx-1.9.3/docs/examples/plot_intermediate_outputs.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_investigate_pipeline.py` & `skl2onnx-1.9.3/docs/examples/plot_investigate_pipeline.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_metadata.py` & `skl2onnx-1.9.3/docs/examples/plot_metadata.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_nmf.py` & `skl2onnx-1.9.3/docs/examples/plot_nmf.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_onnx_operators.py` & `skl2onnx-1.9.3/docs/examples/plot_onnx_operators.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_pipeline.py` & `skl2onnx-1.9.3/docs/examples/plot_pipeline.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_pipeline_lightgbm.py` & `skl2onnx-1.9.3/docs/examples/plot_pipeline_lightgbm.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_pipeline_xgboost.py` & `skl2onnx-1.9.3/docs/examples/plot_pipeline_xgboost.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/examples/plot_tfidfvectorizer.py` & `skl2onnx-1.9.3/docs/examples/plot_tfidfvectorizer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/exts/github_link.py` & `skl2onnx-1.9.3/docs/exts/github_link.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/exts/sphinx_skl2onnx_extension.py` & `skl2onnx-1.9.3/docs/exts/sphinx_skl2onnx_extension.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/index.rst` & `skl2onnx-1.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/index_tutorial.rst` & `skl2onnx-1.9.3/docs/index_tutorial.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/introduction.rst` & `skl2onnx-1.9.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/logo_main.png` & `skl2onnx-1.9.3/docs/logo_main.png`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/parameterized.rst` & `skl2onnx-1.9.3/docs/parameterized.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/pipeline.png` & `skl2onnx-1.9.3/docs/pipeline.png`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/pipeline.rst` & `skl2onnx-1.9.3/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/supported.rst` & `skl2onnx-1.9.3/docs/supported.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tests/test_documentation_examples.py` & `skl2onnx-1.9.3/docs/tests/test_documentation_examples.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tests/test_documentation_tutorial.py` & `skl2onnx-1.9.3/docs/tests/test_documentation_tutorial.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tests/test_utils_benchmark.py` & `skl2onnx-1.9.3/docs/tests/test_utils_benchmark.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_abegin_convert_pipeline.py` & `skl2onnx-1.9.3/docs/tutorial/plot_abegin_convert_pipeline.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_bbegin_measure_time.py` & `skl2onnx-1.9.3/docs/tutorial/plot_bbegin_measure_time.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_cbegin_opset.py` & `skl2onnx-1.9.3/docs/tutorial/plot_cbegin_opset.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_dbegin_options.py` & `skl2onnx-1.9.3/docs/tutorial/plot_dbegin_options.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_dbegin_options_list.py` & `skl2onnx-1.9.3/docs/tutorial/plot_dbegin_options_list.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_ebegin_float_double.py` & `skl2onnx-1.9.3/docs/tutorial/plot_ebegin_float_double.py`

 * *Files 3% similar despite different names*

```diff
@@ -273,15 +273,20 @@
 ])
 
 model_onx.fit(Xi_train, yi_train)
 
 #############################################
 # The conversion.
 
-onx4 = to_onnx(model_onx, Xi_train[:1].astype(numpy.float32))
+try:
+    onx4 = to_onnx(model_onx, Xi_train[:1].astype(numpy.float32))
+except ValueError as e:
+    print("Failing due to %r.\nYou need to update mlprodict." % e)
+    import sys
+    sys.exit(0)
 
 sess4 = InferenceSession(onx4.SerializeToString())
 
 skl4 = model_onx.predict(X32)
 ort4 = sess4.run(None, {'X': X32})[0]
 
 print(diff(skl4, ort4))
```

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_fbegin_investigate.py` & `skl2onnx-1.9.3/docs/tutorial/plot_fbegin_investigate.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_gbegin_dataframe.py` & `skl2onnx-1.9.3/docs/tutorial/plot_gbegin_dataframe.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_gbegin_transfer_learning.py` & `skl2onnx-1.9.3/docs/tutorial/plot_gbegin_transfer_learning.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_gexternal_lightgbm.py` & `skl2onnx-1.9.3/docs/tutorial/plot_gexternal_lightgbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 """
 .. _example-lightgbm:
 
-Convert a pipeline with a LightGBM model
-========================================
+Convert a pipeline with a LightGBM classifier
+=============================================
 
 .. index:: LightGBM
 
 :epkg:`sklearn-onnx` only converts :epkg:`scikit-learn` models into *ONNX*
 but many libraries implement :epkg:`scikit-learn` API so that their models
 can be included in a :epkg:`scikit-learn` pipeline. This example considers
 a pipeline including a :epkg:`LightGBM` model. :epkg:`sklearn-onnx` can convert
```

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_gexternal_xgboost.py` & `skl2onnx-1.9.3/docs/tutorial/plot_gexternal_xgboost.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_icustom_converter.py` & `skl2onnx-1.9.3/docs/tutorial/plot_icustom_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,15 +152,18 @@
 # add tells the output type has the same type,
 # the same number of rows and a specific number of columns.
 
 
 def decorrelate_transformer_shape_calculator(operator):
     op = operator.raw_operator
     input_type = operator.inputs[0].type.__class__
-    input_dim = operator.inputs[0].type.shape[0]
+    # The shape may be unknown. *get_first_dimension*
+    # returns the appropriate value, None in most cases
+    # meaning the transformer can process any batch of observations.
+    input_dim = operator.inputs[0].get_first_dimension()
     output_type = input_type([input_dim, op.coef_.shape[1]])
     operator.outputs[0].type = output_type
 
 
 ###################################
 # The converter. One thing we need to pay attention to
 # is the target opset. This information is important
```

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_jcustom_syntax.py` & `skl2onnx-1.9.3/docs/tutorial/plot_jcustom_syntax.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,15 +89,18 @@
 # ++++++++++++++++++++
 #
 # The shape calculator does not change.
 
 def decorrelate_transformer_shape_calculator(operator):
     op = operator.raw_operator
     input_type = operator.inputs[0].type.__class__
-    input_dim = operator.inputs[0].type.shape[0]
+    # The shape may be unknown. *get_first_dimension*
+    # returns the appropriate value, None in most cases
+    # meaning the transformer can process any batch of observations.
+    input_dim = operator.inputs[0].get_first_dimension()
     output_type = input_type([input_dim, op.coef_.shape[1]])
     operator.outputs[0].type = output_type
 
 
 ###################################
 # The converter is different.
```

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_kcustom_converter_wrapper.py` & `skl2onnx-1.9.3/docs/tutorial/plot_kcustom_converter_wrapper.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_lcustom_options.py` & `skl2onnx-1.9.3/docs/tutorial/plot_lcustom_options.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_mcustom_parser.py` & `skl2onnx-1.9.3/docs/tutorial/plot_mcustom_parser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_pextend_python_runtime.py` & `skl2onnx-1.9.3/docs/tutorial/plot_pextend_python_runtime.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_qextend_onnxruntime.py` & `skl2onnx-1.9.3/docs/tutorial/plot_qextend_onnxruntime.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_usparse_xgboost.py` & `skl2onnx-1.9.3/docs/tutorial/plot_usparse_xgboost.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial/plot_wext_pyod_forest.py` & `skl2onnx-1.9.3/docs/tutorial/plot_wext_pyod_forest.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial_1_simple.rst` & `skl2onnx-1.9.3/docs/tutorial_1_simple.rst`

 * *Files 5% similar despite different names*

```diff
@@ -19,9 +19,10 @@
     auto_tutorial/plot_abegin_convert_pipeline
     auto_tutorial/plot_bbegin_measure_time
     auto_tutorial/plot_cbegin_opset
     auto_tutorial/plot_dbegin_options
     auto_tutorial/plot_dbegin_options_list
     auto_tutorial/plot_ebegin_float_double
     auto_tutorial/plot_fbegin_investigate
+    auto_tutorial/plot_gbegin_cst
     auto_tutorial/plot_gbegin_dataframe
     auto_tutorial/plot_gbegin_transfer_learning
```

### Comparing `skl2onnx-1.9.2/docs/tutorial_2-5_extlib.rst` & `skl2onnx-1.9.3/docs/tutorial_2-5_extlib.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial_2_new_converter.rst` & `skl2onnx-1.9.3/docs/tutorial_2_new_converter.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/docs/tutorial_3_new_operator.rst` & `skl2onnx-1.9.3/docs/tutorial_3_new_operator.rst`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/setup.py` & `skl2onnx-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/__init__.py` & `skl2onnx-1.9.3/skl2onnx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Main entry point to the converter from the *scikit-learn* to *onnx*.
 """
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 __author__ = "Microsoft"
 __producer__ = "skl2onnx"
 __producer_version__ = __version__
 __domain__ = "ai.onnx"
 __model_version__ = 0
 __max_supported_opset__ = 14  # Converters are tested up to this version.
```

### Comparing `skl2onnx-1.9.2/skl2onnx/_parse.py` & `skl2onnx-1.9.3/skl2onnx/_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # SPDX-License-Identifier: Apache-2.0
 
+import warnings
 import numpy as np
 
 from sklearn import pipeline
 from sklearn.base import (
-    ClassifierMixin, ClusterMixin, is_classifier
-)
+    ClassifierMixin, ClusterMixin, is_classifier)
 try:
     from sklearn.base import OutlierMixin
 except ImportError:
     # scikit-learn <= 0.19
     class OutlierMixin:
         pass
 
+from sklearn.ensemble import IsolationForest
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.linear_model import BayesianRidge
 from sklearn.model_selection import GridSearchCV
-from sklearn.neighbors import NearestNeighbors
+from sklearn.neighbors import NearestNeighbors, LocalOutlierFactor
 from sklearn.mixture import GaussianMixture, BayesianGaussianMixture
+from sklearn.multioutput import MultiOutputClassifier
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.pipeline import Pipeline
 from sklearn.svm import LinearSVC, NuSVC, SVC
 try:
     from sklearn.compose import ColumnTransformer
 except ImportError:
     # ColumnTransformer was introduced in 0.20.
@@ -45,15 +47,15 @@
 from .common._topology import Topology, Variable
 from .common.data_types import (
     DictionaryType, Int64TensorType, SequenceType,
     StringTensorType, TensorType, guess_tensor_type)
 from .common.utils import get_column_indices
 from .common.utils_checking import check_signature
 from .common.utils_classifier import get_label_classes
-from .common.utils_sklearn import has_pipeline, _process_options
+from .common.utils_sklearn import _process_options
 
 
 do_not_merge_columns = tuple(
     filter(lambda op: op is not None,
            [OneHotEncoder, ColumnTransformer]))
 
 
@@ -92,27 +94,54 @@
     :return: A list of output variables which will be passed to next
         stage
     """
     # alias can be None
     if isinstance(model, str):
         raise RuntimeError("Parameter model must be an object not a "
                            "string '{0}'.".format(model))
+    if any(not isinstance(i, Variable) for i in inputs):
+        raise TypeError(
+            "One input is not a Variable for model %r - %r."
+            "" % (model, inputs))
     alias = _get_sklearn_operator_name(type(model))
     this_operator = scope.declare_local_operator(alias, model)
     this_operator.inputs = inputs
 
     if hasattr(model, 'onnx_parser'):
-        parser_names = model.onnx_parser(scope=scope, inputs=inputs)
+        parser_names = model.onnx_parser()
         if parser_names is not None:
-            names = parser_names()
-            for name in names:
-                var = scope.declare_local_variable(
-                    name, guess_tensor_type(inputs[0].type))
-                this_operator.outputs.append(var)
-            return this_operator.outputs
+            try:
+                names = parser_names(scope=scope, inputs=inputs)
+            except TypeError as e:
+                warnings.warn(
+                    "Calling parser %r for model type %r failed due to %r. "
+                    "This warnings will become an exception in version 1.11. "
+                    "The parser signature should parser(scope=None, "
+                    "inputs=None)." % (
+                        parser_names, e, type(model)),
+                    DeprecationWarning)
+                names = parser_names()
+            if names is not None:
+                for name in names:
+                    if isinstance(name, Variable):
+                        this_operator.outputs.append(name)
+                    elif isinstance(name, str):
+                        var = scope.declare_local_variable(
+                            name, guess_tensor_type(inputs[0].type))
+                        this_operator.outputs.append(var)
+                    elif isinstance(name, tuple) and len(name) == 2:
+                        var = scope.declare_local_variable(
+                            name[0], guess_tensor_type(name[1]))
+                        this_operator.outputs.append(var)
+                    else:
+                        raise RuntimeError(
+                            "Unexpected output type %r (value=%r) for "
+                            "operator %r." % (
+                                type(name), name, type(model)))
+                return this_operator.outputs
 
     if (type(model) in sklearn_classifier_list
             or isinstance(model, ClassifierMixin)
             or (isinstance(model, GridSearchCV)
                 and is_classifier(model))):
         # For classifiers, we may have two outputs, one for label and
         # the other one for probabilities of all classes. Notice that
@@ -133,16 +162,29 @@
         label_variable = scope.declare_local_variable(
             'label', Int64TensorType())
         score_tensor_variable = scope.declare_local_variable(
             'scores', guess_tensor_type(inputs[0].type))
         this_operator.outputs.append(label_variable)
         this_operator.outputs.append(score_tensor_variable)
 
+    elif type(model) in {IsolationForest, LocalOutlierFactor}:
+        label_variable = scope.declare_local_variable(
+            'label', Int64TensorType())
+        score_tensor_variable = scope.declare_local_variable(
+            'scores', guess_tensor_type(inputs[0].type))
+        this_operator.outputs.append(label_variable)
+        this_operator.outputs.append(score_tensor_variable)
+        options = scope.get_options(model, dict(score_samples=False))
+        if options['score_samples']:
+            scores_var = scope.declare_local_variable(
+                'score_samples', guess_tensor_type(inputs[0].type))
+            this_operator.outputs.append(scores_var)
+
     elif type(model) in outlier_list or isinstance(model, OutlierMixin):
-        # For clustering, we may have two outputs, one for label and
+        # For outliers, we may have two outputs, one for label and
         # the other one for scores.
         label_variable = scope.declare_local_variable(
             'label', Int64TensorType())
         score_tensor_variable = scope.declare_local_variable(
             'scores', guess_tensor_type(inputs[0].type))
         this_operator.outputs.append(label_variable)
         this_operator.outputs.append(score_tensor_variable)
@@ -341,77 +383,96 @@
             'transformed_column', ty)
         concat_operator.outputs.append(transformed_column_name)
         return concat_operator.outputs
     return transformed_result_names
 
 
 def _parse_sklearn_grid_search_cv(scope, model, inputs, custom_parsers=None):
-    return (_parse_sklearn_classifier(
-        scope, model, inputs, custom_parsers=None)
-        if is_classifier(model) else
-        _parse_sklearn_simple_model(scope, model, inputs,
-                                    custom_parsers=custom_parsers))
+    options = scope.get_options(model)
+    if options:
+        scope.add_options(id(model.best_estimator_), options)
+    res = parse_sklearn(scope, model.best_estimator_, inputs,
+                        custom_parsers=custom_parsers)
+    scope.replace_raw_operator(
+        model.best_estimator_, model, "SklearnGridSearchCV")
+    return res
 
 
 def _parse_sklearn_classifier(scope, model, inputs, custom_parsers=None):
+    options = scope.get_options(model, dict(zipmap=True))
+    no_zipmap = (
+        (isinstance(options['zipmap'], bool) and not options['zipmap']) or
+        (model.__class__ in [NuSVC, SVC] and not model.probability))
     probability_tensor = _parse_sklearn_simple_model(
         scope, model, inputs, custom_parsers=custom_parsers)
-    if model.__class__ in [NuSVC, SVC] and not model.probability:
-        return probability_tensor
-    options = scope.get_options(model, dict(zipmap=True))
-    if isinstance(options['zipmap'], bool) and not options['zipmap']:
+    if no_zipmap:
         return probability_tensor
 
     if options['zipmap'] == 'columns':
-        this_operator = scope.declare_local_operator('SklearnZipMapColumns')
+        zipmap_operator = scope.declare_local_operator('SklearnZipMapColumns')
         classes = get_label_classes(scope, model)
         classes_names = get_label_classes(scope, model, node_names=True)
     else:
-        this_operator = scope.declare_local_operator('SklearnZipMap')
+        zipmap_operator = scope.declare_local_operator('SklearnZipMap')
         classes = get_label_classes(scope, model)
 
-    this_operator.inputs = probability_tensor
+    zipmap_operator.inputs = probability_tensor
     label_type = Int64TensorType([None])
 
     if (isinstance(model.classes_, list) and
             isinstance(model.classes_[0], np.ndarray)):
         # multi-label problem
         pass
     elif np.issubdtype(classes.dtype, np.floating):
         classes = np.array(list(map(lambda x: int(x), classes)))
         if set(map(lambda x: float(x), classes)) != set(model.classes_):
             raise RuntimeError("skl2onnx implicitly converts float class "
                                "labels into integers but at least one label "
                                "is not an integer. Class labels should "
                                "be integers or strings.")
-        this_operator.classlabels_int64s = classes
+        zipmap_operator.classlabels_int64s = classes
     elif np.issubdtype(classes.dtype, np.signedinteger):
-        this_operator.classlabels_int64s = classes
+        zipmap_operator.classlabels_int64s = classes
     elif np.issubdtype(classes.dtype, np.unsignedinteger):
-        this_operator.classlabels_int64s = classes
+        zipmap_operator.classlabels_int64s = classes
     else:
         classes = np.array([s.encode('utf-8') for s in classes])
-        this_operator.classlabels_strings = classes
+        zipmap_operator.classlabels_strings = classes
         label_type = StringTensorType([None])
 
-    output_label = scope.declare_local_variable('output_label', label_type)
-    this_operator.outputs.append(output_label)
+    zip_label = scope.declare_local_variable('output_label', label_type)
+    zipmap_operator.outputs.append(zip_label)
 
     if options['zipmap'] == 'columns':
         prob_type = probability_tensor[1].type
         for cl in classes_names:
             output_cl = scope.declare_local_variable(cl, prob_type.__class__())
-            this_operator.outputs.append(output_cl)
+            zipmap_operator.outputs.append(output_cl)
     else:
-        output_probability = scope.declare_local_variable(
+        zip_probability = scope.declare_local_variable(
             'output_probability',
             SequenceType(
                 DictionaryType(
                     label_type, guess_tensor_type(inputs[0].type))))
-        this_operator.outputs.append(output_probability)
+        zipmap_operator.outputs.append(zip_probability)
+
+    zipmap_operator.init_status(is_evaluated=True)
+    return zipmap_operator.outputs
+
+
+def _parse_sklearn_multi_output_classifier(scope, model, inputs,
+                                           custom_parsers=None):
+    alias = _get_sklearn_operator_name(type(model))
+    this_operator = scope.declare_local_operator(alias, model)
+    this_operator.inputs = inputs
+    label = scope.declare_local_variable("label", Int64TensorType())
+    proba = scope.declare_local_variable(
+        "probabilities", SequenceType(guess_tensor_type(inputs[0].type)))
+    this_operator.outputs.append(label)
+    this_operator.outputs.append(proba)
     return this_operator.outputs
 
 
 def _parse_sklearn_gaussian_process(scope, model, inputs, custom_parsers=None):
     options = scope.get_options(
         model, dict(return_cov=False, return_std=False))
     if options['return_std'] and options['return_cov']:
@@ -447,64 +508,35 @@
         # covariance or standard deviation
         covstd_tensor = scope.declare_local_variable(
             'std', guess_tensor_type(inputs[0].type))
         this_operator.outputs.append(covstd_tensor)
     return this_operator.outputs
 
 
-def _parse_sklearn(scope, model, inputs, custom_parsers=None,
-                   final_types=None):
+def _parse_sklearn(scope, model, inputs, custom_parsers=None):
     """
     This is a delegate function. It does nothing but invokes the
     correct parsing function according to the input model's type.
 
     :param scope: Scope object
     :param model: A scikit-learn object (e.g., OneHotEncoder
         and LogisticRegression)
     :param inputs: A list of variables
     :param custom_parsers: parsers determines which outputs is expected
         for which particular task, default parsers are defined for
         classifiers, regressors, pipeline but they can be rewritten,
         *custom_parsers* is a dictionary ``{ type: fct_parser(scope,
         model, inputs, custom_parsers=None) }``
-    :param final_types: a python list. Works the same way as initial_types
-        but not mandatory, it is used to overwrites the type
-        (if type is not None) and the name of every output.
     :return: The output variables produced by the input model
     """
     for i, inp in enumerate(inputs):
         if not isinstance(inp, Variable):
             raise TypeError(
                 "Unexpected input type %r for input %r: %r." % (
                     type(inp), i, inp))
-    if final_types is not None:
-        outputs = []
-        for name, ty in final_types:
-            var = scope.declare_local_variable(name, ty)
-            if var.onnx_name != name:
-                raise RuntimeError(
-                    "Unable to add duplicated output '{}', '{}'.".format(
-                        var.onnx_name, name))
-            outputs.append(var)
-        hidden_outputs = _parse_sklearn(
-            scope, model, inputs, custom_parsers=custom_parsers)
-        if len(hidden_outputs) != len(outputs):
-            raise RuntimeError(
-                "Number of declared outputs is unexpected, declared '{}' "
-                "found '{}'.".format(
-                    ", ".join(_.onnx_name for _ in outputs),
-                    ", ".join(_.onnx_name for _ in hidden_outputs)))
-        for h, o in zip(hidden_outputs, outputs):
-            if o.type is None:
-                iop = scope.declare_local_operator('SklearnIdentity')
-            else:
-                iop = scope.declare_local_operator('SklearnCast')
-            iop.inputs = [h]
-            iop.outputs = [o]
-        return outputs
 
     tmodel = type(model)
     if custom_parsers is not None and tmodel in custom_parsers:
         outputs = custom_parsers[tmodel](scope, model, inputs,
                                          custom_parsers=custom_parsers)
     elif tmodel in sklearn_parsers_map:
         outputs = sklearn_parsers_map[tmodel](scope, model, inputs,
@@ -533,48 +565,51 @@
         *custom_parsers* is a dictionary ``{ type: fct_parser(scope,
         model, inputs, custom_parsers=None) }``
     :param final_types: a python list. Works the same way as initial_types
         but not mandatory, it is used to overwrites the type
         (if type is not None) and the name of every output.
     :return: The output variables produced by the input model
     """
-    if final_types is None and has_pipeline(model):
-        try:
-            outputs = _parse_sklearn(
-                scope.temp(), model, inputs, custom_parsers=custom_parsers)
-        except RuntimeError:
-            return _parse_sklearn(
-                scope, model, inputs, custom_parsers=custom_parsers)
-
-        reserved = []
-        for o in outputs:
-            reserved.append(scope.reserve_name(o.raw_name))
-    else:
-        reserved = None
-
-    res = _parse_sklearn(
-        scope, model, inputs, custom_parsers=custom_parsers,
-        final_types=final_types)
-
-    if final_types is None and reserved is not None:
-        for r in reserved:
-            scope.unreserve_name(r)
-
+    if final_types is not None:
         outputs = []
-        for var, name in zip(res, reserved):
-            var2 = scope.declare_local_variable(name, var.type)
-            outputs.append(var2)
+        for name, ty in final_types:
+            var = scope.declare_local_output(name, ty, missing_type=True)
+            if var.onnx_name != name:
+                raise RuntimeError(
+                    "Unable to add duplicated output '{}', '{}'. "
+                    "Output and input must have different names."
+                    "".format(var.onnx_name, name))
+            outputs.append(var)
 
-        for h, o in zip(res, outputs):
-            iop = scope.declare_local_operator('SklearnIdentity')
+        hidden_outputs = _parse_sklearn(
+            scope, model, inputs, custom_parsers=custom_parsers)
+
+        if len(hidden_outputs) != len(outputs):
+            raise RuntimeError(
+                "Number of declared outputs is unexpected, declared '{}' "
+                "found '{}'.".format(
+                    ", ".join(_.onnx_name for _ in outputs),
+                    ", ".join(_.onnx_name for _ in hidden_outputs)))
+        for h, o in zip(hidden_outputs, outputs):
+            if o.type is None:
+                iop = scope.declare_local_operator('SklearnIdentity')
+            else:
+                iop = scope.declare_local_operator('SklearnCast')
             iop.inputs = [h]
             iop.outputs = [o]
-
+            h.init_status(is_leaf=False)
+            o.init_status(is_leaf=True)
+            if o.type is None and h.type is not None:
+                o.type = h.type
         return outputs
 
+    res = _parse_sklearn(
+        scope, model, inputs, custom_parsers=custom_parsers)
+    for r in res:
+        r.init_status(is_leaf=True)
     return res
 
 
 def parse_sklearn_model(model, initial_types=None, target_opset=None,
                         custom_conversion_functions=None,
                         custom_shape_calculators=None,
                         custom_parsers=None,
@@ -626,48 +661,46 @@
             conv=_converter_pool, shape=_shape_calculator_pool,
             aliases=sklearn_operator_name_map))
 
     # Declare an object to provide variables' and operators' naming mechanism.
     # In contrast to CoreML, one global scope
     # is enough for parsing scikit-learn models.
     scope = topology.declare_scope('__root__', options=options)
-
-    # Declare input variables. They should be the inputs of the scikit-learn
-    # model you want to convert into ONNX.
-    inputs = []
-    for var_name, initial_type in initial_types:
-        inputs.append(scope.declare_local_variable(var_name, initial_type))
+    inputs = scope.input_variables
 
     # The object raw_model_container is a part of the topology
     # we're going to return. We use it to store the inputs of
     # the scikit-learn's computational graph.
     for variable in inputs:
+        variable.init_status(is_root=True)
         raw_model_container.add_input(variable)
 
     # Parse the input scikit-learn model as a Topology object.
     outputs = parse_sklearn(scope, model, inputs,
                             custom_parsers=custom_parsers,
                             final_types=final_types)
 
     # The object raw_model_container is a part of the topology we're
     # going to return. We use it to store the outputs of the
     # scikit-learn's computational graph.
-    for variable in outputs:
-        raw_model_container.add_output(variable)
-
+    if final_types is not None and len(final_types) != len(outputs):
+        raise RuntimeError(
+            "Unexpected number of outputs, expected %d, got %d "
+            "after parsing." % (len(final_types), len(outputs)))
     return topology
 
 
 def build_sklearn_parsers_map():
     map_parser = {
         pipeline.Pipeline: _parse_sklearn_pipeline,
         pipeline.FeatureUnion: _parse_sklearn_feature_union,
         BayesianRidge: _parse_sklearn_bayesian_ridge,
         GaussianProcessRegressor: _parse_sklearn_gaussian_process,
         GridSearchCV: _parse_sklearn_grid_search_cv,
+        MultiOutputClassifier: _parse_sklearn_multi_output_classifier,
     }
     if ColumnTransformer is not None:
         map_parser[ColumnTransformer] = _parse_sklearn_column_transformer
 
     for tmodel in sklearn_classifier_list:
         if tmodel not in [LinearSVC]:
             map_parser[tmodel] = _parse_sklearn_classifier
```

### Comparing `skl2onnx-1.9.2/skl2onnx/_supported_operators.py` & `skl2onnx-1.9.3/skl2onnx/_supported_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,22 +77,28 @@
 from sklearn.gaussian_process import (
     GaussianProcessClassifier, GaussianProcessRegressor
 )
 
 # GridSearchCV
 from sklearn.model_selection import GridSearchCV
 
+# MultiOutput
+from sklearn.multioutput import MultiOutputClassifier, MultiOutputRegressor
+
 # Support vector machines
 from sklearn.svm import NuSVC, NuSVR, SVC, SVR
 
 # K-nearest neighbors
 from sklearn.neighbors import (
-    KNeighborsClassifier, RadiusNeighborsClassifier,
-    KNeighborsRegressor, RadiusNeighborsRegressor,
+    KNeighborsClassifier,
+    KNeighborsRegressor,
+    LocalOutlierFactor,
     NearestNeighbors,
+    RadiusNeighborsClassifier,
+    RadiusNeighborsRegressor,
 )
 try:
     from sklearn.neighbors import (
         KNeighborsTransformer,
         NeighborhoodComponentsAnalysis,
     )
 except ImportError:
@@ -122,15 +128,18 @@
 
 # Clustering
 from sklearn.cluster import KMeans, MiniBatchKMeans
 
 # Operators for preprocessing and feature engineering
 from sklearn.cross_decomposition import PLSRegression
 from sklearn.decomposition import (
-    PCA, IncrementalPCA, TruncatedSVD,
+    KernelPCA,
+    IncrementalPCA,
+    PCA,
+    TruncatedSVD,
 )
 from sklearn.feature_extraction import DictVectorizer
 from sklearn.feature_extraction.text import (
     CountVectorizer, TfidfTransformer, TfidfVectorizer
 )
 from sklearn.feature_selection import (
     GenericUnivariateSelect, RFE, RFECV,
@@ -166,18 +175,21 @@
 )
 try:
     from sklearn.preprocessing import OrdinalEncoder
 except ImportError:
     # Not available in scikit-learn < 0.20.0
     OrdinalEncoder = None
 from sklearn.preprocessing import (
-    MinMaxScaler, MaxAbsScaler,
     FunctionTransformer,
-    PolynomialFeatures, RobustScaler,
-    StandardScaler,
+    KernelCenterer,
+    MaxAbsScaler,
+    MinMaxScaler,
+    PolynomialFeatures,
+    RobustScaler,
+    StandardScaler
 )
 
 try:
     from sklearn.preprocessing import PowerTransformer
 except ImportError:
     # Not available in scikit-learn < 0.20.0
     PowerTransformer = None
@@ -197,14 +209,22 @@
         )
     except ImportError:
         HistGradientBoostingRegressor = None
         HistGradientBoostingClassifier = None
 
 from sklearn.random_projection import GaussianRandomProjection
 
+try:
+    from sklearn.compose import ColumnTransformer
+except ImportError:
+    # ColumnTransformer was introduced in 0.20.
+    ColumnTransformer = None
+
+from sklearn.pipeline import Pipeline, FeatureUnion
+
 # Custom extension
 from .sklapi import CastRegressor, CastTransformer, ReplaceTransformer
 
 from .common._registration import register_converter, register_shape_calculator
 
 # In most cases, scikit-learn operator produces only one output.
 # However, each classifier has basically two outputs; one is the
@@ -247,15 +267,15 @@
 
 # Clustering algorithms: produces two outputs, label and score for
 # each cluster in most cases.
 cluster_list = [KMeans, MiniBatchKMeans]
 
 # Outlier detection algorithms:
 # produces two outputs, label and scores
-outlier_list = [OneClassSVM, IsolationForest]
+outlier_list = [IsolationForest, LocalOutlierFactor, OneClassSVM]
 
 
 # Associate scikit-learn types with our operator names. If two
 # scikit-learn models share a single name, it means their are
 # equivalent in terms of conversion.
 def build_sklearn_operator_name_map():
     res = {k: "Sklearn" + k.__name__ for k in [
@@ -267,24 +287,26 @@
         BayesianRidge,
         BernoulliNB,
         Binarizer,
         CalibratedClassifierCV,
         CategoricalNB,
         CastRegressor,
         CastTransformer,
+        ColumnTransformer,
         ComplementNB,
         CountVectorizer,
         DictVectorizer,
         GaussianNB,
         DecisionTreeClassifier,
         DecisionTreeRegressor,
         ExtraTreeClassifier,
         ExtraTreeRegressor,
         ExtraTreesClassifier,
         ExtraTreesRegressor,
+        FeatureUnion,
         FunctionTransformer,
         GaussianMixture,
         GaussianProcessClassifier,
         GaussianProcessRegressor,
         GaussianRandomProjection,
         GenericUnivariateSelect,
         GradientBoostingClassifier,
@@ -296,34 +318,40 @@
         IsolationForest,
         KMeans,
         LabelBinarizer,
         LabelEncoder,
         LinearRegression,
         LinearSVC,
         LinearSVR,
+        LocalOutlierFactor,
         MaxAbsScaler,
         MiniBatchKMeans,
         MinMaxScaler,
         MLPClassifier,
         MLPRegressor,
         MultinomialNB,
+        MultiOutputClassifier,
+        MultiOutputRegressor,
         KBinsDiscretizer,
+        KernelCenterer,
+        KernelPCA,
         KNeighborsClassifier,
         KNeighborsRegressor,
         KNeighborsTransformer,
         KNNImputer,
         NearestNeighbors,
         NeighborhoodComponentsAnalysis,
         Normalizer,
         OneClassSVM,
         OneHotEncoder,
         OneVsRestClassifier,
         OrdinalEncoder,
         PCA,
         PLSRegression,
+        Pipeline,
         PolynomialFeatures,
         PowerTransformer,
         RadiusNeighborsClassifier,
         RadiusNeighborsRegressor,
         RandomForestClassifier,
         RandomForestRegressor,
         RANSACRegressor,
```

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/automation.py` & `skl2onnx-1.9.3/skl2onnx/algebra/automation.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/complex_functions.py` & `skl2onnx-1.9.3/skl2onnx/algebra/complex_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,20 @@
     """
     Returns the ONNX graph which computes
     ``squareform(pdist(X, metric=metric))``.
     """
     if metric == 'sqeuclidean':
         return _onnx_squareform_pdist_sqeuclidean(
             X, dtype=dtype, op_version=op_version, **kwargs)
-    elif metric == 'euclidean':
+    if metric == 'euclidean':
         res = _onnx_squareform_pdist_sqeuclidean(
             X, dtype=dtype, op_version=op_version)
         return OnnxSqrt(res, op_version=op_version, **kwargs)
-    else:
-        raise NotImplementedError("metric='{}' is not implemented.".format(
-            metric))
+    raise NotImplementedError(
+        "metric='{}' is not implemented.".format(metric))
 
 
 def _onnx_squareform_pdist_sqeuclidean(X, dtype=None, op_version=None,
                                        **kwargs):
     """
     Returns the ONNX graph which computes
     ``squareform(pdist(X, metric='sqeuclidean'))``.
```

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/custom_ops.py` & `skl2onnx-1.9.3/skl2onnx/algebra/custom_ops.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/graph_state.py` & `skl2onnx-1.9.3/skl2onnx/algebra/graph_state.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # SPDX-License-Identifier: Apache-2.0
 
+from logging import getLogger
 import numpy as np
 from scipy.sparse import coo_matrix
 from ..proto import onnx_proto, TensorProto
 from ..common.data_types import (
     guess_proto_type, _guess_numpy_type, _guess_type_proto_str,
     _guess_type_proto, FloatType, DoubleType, Int64Type, copy_type)
 from ..common._topology import Variable
 from ..common._registration import get_shape_calculator, get_converter
 
 
+logger = getLogger('skl2onnx')
+
+
 class GraphStateVar:
     pass
 
 
 class GraphState:
 
     def __init__(self, inputs, output_names, operator_name, scope,
                  container, converter, onnx_prefix_name=None,
                  options=None, expected_inputs=None,
                  expected_outputs=None, input_range=None,
                  output_range=None, operator=None,
-                 run_converters=False, **attrs):
+                 run_converters=False, input_types=None, **attrs):
+
         self.inputs = inputs
         self._output_names = output_names
         self._input_range = input_range.copy() if input_range else [1, 1e9]
         self._output_range = output_range.copy() if output_range else [1, 1e9]
         self.scope = scope
         self.run_converters = run_converters
         self.operator = operator
@@ -45,14 +50,15 @@
             None if expected_outputs is None else expected_outputs.copy())
         self.computed_inputs_ = None
         self.computed_outputs_ = None
         self.sub_op_ = None
         self.onnx_prefix_name = onnx_prefix_name
         self.attrs = attrs
         self.options = options
+        self.input_types = input_types
 
         for att in ['inputs', '_expected_inputs',
                     '_expected_outputs', 'computed_inputs_',
                     'computed_outputs_', '_outputs']:
             v = getattr(self, att, None)
             if v is None:
                 continue
@@ -283,23 +289,23 @@
         if isinstance(output, str):
             if output in output_names:
                 return (output, None)
             return (scope.get_unique_variable_name(output), None)
         if isinstance(output, tuple):
             if output[0] in output_names:
                 return output
-            return (scope.get_unique_variable_name(output[0]),
-                    output[1])
+            return (scope.get_unique_variable_name(output[0]), output[1])
         raise NotImplementedError(
             "Unexpected output type {} [{}]. "
             "You may raise an issue at https://github.com/onnx/"
             "sklearn-onnx/issues.".format(type(output), output))
 
     @staticmethod
-    def _update_inputs(inputs, names, scope, expected_inputs, input_range):
+    def _update_inputs(inputs, names, scope, expected_inputs,
+                       input_range, input_types=None):
         new_inputs = []
         for inp in inputs:
             if isinstance(inp, (Variable, tuple, GraphStateVar)):
                 new_inputs.append(inp)
                 continue
             if hasattr(inp, 'get_output_type_inference'):
                 etype = inp.get_output_type_inference(inputs)
@@ -308,32 +314,48 @@
             raise TypeError(
                 "Unable to infer shape of inputs %r (type is %r)"
                 "." % (inp, type(inp)))
 
         for i in range(0, len(new_inputs)):
             inp = new_inputs[i]
             if isinstance(inp, tuple) and len(inp) == 2:
-                stype = None if isinstance(inp[1], str) else inp[1]
-                new_inputs[i] = Variable(
-                    inp[0], inp[0], type=stype, scope=scope)
+                if input_types is not None and i < len(input_types):
+                    stype = input_types[i]
+                else:
+                    stype = None if isinstance(inp[1], str) else inp[1]
+                if scope is not None:
+                    if inp[0] in scope.variables:
+                        var = scope.variables[inp[0]]
+                        if stype is not None:
+                            var.check_compatible_type(stype)
+                    else:
+                        onnx_name = scope.get_unique_variable_name(inp[0])
+                        var = Variable(
+                            inp[0], onnx_name, type=stype, scope=scope)
+                        scope.register_variable(var)
+                else:
+                    var = Variable(inp[0], inp[0], type=stype, scope=scope)
+                new_inputs[i] = var
                 inp = new_inputs[i]
             elif isinstance(inp, GraphStateVar):
                 new_inputs[i] = inp.as_variable(scope)
                 inp = new_inputs[i]
             elif not isinstance(inp, Variable):
                 raise TypeError(
                     "Inputs %d - %r must be of type Variable." % (i, inp))
+
             if names is not None:
                 try:
-                    inp.onnx_name = (
+                    onnx_name = (
                         names[i] if isinstance(names[i], str)
                         else names[i][0])
                 except IndexError as e:
                     raise IndexError(
                         "Wrong index %d, list=%s." % (i, names)) from e
+                inp.set_onnx_name(onnx_name)
 
         # Second pass.
         if expected_inputs is not None:
             memo = {}
             for i, (name, ct) in enumerate(expected_inputs):
                 if ct in memo:
                     memo[ct].append(i)
@@ -345,18 +367,28 @@
                     ct = expected_inputs[i][1]
                     if ct in memo:
                         for j in memo[ct]:
                             if (j >= len(new_inputs) and
                                     j >= input_range[0]):
                                 continue
                             if new_inputs[j].type is not None:
-                                new_inputs[i].type = (
+                                new_inputs[i].set_type(
                                     new_inputs[j].type.__class__())
                                 break
 
+        # Overwrite types if input_types is specified.
+        if input_types is not None:
+            for i in range(len(new_inputs)):
+                if i >= len(input_types):
+                    raise RuntimeError(
+                        "Mismatch between computed inputs[%d]=%r and "
+                        "overwritten input_types[%d]=%r." % (
+                            i, new_inputs, i, input_types))
+                if input_types[i] is not None:
+                    new_inputs[i].type = input_types[i]
         return new_inputs
 
     @staticmethod
     def _update_contraints(vars1, expected1, vars2, expected2, debug=None):
         memo = {}
         for va, ex in [(vars1, expected1), (vars2, expected2)]:
             if va is None or ex is None:
@@ -383,15 +415,15 @@
         for i in range(0, len(vars1)):
             inp = vars1[i]
             if isinstance(inp, str):
                 continue
             if hasattr(inp, 'type') and inp.type is None:
                 ct = expected1[i][1]
                 if ct in memo:
-                    vars1[i].type = copy_type(memo[ct][0])
+                    vars1[i].set_type(copy_type(memo[ct][0]))
             elif isinstance(inp, tuple):
                 ct = expected1[i][1]
                 if ct in memo:
                     vars1[i] = (inp[0], copy_type(memo[ct][0]))
 
     def run(self):
         if self.computed_outputs_ is None:
@@ -413,31 +445,53 @@
             for i in self.inputs:
                 v = self._get_var_name(i, False, index=None)
                 inputs.extend(v)
 
             self.computed_inputs_ = GraphState._update_inputs(
                 self.inputs, inputs, scope=self.scope,
                 expected_inputs=self._expected_inputs,
-                input_range=self._input_range)
+                input_range=self._input_range,
+                input_types=self.input_types)
 
             name = self.scope.get_unique_operator_name(self.onnx_prefix)
             if self.is_model:
                 if self.sub_op_ is not None:
                     raise NotImplementedError(
                         "Attribute 'sub_op_' is not empty.")
 
                 # a model is converted into a subgraph
                 sub_op_inputs = self.computed_inputs_
+                for v in sub_op_inputs:
+                    if not isinstance(v, Variable):
+                        raise TypeError(
+                            "Every input variable must be a Variable not %r,"
+                            " v=%r." % (type(v), v))
+                    scope = v.scope
+                    if hasattr(scope, 'variables'):
+                        if v.onnx_name not in scope.variables:
+                            raise RuntimeError(
+                                "Variable %r missing from scope "
+                                "(operator=%r, model=%r), list=%r." % (
+                                    v, self.operator,
+                                    type(self.operator_instance),
+                                    list(sorted(self.scope.variables))))
 
                 # output are not defined, we need to call a parser.
                 from .._parse import _parse_sklearn
                 self.scope.add_options(
                     id(self.operator_instance), self.options)
-                sub_outputs = _parse_sklearn(
-                    self.scope, self.operator_instance, sub_op_inputs)
+                try:
+                    sub_outputs = _parse_sklearn(
+                        self.scope, self.operator_instance, sub_op_inputs)
+                except RuntimeError as e:
+                    raise RuntimeError(
+                        "Unable to run parser for model type %r, inputs=%r "
+                        "(input_types=%r)." % (
+                            type(self.operator_instance), sub_op_inputs,
+                            self.input_types)) from e
                 set_input_names = set(v.onnx_name for v in sub_op_inputs)
                 sub_op = None
                 for op in self.scope.operators.values():
                     for inp in op.inputs:
                         if inp.onnx_name in set_input_names:
                             sub_op = op
                 if (sub_outputs is None or
@@ -451,59 +505,99 @@
                     if not isinstance(out, Variable):
                         raise TypeError(
                             "Output %s must be of type Variable." % out)
                 self.sub_op_ = sub_op
                 sub_op.outputs = sub_outputs
 
                 shape_calc = get_shape_calculator(self.operator_name)
+                logger.debug("[StateShape] call %r fed %r - %r" % (
+                    sub_op,
+                    "".join(str(i.is_fed) for i in sub_op.inputs),
+                    "".join(str(i.is_fed) for i in sub_op.outputs)))
                 shape_calc(sub_op)
+                logger.debug("[StateShape] end - %r" % sub_op)
 
                 # Add Identity nodes to be consistent with `is_fed`
                 # in Topology.
-                if expected_outputs is not None:
+                if sub_op.outputs is not None and len(sub_op.outputs) > 0:
+                    outputs = [
+                        self.scope.declare_local_variable(
+                            o.onnx_name, type=o.type)
+                        for o in sub_op.outputs]
+                elif (expected_outputs is not None and
+                        len(expected_outputs) > 0):
                     outputs = [
                         self._get_output_name(
                             self._output_names, o, self.scope)
                         for o in expected_outputs]
                 else:
-                    outputs = [
-                        self.scope.declare_local_variable(
-                            o.onnx_name, type=o.type)
-                        for o in sub_op.outputs]
+                    raise RuntimeError(
+                        "sub_op.outputs is None as well as expected_outputs "
+                        "for operator %r." % sub_op)
+
                 if len(outputs) != len(sub_op.outputs):
                     raise RuntimeError(
                         "Mismatched number of outputs %s and %s." % (
                             outputs, sub_op.outputs))
 
                 for i, out in enumerate(sub_op.outputs):
                     var = outputs[i]
                     self.container.add_node(
                         'Identity', [out.onnx_name], [var[0]],
                         name=self.scope.get_unique_operator_name("SubOpId"))
                 self.computed_outputs_ = outputs
                 self.computed_inputs2_ = sub_op.inputs
                 self.computed_outputs2_ = [
-                    (v.raw_name, v.type) for v in self.computed_outputs_]
+                    (v[0], v[1]) for v in self.computed_outputs_]
 
                 if self.run_converters:
                     # The parser was run on sub-operators but not the
                     # converter.
                     conv = get_converter(self.operator_name)
+                    logger.debug("[StateConv] %r fed %r - %r" % (
+                        sub_op,
+                        "".join(str(i.is_fed) for i in sub_op.inputs),
+                        "".join(str(i.is_fed) for i in sub_op.outputs)))
                     conv(self.scope, sub_op, self.container)
+                    logger.debug("[StateConv] %r - end." % sub_op)
+                else:
+                    if (expected_outputs is not None and
+                            len(sub_op.outputs) == len(expected_outputs)):
+                        for v1, v2 in zip(sub_op.outputs, expected_outputs):
+                            if isinstance(v2, tuple):
+                                v2 = v2[0]
+                            if (hasattr(v1, 'onnx_name') and
+                                    hasattr(v2, 'onnx_name')):
+                                if v1.onnx_name != v2.onnx_name:
+                                    # One identity is missing
+                                    n = self.scope.get_unique_operator_name(
+                                        'idgstate')
+                                    self.container.add_node(
+                                        'Identity', [v1.onnx_name],
+                                        [v2.onnx_name], name=n)
             else:
+
+                def _name_(obj):
+                    if isinstance(obj, tuple) and len(obj) == 2:
+                        return obj[0]
+                    if hasattr(obj, 'onnx_name'):
+                        return obj.onnx_name
+                    raise TypeError(
+                        "Unable to extract variable name from %r." % obj)
+
                 # only one node is added
                 if self.options is not None:
                     raise RuntimeError(
                         "Options must be empty for node %r but is it %r." % (
                             self.operator_name, self.options))
                 outputs = [
                     self._get_output_name(self._output_names, o, self.scope)
                     for o in expected_outputs]
-                input_names = [i[0] for i in inputs]
-                output_names = [i[0] for i in outputs]
+                input_names = [_name_(i) for i in inputs]
+                output_names = [_name_(i) for i in outputs]
                 self.container.add_node(
                     self.operator_name, input_names, output_names,
                     name=name, **self.attrs)
                 computed_outputs = [
                     (name, ct[1]) for name, ct in zip(
                         output_names, self._expected_outputs)]
                 self._update_contraints(
@@ -513,13 +607,14 @@
 
                 # Registers the variables into scope.
                 self.computed_outputs_ = []
                 for name, kind in computed_outputs:
                     if isinstance(kind, str):
                         self.computed_outputs_.append((name, kind))
                     else:
-                        var = self.scope.declare_local_variable(name, kind)
+                        var = self.scope.declare_local_variable(
+                            name, kind, missing_type=True)
                         # name already comes from
                         # scope.get_unique_variable_name
-                        var.onnx_name = name
-                        var.is_fed = True
+                        var.set_onnx_name(name)
+                        var.init_status(is_fed=True)
                         self.computed_outputs_.append(var)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/onnx_operator.py` & `skl2onnx-1.9.3/skl2onnx/algebra/onnx_operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import warnings
 import numpy as np
 from scipy.sparse import coo_matrix
 from ..proto import TensorProto
 from ..common.data_types import (
     _guess_type_proto_str, _guess_type_proto_str_inv)
 from ..common._topology import (
-    Variable, Scope, _update_domain_version,
+    Variable, VariableStr, Scope, _update_domain_version, Operator,
     _get_main_opset_version, OPSET_TO_IR_VERSION)
 from ..common._container import ModelComponentContainer
 from ..common import utils
+from ..common.data_types import guess_proto_type, _guess_numpy_type
 from ..common._registration import _converter_pool, _shape_calculator_pool
 from .._supported_operators import sklearn_operator_name_map
 from ..proto import get_latest_tested_opset_version, onnx_proto
-from ..proto.onnx_helper_modified import make_graph, make_model
+from ..proto.onnx_helper_modified import make_graph, make_model, from_array
 from ..helpers.onnx_helper import infer_outputs
 from .graph_state import GraphState, GraphStateVar
 from .type_helper import _guess_type
 
 
 class OnnxOperatorItem:
     """
@@ -65,14 +66,22 @@
         """
         Returns the output.
         """
         if i != 0:
             raise IndexError("Can only return the first item.")
         return self.onx_op.get_output_name(self.index)
 
+    def get_output(self, i=0):
+        """
+        Returns the output.
+        """
+        if i != 0:
+            raise IndexError("Can only return the first item.")
+        return self.onx_op.get_output(self.index)
+
     @property
     def outputs(self):
         """
         Returns the outputs of the node.
         """
         if self.onx_op is None:
             raise RuntimeError(
@@ -132,30 +141,50 @@
 
         def __init__(self, index, name=None):
             self.index = index
             self.name = name
 
         def as_variable(self, scope):
             name = "ov%s" % self.name
-            return Variable(name, name, scope=scope, type=None)
+            if (hasattr(self, "variable_") and
+                    self.variable_.onnx_name == name):
+                return self.variable_
+            var = Variable(name, name, scope=scope, type=None)
+            if scope is not None:
+                scope.register_variable(var)
+            self.variable_ = var
+            return var
 
         def __repr__(self):
             return "OnnxOperatorVariable('%s')" % self.name
 
         def __iter__(self):
             yield self.name
             yield None
 
     class UnscopedVariable(GraphStateVar):
         def __init__(self, name):
             self.name = name
 
         def as_variable(self, scope):
             name = self.name
-            return Variable(name, name, scope=scope, type=None)
+            if (hasattr(self, "variable_") and
+                    self.variable_.onnx_name == name):
+                return self.variable_
+            if scope is not None:
+                if name in scope.variables:
+                    var = scope.variables[name]
+                else:
+                    onnx_name = scope.get_unique_variable_name(name)
+                    var = Variable(name, onnx_name, scope=scope, type=None)
+                    scope.register_variable(var)
+                self.variable_ = var
+            else:
+                var = Variable(name, name, scope=scope, type=None)
+            return var
 
         def __eq__(self, name):
             if isinstance(name, str):
                 return name == self.name
             elif isinstance(name, OnnxOperator.UnscopedVariable):
                 return self.name == name.name
             else:
@@ -170,17 +199,27 @@
             yield None
 
     class ConstantVariable(GraphStateVar):
         def __init__(self, value):
             self.value = value
 
         def as_variable(self, scope):
-            name = "id%d" % id(self)
-            return Variable(name, name, scope=scope,
-                            type=_guess_type(self.value))
+            ha = utils.hash_array(self.value)
+            name = "CST%s" % ha
+            if (hasattr(self, "variable_") and
+                    self.variable_.onnx_name == name):
+                return self.variable_
+            if scope is not None:
+                var = scope.declare_local_variable(
+                    name, type=_guess_type(self.value))
+            else:
+                var = Variable(name, name, scope=scope,
+                               type=_guess_type(self.value))
+            self.variable_ = var
+            return var
 
         @property
         def ConstantValue(self):
             return self.value
 
         def __str__(self):
             return "Cst({})".format(self.value)
@@ -214,21 +253,48 @@
                     op_version, self.since_version))
         return found
 
     def __init__(self, *inputs, op_version=None, output_names=None,
                  domain=None, **kwargs):
 
         if (output_names is None and
-                self.__class__.__name__ in {"OnnxScan"}):
+                self.__class__.__name__.startswith("OnnxScan")):
             raise NotImplementedError(
                 "The class cannot infer the number of variables "
                 "for node '{}' yet. output_names must be specified"
                 ".".format(self.__class__.__name__))
-        if isinstance(output_names, str):
+        if isinstance(output_names, (str, Variable)):
             output_names = [output_names]
+            if isinstance(output_names[0], str):
+                output_names[0] = VariableStr(output_names[0])
+        elif isinstance(output_names, Operator):
+            if len(output_names.outputs) == 0:
+                raise ValueError(
+                    "output_names cannot be empty (operator %r)."
+                    "" % output_names)
+            output_names = output_names.outputs.copy()
+        elif isinstance(output_names, Operator.OperatorList):
+            if len(output_names) == 0:
+                raise ValueError(
+                    "output_names cannot be empty (operator %r)."
+                    "" % self.__class__.__name__)
+            output_names = output_names.copy()
+        elif isinstance(output_names, list):
+            if len(output_names) == 0:
+                raise ValueError(
+                    "output_names cannot be empty (operator %r)."
+                    "" % self.__class__.__name__)
+            output_names = output_names.copy()
+            for i in range(len(output_names)):
+                if isinstance(output_names[i], str):
+                    output_names[i] = VariableStr(output_names[i])
+        elif output_names is not None:
+            raise TypeError(
+                "output_names must be a string or a list not %r."
+                "" % type(output_names))
 
         if op_version is None:
             if domain == '':
                 self.op_version = get_latest_tested_opset_version()
             else:
                 self.op_version = None
         else:
@@ -321,35 +387,32 @@
                     "Operator '{}' expects a number of inputs "
                     "in [{}, {}] not {} (expected opset={}, "
                     "class opset={})".format(
                         self.operator_name, *self.input_range,
                         len(self.inputs), op_version, self.op_version))
 
         # check output
-        if (hasattr(output_names, 'outputs') and
-                output_names.outputs is not None):
-            self.output_names = [out.onnx_name
-                                 for out in output_names.outputs]
-            self.output_variables = output_names
-        else:
-            self.output_names = output_names
-            self.output_variables = None
+        self.output_names = output_names
+        self.output_variables = None
 
-        if self.output_names:
+        if self.output_names is not None:
+            if len(self.output_names) == 0:
+                raise ValueError(
+                    "output_names can be None but cannot be empty for "
+                    "operator %r." % self)
             if self.output_variables is None:
                 self.output_variables = [None for o in self.output_names]
             for i in range(len(self.output_names)):
                 name = self.output_names[i]
                 if isinstance(name, Variable):
-                    self.output_names[i] = name.onnx_name
                     self.output_variables[i] = name
-                elif not isinstance(name, str):
+                else:
                     raise TypeError("output_names must be a list of strings "
-                                    "and element {} is {}".format(
-                                        i, type(name)))
+                                    "and element %r is %r (%r)" % (
+                                        i, type(name), name))
             if all(map(lambda x: x is None, self.output_variables)):
                 self.output_variables = None
 
         if (self.output_names is not None and (
                 self.expected_outputs is None or
                 len(self.output_names) > len(self.expected_outputs))):
             if self.expected_outputs is None:
@@ -377,14 +440,51 @@
                     while name in existing:
                         i += 1
                         name = "input%d" % (10 + i)
                     inp = (name, None)
                 self.expected_inputs.append(inp)
 
         self.output_names_ = None
+        self._post_process_attributes()
+
+    def _post_process_attributes(self):
+        """
+        Walks through attributes and replaces them by ONNX
+        values.
+        """
+        if self.__class__.__name__ == "OnnxConstantOfShape":
+            if "value" in self.kwargs:
+                value = self.kwargs['value']
+                if isinstance(value, TensorProto):
+                    return
+                if isinstance(value, np.ndarray):
+                    if value.shape == (1, ):
+                        val = value[0]
+                    elif len(value.shape) == 0:
+                        val = value
+                    else:
+                        raise RuntimeError(
+                            "Unexpected shape %r for value, it must be "
+                            "an array of one element." % value.shape)
+                    self.kwargs['value'] = from_array(
+                        np.array([val], dtype=value.dtype))
+                    return
+                raise TypeError(
+                    "Unexpected type %r for value. It should be an array "
+                    "of one element." % type(value))
+            return
+
+        if self.__class__.__name__ == "OnnxCast":
+            if "to" in self.kwargs:
+                value = self.kwargs['to']
+                if isinstance(value, int):
+                    return
+                to = guess_proto_type(_guess_numpy_type(value, None))
+                self.kwargs['to'] = to
+            return
 
     def __str__(self):
         """
         usual
         """
         return "{}({} in) -> {}".format(
             self.__class__.__name__,
@@ -428,14 +528,26 @@
         if self.state is not None:
             return self.state.computed_outputs_[i][0]
         if self.output_names_ is not None:
             return self.output_names_[i]
         self._set_output_names_(getattr(self, 'scope', None) or scope, None)
         return self.output_names_[i]
 
+    def get_output(self, i, scope=None):
+        "Returns name of output *i*."
+        if self.state is not None:
+            return self.state.computed_outputs_[i]
+        if self.output_names_ is not None:
+            res = self.output_names_[i]
+            if not isinstance(res, (tuple, Variable)):
+                raise RuntimeError(
+                        "Unable to retrieve output %r from %r."
+                        "" % (i, self))
+            return res
+
     def _set_output_names_(self, scope, operator):
         "Called by add_to."
         if operator is not None:
             self.operator_ = operator
         if self.output_names_ is not None:
             raise RuntimeError(
                 "output_names_ is already set.")
@@ -461,14 +573,19 @@
                 if name.startswith('u(') and name[-1] == ')':
                     name = scope.get_unique_variable_name(name[2:-1])
                 elif operator is not None:
                     oout = operator.outputs[iname]
                     name = oout.onnx_name
                 outputs.append(name)
             self.output_names_ = outputs
+        elif self.expected_outputs is None:
+            raise AttributeError(
+                "expected_outputs is None for operator=%r, output_names=%r, "
+                "output_variables=%r, operator=%r" % (
+                    self, self.output_names, self.output_variables, operator))
         else:
             if scope is None:
                 raise RuntimeError("scope must not be None.")
             outputs = []
             for name in self.expected_outputs:
                 name = scope.get_unique_variable_name(
                     self.onnx_prefix + "_" + name[0])
@@ -667,27 +784,28 @@
                 delattr(self, arg)
         if recursive:
             for obj in self.inputs:
                 if isinstance(obj, OnnxOperator):
                     obj._clean_attributes(*args, recursive=True)
 
     def to_onnx(self, inputs=None, outputs=None, other_outputs=None,
-                target_opset=None, domain=None):
+                target_opset=None, domain=None, verbose=0):
         """
         Converts this operator into an ONNX graph.
 
         :param inputs: specific inputs (as a dictionary) or
             default inputs if not specified
         :param outputs: specific outputs
         :param other_outputs: additional outputs to consider
             as graph outputs but not outputs of this particular
             node
         :param target_opset: dictionary with target opset per domain,
             None for the default one
         :param domain: domain of the operator
+        :param verbose: prints information
         """
         if isinstance(target_opset, dict):
             dom = self.domain or ''
             target_opset = target_opset.get(dom, None)
         elif isinstance(target_opset, int):
             if self.domain not in ('', None):
                 # The target_opset is for the domain ''
@@ -738,19 +856,19 @@
 
         target_opset = self.get_latest_tested_opset_version(target_opset)
         container = ModelComponentContainer(
             target_opset, registered_models=registered_models)
 
         model_name = self.__class__.__name__
         scope = Scope(model_name, target_opset=target_opset,
-                      variable_name_set=set(_[0] for _ in inputs),
                       registered_models=registered_models)
         for inp in inputs:
-            container.add_input(Variable(inp[0], inp[0],
-                                         scope=scope, type=inp[1]))
+            var = Variable(inp[0], inp[0], scope=scope, type=inp[1])
+            container.add_input(var)
+            scope.register_variable(var)
         self.add_to(scope, container, run_converters=True)
         if other_outputs is not None:
             for out in other_outputs:
                 if not hasattr(out, 'add_to'):
                     raise RuntimeError(
                         "Extra outputs must have method 'add_to'.")
                 out.add_to(scope, container, run_converters=True)
@@ -769,26 +887,38 @@
                     else:
                         type_shape = o[1]
                     shapes.append(Variable(o[0], o[0], None, type_shape))
                 else:
                     raise TypeError("Outputs must be Variable or "
                                     "tuple(name, type).")
         else:
+            if verbose > 0:
+                print("[op.to_onnx] infer outputs")
             shapes = infer_outputs(container, container.inputs,
                                    initializer=container.initializers,
                                    target_opset=target_opset)
-
             if self.output_names:
+                set_names = set(v.onnx_name if hasattr(v, 'onnx_name') else v
+                                for v in self.output_names)
                 shapes = [shape for shape in shapes
-                          if shape.onnx_name in self.output_names]
+                          if shape.onnx_name in set_names]
+        if verbose > 0:
+            print("[op.to_onnx] shapes=%r" % shapes)
 
         # add the output to the container
         for shape in shapes:
             container.add_output(shape)
 
+        container.ensure_topological_order()
+        if verbose >= 2:
+            print("---NODES---")
+            for node in container.nodes:
+                print("  %s - %s: %r -> %r" % (
+                    node.op_type, node.name, node.input, node.output))
+
         # convert the graph
         graph = make_graph(
             container.nodes, model_name, container.inputs,
             container.outputs, container.initializers)
         onnx_model = make_model(graph)
 
         # domains
@@ -867,20 +997,24 @@
     expected_inputs = None
     expected_outputs = None
     input_range = [1, 1e9]
     output_range = [1, 1e9]
 
     def __init__(self, skl_op, *inputs, op_version=None,
                  output_names=None, domain=None, options=None,
-                 **kwargs):
+                 input_types=None, **kwargs):
         OnnxOperator.__init__(
             self, *inputs, op_version=op_version,
             output_names=output_names, domain=domain, **kwargs)
         self.operator_instance = skl_op
         self.options = options
+        if skl_op is None and input_types is not None:
+            raise RuntimeError(
+                "input_types is only used when a sub-operator is defined.")
+        self.input_types = input_types
 
     def __repr__(self):
         return "%s(%r, %s, op_version=%r, output_names=%r)" % (
             self.__class__.__name__, self.operator_instance,
             ", ".join("%r" % i for i in self.inputs),
             self.op_version, self.output_names)
 
@@ -899,23 +1033,35 @@
                 kwargs = self.kwargs.copy()
                 del kwargs['op_version']
             else:
                 kwargs = self.kwargs
 
             if self.output_names_ is not None:
                 pass
+            elif operator is not None:
+                self.output_names_ = operator.outputs
             elif self.output_names:
                 if not isinstance(self.output_names, (list, tuple)):
                     louts = [self.output_names]
                 else:
                     louts = self.output_names
                 outputs = []
                 for name in louts:
-                    if name.startswith('u(') and name[-1] == ')':
-                        name = scope.get_unique_variable_name(name[2:-1])
+                    if (isinstance(name, str) and name.startswith('u(') and
+                            name[-1] == ')'):
+                        name = VariableStr(
+                            scope.get_unique_variable_name(name[2:-1]),
+                            scope=scope)
+                    if (isinstance(name, Variable) and
+                            name.raw_name.startswith('u(') and
+                            name.raw_name[-1] == ')'):
+                        name = VariableStr(
+                            scope.get_unique_variable_name(
+                                name.raw_name[2:-1]),
+                            scope=scope, type=name.type)
                     outputs.append(name)
                 self.output_names_ = outputs
             else:
                 self.output_names_ = None
 
             inputs = []
             for input in self.inputs:
@@ -933,33 +1079,39 @@
                             break
                     else:
                         vars = ', '.join(map(lambda o: "'%s'" % o.onnx_name,
                                              operator.inputs))
                         raise RuntimeError("Unable to find variable "
                                            "{} in {}.".format(input, vars))
                 elif isinstance(input, tuple) and len(input) == 2:
-                    inputs.append(
-                        Variable(
-                            input[0], input[0], scope=scope, type=input[1]))
+                    if scope is not None and input[0] in scope.variables:
+                        var = scope.variables[input[0]]
+                    else:
+                        var = Variable(input[0], input[0], scope=scope,
+                                       type=input[1])
+                        if scope is not None:
+                            scope.register_variable(var)
+                    inputs.append(var)
                 else:
                     inputs.append(input)
 
             self.state = GraphState(
                 inputs, self.output_names_, self.operator_instance,
                 scope, container, None, op_version=self.op_version,
                 op_domain=None, onnx_prefix_name=self.onnx_prefix,
-                options=self.options, run_converters=run_converters, **kwargs)
+                options=self.options, run_converters=run_converters,
+                input_types=self.input_types, **kwargs)
             self.state.run()
 
 
 class OnnxSubOperator(OnnxSubEstimator):
     """
     This class is deprecated and will be removed in version 1.9.
     It should be replaced by :class:`OnnxSubEstimator
     <skl2onnx.algebra.onnx_operator.OnnxSubEstimator>`.
     """
 
     def __init__(self, *args, **kwargs):
         OnnxSubEstimator.__init__(self, *args, **kwargs)
-        warnings.warn(("Class OnnxSubOperator will be removed in 1.9. "
+        warnings.warn(("Class OnnxSubOperator will be removed in 1.10. "
                        "It should be replaced by OnnxSubEstimator."),
                       DeprecationWarning)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/onnx_operator_mixin.py` & `skl2onnx-1.9.3/skl2onnx/algebra/onnx_operator_mixin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # SPDX-License-Identifier: Apache-2.0
 
+import warnings
 from sklearn.base import BaseEstimator
 from onnx import shape_inference
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 from ..common._registration import get_converter, get_shape_calculator
 from ..common._topology import Variable
 from .._supported_operators import sklearn_operator_name_map
@@ -15,15 +16,15 @@
     """
     Base class for *scikit-learn* operators
     sharing an API to convert object to *ONNX*.
     """
 
     def to_onnx(self, X=None, name=None,
                 options=None, white_op=None, black_op=None,
-                final_types=None):
+                final_types=None, target_opset=None, verbose=0):
         """
         Converts the model in *ONNX* format.
         It calls method *_to_onnx* which must be
         overloaded.
 
         :param X: training data, at least one sample,
             it is used to guess the type of the input data.
@@ -34,14 +35,16 @@
         :param white_op: white list of ONNX nodes allowed
             while converting a pipeline, if empty, all are allowed
         :param black_op: black list of ONNX nodes allowed
             while converting a pipeline, if empty, none are blacklisted
         :param final_types: a python list. Works the same way as initial_types
             but not mandatory, it is used to overwrites the type
             (if type is not None) and the name of every output.
+        :param target_opset: to overwrite `self.op_version`
+        :param verbose: displays information while converting
         """
         from .. import convert_sklearn
         if X is None:
             initial_types = self.infer_initial_types()
         else:
             initial_types = guess_initial_types(X, None)
         if not hasattr(self, 'op_version'):
@@ -49,17 +52,17 @@
                 name = self.__class__.__name__
             raise AttributeError(
                 "Attribute 'op_version' is missing for '{}' "
                 "(model: '{}').".format(
                     self.__class__.__name__, name))
         return convert_sklearn(
             self, initial_types=initial_types,
-            target_opset=self.op_version, options=options,
-            white_op=white_op, black_op=black_op,
-            final_types=final_types)
+            target_opset=target_opset or self.op_version, options=options,
+            white_op=white_op, black_op=black_op, final_types=final_types,
+            verbose=verbose)
 
     def infer_initial_types(self):
         """
         Infers initial types.
         """
         if hasattr(self, 'enumerate_initial_types'):
             return list(self.enumerate_initial_types())
@@ -80,43 +83,45 @@
         for cl in self.__class__.__bases__:
             if issubclass(cl, BaseEstimator):
                 return cl
         raise RuntimeError("Unable to find any parent inherited from "
                            "BaseEstimator: {}.".format(
                                ", ".join(map(str, self.__class__.__bases__))))
 
-    def to_onnx_operator(self, inputs=None, outputs=None):
+    def to_onnx_operator(self, inputs=None, outputs=None,
+                         target_opset=None, options=None):
         """
         This function must be overloaded.
         """
         raise NotImplementedError()
 
-    def onnx_parser(self, scope=None, inputs=None):
+    def onnx_parser(self):
         """
         Returns a parser for this model.
-        If not overloaded, it fetches the parser
+        If not overloaded, it calls the converter to guess the number
+        of outputs. If it still fails, it fetches the parser
         mapped to the first *scikit-learn* parent
         it can find.
         """
-        if inputs:
-            self.parsed_inputs_ = inputs
-        try:
-            op = self.to_onnx_operator(inputs=inputs)
-        except NotImplementedError:
-            self._find_sklearn_parent()
-            return None
+        def parser(scope=None, inputs=None):
+            try:
+                op = self.to_onnx_operator(inputs=inputs, outputs=None)
+            except NotImplementedError:
+                self._find_sklearn_parent()
+                return None
 
-        def parser():
             names = []
             while True:
                 try:
                     name = op.get_output_name(len(names), scope=scope)
                     if name is None:
                         break
                     names.append(name)
+                except AttributeError:
+                    return None
                 except IndexError:
                     break
             return names
         return parser
 
     def get_inputs(self, inputs, i):
         if i >= len(inputs):
@@ -136,20 +141,16 @@
         it can find.
         """
         if not hasattr(self, 'op_version'):
             raise AttributeError(
                 "Class '{}' should have an attribute 'op_version'.".format(
                     self.__class__.__name__))
 
-        inputs = getattr(self, "parsed_inputs_", None)
         try:
-            if inputs:
-                op = self.to_onnx_operator(inputs=inputs)
-            else:
-                op = self.to_onnx_operator()
+            op = self.to_onnx_operator()
         except NotImplementedError:
             parent = self._find_sklearn_parent()
             name = sklearn_operator_name_map.get(
                 parent, "Sklearn" + parent.__name__)
             return get_shape_calculator(name)
 
         def shape_calculator(operator):
@@ -161,34 +162,60 @@
             for o in operator.outputs:
                 name = o.onnx_name
                 if name not in shapes:
                     raise RuntimeError("Shape of output '{}' cannot be "
                                        "infered. onnx_shape_calculator "
                                        "must be overriden and return "
                                        "a shape calculator.".format(name))
-                o.type = shapes[name].type
+                o.set_type(shapes[name].type)
 
         return shape_calculator
 
     def onnx_converter(self):
         """
         Returns a converter for this model.
         If not overloaded, it fetches the converter
         mapped to the first *scikit-learn* parent
         it can find.
         """
-        inputs = getattr(self, "parsed_inputs_", None)
-        try:
-            if inputs:
-                op = self.to_onnx_operator(inputs=inputs)
-            else:
-                op = self.to_onnx_operator()
-        except NotImplementedError:
-            parent = self._find_sklearn_parent()
-            name = sklearn_operator_name_map[parent]
-            return get_converter(name)
-
         def converter(scope: Scope, operator: Operator,
                       container: ModelComponentContainer):
+            inputs = operator.inputs  # getattr(self, "parsed_inputs_", None)
+            outputs = operator.outputs  # kwargs.get('outputs', None)
+            op_version = container.target_opset
+            options = scope.get_options(operator.raw_operator, fail=False)
+            try:
+                if inputs:
+                    op = self.to_onnx_operator(
+                        inputs=inputs, outputs=outputs,
+                        target_opset=op_version, options=options)
+                else:
+                    op = self.to_onnx_operator(
+                        target_opset=op_version,
+                        outputs=outputs, options=options)
+            except TypeError:
+                warnings.warn(
+                    "Signature should be to_onnx_operator(self, inputs=None, "
+                    "outputs=None, target_opset=None, **kwargs). "
+                    "This will be the case in version 1.11, class=%r."
+                    "" % type(self),
+                    DeprecationWarning)
+                try:
+                    if inputs:
+                        op = self.to_onnx_operator(
+                            inputs=inputs, outputs=outputs)
+                    else:
+                        op = self.to_onnx_operator()
+                except NotImplementedError:
+                    parent = self._find_sklearn_parent()
+                    name = sklearn_operator_name_map[parent]
+                    conv = get_converter(name)
+                    return conv(scope, operator, container)
+            except NotImplementedError:
+                parent = self._find_sklearn_parent()
+                name = sklearn_operator_name_map[parent]
+                conv = get_converter(name)
+                return conv(scope, operator, container)
+
             op.add_to(scope, container, operator=operator)
 
         return converter
```

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/onnx_ops.py` & `skl2onnx-1.9.3/skl2onnx/algebra/onnx_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,16 @@
                      'operator_name': op_name,
                      'input_range': input_range,
                      'output_range': output_range,
                      'domain': domain,
                      'is_deprecated': deprecated,
                      'since_version': since_version,
                      'past_version': past_version,
-                     'attr_names': attr_names})
+                     'attr_names': attr_names,
+                     '__module__': __name__})
     return newclass
 
 
 def dynamic_class_creation():
     """
     Automatically generates classes for each of the operators
     module *onnx* defines and described at
```

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/sklearn_ops.py` & `skl2onnx-1.9.3/skl2onnx/algebra/sklearn_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
                     {'__doc__': doc,
                      'operator_name': skl_obj.__name__,
                      '_fct_converter': conv,
                      '_fct_shape_calc': shape_calc,
                      'input_range': [1, 1e9],
                      'output_range': [1, 1e9],
                      'op_version': None,
-                     'alias': alias})
+                     'alias': alias,
+                     '__module__': __name__})
     return newclass
 
 
 def dynamic_class_creation_sklearn():
     """
     Automatically generates classes for each of the converter.
     """
```

### Comparing `skl2onnx-1.9.2/skl2onnx/algebra/type_helper.py` & `skl2onnx-1.9.3/skl2onnx/algebra/type_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import numpy as np
+try:
+    from pandas import DataFrame
+except ImportError:
+    DataFrame = None
 from scipy.sparse import coo_matrix
 from ..proto import TensorProto, ValueInfoProto
 from ..common._topology import Variable
 from ..common.data_types import (
     _guess_numpy_type,
     _guess_type_proto,
     BooleanTensorType,
@@ -75,10 +79,25 @@
 
 def guess_initial_types(X, initial_types):
     if X is None and initial_types is None:
         raise NotImplementedError("Initial types must be specified.")
     if initial_types is None:
         if isinstance(X, np.ndarray):
             X = X[:1]
-        gt = _guess_type(X)
-        initial_types = [('X', gt)]
+            gt = _guess_type(X)
+            initial_types = [('X', gt)]
+        elif DataFrame is not None and isinstance(X, DataFrame):
+            X = X[:1]
+            initial_types = []
+            for c in X.columns:
+                if isinstance(X[c].values[0], (str, np.str_)):
+                    g = StringTensorType()
+                else:
+                    g = _guess_type(X[c].values)
+                g.shape = [None, 1]
+                initial_types.append((c, g))
+        elif isinstance(X, list):
+            initial_types = X
+        else:
+            raise TypeError(
+                "Unexpected type %r, unable to guess type." % type(X))
     return initial_types
```

### Comparing `skl2onnx-1.9.2/skl2onnx/common/_apply_operation.py` & `skl2onnx-1.9.3/skl2onnx/common/_apply_operation.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/common/_container.py` & `skl2onnx-1.9.3/skl2onnx/common/_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 import inspect
 import re
 import sys
 import traceback
 import warnings
+from logging import getLogger
 import numpy as np
 from scipy.sparse import coo_matrix
 from onnx.defs import onnx_opset_version, get_all_schemas_with_history
 import onnx.onnx_cpp2py_export.defs as C
 from onnxconverter_common.onnx_ops import __dict__ as dict_apply_operation
 from ..proto import TensorProto
 from ..proto.onnx_helper_modified import (
@@ -18,18 +19,20 @@
 try:
     from ..proto import SparseTensorProto
     from ..proto.onnx_helper_modified import make_sparse_tensor
 except ImportError:
     # onnx is too old.
     SparseTensorProto = None
     make_sparse_tensor = None
-from .interface import ModelContainer
 from .utils import get_domain
 
 
+logger = getLogger('skl2onnx')
+
+
 def _get_operation_list():
     """
     Investigates this module to extract all ONNX functions
     which needs to be converted with these functions.
     """
     regs = [re.compile("container.add_node[(]'([A-Z][a-zA-Z0-9]*)', "
                        "\\[?input_name"),
@@ -193,15 +196,15 @@
     def add_output(self, variable):
         # The order of adding variables matters. The final model's
         # output names are sequentially added as this list
         if variable not in self._outputs:
             self._outputs.append(variable)
 
 
-class ModelComponentContainer(ModelContainer, _WhiteBlackContainer):
+class ModelComponentContainer(_WhiteBlackContainer):
     """
     In the conversion phase, this class is used to collect all materials
     required to build an *ONNX* *GraphProto*, which is encapsulated in a
     *ONNX* *ModelProto*.
     """
 
     def __init__(self, target_opset, options=None, registered_models=None,
@@ -245,14 +248,87 @@
             self.target_opset = target_opset
             self.target_opset_all = {'': target_opset}
         # Additional options given to converters.
         self.options = options
         # All registered models.
         self.registered_models = registered_models
 
+    def swap_names(self, old_name, new_name):
+        """
+        Swaps variables names.
+
+        :param old_name: old name
+        :param new_name: new name
+        :return: list of impacted objects
+        """
+        exc_list = {'Scan', 'Loop', 'If'}
+        for node in self.nodes:
+            if node.op_type not in exc_list:
+                continue
+            if (old_name in node.input or old_name in node.output or
+                    new_name in node.input or new_name in node.output):
+                raise NotImplementedError(
+                    "Unable to handle subgraphs for node type %r."
+                    "(%r, %r)" % (node.op_type, old_name, new_name))
+        res = []
+
+        for inp in self.inputs:
+            if inp.name == old_name:
+                inp.name = new_name
+                res.append(('Io', inp))
+            elif inp.name == new_name:
+                inp.name = old_name
+                res.append(('In', inp))
+
+        for inp in self.outputs:
+            if inp.name == old_name:
+                inp.name = new_name
+                res.append(('Oo', inp))
+            elif inp.name == new_name:
+                inp.name = old_name
+                res.append(('On', inp))
+
+        for inp in self.initializers:
+            if inp.name == old_name:
+                inp.name = new_name
+                res.append(('-o', inp))
+            elif inp.name == new_name:
+                inp.name = old_name
+                res.append(('-n', inp))
+
+        for node in self.nodes:
+            modified = False
+            new_input = []
+            for name in node.input:
+                if name == old_name:
+                    name = new_name
+                    modified = True
+                elif name == new_name:
+                    name = old_name
+                    modified = True
+                new_input.append(name)
+            new_output = []
+            for name in node.output:
+                if name == old_name:
+                    name = new_name
+                    modified = True
+                elif name == new_name:
+                    name = old_name
+                    modified = True
+                new_output.append(name)
+            if modified:
+                if node.op_type in exc_list:
+                    raise NotImplementedError(
+                        "Unable to handle subgraphs for node type %r."
+                        "" % node.op_type)
+                node.input[:] = new_input[:]
+                node.output[:] = new_output[:]
+                res.append(("n-", node))
+        return res
+
     def __str__(self):
         """
         Shows internal information.
         """
         rows = []
         if self.inputs:
             rows.append("INPUTS")
@@ -336,14 +412,15 @@
         :param onnx_type: Element types allowed in ONNX tensor, e.g.,
                           TensorProto.FLOAT and TensorProto.STRING.
         :param shape: Tensor shape, a list of integers.
         :param content: Flattened tensor values (i.e., a float list
                         or a float array).
         :return: created tensor
         """
+        logger.debug("[Init] %r, %r, %r" % (name, onnx_type, shape))
         sparse_tensor = None
         tensor = None
 
         cached_value = None
         if isinstance(content, TensorProto):
             tensor = TensorProto()
             tensor.data_type = content.data_type
@@ -500,14 +577,16 @@
         if op_version is None:
             op_version = self._get_op_version(op_domain, op_type)
 
         if isinstance(inputs, str):
             inputs = [inputs]
         if isinstance(outputs, str):
             outputs = [outputs]
+        logger.debug("[Node] %r - %r -> %r (name=%r)" % (
+            op_type, ",".join(inputs), ",".join(outputs), name))
         try:
             common = set(inputs) & set(outputs)
         except TypeError as e:
             raise TypeError(
                 "inputs or outputs are wrong, inputs=%r, outputs=%r, node=%r."
                 "" % (inputs, outputs, op_type)) from e
         if common:
@@ -562,17 +641,19 @@
         self.node_domain_version_pair_sets.add((op_domain, op_version))
         self.nodes.append(node)
         if (self.target_opset is not None and
                 op_version is not None and
                 op_version > self.target_opset_any_domain(op_domain)):
             raise RuntimeError(
                 "Opset number {} is higher than targeted opsets {} for "
-                "node '{}' (domain: '{}').".format(
+                "node type '{}' name='{}' input={} "
+                "output={} (domain='{}').".format(
                     op_version, self.target_opset_all,
-                    node.op_type, op_domain))
+                    node.op_type, node.name,
+                    node.input, node.output, op_domain))
 
     def target_opset_any_domain(self, domain):
         target_opset = self.target_opset_all
         if isinstance(target_opset, dict):
             if domain in target_opset:
                 to = target_opset[domain]
             else:
@@ -699,15 +780,17 @@
         order = {}
         for inp in self.inputs:
             name = inp.name
             order[name] = 0
         for inp in self.initializers:
             name = inp.name
             order[name] = 0
+
         n_iter = 0
+        missing_ops = []
         while n_iter < len(self.nodes) * 2:
             n_iter += 1
             missing_names = set()
             missing_ops = []
             for node in self.nodes:
                 maxi = 0
                 for name in node.input:
@@ -726,16 +809,16 @@
                 maxi += 1
                 order[key] = maxi
                 maxi += 1
                 for name in node.output:
                     if name in order:
                         raise RuntimeError(
                             "Unable to sort a node (cycle). An output was "
-                            "already ordered %r (iteration=%r)." % (
-                                name, n_iter))
+                            "already ordered with name %r (iteration=%r)."
+                            "" % (name, n_iter))
                     order[name] = maxi
             if len(missing_names) == 0:
                 continue
 
         if len(missing_ops) > 0:
             def nstr(name):
                 if name in order:
@@ -746,16 +829,16 @@
                 ', '.join(map(nstr, n.input)),
                 ', '.join(n.output))
                 for n in missing_ops]
             rows.insert(0, "")
             rows.append("--")
             rows.append("--all-nodes--")
             rows.append("--")
-            rows.extend("%s(%s) -> [%s]" % (
-                n.name or n.op_type,
+            rows.extend("%s|%s(%s) -> [%s]" % (
+                n.op_type, n.name or n.op_type,
                 ', '.join(map(nstr, n.input)),
                 ', '.join(n.output))
                 for n in self.nodes)
             raise RuntimeError(
                 "After %d iterations for %d nodes, still unable "
                 "to sort names %r. The graph may be disconnected. "
                 "List of operators: %s" % (
```

### Comparing `skl2onnx-1.9.2/skl2onnx/common/_onnx_optimisation_common.py` & `skl2onnx-1.9.3/skl2onnx/common/_onnx_optimisation_common.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/common/_registration.py` & `skl2onnx-1.9.3/skl2onnx/common/_registration.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,17 @@
                       this function is trying to assign an existing
                       key (i.e., operator_name) a new value
                       (i.e., conversion_function). Set this flag to True
                       to enable overwriting.
     :param options: supported options for this converter
         (dictionary {name: supported values or None})
     """
+    if conversion_function is None:
+        raise ValueError(
+            "A converter cannot be None for %r." % operator_name)
     if not overwrite and operator_name in _converter_pool:
         raise ValueError('We do not overwrite registered converter '
                          'by default')
     if len(_converter_pool) > 0:
         key = next(iter(_converter_pool))
         check_signature(conversion_function, _converter_pool[key]._fct,
                         skip=('operator', ))
@@ -78,14 +81,17 @@
     :param calculator_function: A callable object
     :param overwrite: By default, we raise an exception if the caller
                       of this function is trying to assign an existing
                       key (i.e., operator_name) a new value
                       (i.e., calculator_function). Set this flag to True
                       to enable overwriting.
     """
+    if calculator_function is None:
+        raise ValueError(
+            "A shape calculator cannot be None for %r." % operator_name)
     if not overwrite and operator_name in _shape_calculator_pool:
         raise ValueError('We do not overwrite registrated shape calculator '
                          'by default')
     if calculator_function is not None and len(_shape_calculator_pool) > 0:
         key = next(iter(_shape_calculator_pool))
         check_signature(calculator_function, _shape_calculator_pool[key],
                         skip=('operator', ))
```

### Comparing `skl2onnx-1.9.2/skl2onnx/common/_topology.py` & `skl2onnx-1.9.3/skl2onnx/common/_topology.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 import re
 import warnings
 import pprint
+from logging import getLogger
+from collections import OrderedDict
 import numpy as np
 from onnx import onnx_pb as onnx_proto
 from onnxconverter_common.data_types import (  # noqa
     DataType, TensorType,
     FloatType, Int64Type, StringType,
     DictionaryType, FloatTensorType,  # noqa
     Int64TensorType, SequenceType,  # noqa
@@ -27,37 +29,44 @@
 from ..proto.onnx_helper_modified import (
     make_graph, make_model, make_tensor_value_info
 )
 from . import _registration
 from . import utils
 from .exceptions import MissingShapeCalculator, MissingConverter
 from ._container import ModelComponentContainer, _build_options
-from .interface import OperatorBase
 from .onnx_optimisation_identity import onnx_remove_node_identity
+
 type_fct = type
 
 
+def _default_OPSET_TO_IR_VERSION():
+    return {
+        1: 3, 2: 3, 3: 3, 4: 3, 5: 3, 6: 3,
+        7: 3, 8: 4, 9: 4, 10: 5, 11: 6, 12: 7,
+        13: 7, 14: 7, 15: 8
+    }
+
+
 try:
     from onnxconverter_common.topology import OPSET_TO_IR_VERSION
     assert OPSET_TO_IR_VERSION[14] is not None
 except (ImportError, KeyError):
-    OPSET_TO_IR_VERSION = {
-        1: 3, 2: 3, 3: 3, 4: 3, 5: 3, 6: 3,
-        7: 3, 8: 4, 9: 4, 10: 5, 11: 6, 12: 7,
-        13: 7, 14: 7
-    }
+    OPSET_TO_IR_VERSION = _default_OPSET_TO_IR_VERSION()
 
-OPSET_ML_TO_OPSET = {1: 11, 2: 13}
+OPSET_ML_TO_OPSET = {1: 11, 2: 14}
+
+logger = getLogger('skl2onnx')
 
 
 class Variable:
     """
     Defines a variable which holds any data defined
     from *ONNX* types.
     """
+    _UNIQUE_NUMBER_ = 0
 
     def __init__(self, raw_name, onnx_name, scope, type=None):
         """
         :param raw_name: A string indicating the variable's name in the
                          original model. Usually, it's the seed string
                          used to created its ONNX name (i.e., the
                          field *onnx_name* below).
@@ -67,75 +76,192 @@
                       variable is declared
         :param type: A type object defined in .common.data_types.py;
                      e.g., FloatTensorType
         """
         if not isinstance(raw_name, str):
             raise TypeError(
                 "raw_name must be a string not '%s'." % raw_name.__class__)
-        if not isinstance(onnx_name, str) or '(' in onnx_name:
+        if type is not None and not hasattr(type, 'shape'):
             raise TypeError(
-                "raw_name must be a string not %r." % type(onnx_name))
+                "Unexpected type for variable raw_name=%r, type=%r." % (
+                    raw_name, type))
+        if not isinstance(onnx_name, str) or '(' in onnx_name:
+            if onnx_name.startswith('u(') and onnx_name[-1] == ')':
+                onnx_name0 = onnx_name
+                if scope is None:
+                    onnx_name = "UU%03dUU" % Variable._UNIQUE_NUMBER_
+                    Variable._UNIQUE_NUMBER_ += 1
+                else:
+                    onnx_name = scope.get_unique_variable_name("U")
+                logger.debug(
+                    '[Var] rename raw_name=%r, onnx_name=%r into %r' % (
+                        raw_name, onnx_name0, onnx_name))
+            else:
+                raise TypeError(
+                    "onnx_name must be a string not %r." % onnx_name)
 
         if type is not None:
             shape = type.shape
             if shape is not None:
                 not_none = [v for v in shape if v is not None]
                 if len(not_none) and min(not_none) == 0:
                     raise RuntimeError(
                         "A variable cannot be empty, raw_name=%r, "
                         "onnx_name=%r, shape=%r, type=%r." % (
                             raw_name, onnx_name, shape, type))
 
-        self.raw_name = raw_name  #
-        self.onnx_name = onnx_name  #
-        self.scope = scope
-        self.type = type
+        self._raw_name = raw_name
+        self._onnx_name = onnx_name
+        self._scope = scope
+        self._type = type
+        self._parent = None
+
         # The following fields are bool variables used in parsing and
         # compiling stages
-        self.is_fed = None
-        self.is_root = None
-        self.is_leaf = None
-        self.is_abandoned = False
+        self._is_fed = None
+        self._is_root = None
+        self._is_leaf = None
         if self.type is not None and not isinstance(self.type, DataType):
             raise TypeError(
                 "shape must be a DataType not {}.".format(self.type))
         if isinstance(self.type, TensorType):
             shape = self.type.shape
             if not isinstance(shape, (list, tuple)):
                 try:
                     shape = list(shape)
                 except TypeError:
                     raise TypeError("shape must be a tuple or a list not "
                                     "{}.".format(type_fct(shape)))
             for dim in shape:
                 if dim is None:
                     continue
-                if not isinstance(dim, (int, np.int32, np.int64)):
-                    raise TypeError("shape must contains integers not "
-                                    "'{}'.".format(dim))
+                if not isinstance(dim, (int, np.int32, np.int64, np.intc)):
+                    raise TypeError(
+                        "shape must contains integers not %r (type=%r)."
+                        "" % (dim, dim.__class__))
+        logger.debug('[Var] +%s' % self)
+
+        # links to operators using those variables
+        self.operators_outputs_ = []
+        self.operators_inputs_ = []
+        self._check()
+
+    def _check(self):
+        if self.type is not None and self.type.shape is not None:
+            for k in self.type.shape:
+                if k is None:
+                    continue
+                if not isinstance(k, (int, np.int64, np.intc)):
+                    raise ValueError(
+                        "Unexpected type %r for shape %r."
+                        "" % (type(k), self))
+
+    @property
+    def raw_name(self):
+        return self._raw_name
+
+    @property
+    def onnx_name(self):
+        return self._onnx_name
+
+    @property
+    def scope(self):
+        return self._scope
+
+    @property
+    def type(self):
+        return self._type
+
+    @property
+    def is_fed(self):
+        return self._is_fed
+
+    @property
+    def is_root(self):
+        return self._is_root
+
+    @property
+    def is_leaf(self):
+        return self._is_leaf
+
+    def init_status(self, is_fed=None, is_root=None, is_leaf=None):
+        if is_fed is not None and is_fed != self.is_fed:
+            logger.debug('[Var] update is_fed=%r for %r, parent=%r' % (
+                is_fed, self, self._parent))
+            self._is_fed = is_fed
+        if is_root is not None and is_root != self.is_root:
+            logger.debug('[Var] update is_root=%r for %r' % (is_root, self))
+            self._is_root = is_root
+        if is_leaf is not None and is_leaf != self.is_leaf:
+            logger.debug('[Var] update is_leaf=%r for %r' % (is_leaf, self))
+            self._is_leaf = is_leaf
+
+    def __setattr__(self, name, value):
+        if name == "type":
+            self.set_type(value)
+        elif name == "onnx_name":
+            raise AttributeError("You must use method set_onnx_name.")
+        elif name in {"is_fed", "is_root", "is_leaf"}:
+            raise AttributeError("You must use method init_status.")
+        elif name in {'scope', 'raw_name'}:
+            raise AttributeError("scope or raw_name cannot be changed.")
+        self.__dict__[name] = value
+
+    def set_type(self, new_type):
+        if (new_type is None or isinstance(new_type, (str, Variable)) or
+                not hasattr(new_type, 'shape')):
+            raise TypeError(
+                "Unexpected new type for variable %r, new_type=%r." % (
+                    self, new_type))
+        logger.debug('[Var] update type for %r' % self)
+        self._type = new_type
+        self._check()
+
+    def set_onnx_name(self, onnx_name):
+        if onnx_name != self._onnx_name:
+            logger.debug('[Var] update onnx_name, from %r to %r in %r' % (
+                self.onnx_name, onnx_name, self))
+            if self.scope is not None and not isinstance(self.scope, str):
+                self.scope.rename_onnx_name(self._onnx_name, onnx_name)
+            self._onnx_name = onnx_name
+
+    def set_parent(self, operator):
+        if self._parent is not None:
+            raise RuntimeError(
+                "This variable is already the output of operator %r. "
+                "It cannot be the output of %r." % (self._parent, operator))
+        logger.debug('[Var] set parent for %r, parent=%r' % (
+            self, operator))
+        self._parent = operator
 
     def get_first_dimension(self):
         """
         Returns the first dimension (batch dimension) or
         None if not specified (shape is empty).
         """
         if (self.type is None or self.type.shape is None or
                 len(self.type.shape) == 0):
             return None
         return self.type.shape[0]
 
+    def get_second_dimension(self):
+        if (self.type is None or self.type.shape is None or
+                len(self.type.shape) < 2):
+            return None
+        return self.type.shape[1]
+
     @property
     def full_name(self):
         """
         Return a globally unique variable ID
         """
         return self.onnx_name
 
     def __repr__(self):
-        return ("Variable(raw_name='{0}', onnx_name='{1}', type={2})".format(
+        return ("Variable('{0}', '{1}', type={2})".format(
                 self.raw_name, self.onnx_name, self.type))
 
     @staticmethod
     def from_pb(obj):
         """
         Creates a data type from a protobuf object.
         """
@@ -199,19 +325,124 @@
     def __getitem__(self, index):
         if index == 0:
             return self.onnx_name
         if index == 1:
             return self.type
         raise IndexError("Unreachable element at index %d." % index)
 
+    def add_operator(self, op, in_or_out):
+        "Add a link to an operator, True for output, False for input."
+        if in_or_out:
+            self.operators_outputs_.append(op)
+        else:
+            self.operators_inputs_.append(op)
+
+    def check_compatible_type(self, other_type):
+
+        def empty_shape(shape):
+            return shape is None or len(shape) == 0
+
+        if self.type is None:
+            if other_type is None:
+                return
+        elif other_type is not None:
+            if type(self.type) == type(other_type):
+                if self.type.shape == other_type.shape:
+                    return
+                if empty_shape(other_type.shape):
+                    return
+        raise TypeError(
+            "Incompatible type for variable %r and type %r." % (
+                self, other_type))
+
 
-class Operator(OperatorBase):
+class VariableStr(Variable):
+    """
+    Defines a variable a string. This should be avoided.
+    """
+
+    def __init__(self, name, scope=None, type=None):
+        Variable.__init__(self, name, name, scope=scope, type=type)
+
+    @property
+    def raw_name(self):
+        return self._raw_name
+
+    @property
+    def onnx_name(self):
+        if self._onnx_name.startswith("u("):
+            raise RuntimeError(
+                "Variable should be renamed as onnx_name=%r."
+                "" % self._onnx_name)
+        return self._onnx_name
+
+
+class Operator:
     """
     Defines an operator available in *ONNX*.
     """
+    class OperatorList(list):
+        def __init__(self, parent, kind):
+            super(Operator.OperatorList, self).__init__()
+            self.parent = parent
+            self.kind = kind
+
+        def __eq__(self, second):
+            raise NotImplementedError(
+                "Operator equal not implemented and not needed.")
+
+        def append(self, v):
+            if not isinstance(v, Variable):
+                raise TypeError(
+                    "Input and output must be of type Variable not %r."
+                    "" % type(v))
+            if self.kind == 'Out':
+                v.set_parent(self.parent)
+            super(Operator.OperatorList, self).append(v)
+            logger.debug("[Op] add %s %r to %r" % (self.kind, v, self.parent))
+            if self.kind == 'In':
+                v.add_operator(self.parent, False)
+            elif self.kind == "Out":
+                v.add_operator(self.parent, True)
+            else:
+                raise RuntimeError(
+                    "Unexpected value for kind=%r." % self.kind)
+
+        def extend(self, vs):
+            for v in vs:
+                self.append(v)
+
+        def __getitem__(self, i):
+            v = list.__getitem__(self, i)
+            if isinstance(i, int) and not isinstance(v, Variable):
+                raise TypeError("Element %d must be a Variable not %r." % (
+                    i, type(v)))
+            return v
+
+        def __setitem__(self, i, v):
+            raise LookupError(
+                "Setter should not be used to modify an element.")
+
+        def set_element(self, i, v):
+            "Updates element i."
+            if not isinstance(v, Variable):
+                raise TypeError(
+                    "Value v must be a Variable not %r." % type(v))
+            logger.debug("[Op] %s-change element %d from %r to %r in %r" % (
+                self.kind, i, self[i], v, self.parent))
+            list.__setitem__(self, i, v)
+
+        def to_string(self):
+            names = []
+            for o in self:
+                if hasattr(o, 'onnx_name'):
+                    names.append(o.onnx_name)
+                else:
+                    names.append('"%s"' % str(o))
+            return ",".join(names)
 
     def __init__(self, onnx_name, scope, type, raw_operator,
                  target_opset, scope_inst):
         """
         :param onnx_name: A unique ID, which is a string
         :param scope: The name of the scope where this operator is
                       declared. It's a string.
@@ -232,28 +463,79 @@
         # is not None, output_shapes can be guessed
         # from the raw model. Otherwise, it can be guessed
         # from the input shapes.
         self.onnx_name = onnx_name
         self.scope = scope
         self.type = type
         self.raw_operator = raw_operator
-        self.inputs = []
-        self.outputs = []
-        self.is_evaluated = None
-        self.is_abandoned = False
+        self.inputs = Operator.OperatorList(self, 'In')
+        self.outputs = Operator.OperatorList(self, 'Out')
+        self._is_evaluated = None
         self.target_opset = target_opset
         self.scope_inst = scope_inst
+        logger.debug('[Op] +%r' % self)
+
+    def new_raw_operator(self, raw_operator, alias):
+        """
+        Returns a shallow copy of this operator,
+        changes the raw_operator but keeps the same inputs
+        and outputs.
+        """
+        op = Operator(self.onnx_name, self.scope, alias, raw_operator,
+                      self.target_opset, self.scope_inst)
+        op.inputs = self.inputs
+        op.outputs = self.outputs
+        return op
 
     def __repr__(self):
+        try:
+            textop = repr(self.raw_operator)
+        except AttributeError:
+            textop = "MISSING OP"
+        except KeyError:
+            # The line above fails for python 3.7
+            textop = type(self.raw_operator)
+        if isinstance(textop, str) and "\n" in textop:
+            textop = textop.replace('\n', '').replace(' ', '')
         return ("Operator(type='{0}', onnx_name='{1}', inputs='{2}', "
                 "outputs='{3}', raw_operator={4})".format(
                     self.type, self.onnx_name,
-                    ','.join(v.onnx_name for v in self.inputs),
-                    ','.join(v.onnx_name for v in self.outputs),
-                    self.raw_operator))
+                    self.inputs.to_string(),
+                    self.outputs.to_string(),
+                    textop))
+
+    def __setattr__(self, name, value):
+        if name in ('inputs', 'outputs'):
+            if (isinstance(value, list) and
+                    not isinstance(value, Operator.OperatorList)):
+                if name == 'inputs':
+                    self.inputs = Operator.OperatorList(self, 'In')
+                    self.inputs.extend(value)
+                    return
+                if name == 'outputs':
+                    self.outputs = Operator.OperatorList(self, 'Out')
+                    self.outputs.extend(value)
+                    return
+            if not isinstance(value, Operator.OperatorList):
+                raise TypeError(
+                    "inputs or outputs must be of type Operator.OperatorList.")
+            ioo = name == 'outputs'
+            for v in value:
+                v.add_operator(self, ioo)
+        self.__dict__[name] = value
+
+    @property
+    def is_evaluated(self):
+        return self._is_evaluated
+
+    def init_status(self, is_evaluated=None):
+        if is_evaluated is not None and is_evaluated != self.is_evaluated:
+            logger.debug('[Op] update is_evaluated=%r for %r' % (
+                is_evaluated, self))
+            self._is_evaluated = is_evaluated
 
     @property
     def full_name(self):
         """
         Return a globally unique operator ID
         """
         return self.onnx_name
@@ -287,95 +569,81 @@
                     type(self.raw_operator)))
         try:
             shape_calc = _registration.get_shape_calculator(self.type)
         except ValueError:
             raise MissingShapeCalculator(
                 "Unable to find a shape calculator for alias '{}' "
                 "and type '{}'.".format(self.type, type(self.raw_operator)))
+        if shape_calc is None:
+            raise MissingShapeCalculator(
+                "Unexpected shape calculator for alias '{}' "
+                "and type '{}'.".format(self.type, type(self.raw_operator)))
+        logger.debug("[Shape-a] %r fed %r - %r" % (
+            self,
+            "".join(str(i.is_fed) for i in self.inputs),
+            "".join(str(i.is_fed) for i in self.outputs)))
         shape_calc(self)
+        logger.debug("[Shape-b] %r inputs=%r - outputs=%r" % (
+            self, self.inputs, self.outputs))
 
 
 class Scope:
     """
     Every node of an *ONNX* graph must be unique. This class holds the list
     of existing name for every node already defined in graph. It also
     provides functions to create a unique unused name.
     """
 
-    def __init__(self, name, parent_scopes=None, variable_name_set=None,
-                 operator_name_set=None, target_opset=None,
+    def __init__(self, name, target_opset=None,
                  custom_shape_calculators=None, options=None,
                  registered_models=None):
         """
         :param name: A string, the unique ID of this scope in a
                      Topology object
-        :param parent_scopes: A list of Scope objects. The last element
-                              should be the direct parent scope (i.e.,
-                              where this scope is declared).
-        :param variable_name_set: A set of strings serving as the name
-                                  pool of variables
-        :param operator_name_set: A set of strings serving as the name
-                                  pool of operators
         :param target_opset: The target opset number for the converted
                              model.
         :param custom_conversion_functions: a dictionary for specifying
                                 the user customized conversion function
         :param custom_shape_calculators: a dictionary for specifying
                                 the user customized shape calculator
         :param options: see :ref:`l-conv-options`
         :param registered_models: registered models
         """
         self.name = name
-        self.parent_scopes = parent_scopes if parent_scopes else list()
-        self.onnx_variable_names = (
-            variable_name_set if variable_name_set is not None else set())
-        self.onnx_operator_names = (
-            operator_name_set if operator_name_set is not None else set())
+        self.onnx_variable_names = set()
+        self.onnx_operator_names = set()
         self.target_opset = target_opset
         self.custom_shape_calculators = custom_shape_calculators
 
         # An one-to-many map from raw variable name to ONNX variable
         # names. It looks like
         # (key, value) = (raw_name, [onnx_name, onnx_name1, onnx_name2, ..., onnx_nameN]) # noqa
         # The last name may hide all other names in this scope.
         self.variable_name_mapping = {}
 
         # A map of local variables defined in this scope.
         # (key, value) = (onnx_name, variable)
-        self.variables = {}
+        self.variables = OrderedDict()
+        self.input_variables = []
+        self.output_variables = []
 
         # A map of local operators defined in this scope.
         # (key, value) = (onnx_name, operator)
         self.operators = {}
 
         # Additional options given to converters.
         self.options = options
 
         # Registered models
         self.registered_models = registered_models
 
-        # Reserved variables.
-        self.reserved = {}
-
     def get(self, var_name, default_value):
         "Returns variable with 'name' or default value is not found."
         return self.variables.get(var_name, default_value)
 
-    def temp(self):
-        """
-        Creates a new Scope with the same options but no names.
-        """
-        scope = Scope(
-            'temp', parent_scopes=self.parent_scopes,
-            target_opset=self.target_opset,
-            custom_shape_calculators=self.custom_shape_calculators,
-            options=self.options,
-            registered_models=self.registered_models)
-        return scope
-
     def has_variable_name(self, name):
         """
         Tells if a variable is already registered.
         """
         return name in self.onnx_variable_names
 
     def get_shape_calculator(self, model_type):
@@ -399,89 +667,96 @@
 
     def get_unique_operator_name(self, seed):
         """
         Creates a unique operator ID based on the given seed.
         """
         return Topology._generate_unique_name(seed, self.onnx_operator_names)
 
-    def declare_local_variable(self, raw_name, type=None, prepend=False):
+    def declare_local_variable(self, raw_name, type=None, prepend=False,
+                               missing_type=False):
         """
         This function may create a new variable in this scope. If
         *raw_name* has been used to create other variables, the new
         variable will hide all other variables created using *raw_name*.
         """
+        if type is None and not missing_type:
+            raise RuntimeError(
+                "Unknown type for %r (type=%r)." % (raw_name, type))
         # Get unique ID for the new variable
         onnx_name = self.get_unique_variable_name(raw_name)
 
         # Create the variable
         variable = Variable(raw_name, onnx_name, self.name, type)
-        self.variables[onnx_name] = variable
+        self.register_variable(variable, prepend=prepend)
+        return variable
+
+    def register_variable(self, var, prepend=False):
+        "Adds a variable to the scope."
+        if var.onnx_name in self.variables:
+            raise RuntimeError(
+                "Variable %r already registered (other=%r)." % (
+                    var, self.variables[var.onnx_name]))
 
-        if raw_name in self.variable_name_mapping:
+        if var.raw_name in self.variable_name_mapping:
             # Hide existing variables with the same raw_name
             if not prepend:
-                self.variable_name_mapping[raw_name].append(onnx_name)
+                self.variable_name_mapping[var.raw_name].append(var.onnx_name)
             else:
-                self.variable_name_mapping[raw_name].insert(0, onnx_name)
+                self.variable_name_mapping[var.raw_name].insert(
+                    0, var.onnx_name)
         else:
-            self.variable_name_mapping[raw_name] = [onnx_name]
-        return variable
+            self.variable_name_mapping[var.raw_name] = [var.onnx_name]
 
-    def reserve_name(self, raw_name):
-        """
-        Keeps this name to be used by other converters.
-        """
-        if raw_name in self.reserved:
-            raise RuntimeError(
-                "Name '{}' already reserved.".format(raw_name))
-        self.reserved[raw_name] = self.get_unique_variable_name(raw_name)
-        return raw_name
+        self.variables[var.onnx_name] = var
 
-    def unreserve_name(self, name):
-        """
-        Deletes a name from the reserved list.
-        """
-        if name not in self.reserved:
+    def rename_onnx_name(self, old_name, new_name):
+        if new_name in self.variables:
+            raise RuntimeError(
+                "Name %r already in variables (%r)." % (
+                    new_name, self.variables[new_name]))
+        if old_name not in self.variables:
             raise RuntimeError(
-                "Name '{}' not reserved.".format(name))
-        self.onnx_variable_names.discard(name)
-        del self.reserved[name]
+                "Unable to find name %r in variables." % old_name)
+        logger.debug('[Scope] update onnx_name, from %r to %r' % (
+            old_name, new_name))
+        self.variables[new_name] = self.variables[old_name]
+        del self.variables[old_name]
+
+    def declare_local_input(self, raw_name, type=None, prepend=False):
+        """
+        Calls `declare_local_variable`. Registers this variable
+        as an input.
+        """
+        var = self.declare_local_variable(
+            raw_name, type=type, prepend=prepend)
+        self.input_variables.append(var)
+        return var
+
+    def declare_local_output(self, raw_name, type=None, prepend=False,
+                             missing_type=False):
+        """
+        Calls `declare_local_variable`. Registers this variable
+        as an output.
+        """
+        var = self.declare_local_variable(
+            raw_name, type=type, prepend=prepend,
+            missing_type=missing_type)
+        self.output_variables.append(var)
+        return var
 
     def declare_local_operator(self, type, raw_model=None):
         """
         This function is used to declare new local operator.
         """
         onnx_name = self.get_unique_operator_name(str(type))
         operator = Operator(onnx_name, self.name, type, raw_model,
                             self.target_opset, scope_inst=self)
         self.operators[onnx_name] = operator
         return operator
 
-    def delete_local_operator(self, onnx_name):
-        """
-        Removes the operator whose onnx_name is the input *onnx_name*.
-        """
-        if (onnx_name not in self.onnx_operator_names or
-                onnx_name not in self.operators):
-            raise RuntimeError('The operator to remove was not found.')
-        self.onnx_operator_names.discard(onnx_name)
-        del self.operators[onnx_name]
-
-    def delete_local_variable(self, onnx_name):
-        """
-        Removes the variable whose *onnx_name* is the input *onnx_name*.
-        """
-        if (onnx_name not in self.onnx_variable_names or
-                onnx_name not in self.variables):
-            raise RuntimeError('The variable to remove was not found.')
-        self.onnx_variable_names.discard(onnx_name)
-        raw_name = self.variables[onnx_name].raw_name
-        self.variable_name_mapping[raw_name].remove(onnx_name)
-        del self.variables[onnx_name]
-
     def _get_allowed_options(self, model, fail=True):
         if self.registered_models is not None:
             if type(model) not in self.registered_models['aliases']:
                 if fail:
                     raise NotImplementedError(
                         "No registered models, no known allowed options "
                         "for model '{}'.".format(model.__class__.__name__))
@@ -525,27 +800,36 @@
         :return: dictionary
         """
         return _build_options(
             model, self.options, default_values,
             self._get_allowed_options(model, fail=fail),
             fail=fail)
 
+    def replace_raw_operator(self, op1, op2, alias):
+        """
+        Replaces every raw operator op1 by op2.
+        The function uses `id()` to detect op1.
+        """
+        for v in self.operators.values():
+            if id(v.raw_operator) == id(op1):
+                logger.debug('[Scope] replace %d by %d in %r.' % (
+                    id(v.raw_operator), id(op1), v))
+                v.raw_operator = op2
+                v.type = alias
+
 
 class Topology:
     """
     Holds instances on :class:`Scope <skl2onnx.common._topology.Scope>` and
-    :class:`SklearnModelContainer <skl2onnx.common._container.SklearnModelContainer>`.
+    :class:`SklearnModelContainer
+    <skl2onnx.common._container.SklearnModelContainer>`.
     These are filled by the converters while a pipeline is being converted.
-    When all converters were called, method
-    :meth:`Topology.compile <skl2onnx.common._topology.Topology.compile>`
-    must be called to convert the topological graph into *ONNX* graph.
-    """  # noqa
+    """
 
     def __init__(self, model, default_batch_size=1, initial_types=None,
-                 reserved_variable_names=None, reserved_operator_names=None,
                  target_opset=None, custom_conversion_functions=None,
                  custom_shape_calculators=None, registered_models=None):
         """
         Initializes a *Topology* object, which is an intermediate
         representation of a computational graph.
 
         :param model: RawModelContainer object or one of its derived
@@ -553,53 +837,31 @@
         :param default_batch_size: batch_size prepend to scalar and
                                    array types from CoreML. It's usually
                                    1 or None.
         :param initial_types: A list providing some types for some
                               root variables.
         Each element is a tuple of a variable name and a type defined
         in *data_types.py*.
-        :param reserved_variable_names: A set of strings which are not
-                                        allowed to be used as a variable
-                                        name
-        :param reserved_operator_names: A set of strings which are not
-                                        allowed to be used as a operator
-                                        name
         :param custom_conversion_functions: a dictionary for specifying
                                 the user customized conversion function
         :param custom_shape_calculators: a dictionary for specifying the
                                         user customized shape calculator
         :param registered_models: registered models
         """
         self.scopes = []
         self.raw_model = model
         self.scope_names = set()
-        self.variable_name_set = (
-            reserved_variable_names
-            if reserved_variable_names is not None else set())
-        self.operator_name_set = (
-            reserved_operator_names
-            if reserved_operator_names is not None else set())
         self.initial_types = initial_types if initial_types else list()
         self.default_batch_size = default_batch_size
         self.target_opset = target_opset
         self.custom_conversion_functions = (
             custom_conversion_functions if custom_conversion_functions else {})
         self.custom_shape_calculators = (
             custom_shape_calculators if custom_shape_calculators else {})
 
-        # This attribute is used in optimizing the graph structure. If
-        # root_names is not empty, only the variables specified will be
-        # treated as the roots (i.e., set is_fed to True in the
-        # beginning of a graph evaluation) of the graph. Specifying all
-        # root variables in this list and leaving it empty are
-        # equivalent. This attribute directly affects
-        # _initialize_graph_status_for_traversing function and
-        # indirectly affects _infer_all_shapes and _prune functions.
-        self.root_names = list()
-
         for k in self.custom_conversion_functions:
             if not callable(k):
                 raise TypeError("Keys in custom_conversion_functions must be "
                                 "types not strings.")
         for k in self.custom_shape_calculators:
             if not callable(k):
                 raise TypeError("Keys in custom_shape_calculators must be "
@@ -614,14 +876,21 @@
             self.model_aliases[mtype] = alias
 
         # Registered models
         if registered_models is None:
             raise AssertionError()
         self.registered_models = registered_models
 
+    @property
+    def scope(self):
+        if len(self.scopes) != 1:
+            raise RuntimeError(
+                "Only one scope is allowed not %d." % len(self.scopes))
+        return self.scopes[0]
+
     @staticmethod
     def _generate_unique_name(seed, existing_names):
         """
         Produce an unique string based on the seed
         :param seed: a string
         :param existing_names: a set containing strings which cannot be
                                produced
@@ -654,400 +923,360 @@
         return Topology._generate_unique_name(seed, self.scope_names)
 
     def declare_scope(self, seed, parent_scopes=None, options=None):
         """
         Creates a new :class:`Scope <skl2onnx.common._topology.Scope>`
         and appends it to the list of existing scopes.
         """
+        if len(self.scopes) != 0:
+            raise RuntimeError(
+                "Only one scope can be created.")
         scope = Scope(
-            self.get_unique_scope_name(seed), parent_scopes,
-            self.variable_name_set, self.operator_name_set, self.target_opset,
+            self.get_unique_scope_name(seed), target_opset=self.target_opset,
             custom_shape_calculators=self.custom_shape_calculators,
             options=options, registered_models=self.registered_models)
+
+        # Declare input variables.
+        # They should be the inputs of the scikit-learn
+        # model you want to convert into ONNX.
+        for var_name, initial_type in self.initial_types:
+            scope.declare_local_input(var_name, initial_type)
         self.scopes.append(scope)
         return scope
 
     def unordered_operator_iterator(self):
         for scope in self.scopes:
             for operator in scope.operators.values():
                 yield operator
 
     def unordered_variable_iterator(self):
         for scope in self.scopes:
             for variable in scope.variables.values():
                 yield variable
 
-    def topological_operator_iterator(self):
-        """
-        This is an iterator of all operators in Topology object.
-        Operators may be produced in a topological order. If you want to
-        simply go though all operators without considering their
-        topological structure, please use another function,
-        unordered_operator_iterator.
-        """
-        self._initialize_graph_status_for_traversing()
-        priorities = {
-            'tensorToProbabilityMap': 2,
-            'tensorToLabel': 1
-        }
-        while not all(operator.is_evaluated for scope in self.scopes
-                      for operator in scope.operators.values()):
-            is_evaluation_happened = False
-            for operator in sorted(self.unordered_operator_iterator(),
-                                   key=lambda op: priorities[op.type]
-                                   if op.type in priorities else 0):
-                if not isinstance(operator.inputs, list):
-                    raise TypeError(
-                        "operator.inputs must be a list not {}".format(
-                            type(operator.inputs)))
+    def call_converter(self, operator, container, verbose=0):
+        "Calls converter for operator *operator*."
+        mtype = type(operator.raw_operator)
+        if mtype in self.custom_conversion_functions:
+            conv = self.custom_conversion_functions[mtype]
+        elif operator.type in self.custom_conversion_functions:
+            conv = self.custom_conversion_functions[operator.type]
+        elif hasattr(operator.raw_operator, "onnx_converter"):
+            conv = operator.raw_operator.onnx_converter()
+        else:
+            # Convert the selected operator into some ONNX objects and
+            # save them into the container
+            try:
+                conv = _registration.get_converter(operator.type)
+            except ValueError:
+                raise MissingConverter(
+                    "Unable to find converter for alias '{}' type "
+                    "'{}'. You may raise an issue at "
+                    "https://github.com/onnx/sklearn-onnx/issues."
+                    "".format(operator.type,
+                              type(getattr(operator, 'raw_model', None))))
 
-                if (all(variable.is_fed for variable in operator.inputs)
-                        and not operator.is_evaluated):
-                    # Check if over-writing problem occurs (i.e., multiple
-                    # operators produce results on one variable).
-                    for variable in operator.outputs:
-                        # Throw an error if this variable has been treated as
-                        # an output somewhere
-                        if variable.is_fed:
-                            add = ["", "--DEBUG-INFO--"]
-                            add.append("self.variable_name_set=%s" % (
-                                pprint.pformat(self.variable_name_set)))
-                            add.append("self.operator_name_set=%s" % (
-                                pprint.pformat(self.operator_name_set)))
-                            for scope in self.scopes:
-                                add.append(pprint.pformat(
-                                    scope.variable_name_mapping))
-                                for var in scope.variables.values():
-                                    add.append("   is_fed=%s %s" % (
-                                        getattr(var, 'is_fed', '?'), var))
-                                for op in scope.operators.values():
-                                    add.append("   is_evaluated=%s %s" % (
-                                        getattr(op, 'is_evaluated', '?'), op))
-                            raise RuntimeError(
-                                "A variable is already assigned ({}) "
-                                "for operator '{}' (name='{}'). This "
-                                "may still happen if a converter is a "
-                                "combination of sub-estimators and one "
-                                "of them is producing this output. "
-                                "In that case, an identity node must be "
-                                "added.{}".format(
-                                    variable, operator.type,
-                                    operator.onnx_name,
-                                    "\n".join(add)))
-                        # Mark this variable as filled
-                        variable.is_fed = True
-
-                    # Make this operator as handled
-                    operator.is_evaluated = True
-                    is_evaluation_happened = True
-
-                    # Send out an operator
-                    yield operator
-
-                    # This step may create new nodes if the
-                    # the converter is called while looping on
-                    # the nodes. The outputs of an operator
-                    # are not necessary the inputs of the next
-                    # one and but can processed by other ONNX nodes
-                    # inserted in the container. As a result, some
-                    # variables never have is_fed set to True which
-                    # is updated now unless they are an operator
-                    # output.
-                    known_outputs = {}
-                    for op in self.unordered_operator_iterator():
-                        for out in op.outputs:
-                            if hasattr(out, 'onnx_name'):
-                                known_outputs[out.onnx_name] = out
-                            else:
-                                known_outputs[out] = out
-                    for variable in self.unordered_variable_iterator():
-                        if variable.is_fed:
-                            continue
-                        if variable.onnx_name in known_outputs:
-                            continue
-                        update = (False if self.root_names and
-                                  variable.onnx_name not in self.root_names
-                                  else True)
-                        if update:
-                            variable.is_fed = True
-                            is_evaluation_happened = True
-
-            # After scanning through the whole computational graph, at
-            # least one operator should be evaluated. If not, we need
-            # to terminate this procedure to avoid dead lock.
-            if not is_evaluation_happened:
-                for op in self.unordered_operator_iterator():
-                    if not op.is_evaluated and op.raw_operator is not None:
-                        raise RuntimeError(
-                            "One operator was not evaluated ("
-                            "inputs fed=%r, outputs fed=%r, op=%r)." % (
-                                all(variable.is_fed
-                                    for variable in operator.inputs),
-                                all(variable.is_fed
-                                    for variable in operator.outputs),
-                                op))
-                break
-
-    def _check_structure(self):
-        """
-        This function applies some rules to check if the parsed model is
-        proper. Currently, it only checks if isolated variable and
-        isolated operator exists.
-        """
-        # Collect all variable names and operator names
-        unused_variables = set()
-        unused_operators = set()
-        for variable in self.unordered_variable_iterator():
-            unused_variables.add(variable.full_name)
-        for operator in self.unordered_operator_iterator():
-            unused_operators.add(operator.full_name)
+        container.validate_options(operator)
+        if verbose > 0:
+            print("[call_converter] call converter for %r." % operator.type)
+        logger.debug("[Conv] call %r fed %r - %r" % (
+            operator,
+            "".join(str(i.is_fed) for i in operator.inputs),
+            "".join(str(i.is_fed) for i in operator.outputs)))
+        conv(self.scopes[0], operator, container)
+        logger.debug("[Conv] end - %r" % operator)
 
-        for operator in self.unordered_operator_iterator():
-            for variable in operator.inputs:
-                # A variable is used by an operator, so we remove the
-                # variable from the unused-variable list.
-                unused_variables.discard(variable.full_name)
-                # A operator has an input, so we remove the operator
-                # from the unused-operator list.
-                unused_operators.discard(operator.full_name)
-            for variable in operator.outputs:
-                # A variable is used by an operator, so we remove the
-                # variable from the unused-variable list.
-                unused_variables.discard(variable.full_name)
-                # A operator has an output, so we remove the operator
-                # from the unused-operator list.
-                unused_operators.discard(operator.full_name)
-
-        if len(unused_variables) > 0:
-            raise RuntimeError('Isolated variables exist: %s'
-                               % unused_variables)
-
-        if len(unused_operators) > 0:
-            raise RuntimeError('Isolated operators exist: %s'
-                               % unused_operators)
+    def call_shape_calculator(self, operator):
+        "Calls shape_calculator for operator *operator*."
+        mtype = type(operator.raw_operator)
+        if mtype in self.custom_shape_calculators:
+            # overwritten operator.
+            source = 'custom'
+            shape_calc = self.custom_shape_calculators[mtype]
+        elif operator.type in self.custom_shape_calculators:
+            source = 'custom'
+            shape_calc = self.custom_shape_calculators[operator.type]
+        elif hasattr(operator.raw_operator, "onnx_shape_calculator"):
+            source = 'onnx_shape_calculator'
+            shape_calc = operator.raw_operator.onnx_shape_calculator()
+        else:
+            source = ""
+            shape_calc = None
+
+        if shape_calc is not None:
+            logger.debug("[Shape1] %r fed %r - %r (source=%r)" % (
+                operator,
+                ",".join(str(i.is_fed) for i in operator.inputs),
+                ",".join(str(i.is_fed) for i in operator.outputs),
+                source))
+            shape_calc(operator)
+        else:
+            logger.debug('[Shape2] call infer_types for %r' % operator)
+            operator.infer_types()
 
     def _initialize_graph_status_for_traversing(self):
         """
-        Initialize the status of all variables and operators for
-        traversing the underline graph
+        Initialize the status of all variables and operators before
+        traversing the graph. Only used by convert_operators.
         """
-        # In the beginning, we set is_root and is_leaf true. For is_fed,
-        # we have two different behaviors depending on whether
-        # root_names is empty.
+        if len(self.scopes) != 1:
+            raise RuntimeError(
+                "Only one scope is allowed not %d." % len(self.scopes))
+        input_names = set(v.onnx_name for v in self.scopes[0].input_variables)
+        if len(input_names) == 0:
+            raise RuntimeError("No detected inputs.")
         for variable in self.unordered_variable_iterator():
-            # If root_names is set, we only set those variable to be
-            # fed. Otherwise, all roots would be fed.
-            variable.is_fed = (False if self.root_names and variable.onnx_name
-                               not in self.root_names else True)
-            variable.is_root = True
-            variable.is_leaf = True
-
-        # Then, we flip some flags by applying some simple rules so
-        # that only
-        #   1. all roots get is_root=True and is_fed=True
-        #   2. all leaves get is_leaf=True
+            is_input = variable.onnx_name in input_names
+            variable.init_status(is_fed=is_input)
+
         for operator in self.unordered_operator_iterator():
-            # All operators are not processed in the beginning
-            operator.is_evaluated = False
-            for variable in operator.outputs:
-                # Output cannot be fed before graph traversing
-                variable.is_fed = False
-                # If the variable is an output of one operator,
-                # it must not be a root
-                variable.is_root = False
-            for variable in operator.inputs:
-                # If the variable is an input of one operator,
-                # it must not be a leaf
-                variable.is_leaf = False
+            operator.init_status(is_evaluated=False)
 
-    def _infer_all_types(self):
+    def _propagate_status(self, operator, container, fed_variables):
         """
-        Infer all variables' shapes in the computational graph.
+        Propagates status *is_fed* based on output variable
+        and node added in the container.
         """
-        self._initialize_graph_status_for_traversing()
-
-        # Deliver user-specified types to root variables
-        for raw_name, initial_type in self.initial_types:
-            # Check all variables declared using raw_name in
-            # the whole graph
-            for scope in self.scopes:
-                # Skip scopes without having the considered variable
-                # name
-                if raw_name not in scope.variable_name_mapping:
+        vars = {}
+        for node in container.nodes:
+            for i in node.input:
+                if i not in vars:
+                    vars[i] = []
+                vars[i].append(node)
+
+        stack = [v.onnx_name for v in operator.outputs if v.is_fed]
+        stack.extend(v.onnx_name for v in operator.inputs if v.is_fed)
+        scope = self.scopes[0]
+        while len(stack) > 0:
+            nodes = {}
+            for name in stack:
+                if name not in vars:
                     continue
-                # Assign initial_type to all variables declared using
-                # raw_name
-                for onnx_name in scope.variable_name_mapping[raw_name]:
-                    variable = scope.variables[onnx_name]
-                    if variable.is_root:
-                        # Assign type to the root; existing type
-                        # produced by parser may be overwritten
-                        variable.type = initial_type
-
-        # Traverse the graph from roots to leaves
-        for operator in self.topological_operator_iterator():
-            mtype = type(operator.raw_operator)
-            if mtype in self.custom_shape_calculators:
-                # overwritten operator.
-                self.custom_shape_calculators[mtype](operator)
-            elif operator.type in self.custom_shape_calculators:
-                self.custom_shape_calculators[operator.type](operator)
-            elif hasattr(operator.raw_operator, "onnx_shape_calculator"):
-                shape_calc = operator.raw_operator.onnx_shape_calculator()
-                shape_calc(operator)
-            else:
-                operator.infer_types()
+                for n in vars[name]:
+                    nodes[id(n)] = n
+            stack = []
+            for node in nodes.values():
+                if all(fed_variables.get(n, False) for n in node.input):
+                    for o in node.output:
+                        if o not in fed_variables:
+                            fed_variables[o] = o
+                            stack.append(o)
+                            if o in scope.variables:
+                                var = scope.variables[o]
+                                var.init_status(is_fed=True)
+
+    def convert_operators(self, container=None, verbose=0):
+        """
+        Calls all converters and shape_calculator for existing
+        operators. It also processes new operators created by
+        converters.
+        """
+        def _check_operator_(operator):
+            if not isinstance(operator.inputs, Operator.OperatorList):
+                raise TypeError(
+                    "operator.inputs must be a Operator.OperatorList "
+                    "not %r." % type(operator.inputs))
+            if not isinstance(operator.outputs, Operator.OperatorList):
+                raise TypeError(
+                    "operator.outputs must be a Operator.OperatorList "
+                    "not %r." % type(operator.outputs))
+            if any(not isinstance(i, Variable) for i in operator.inputs):
+                raise TypeError(
+                    "One input is not a Variable for operator %r - %r."
+                    "" % (type(operator.raw_operator), operator))
+            if any(not isinstance(i, Variable) for i in operator.outputs):
+                raise TypeError(
+                    "One output is not a Variable for operator %r - %r."
+                    "" % (type(operator.raw_operator), operator))
+
+        def _check_variable_in_(variable, operator):
+            idop = id(operator)
+            ids = set(id(op) for op in variable.operators_inputs_)
+            if idop not in ids:
+                raise RuntimeError(
+                    "Operator %r not registered in the list of operators "
+                    "of %r taking it as an input [\n%s]." % (
+                        operator, variable,
+                        "\n".join(map(str, variable.operators_inputs_))))
+
+        def _check_variable_out_(variable, operator):
+            if variable.is_fed:
+                add = ["", "--DEBUG-INFO--"]
+                for scope in self.scopes:
+                    add.append('---')
+                    add.append(pprint.pformat(
+                        scope.variable_name_mapping))
+                    add.append('---')
+                    for var in scope.variables.values():
+                        add.append("   is_fed=%s %s - n_in=%d n_out=%d" % (
+                            getattr(var, 'is_fed', '?'), var,
+                            len(var.operators_inputs_),
+                            len(var.operators_outputs_)))
+                    add.append('---')
+                    for op in scope.operators.values():
+                        add.append("   is_evaluated=%s %s" % (
+                            getattr(op, 'is_evaluated', '?'), op))
+                add.append('---')
+                for v in operator.inputs:
+                    add.append(" inputs={}".format(v))
+                for v in operator.outputs:
+                    add.append(" outputs={}".format(v))
+                add.append('--- operator producing this variable--')
+                for op in variable.operators_outputs_:
+                    add.append(str(op))
+                raise RuntimeError(
+                    "A variable is already assigned ({}) "
+                    "for operator '{}' (name='{}'). "
+                    "operator.is_evaluated={}, inputs.is_fed={}, "
+                    "outputs.is_fed={}. "
+                    "This may still happen if a converter is a "
+                    "combination of sub-estimators and one "
+                    "of them is producing this output. "
+                    "In that case, an identity node must be "
+                    "added.{}".format(
+                        variable, operator.type,
+                        operator.onnx_name, operator.is_evaluated,
+                        [v.is_fed for v in operator.inputs],
+                        [v.is_fed for v in operator.outputs],
+                        "\n".join(add)))
 
-    def _resolve_duplicates(self):
-        """
-        Merge variables connected by identity operator to reduce the
-        number of redundant variables
-        """
+        if verbose > 0:
+            print("[convert_operators] begin")
         self._initialize_graph_status_for_traversing()
+        fed_variables = {i.name: i for i in container.initializers}
+        changes = 1
+        n_iter = 0
+        while changes > 0:
+            n_iter += 1
+            changes = 0
+            ops = list(self.unordered_operator_iterator())
+            if verbose > 0:
+                print("[convert_operators] iteration %d - n_vars=%d "
+                      "n_ops=%d" % (
+                        n_iter, len(fed_variables), len(ops)))
+            for operator in ops:
+                _check_operator_(operator)
+                for var in operator.inputs:
+                    if var.is_fed:
+                        fed_variables[var.onnx_name] = var
+                if (all(variable.is_fed for variable in operator.inputs) and
+                        not operator.is_evaluated):
 
-        # Traverse the graph from roots to leaves
-        for operator in self.topological_operator_iterator():
-            if operator.type != 'identity':
-                continue
-
-            if (any(variable.is_root for variable in operator.inputs) and
-                    any(variable.is_leaf for variable in operator.outputs)):
-                continue
-
-            # Replace the output variable with the input variable everywhere
-            original = operator.inputs[0]
-            duplicate = operator.outputs[0]
-            for another_scope in self.scopes:
-                for another_operator in another_scope.operators.values():
-                    for i in range(len(another_operator.inputs)):
-                        if (another_operator.inputs[i].onnx_name
-                                != duplicate.onnx_name):
-                            continue
-                        another_operator.inputs[i] = original
-
-            # When original variable's documentation string or
-            # denotation is empty but duplicate's is not, we copy that
-            # field to the original variable to avoid information loss.
-            if not original.type.doc_string and duplicate.type.doc_string:
-                original.type.doc_string = duplicate.type.doc_string
-
-            if (isinstance(original.type, TensorType) and
-                    isinstance(duplicate.type, TensorType)):
-                if not original.type.denotation and duplicate.type.denotation:
-                    original.type.denotation = duplicate.type.denotation
-                if not original.type.channel_denotations:
-                    original.type.channel_denotations = (
-                        duplicate.type.channel_denotations)
-                elif duplicate.type.channel_denotations:
-                    # Merge the channel denotations if available in both
-                    # the original and the duplicate
-                    for i in range(len(original.type.channel_denotations)):
-                        if original.type.channel_denotations[i]:
-                            continue
-                        original.type.channel_denotations[i] = (
-                            duplicate.type.channel_denotations[i])
-                # Sometime, shapes of duplicates are different. We try
-                # to replace the original variable's unknown dimensions
-                # as many as possible because we will get rid of the
-                # duplicate.
-                if len(original.type.shape) == len(duplicate.type.shape):
-                    for i in range(len(original.type.shape)):
-                        if original.type.shape[i] is not None:
-                            continue
-                        original.type.shape[i] = duplicate.type.shape[i]
-
-            # Because we're iterating through the topology, we cannot
-            # delete any operator or variable. Otherwise, the traversing
-            # function may be broken. We will delete those abandoned
-            # ones later.
-            duplicate.is_abandoned = True
-            operator.is_abandoned = True
-
-        for scope in self.scopes:
-            # Find out who is going to be abandoned
-            abandoned_operator_names = set(
-                onnx_name for onnx_name, operator in scope.operators.items()
-                if operator.is_abandoned)
-            abandoned_variable_names = set(
-                onnx_name for onnx_name, variable in scope.variables.items()
-                if variable.is_abandoned)
-
-            # Remove abandoned operators
-            for name in abandoned_operator_names:
-                scope.delete_local_operator(name)
-
-            # Remove abandoned variables
-            for name in abandoned_variable_names:
-                scope.delete_local_variable(name)
+                    for variable in operator.inputs:
+                        _check_variable_in_(variable, operator)
+                    for variable in operator.outputs:
+                        _check_variable_out_(variable, operator)
 
-    def _fix_shapes(self):
-        """
-        This function applies some rules to adjust graph inputs
-        (i.e., roots) before doing shape inference
-        """
+                    self.call_shape_calculator(operator)
+                    self.call_converter(operator, container, verbose=verbose)
 
-        # Identify roots of a graph
-        self._initialize_graph_status_for_traversing()
+                    # If an operator contains a sequence of operators,
+                    # output variables are not necessarily known at this stage.
+                    operator.init_status(is_evaluated=True)
+                    for variable in operator.outputs:
+                        if all(op.is_evaluated
+                               for op in variable.operators_outputs_):
+                            variable.init_status(is_fed=True)
+                            fed_variables[variable.onnx_name] = variable
+                    fed_variables.update(
+                        {i.name: i for i in container.initializers
+                         if i.name not in fed_variables})
+                    self._propagate_status(operator, container, fed_variables)
+                    # unfed some variables (it happens when a node
+                    # shares an output with another node)
+                    rem = []
+                    for n, var in fed_variables.items():
+                        if not hasattr(var, 'operators_outputs_'):
+                            # initializer
+                            continue
+                        if any(not o.is_evaluated
+                               for o in var.operators_outputs_):
+                            rem.append(n)
+                    for r in rem:
+                        v = fed_variables[r]
+                        v.init_status(is_fed=False)
+                        del fed_variables[v.onnx_name]
+                    changes += 1
+
+            if verbose > 0:
+                print("[convert_operators] end iter: %d - n_vars=%d" % (
+                    n_iter, len(fed_variables)))
+        if verbose > 0:
+            print("[convert_operators] end.")
+
+        # Last verification.
+        not_evaluated = []
+        for op in self.unordered_operator_iterator():
+            if not op.is_evaluated:
+                not_evaluated.append(op)
+        if len(not_evaluated) > 0:
+            rows = ["---VARS---"]
+            for var in self.unordered_variable_iterator():
+                rows.append(
+                    "is_fed=%r is_leaf=%r is_root=%r - %r - n_in=%d n_out=%d"
+                    "" % (var.is_fed, var.is_leaf, var.is_root, var,
+                          len(var.operators_inputs_),
+                          len(var.operators_outputs_)))
+            rows.append("---OPERATORS---")
+            for op in self.unordered_operator_iterator():
+                rows.append("is_eval=%r - %r" % (op.is_evaluated, op))
+            rows.append("---NODES---")
+            for node in container.nodes:
+                rows.append("%s: %r -> %r" % (
+                    node.op_type, node.input, node.output))
+            raise RuntimeError(
+                "Not all operators have been evaluated. A variable name "
+                "is probably misspelled.\n%s"
+                "" % "\n".join(rows))
+
+        # Input and output
+        if len(self.scopes[0].input_variables) > 0:
+            inputs = self.scopes[0].input_variables
+        else:
+            inputs = [v for v in self.unordered_variable_iterator()
+                      if v.is_root]
+        for i in inputs:
+            container.add_input(i)
+        outputs = [v for v in self.unordered_variable_iterator()
+                   if v.is_leaf]
+
+        # The function checks that for output variable,
+        # raw_name equal onnx_name. It swaps names if it is not the case.
+        to_swap = []
+        for out in outputs:
+            if out.raw_name != out.onnx_name:
+                to_swap.append(out)
+        if len(to_swap) != 0:
+            swaped = set()
+            for var in to_swap:
+                if var.raw_name in swaped:
+                    continue
+                swaped.add(var.raw_name)
+                if verbose > 1:
+                    print("[convert_operators] %r <-> %r." % (
+                        var.raw_name, var.onnx_name))
+                old_name = var.onnx_name
+                new_name = var.raw_name
 
-        # Scan through all operators and adjust their variables' shapes
-        # if needed
-        for operator in self.unordered_operator_iterator():
-            # Rule 1 (CoreML):
-            # Some operator in CoreML only accepts 4-D tensors but
-            # their protobuf models might specify a 2-D one.
-            # We fix this problem here.
-            if operator.type in [
-                    'bias', 'concat', 'convolution', 'crop', 'flatten',
-                    'scalerPreprocessor', 'lrn', 'meanImagePreprocessor',
-                    'padding', 'permute', 'pooling', 'reduce',
-                    'reorganizeData', 'reshape', 'scale', 'slice', 'upsample']:
-                # We only adjust inputs because outputs will be
-                # automatically fixed at our shape inference stage
-                for variable in operator.inputs:
-                    if variable.is_root:
-                        # Convert [N, C] to [N, C, 1, 1] while
-                        # [N, C, H, W] is unchanged
-                        variable.type.shape += [1] * (
-                            4 - len(variable.type.shape))
-
-    def _prune(self):
-        # Conduct a dummy evaluation of this topology. It may set all
-        # reachable operators evaluated and all reachable variables fed.
-        for operator in self.topological_operator_iterator():
-            pass
+                try:
+                    container.swap_names(old_name, new_name)
+                except NotImplementedError as e:
+                    logger.debug(
+                        '[Topo] unable to swap %r and %r (%r).' % (
+                            old_name, new_name, e))
+                    continue
 
-        for scope in self.scopes:
-            # Remove unused operators
-            abandoned_operator_names = []
-            for operator in scope.operators.values():
-                if not operator.is_evaluated:
-                    abandoned_operator_names.append(operator.onnx_name)
-            for onnx_name in abandoned_operator_names:
-                scope.delete_local_operator(onnx_name)
+                for v in self.unordered_variable_iterator():
+                    if v.onnx_name == old_name:
+                        v.set_onnx_name(new_name)
+                    elif v.onnx_name == new_name:
+                        v.set_onnx_name(old_name)
 
-            # Remove unused variables
-            abandoned_variable_names = []
-            for variable in scope.variables.values():
-                if not variable.is_fed:
-                    abandoned_variable_names.append(variable.onnx_name)
-            for onnx_name in abandoned_variable_names:
-                scope.delete_local_variable(onnx_name)
-
-    def compile(self):
-        """
-        This function aims at giving every operator enough information
-        so that all operator conversions can happen independently. We
-        also want to check, fix, and simplify the network structure
-        here.
-        """
-        self._prune()
-        self._resolve_duplicates()
-        self._fix_shapes()
-        self._infer_all_types()
-        self._check_structure()
+        for o in outputs:
+            container.add_output(o)
 
 
 def convert_topology(topology, model_name, doc_string, target_opset,
                      channel_first_inputs=None,
                      options=None, remove_identity=True,
                      verbose=0):
     """
@@ -1088,125 +1317,36 @@
         warnings.warn(
             "Parameter target_opset {} > {} is higher than the "
             "the latest tested version"
             ".".format(
                 onnx_target_opset,
                 get_latest_tested_opset_version()))
 
-    topology._initialize_graph_status_for_traversing()
-
     container = ModelComponentContainer(
         target_opset, options=options,
         registered_models=topology.registered_models,
         white_op=topology.raw_model._white_op,
         black_op=topology.raw_model._black_op,
         verbose=verbose)
 
-    # Put roots and leaves as ONNX's model into buffers. They will be
-    # added into ModelComponentContainer later.
-    tensor_inputs = {}
-    other_inputs = {}
-    tensor_outputs = {}
-    other_outputs = {}
-    for scope in topology.scopes:
-        for variable in scope.variables.values():
-            if variable.is_root:
-                if isinstance(variable.type, (TensorType, Int64Type,
-                                              FloatType, StringType)):
-                    tensor_inputs[variable.raw_name] = variable
-                else:
-                    other_inputs[variable.raw_name] = variable
-            if variable.is_leaf:
-                if isinstance(variable.type, (TensorType, Int64Type,
-                                              FloatType, StringType)):
-                    tensor_outputs[variable.onnx_name] = variable
-                else:
-                    other_outputs[variable.onnx_name] = variable
-
-    # Add roots the graph according to their order in the original model
-    invalid_name = []
-    nhwc_inputs = []
-    if channel_first_inputs is None:
-        channel_first_inputs = []
-    for variable in topology.raw_model._inputs:
-        name = variable.raw_name
-        # Check input naming convention
-        input_name = (
-            variable.onnx_name.replace('_', '')
-            .replace(":", "").replace("/", "")
-        )
-        if input_name and (input_name[0].isdigit() or
-                           (not input_name.isalnum())):
-            invalid_name.append(name)
-        if name in tensor_inputs:
-            # type: Variable
-            onnx_input = tensor_inputs[name]
-            if (name in channel_first_inputs or
-                    (name.endswith(':0') and
-                     name[:-2] in channel_first_inputs)):
-                nhwc_inputs.append(onnx_input.full_name)
-                s = onnx_input.type.shape
-                onnx_input.type.shape = [s[0], s[3], s[1], s[2]]
-            container.add_input(onnx_input)
-
-    if invalid_name:
-        warnings.warn('Some input names are not compliant with ONNX naming '
-                      'convention: %s' % invalid_name)
-    for variable in topology.raw_model._inputs:
-        name = variable.raw_name
-        if name in other_inputs:
-            container.add_input(other_inputs[name])
-
-    # Add leaves the graph according to their order in
-    # the original model
-    invalid_name = []
-    for name in topology.raw_model.output_names:
-        # Check output naming convention
-        output_name = name.replace('_', '').replace(":", "").replace("/", "")
-        if output_name and (output_name[0].isdigit() or
-                            (not output_name.isalnum())):
-            invalid_name.append(name)
-        if name in tensor_outputs:
-            container.add_output(tensor_outputs[name])
-    if invalid_name:
-        warnings.warn('Some output names are not compliant with ONNX naming '
-                      'convention: %s' % invalid_name)
-    for name in topology.raw_model.output_names:
-        if name in other_outputs:
-            container.add_output(other_outputs[name])
-
     # Traverse the graph from roots to leaves
     # This loop could eventually be parallelized.
-    for operator in topology.topological_operator_iterator():
-        scope = next(scope for scope in topology.scopes
-                     if scope.name == operator.scope)
-        mtype = type(operator.raw_operator)
-        if mtype in topology.custom_conversion_functions:
-            conv = topology.custom_conversion_functions[mtype]
-        elif operator.type in topology.custom_conversion_functions:
-            conv = topology.custom_conversion_functions[operator.type]
-        elif hasattr(operator.raw_operator, "onnx_converter"):
-            conv = operator.raw_operator.onnx_converter()
-        else:
-            # Convert the selected operator into some ONNX objects and
-            # save them into the container
-            try:
-                conv = _registration.get_converter(operator.type)
-            except ValueError:
-                raise MissingConverter(
-                    "Unable to find converter for alias '{}' type "
-                    "'{}'. You may raise an issue at "
-                    "https://github.com/onnx/sklearn-onnx/issues."
-                    "".format(operator.type,
-                              type(getattr(operator, 'raw_model', None))))
-        container.validate_options(operator)
-        conv(scope, operator, container)
-
+    topology.convert_operators(container=container, verbose=verbose)
     container.ensure_topological_order()
 
+    if len(container.inputs) == 0:
+        raise RuntimeError("No detected inputs after conversion.")
+    if len(container.outputs) == 0:
+        raise RuntimeError("No detected outputs after conversion.")
+    if verbose >= 2:
+        print("---NODES---")
+        for node in container.nodes:
+            print("  %s - %s: %r -> %r" % (
+                node.op_type, node.name, node.input, node.output))
+
     # Create a graph from its main components
     if container.target_opset_onnx < 9:
         # When calling ModelComponentContainer's add_initializer(...),
         # nothing is added into the input list. However, for ONNX target
         # opset < 9, initializers should also be a part of model's
         # (GraphProto) inputs. Thus, we create ValueInfoProto objects
         # from initializers (type: TensorProto) directly and then add
```

### Comparing `skl2onnx-1.9.2/skl2onnx/common/data_types.py` & `skl2onnx-1.9.3/skl2onnx/common/data_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,17 +284,17 @@
         return Float16TensorType(dims)
     if Complex64TensorType is not None:
         if data_type == np.complex64:
             return Complex64TensorType(dims)
         if data_type == np.complex128:
             return Complex128TensorType(dims)
     raise NotImplementedError(
-        "Unsupported data_type '{}'. You may raise an issue "
+        "Unsupported data_type %r (type=%r). You may raise an issue "
         "at https://github.com/onnx/sklearn-onnx/issues."
-        "".format(data_type))
+        "" % (data_type, type(data_type)))
 
 
 def guess_data_type(type_, shape=None):
     """
     Guess the datatype given the type type_
     """
     if isinstance(type_, TensorProto):
```

### Comparing `skl2onnx-1.9.2/skl2onnx/common/exceptions.py` & `skl2onnx-1.9.3/skl2onnx/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/common/onnx_optimisation_identity.py` & `skl2onnx-1.9.3/skl2onnx/common/onnx_optimisation_identity.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/common/shape_calculator.py` & `skl2onnx-1.9.3/skl2onnx/common/shape_calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,40 +28,42 @@
         1. [N, C] ---> [N, 1], A sequence of map
 
     """
     _calculate_linear_classifier_output_shapes(operator)
 
 
 def _calculate_linear_classifier_output_shapes(
-        operator, decision_path=False, decision_leaf=False):
+        operator, decision_path=False, decision_leaf=False,
+        enable_type_checking=True):
     n_out = 0
     if decision_path:
         n_out += 1
     if decision_leaf:
         n_out += 1
     out_range = [2, 2 + n_out]
     check_input_and_output_numbers(operator, input_count_range=1,
                                    output_count_range=out_range)
-    check_input_and_output_types(operator, good_input_types=[
-        BooleanTensorType, DoubleTensorType,
-        FloatTensorType, Int64TensorType])
+    if enable_type_checking:
+        check_input_and_output_types(operator, good_input_types=[
+            BooleanTensorType, DoubleTensorType,
+            FloatTensorType, Int64TensorType])
 
     N = operator.inputs[0].get_first_dimension()
     op = operator.raw_operator
     class_labels = get_label_classes(operator.scope_inst, op)
 
     number_of_classes = len(class_labels)
     if all(isinstance(i, np.ndarray) for i in class_labels):
         class_labels = np.concatenate(class_labels)
     if all(isinstance(i, str) for i in class_labels):
         shape = ([N, len(op.classes_)]
                  if (getattr(op, 'multilabel_', False) or (
                      isinstance(op.classes_, list) and
                      isinstance(op.classes_[0], np.ndarray))) else [N])
-        operator.outputs[0].type = StringTensorType(shape=shape)
+        operator.outputs[0].set_type(StringTensorType(shape=shape))
         if number_of_classes > 2 or operator.type != 'SklearnLinearSVC':
             shape = ([len(op.classes_), N, max([len(x) for x in op.classes_])]
                      if isinstance(op.classes_, list)
                      and isinstance(op.classes_[0], np.ndarray)
                      else [N, number_of_classes])
             operator.outputs[1].type.shape = shape
         else:
@@ -70,15 +72,15 @@
             operator.outputs[1].type.shape = [N, 1]
     elif all(isinstance(i, (numbers.Real, bool, np.bool_))
              for i in class_labels):
         shape = ([N, len(op.classes_)]
                  if (getattr(op, 'multilabel_', False) or (
                      isinstance(op.classes_, list) and
                      isinstance(op.classes_[0], np.ndarray))) else [N])
-        operator.outputs[0].type = Int64TensorType(shape=shape)
+        operator.outputs[0].set_type(Int64TensorType(shape=shape))
         if number_of_classes > 2 or operator.type != 'SklearnLinearSVC':
             shape = ([len(op.classes_), N, max([len(x) for x in op.classes_])]
                      if isinstance(op.classes_, list)
                      and isinstance(op.classes_[0], np.ndarray)
                      else [N, number_of_classes])
             operator.outputs[1].type.shape = shape
         else:
@@ -98,30 +100,36 @@
     Allowed input/output patterns are
         1. [N, C] ---> [N, 1]
 
     This operator produces a scalar prediction for every example in a
     batch. If the input batch size is N, the output shape may be
     [N, 1].
     """
+    _calculate_linear_regressor_output_shapes(operator)
+
+
+def _calculate_linear_regressor_output_shapes(
+        operator, enable_type_checking=True):
     check_input_and_output_numbers(operator, input_count_range=1,
                                    output_count_range=1)
-    check_input_and_output_types(operator, good_input_types=[
-        BooleanTensorType, DoubleTensorType,
-        FloatTensorType, Int64TensorType])
+    if enable_type_checking:
+        check_input_and_output_types(operator, good_input_types=[
+            BooleanTensorType, DoubleTensorType,
+            FloatTensorType, Int64TensorType])
 
     inp0 = operator.inputs[0].type
     if isinstance(inp0, (FloatTensorType, DoubleTensorType)):
         cls_type = inp0.__class__
     else:
         cls_type = FloatTensorType
 
     N = operator.inputs[0].get_first_dimension()
     if (hasattr(operator.raw_operator, 'coef_') and
             len(operator.raw_operator.coef_.shape) > 1):
-        operator.outputs[0].type = cls_type([
-            N, operator.raw_operator.coef_.shape[0]])
+        operator.outputs[0].set_type(cls_type([
+            N, operator.raw_operator.coef_.shape[0]]))
     else:
-        operator.outputs[0].type = cls_type([N, 1])
+        operator.outputs[0].set_type(cls_type([N, 1]))
 
     # decision_path, decision_leaf
     for n in range(1, len(operator.outputs)):
         operator.outputs[n].type.shape = [N, 1]
```

### Comparing `skl2onnx-1.9.2/skl2onnx/common/tree_ensemble.py` & `skl2onnx-1.9.3/skl2onnx/common/tree_ensemble.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/common/utils_checking.py` & `skl2onnx-1.9.3/skl2onnx/common/utils_checking.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/common/utils_classifier.py` & `skl2onnx-1.9.3/skl2onnx/common/utils_classifier.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/common/utils_sklearn.py` & `skl2onnx-1.9.3/skl2onnx/common/utils_sklearn.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/convert.py` & `skl2onnx-1.9.3/skl2onnx/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,73 +16,94 @@
                     target_opset=None, custom_conversion_functions=None,
                     custom_shape_calculators=None,
                     custom_parsers=None, options=None,
                     intermediate=False,
                     white_op=None, black_op=None, final_types=None,
                     dtype=None, verbose=0):
     """
-    This function produces an equivalent ONNX model of the given scikit-learn model.
+    This function produces an equivalent
+    ONNX model of the given scikit-learn model.
     The supported converters is returned by function
     :func:`supported_converters <skl2onnx.supported_converters>`.
 
     For pipeline conversion, user needs to make sure each component
     is one of our supported items.
     This function converts the specified *scikit-learn* model
     into its *ONNX* counterpart.
     Note that for all conversions, initial types are required.
     *ONNX* model name can also be specified.
 
     :param model: A scikit-learn model
-    :param initial_types: a python list. Each element is a tuple of a variable name
+    :param initial_types: a python list.
+        Each element is a tuple of a variable name
         and a type defined in `data_types.py`
-    :param name: The name of the graph (type: GraphProto) in the produced ONNX model (type: ModelProto)
+    :param name: The name of the graph (type: GraphProto)
+        in the produced ONNX model (type: ModelProto)
     :param doc_string: A string attached onto the produced ONNX model
-    :param target_opset: number, for example, 7 for ONNX 1.2, and 8 for ONNX 1.3,
-        if value is not specified, the function will choose the latest tested opset
+    :param target_opset: number, for example, 7 for
+        ONNX 1.2, and 8 for ONNX 1.3,
+        if value is not specified, the function will
+        choose the latest tested opset
         (see :py:func:`skl2onnx.get_latest_tested_opset_version`)
-    :param custom_conversion_functions: a dictionary for specifying the user customized conversion function,
+    :param custom_conversion_functions: a dictionary for
+        specifying the user customized conversion function,
         it takes precedence over registered converters
-    :param custom_shape_calculators: a dictionary for specifying the user customized shape calculator
+    :param custom_shape_calculators: a dictionary for
+        specifying the user customized shape calculator
         it takes precedence over registered shape calculators.
-    :param custom_parsers: parsers determines which outputs is expected for which particular task,
-        default parsers are defined for classifiers, regressors, pipeline but they can be rewritten,
-        *custom_parsers* is a dictionary ``{ type: fct_parser(scope, model, inputs, custom_parsers=None) }``
-    :param options: specific options given to converters (see :ref:`l-conv-options`)
-    :param intermediate: if True, the function returns the converted model and , and :class:`Topology`,
+    :param custom_parsers: parsers determines which outputs
+        is expected for which particular task,
+        default parsers are defined for classifiers,
+        regressors, pipeline but they can be rewritten,
+        *custom_parsers* is a dictionary
+        ``{ type: fct_parser(scope, model, inputs, custom_parsers=None) }``
+    :param options: specific options given to converters
+        (see :ref:`l-conv-options`)
+    :param intermediate: if True, the function returns the
+        converted model and , and :class:`Topology`,
         it returns the converted model otherwise
-    :param white_op: white list of ONNX nodes allowed while converting a pipeline,
+    :param white_op: white list of ONNX nodes allowed
+        while converting a pipeline,
         if empty, all are allowed
-    :param black_op: black list of ONNX nodes allowed while converting a pipeline,
+    :param black_op: black list of ONNX nodes
+        allowed while converting a pipeline,
         if empty, none are blacklisted
     :param final_types: a python list. Works the same way as initial_types
         but not mandatory, it is used to overwrites the type
         (if type is not None) and the name of every output.
-    :param dtype: removed in version 1.7.5, dtype is now inferred from input types,
-        converters may add operators Cast to switch to double when it is necessary
+    :param dtype: removed in version 1.7.5, dtype is
+        now inferred from input types,
+        converters may add operators Cast to switch
+        to double when it is necessary
     :param verbose: display progress while converting a model
-    :return: An ONNX model (type: ModelProto) which is equivalent to the input scikit-learn model
+    :return: An ONNX model (type: ModelProto) which is
+        equivalent to the input scikit-learn model
 
     Example of *initial_types*:
-    Assume that the specified *scikit-learn* model takes a heterogeneous list as its input.
+    Assume that the specified *scikit-learn* model takes
+    a heterogeneous list as its input.
     If the first 5 elements are floats and the last 10 elements are integers,
-    we need to specify initial types as below. The [None] in [None, 5] indicates
-    the batch size here is unknown.
+    we need to specify initial types as below. The [None] in
+    [None, 5] indicates the batch size here is unknown.
 
     ::
 
         from skl2onnx.common.data_types import FloatTensorType, Int64TensorType
         initial_type = [('float_input', FloatTensorType([None, 5])),
                         ('int64_input', Int64TensorType([None, 10]))]
 
     .. note::
 
         If a pipeline includes an instance of
-        `ColumnTransformer <https://scikit-learn.org/stable/modules/generated/sklearn.compose.ColumnTransformer.html>`_,
-        *scikit-learn* allow the user to specify columns by names. This option is not supported
-        by *sklearn-onnx* as features names could be different in input data and the ONNX graph
+        `ColumnTransformer <https://scikit-learn.org/stable/modules/
+        generated/sklearn.compose.ColumnTransformer.html>`_,
+        *scikit-learn* allow the user to specify columns by names.
+        This option is not supported
+        by *sklearn-onnx* as features names could be different
+        in input data and the ONNX graph
         (defined by parameter *initial_types*), only integers are supported.
 
     .. _l-conv-options:
 
     Converters options
     ++++++++++++++++++
 
@@ -98,37 +119,39 @@
     The default value is short and may not include all
     the necessary values. It can be overwritten as:
 
     ::
 
         extra = {TfidfVectorizer: {"separators": [' ', '[.]', '\\\\?',
                     ',', ';', ':', '\\\\!', '\\\\(', '\\\\)']}}
-        model_onnx = convert_sklearn(model, "tfidf",
-                                     initial_types=[("input", StringTensorType([None, 1]))],
-                                     options=extra)
+        model_onnx = convert_sklearn(
+            model, "tfidf",
+            initial_types=[("input", StringTensorType([None, 1]))],
+            options=extra)
 
     But if a pipeline contains two model of the same class,
     it is possible to distinguish between the two with function *id*:
 
     ::
 
         extra = {id(model): {"separators": [' ', '.', '\\\\?', ',', ';',
                     ':', '\\\\!', '\\\\(', '\\\\)']}}
-        model_onnx = convert_sklearn(pipeline, "pipeline-with-2-tfidf",
-                                     initial_types=[("input", StringTensorType([None, 1]))],
-                                     options=extra)
+        model_onnx = convert_sklearn(
+            pipeline, "pipeline-with-2-tfidf",
+            initial_types=[("input", StringTensorType([None, 1]))],
+            options=extra)
 
     It is used in example :ref:`l-example-tfidfvectorizer`.
 
     .. versionchanged:: 1.7
         Parameter `target_opset`, if not specified, is now set to
         the latest tested opset returned by
         :py:func:`skl2onnx.get_latest_tested_opset_version` and
         not the version of the *onnx* package.
-    """  # noqa
+    """
     if initial_types is None:
         if hasattr(model, 'infer_initial_types'):
             initial_types = model.infer_initial_types()
         else:
             raise ValueError('Initial types are required. See usage of '
                              'convert(...) in skl2onnx.convert for details')
 
@@ -148,28 +171,40 @@
         print("[convert_sklearn] parse_sklearn_model")
     topology = parse_sklearn_model(
         model, initial_types, target_opset, custom_conversion_functions,
         custom_shape_calculators, custom_parsers, options=options,
         white_op=white_op, black_op=black_op,
         final_types=final_types)
 
-    # Infer variable shapes
-    topology.compile()
-
     # Convert our Topology object into ONNX. The outcome is an ONNX model.
     options = _process_options(model, options)
     if verbose >= 1:
         print("[convert_sklearn] convert_topology")
-    onnx_model = convert_topology(topology, name, doc_string, target_opset,
-                                  options=options,
-                                  remove_identity=not intermediate,
-                                  verbose=verbose)
-
+    onnx_model = convert_topology(
+        topology, name, doc_string, target_opset, options=options,
+        remove_identity=not intermediate, verbose=verbose)
     if verbose >= 1:
         print("[convert_sklearn] end")
+        if verbose >= 2:
+            scope = topology.scopes[0]
+            print("---INPUTS---")
+            for inp in scope.input_variables:
+                print("  %r" % inp)
+            print("---OUTPUTS---")
+            for inp in scope.output_variables:
+                print("  %r" % inp)
+            print("---VARIABLESS---")
+            for k, v in sorted(scope.variables.items()):
+                print("  %r: is.fed=%r is_leaf=%r - %r" % (
+                    k, v.is_fed, v.is_leaf, v))
+            print("---OPERATORS---")
+            for k, v in sorted(scope.operators.items()):
+                print("  %r: is.evaluated=%r - %r" % (
+                    k, v.is_evaluated, v))
+
     return (onnx_model, topology) if intermediate else onnx_model
 
 
 def to_onnx(model, X=None, name=None, initial_types=None,
             target_opset=None, options=None,
             white_op=None, black_op=None, final_types=None,
             dtype=None, verbose=0):
```

### Comparing `skl2onnx-1.9.2/skl2onnx/helpers/investigate.py` & `skl2onnx-1.9.3/skl2onnx/helpers/investigate.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         model_onnx, topology = convert_sklearn(
             model, *args, intermediate=True, **kwargs)
     except (MissingShapeCalculator, MissingConverter):
         # The model cannot be converted.
         raise
 
     steps = []
-    for operator in topology.topological_operator_iterator():
+    for operator in topology.unordered_operator_iterator():
         if operator.raw_operator is None:
             continue
         _alter_model_for_debugging(operator.raw_operator)
         inputs = [i.full_name for i in operator.inputs]
         outputs = [o.full_name for o in operator.outputs]
         steps.append({
             'model': operator.raw_operator,
```

### Comparing `skl2onnx-1.9.2/skl2onnx/helpers/onnx_helper.py` & `skl2onnx-1.9.3/skl2onnx/helpers/onnx_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 from io import BytesIO
+import numpy as np
 import onnx  # noqa
-from onnx import shape_inference
+from onnx import shape_inference, TensorProto
+from onnx.numpy_helper import from_array
+from onnx.helper import make_tensor
 from ..proto.onnx_helper_modified import (
     make_node, make_tensor_value_info, make_graph,
     make_model, ValueInfoProto
 )
 from ..proto import get_latest_tested_opset_version
 from onnx import onnx_pb as onnx_proto
 from ..common._topology import Variable
@@ -307,7 +310,106 @@
             has_domain = oimp.domain in domain_set
     for v in ops.values():
         if v[1] not in domain_set:
             op_set = onnx_model.opset_import.add()
             op_set.domain = v[1]
             op_set.version = 1
     return onnx_model
+
+
+def add_output_initializer(model_onnx, name, value, suffix='_init'):
+    """
+    Add a constant and link it to one output.
+    It allows the user to store arrays into the graph
+    and retrieve them when using it.
+    The initializer is named `name + suffix`, the output
+    is named `name`.
+
+    :param model_onnx: ONNX graph
+    :param name: initializer name (initializer name, output name)
+    :param value: array to store
+    :param suffix: name of the initializer
+    :return: new model
+
+    It is possible to add multiple constant by using list:
+    ``add_output_initializer(model_onnx, ['name1', 'name2'], [v1, v2])``.
+    """
+    if isinstance(name, str):
+        name_list = [name]
+        value_list = [value]
+    else:
+        name_list = name
+        value_list = value
+
+    if len(name_list) != len(value_list):
+        raise ValueError(
+            "Mismatched names and values. There are %d names and %d values."
+            "" % (len(name_list), len(value_list)))
+
+    nodes = list(model_onnx.graph.node)
+    inits = list(model_onnx.graph.initializer)
+    outputs = list(model_onnx.graph.output)
+
+    for name, value in zip(name_list, value_list):
+        name_output = name
+        name_init = name + suffix
+        names = set(i.name for i in model_onnx.graph.initializer)
+        if name_output in names or name_init in names:
+            raise ValueError(
+                "Names %r or %r is already taken by an initializer: %r." % (
+                    name_output, name_init, ", ".join(sorted(names))))
+        names = set(i.name for i in model_onnx.graph.output)
+        if name_output in names or name_init in names:
+            raise ValueError(
+                "Names %r or %r is already taken by an output: %r." % (
+                    name_output, name_init, ", ".join(sorted(names))))
+        names = set(i.name for i in model_onnx.graph.input)
+        if name_output in names or name_init in names:
+            raise ValueError(
+                "Names %r or %r is already taken by an output: %r." % (
+                    name_output, name_init, ", ".join(sorted(names))))
+
+        try:
+            cst = from_array(value, name=name_init)
+        except RuntimeError as e:
+            st = str(value.dtype).lower()
+            if st.startswith('u') or st.startswith("<u"):
+                cst_value = np.array([s.encode('utf-8') for s in value])
+                cst = make_tensor(
+                    name_init, data_type=TensorProto.STRING,
+                    dims=value.shape, vals=list(cst_value))
+            else:
+                raise e
+
+        inits.append(cst)
+
+        outputs.append(make_tensor_value_info(
+            name_output, cst.data_type, cst.dims))
+
+        nodes.append(make_node('Identity', [name_init], [name_output]))
+
+    graph = make_graph(
+            nodes, model_onnx.graph.name, model_onnx.graph.input,
+            outputs, inits)
+
+    onnx_model = make_model(graph)
+    onnx_model.ir_version = model_onnx.ir_version
+    onnx_model.producer_name = model_onnx.producer_name
+    onnx_model.producer_version = model_onnx.producer_version
+    onnx_model.domain = model_onnx.domain
+    onnx_model.model_version = model_onnx.model_version
+    onnx_model.doc_string = model_onnx.doc_string
+    if len(model_onnx.metadata_props) > 0:
+        values = {p.key: p.value for p in model_onnx.metadata_props}
+        onnx.helper.set_model_props(onnx_model, values)
+
+    if len(onnx_model.graph.input) != len(model_onnx.graph.input):
+        raise RuntimeError("Input mismatch {} != {}".format(
+            len(onnx_model.input), len(model_onnx.input)))
+
+    # fix opset import
+    del onnx_model.opset_import[:]
+    for oimp in model_onnx.opset_import:
+        op_set = onnx_model.opset_import.add()
+        op_set.domain = oimp.domain
+        op_set.version = oimp.version
+    return onnx_model
```

### Comparing `skl2onnx-1.9.2/skl2onnx/helpers/onnx_rare_helper.py` & `skl2onnx-1.9.3/skl2onnx/helpers/onnx_rare_helper.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/__init__.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,32 @@
 from . import gaussian_process
 from . import gaussian_mixture
 from . import gradient_boosting
 from . import grid_search_cv
 from . import id_op
 from . import imputer_op
 from . import isolation_forest
+from . import kernel_pca
 from . import k_bins_discretiser
 from . import k_means
 from . import label_binariser
 from . import label_encoder
 from . import linear_classifier
 from . import linear_regressor
+from . import local_outlier_factor
 from . import multilayer_perceptron
+from . import multioutput
 from . import multiply_op
 from . import naive_bayes
 from . import nearest_neighbours
 from . import normaliser
 from . import one_hot_encoder
 from . import one_vs_rest_classifier
 from . import ordinal_encoder
+from . import pipelines
 from . import polynomial_features
 from . import power_transformer
 from . import random_forest
 from . import random_projection
 from . import ransac_regressor
 from . import replace_op
 from . import scaler_op
@@ -73,28 +77,32 @@
     gaussian_process,
     gaussian_mixture,
     gradient_boosting,
     grid_search_cv,
     id_op,
     imputer_op,
     isolation_forest,
+    kernel_pca,
     k_bins_discretiser,
     k_means,
     label_binariser,
     label_encoder,
     linear_classifier,
     linear_regressor,
+    local_outlier_factor,
     multilayer_perceptron,
+    multioutput,
     multiply_op,
     naive_bayes,
     nearest_neighbours,
     normaliser,
     one_hot_encoder,
     one_vs_rest_classifier,
     ordinal_encoder,
+    pipelines,
     polynomial_features,
     power_transformer,
     random_forest,
     random_projection,
     ransac_regressor,
     replace_op,
     scaler_op,
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/_gp_kernels.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/_gp_kernels.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/ada_boost.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/ada_boost.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 from ..common._apply_operation import (
     apply_add, apply_cast, apply_clip, apply_concat, apply_div, apply_exp,
     apply_mul, apply_reshape, apply_sub, apply_topk, apply_transpose
 )
 from ..common.data_types import (
-    FloatTensorType, DoubleTensorType, guess_proto_type, guess_numpy_type)
+    FloatTensorType, DoubleTensorType, guess_proto_type, guess_numpy_type,
+    Int64TensorType)
 from ..common._registration import register_converter
 from .._supported_operators import sklearn_operator_name_map
 
 
 def _scikit_learn_before_022():
     if '.dev' in __version__:
         return StrictVersion(
@@ -281,15 +282,16 @@
     if proto_dtype != onnx_proto.TensorProto.DOUBLE:
         proto_dtype = onnx_proto.TensorProto.FLOAT
     dtype = guess_numpy_type(operator.inputs[0].type)
     if dtype != np.float64:
         dtype = np.float32
 
     for i_est, estimator in enumerate(op.estimators_):
-        label_name = scope.declare_local_variable('elab_name_%d' % i_est)
+        label_name = scope.declare_local_variable(
+            'elab_name_%d' % i_est, Int64TensorType())
         proba_name = scope.declare_local_variable(
             'eprob_name_%d' % i_est, operator.inputs[0].type.__class__())
 
         op_type = sklearn_operator_name_map[type(estimator)]
 
         this_operator = scope.declare_local_operator(op_type, estimator)
         this_operator.inputs = operator.inputs
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/array_feature_extractor.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/bagging.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/bagging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 import numpy as np
 from .._supported_operators import sklearn_operator_name_map
+from ..common.data_types import Int64TensorType
 from ..common._apply_operation import (
     apply_cast, apply_concat,
     apply_div, apply_reshape)
 from ..common._registration import register_converter
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 from ..proto import onnx_proto
@@ -27,28 +28,31 @@
     for index, estimator in enumerate(model.estimators_):
         op_type = sklearn_operator_name_map[type(estimator)]
 
         this_operator = scope.declare_local_operator(op_type, estimator)
         if container.has_options(estimator, 'raw_scores'):
             container.add_options(
                 id(estimator), {'raw_scores': use_raw_scores})
+            scope.add_options(id(estimator), {'raw_scores': use_raw_scores})
 
-        label_name = scope.declare_local_variable('label_%d' % index)
+        label_name = scope.declare_local_variable(
+            'label_%d' % index, Int64TensorType())
         proba_name = scope.declare_local_variable(
             'proba_%d' % index, operator.inputs[0].type.__class__())
 
         features = model.estimators_features_[index]
         if (len(features) == model.n_features_ and
                 list(features) == list(range(model.n_features_))):
             this_operator.inputs = operator.inputs
         else:
             # subset of features
             feat_name = scope.declare_local_variable(
                 'fsel_%d' % index, operator.inputs[0].type.__class__())
-            index_name = scope.get_unique_variable_name('index_name')
+            index_name = scope.get_unique_variable_name(
+                'index_name_%d' % index)
             container.add_initializer(
                 index_name, onnx_proto.TensorProto.INT64,
                 (len(features), ), list(features))
             container.add_node(
                 'Gather', [operator.inputs[0].full_name, index_name],
                 [feat_name.full_name],
                 name=scope.get_unique_operator_name('GatherBG'), axis=1)
@@ -189,15 +193,16 @@
                 (len(features), ), list(features))
             container.add_node(
                 'Gather', [operator.inputs[0].full_name, index_name],
                 [feat_name.full_name],
                 name=scope.get_unique_operator_name('GatherBG'), axis=1)
             this_operator.inputs.append(feat_name)
 
-        label_name = scope.declare_local_variable('label_%d' % index)
+        label_name = scope.declare_local_variable(
+            'variable_%d' % index, this_operator.inputs[0].type.__class__())
         this_operator.outputs.append(label_name)
         reshaped_proba_name = scope.get_unique_variable_name('reshaped_proba')
         apply_reshape(scope, label_name.onnx_name, reshaped_proba_name,
                       container, desired_shape=(1, -1, 1))
         proba_list.append(reshaped_proba_name)
 
     merged_proba_name = scope.get_unique_variable_name('merged_proba')
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/binariser.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/binariser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/calibrated_classifier_cv.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/calibrated_classifier_cv.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 from ..proto import onnx_proto
 from ..common._apply_operation import (
     apply_abs, apply_add, apply_cast, apply_concat, apply_clip,
     apply_div, apply_exp, apply_mul, apply_reshape, apply_sub)
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
-from ..common.data_types import guess_numpy_type
+from ..common.data_types import guess_numpy_type, Int64TensorType
 from ..common._registration import register_converter
 from .._supported_operators import sklearn_operator_name_map
 
 
 def _handle_zeros(scope, container, concatenated_prob_name,
                   reduced_prob_name, n_classes):
     """
@@ -152,15 +152,15 @@
     apply_reshape(scope, nearest_y_name,
                   nearest_y_name_reshaped, container,
                   desired_shape=(-1, 1))
     return nearest_y_name_reshaped
 
 
 def convert_calibrated_classifier_base_estimator(scope, operator, container,
-                                                 model):
+                                                 model, model_index):
     # Computational graph:
     #
     # In the following graph, variable names are in lower case characters only
     # and operator names are in upper case characters. We borrow operator names
     # from the official ONNX spec:
     # https://github.com/onnx/onnx/blob/master/docs/Operators.md
     # All variables are followed by their shape in [].
@@ -257,73 +257,67 @@
     n_classes = (len(model.classes_) if hasattr(model, 'classes_') else
                  len(base_model.classes_))
     prob_name = [None] * n_classes
 
     this_operator = scope.declare_local_operator(op_type, base_model)
     if container.has_options(base_model, 'raw_scores'):
         container.add_options(id(base_model), {'raw_scores': True})
+        scope.add_options(id(base_model), {'raw_scores': True})
     this_operator.inputs = operator.inputs
-    label_name = scope.declare_local_variable('label')
+    label_name = scope.declare_local_variable('label', Int64TensorType())
     df_name = scope.declare_local_variable(
         'probability_tensor', operator.inputs[0].type.__class__())
     this_operator.outputs.append(label_name)
     this_operator.outputs.append(df_name)
     df_inp = df_name.full_name
 
     for k in range(n_classes):
         cur_k = k
         if n_classes == 2:
             cur_k += 1
-            # In case of binary classification, SVMs only return
-            # scores for the positive class. We concat the same
-            # column twice as we just use the second column.
-            if op_type in ('SklearnLinearSVC', 'SklearnSVC'):
-                df_input_name = scope.get_unique_variable_name('df_input')
-                merged_input_name = scope.get_unique_variable_name(
-                    'merged_input')
-
-                apply_reshape(scope, df_inp,
-                              df_input_name, container,
-                              desired_shape=(-1, 1))
-                apply_concat(scope, [df_input_name, df_input_name],
-                             merged_input_name, container, axis=1)
-                df_inp = merged_input_name
         k_name = scope.get_unique_variable_name('k')
-        df_col_name = scope.get_unique_variable_name('transposed_df_col')
-        prob_name[k] = scope.get_unique_variable_name('prob_{}'.format(k))
+        df_col_name = scope.get_unique_variable_name(
+            'tdf_col_%d_c%d' % (model_index, k))
+        prob_name[k] = scope.get_unique_variable_name(
+            'prob_{}_c{}'.format(model_index, k))
 
         container.add_initializer(k_name, onnx_proto.TensorProto.INT64,
                                   [], [cur_k])
 
         container.add_node(
             'ArrayFeatureExtractor', [df_inp, k_name], df_col_name,
-            name=scope.get_unique_operator_name('ArrayFeatureExtractor'),
+            name=scope.get_unique_operator_name(
+                'CaliAFE_%d_c%d' % (model_index, k)),
             op_domain='ai.onnx.ml')
         T = (_transform_sigmoid(scope, container, model, df_col_name, k)
              if model.method == 'sigmoid' else
              _transform_isotonic(
             scope, container, model, df_col_name, k, dtype))
 
         prob_name[k] = T
         if n_classes == 2:
             break
 
     if n_classes == 2:
-        zeroth_col_name = scope.get_unique_variable_name('zeroth_col')
-        merged_prob_name = scope.get_unique_variable_name('merged_prob')
+        zeroth_col_name = scope.get_unique_variable_name(
+            'zeroth_col%d' % model_index)
+        merged_prob_name = scope.get_unique_variable_name(
+            'merged_prob%d' % model_index)
         unit_float_tensor_name = scope.get_unique_variable_name(
-            'unit_float_tensor')
+            'unit_float_tensor%d' % model_index)
 
         container.add_initializer(unit_float_tensor_name,
                                   onnx_proto.TensorProto.FLOAT, [], [1.0])
 
         apply_sub(scope, [unit_float_tensor_name, prob_name[0]],
                   zeroth_col_name, container, broadcast=1)
         apply_concat(scope, [zeroth_col_name, prob_name[0]],
-                     merged_prob_name, container, axis=1)
+                     merged_prob_name, container, axis=1,
+                     operator_name=scope.get_unique_variable_name(
+                        'CaliConc%d' % model_index))
         class_prob_tensor_name = merged_prob_name
     else:
         concatenated_prob_name = scope.get_unique_variable_name(
             'concatenated_prob')
         reduced_prob_name = scope.get_unique_variable_name('reduced_prob')
         calc_prob_name = scope.get_unique_variable_name('calc_prob')
 
@@ -341,15 +335,17 @@
             container.add_node(
                 'ReduceSum', [concatenated_prob_name, axis_name],
                 reduced_prob_name,
                 name=scope.get_unique_operator_name('ReduceSum'))
         num, deno = _handle_zeros(scope, container, concatenated_prob_name,
                                   reduced_prob_name, n_classes)
         apply_div(scope, [num, deno],
-                  calc_prob_name, container, broadcast=1)
+                  calc_prob_name, container, broadcast=1,
+                  operator_name=scope.get_unique_variable_name(
+                    'CaliDiv%d' % model_index))
         class_prob_tensor_name = calc_prob_name
     return class_prob_tensor_name
 
 
 def convert_sklearn_calibrated_classifier_cv(
         scope: Scope, operator: Operator, container: ModelComponentContainer):
     # Computational graph:
@@ -420,17 +416,17 @@
         'array_feature_extractor_result')
     add_result_name = scope.get_unique_variable_name('add_result')
 
     container.add_initializer(classes_name, class_type, classes.shape, classes)
     container.add_initializer(clf_length_name, onnx_proto.TensorProto.FLOAT,
                               [], [clf_length])
 
-    for clf in op.calibrated_classifiers_:
+    for clf_index, clf in enumerate(op.calibrated_classifiers_):
         prob_scores_name.append(convert_calibrated_classifier_base_estimator(
-            scope, operator, container, clf))
+            scope, operator, container, clf, clf_index))
 
     container.add_node('Sum', [s for s in prob_scores_name],
                        add_result_name, op_version=7,
                        name=scope.get_unique_operator_name('Sum'))
     apply_div(scope, [add_result_name, clf_length_name],
               operator.outputs[1].full_name, container, broadcast=1)
     class_prob_name = operator.outputs[1].full_name
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/cast_op.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/cast_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/common.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/common.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/concat_op.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/concat_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from ..common._registration import register_converter
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 
 
 def convert_sklearn_concat(scope: Scope, operator: Operator,
                            container: ModelComponentContainer):
-    exptype = operator.outputs[0]
+    exptype = operator.outputs[0].type
     new_inputs = []
     for inp in operator.inputs:
         if inp.type == exptype:
             new_inputs.append(inp.full_name)
             continue
         name = scope.get_unique_variable_name("{}_cast".format(inp.full_name))
-        res = exptype.type.to_onnx_type()
+        res = exptype.to_onnx_type()
         et = res.tensor_type.elem_type
         apply_cast(scope, inp.full_name, name, container, to=et)
         new_inputs.append(name)
 
     apply_concat(scope, new_inputs, operator.outputs[0].full_name,
                  container, axis=1)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/cross_decomposition.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/cross_decomposition.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/decision_tree.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/decision_tree.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/decomposition.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/decomposition.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/dict_vectoriser.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/dict_vectoriser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/feature_selection.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/feature_selection.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/flatten_op.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/flatten_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/function_transformer.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/function_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/gaussian_mixture.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/gaussian_mixture.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,277 +1,277 @@
-# SPDX-License-Identifier: Apache-2.0
-
-
-import numpy as np
-from scipy.special import digamma
-from sklearn.mixture import BayesianGaussianMixture, GaussianMixture
-try:
-    from sklearn.mixture._gaussian_mixture import _compute_log_det_cholesky
-except ImportError:
-    # scikit-learn < 0.22
-    from sklearn.mixture.gaussian_mixture import _compute_log_det_cholesky
-from ..common._registration import register_converter
-from ..common._topology import Scope, Operator
-from ..common._container import ModelComponentContainer
-from ..common.data_types import guess_numpy_type
-from ..algebra.onnx_ops import (
-    OnnxAdd, OnnxSub, OnnxMul, OnnxGemm, OnnxReduceSumSquare,
-    OnnxReduceLogSumExp, OnnxExp, OnnxArgMax, OnnxConcat,
-    OnnxReduceSumApi11, OnnxLog, OnnxReduceMax, OnnxEqual, OnnxCast
-)
-from ..proto import onnx_proto
-
-
-def _estimate_log_gaussian_prob(X, means, precisions_chol,
-                                covariance_type, dtype, op_version,
-                                combined_reducesum):
-    """
-    Converts the same function into ONNX.
-    Returns log probabilities.
-    """
-    n_components = means.shape[0]
-    n_features = means.shape[1]
-    opv = op_version
-
-    # self._estimate_log_prob(X)
-    log_det = _compute_log_det_cholesky(
-        precisions_chol, covariance_type, n_features).astype(
-            dtype)
-
-    if covariance_type == 'full':
-        # shape(op.means_) = (n_components, n_features)
-        # shape(op.precisions_cholesky_) =
-        #   (n_components, n_features, n_features)
-
-        # log_prob = np.empty((n_samples, n_components))
-        # for k, (mu, prec_chol) in enumerate(zip(means, precisions_chol)):
-        #     y = np.dot(X, prec_chol) - np.dot(mu, prec_chol)
-        #     log_prob[:, k] = np.sum(np.square(y), axis=1)
-
-        ys = []
-        for c in range(n_components):
-            prec_chol = precisions_chol[c, :, :]
-            cst = - np.dot(means[c, :], prec_chol)
-            y = OnnxGemm(X, prec_chol.astype(dtype),
-                         cst.astype(dtype), alpha=1.,
-                         beta=1., op_version=opv)
-            if combined_reducesum:
-                y2s = OnnxReduceSumApi11(OnnxMul(y, y, op_version=opv),
-                                         axes=[1], op_version=opv)
-            else:
-                y2s = OnnxReduceSumSquare(y, axes=[1], op_version=opv)
-            ys.append(y2s)
-        log_prob = OnnxConcat(*ys, axis=1, op_version=opv)
-
-    elif covariance_type == 'tied':
-        # shape(op.means_) = (n_components, n_features)
-        # shape(op.precisions_cholesky_) =
-        #   (n_features, n_features)
-
-        # log_prob = np.empty((n_samples, n_components))
-        # for k, mu in enumerate(means):
-        #     y = np.dot(X, precisions_chol) - np.dot(mu, precisions_chol)
-        #     log_prob[:, k] = np.sum(np.square(y), axis=1)
-
-        ys = []
-        for f in range(n_components):
-            cst = - np.dot(means[f, :], precisions_chol)
-            y = OnnxGemm(X, precisions_chol.astype(dtype),
-                         cst.astype(dtype),
-                         alpha=1., beta=1., op_version=opv)
-            if combined_reducesum:
-                y2s = OnnxReduceSumApi11(OnnxMul(y, y, op_version=opv),
-                                         axes=[1], op_version=opv)
-            else:
-                y2s = OnnxReduceSumSquare(y, axes=[1], op_version=opv)
-            ys.append(y2s)
-        log_prob = OnnxConcat(*ys, axis=1, op_version=opv)
-
-    elif covariance_type == 'diag':
-        # shape(op.means_) = (n_components, n_features)
-        # shape(op.precisions_cholesky_) =
-        #   (n_components, n_features)
-
-        # precisions = precisions_chol ** 2
-        # log_prob = (np.sum((means ** 2 * precisions), 1) -
-        #             2. * np.dot(X, (means * precisions).T) +
-        #             np.dot(X ** 2, precisions.T))
-
-        precisions = (precisions_chol ** 2).astype(dtype)
-        mp = np.sum((means ** 2 * precisions), 1).astype(dtype)
-        zeros = np.zeros((n_components, ), dtype=dtype)
-        xmp = OnnxGemm(
-            X, (means * precisions).T.astype(dtype),
-            zeros, alpha=-2., beta=0., op_version=opv)
-        term = OnnxGemm(OnnxMul(X, X, op_version=opv),
-                        precisions.T.astype(dtype),
-                        zeros, alpha=1., beta=0., op_version=opv)
-        log_prob = OnnxAdd(
-            OnnxAdd(mp.astype(dtype), xmp, op_version=opv),
-            term, op_version=opv)
-
-    elif covariance_type == 'spherical':
-        # shape(op.means_) = (n_components, n_features)
-        # shape(op.precisions_cholesky_) = (n_components, )
-
-        # precisions = precisions_chol ** 2
-        # log_prob = (np.sum(means ** 2, 1) * precisions -
-        #             2 * np.dot(X, means.T * precisions) +
-        #             np.outer(row_norms(X, squared=True), precisions))
-
-        zeros = np.zeros((n_components, ), dtype=dtype)
-        precisions = (precisions_chol ** 2).astype(dtype)
-        if combined_reducesum:
-            normX = OnnxReduceSumApi11(OnnxMul(X, X, op_version=opv),
-                                       axes=[1], op_version=opv)
-        else:
-            normX = OnnxReduceSumSquare(X, axes=[1], op_version=opv)
-        outer = OnnxGemm(
-            normX, precisions[np.newaxis, :].astype(dtype),
-            zeros.astype(dtype), alpha=1., beta=1., op_version=opv)
-        xmp = OnnxGemm(
-            X, (means.T * precisions).astype(dtype),
-            zeros, alpha=-2., beta=0., op_version=opv)
-        mp = (np.sum(means ** 2, 1) * precisions).astype(dtype)
-        log_prob = OnnxAdd(mp, OnnxAdd(xmp, outer, op_version=opv),
-                           op_version=opv)
-    else:
-        raise RuntimeError("Unknown op.covariance_type='{}'. Upgrade "
-                           "to a more recent version of skearn-onnx "
-                           "or raise an issue.".format(covariance_type))
-    # -.5 * (cst + log_prob) + log_det
-    cst = np.array([n_features * np.log(2 * np.pi)]).astype(dtype)
-    add = OnnxAdd(cst, log_prob, op_version=opv)
-    mul = OnnxMul(add, np.array([-0.5], dtype=dtype),
-                  op_version=opv)
-    if isinstance(log_det, (np.float32, np.float64, float)):
-        log_det = np.array([log_det], dtype=dtype)
-
-    return OnnxAdd(mul, log_det.astype(dtype), op_version=opv)
-
-
-def convert_sklearn_gaussian_mixture(scope: Scope, operator: Operator,
-                                     container: ModelComponentContainer):
-    """
-    Converter for *GaussianMixture*,
-    *BayesianGaussianMixture*.
-    """
-    X = operator.inputs[0]
-    dtype = guess_numpy_type(X.type)
-    if dtype != np.float64:
-        dtype = np.float32
-    elif operator.target_opset < 11:
-        raise RuntimeError(
-            "Some needed operators are not available below opset 11"
-            " to convert model %r" % type(operator.raw_operator))
-    out = operator.outputs
-    op = operator.raw_operator
-    n_components = op.means_.shape[0]
-    opv = container.target_opset
-    options = container.get_options(op, dict(score_samples=None))
-    add_score = options.get('score_samples', False)
-    combined_reducesum = not container.is_allowed(
-        {'ReduceLogSumExp', 'ReduceSumSquare'})
-    if add_score and len(out) != 3:
-        raise RuntimeError("3 outputs are expected.")
-
-    if X.type is not None:
-        if X.type.shape[1] != op.means_.shape[1]:
-            raise RuntimeError(
-                "Dimension mismath between expected number of features {} "
-                "and ONNX graphs expectations {}.".format(
-                    op.means_.shape[1], X.type.shape[1]))
-    n_features = op.means_.shape[1]
-
-    # All comments come from scikit-learn code and tells
-    # which functions is being onnxified.
-    # def _estimate_weighted_log_prob(self, X):
-    log_weights = op._estimate_log_weights().astype(dtype)
-
-    log_gauss = _estimate_log_gaussian_prob(
-        X, op.means_, op.precisions_cholesky_, op.covariance_type,
-        dtype, opv, combined_reducesum)
-
-    if isinstance(op, BayesianGaussianMixture):
-        # log_gauss = (_estimate_log_gaussian_prob(
-        #   X, self.means_, self.precisions_cholesky_, self.covariance_type) -
-        #   .5 * n_features * np.log(self.degrees_of_freedom_))
-
-        log_lambda = n_features * np.log(2.) + np.sum(digamma(
-            .5 * (op.degrees_of_freedom_ -
-                  np.arange(0, n_features)[:, np.newaxis])), 0)
-        cst_log_lambda = .5 * (log_lambda - n_features / op.mean_precision_)
-        cst = cst_log_lambda - .5 * n_features * np.log(op.degrees_of_freedom_)
-        if isinstance(cst, np.ndarray):
-            cst_array = cst.astype(dtype)
-        else:
-            cst_array = np.array([cst], dtype=dtype)
-        log_gauss = OnnxAdd(log_gauss, cst_array, op_version=opv)
-    elif not isinstance(op, GaussianMixture):
-        raise RuntimeError(
-            "The converter does not support type {}.".format(
-                type(op)))
-
-    # self._estimate_log_prob(X) + self._estimate_log_weights()
-    weighted_log_prob = OnnxAdd(log_gauss, log_weights, op_version=opv)
-
-    # labels
-    if container.is_allowed('ArgMax'):
-        labels = OnnxArgMax(weighted_log_prob, axis=1,
-                            output_names=out[:1], op_version=opv)
-    else:
-        mxlabels = OnnxReduceMax(weighted_log_prob, axes=[1], op_version=opv)
-        zeros = OnnxEqual(
-            OnnxSub(weighted_log_prob, mxlabels, op_version=opv),
-            np.array([0], dtype=dtype),
-            op_version=opv)
-        toint = OnnxCast(zeros, to=onnx_proto.TensorProto.INT64,
-                         op_version=opv)
-        mulind = OnnxMul(toint,
-                         np.arange(n_components).astype(np.int64),
-                         op_version=opv)
-        labels = OnnxReduceMax(mulind, axes=[1], output_names=out[:1],
-                               op_version=opv)
-
-    # def _estimate_log_prob_resp():
-    # np.exp(log_resp)
-    # weighted_log_prob = self._estimate_weighted_log_prob(X)
-    # log_prob_norm = logsumexp(weighted_log_prob, axis=1)
-    # with np.errstate(under='ignore'):
-    #    log_resp = weighted_log_prob - log_prob_norm[:, np.newaxis]
-    if add_score:
-        outnames = out[2:3]
-    else:
-        outnames = None
-
-    if combined_reducesum:
-        max_weight = OnnxReduceMax(weighted_log_prob, axes=[1], op_version=opv)
-        log_prob_norm_demax = OnnxLog(
-            OnnxReduceSumApi11(
-                OnnxExp(
-                    OnnxSub(weighted_log_prob, max_weight, op_version=opv),
-                    op_version=opv),
-                axes=[1], op_version=opv),
-            op_version=opv)
-        log_prob_norm = OnnxAdd(log_prob_norm_demax, max_weight,
-                                op_version=opv, output_names=out[2:3])
-    else:
-        log_prob_norm = OnnxReduceLogSumExp(
-            weighted_log_prob, axes=[1], op_version=opv,
-            output_names=outnames)
-    log_resp = OnnxSub(weighted_log_prob, log_prob_norm, op_version=opv)
-
-    # probabilities
-    probs = OnnxExp(log_resp, output_names=out[1:2], op_version=opv)
-
-    # final
-    labels.add_to(scope, container)
-    probs.add_to(scope, container)
-    if add_score:
-        log_prob_norm.add_to(scope, container)
-
-
-register_converter('SklearnGaussianMixture', convert_sklearn_gaussian_mixture,
-                   options={'score_samples': [True, False]})
-register_converter('SklearnBayesianGaussianMixture',
-                   convert_sklearn_gaussian_mixture,
-                   options={'score_samples': [True, False]})
+# SPDX-License-Identifier: Apache-2.0
+
+
+import numpy as np
+from scipy.special import digamma
+from sklearn.mixture import BayesianGaussianMixture, GaussianMixture
+try:
+    from sklearn.mixture._gaussian_mixture import _compute_log_det_cholesky
+except ImportError:
+    # scikit-learn < 0.22
+    from sklearn.mixture.gaussian_mixture import _compute_log_det_cholesky
+from ..common._registration import register_converter
+from ..common._topology import Scope, Operator
+from ..common._container import ModelComponentContainer
+from ..common.data_types import guess_numpy_type
+from ..algebra.onnx_ops import (
+    OnnxAdd, OnnxSub, OnnxMul, OnnxGemm, OnnxReduceSumSquare,
+    OnnxReduceLogSumExp, OnnxExp, OnnxArgMax, OnnxConcat,
+    OnnxReduceSumApi11, OnnxLog, OnnxReduceMax, OnnxEqual, OnnxCast
+)
+from ..proto import onnx_proto
+
+
+def _estimate_log_gaussian_prob(X, means, precisions_chol,
+                                covariance_type, dtype, op_version,
+                                combined_reducesum):
+    """
+    Converts the same function into ONNX.
+    Returns log probabilities.
+    """
+    n_components = means.shape[0]
+    n_features = means.shape[1]
+    opv = op_version
+
+    # self._estimate_log_prob(X)
+    log_det = _compute_log_det_cholesky(
+        precisions_chol, covariance_type, n_features).astype(
+            dtype)
+
+    if covariance_type == 'full':
+        # shape(op.means_) = (n_components, n_features)
+        # shape(op.precisions_cholesky_) =
+        #   (n_components, n_features, n_features)
+
+        # log_prob = np.empty((n_samples, n_components))
+        # for k, (mu, prec_chol) in enumerate(zip(means, precisions_chol)):
+        #     y = np.dot(X, prec_chol) - np.dot(mu, prec_chol)
+        #     log_prob[:, k] = np.sum(np.square(y), axis=1)
+
+        ys = []
+        for c in range(n_components):
+            prec_chol = precisions_chol[c, :, :]
+            cst = - np.dot(means[c, :], prec_chol)
+            y = OnnxGemm(X, prec_chol.astype(dtype),
+                         cst.astype(dtype), alpha=1.,
+                         beta=1., op_version=opv)
+            if combined_reducesum:
+                y2s = OnnxReduceSumApi11(OnnxMul(y, y, op_version=opv),
+                                         axes=[1], op_version=opv)
+            else:
+                y2s = OnnxReduceSumSquare(y, axes=[1], op_version=opv)
+            ys.append(y2s)
+        log_prob = OnnxConcat(*ys, axis=1, op_version=opv)
+
+    elif covariance_type == 'tied':
+        # shape(op.means_) = (n_components, n_features)
+        # shape(op.precisions_cholesky_) =
+        #   (n_features, n_features)
+
+        # log_prob = np.empty((n_samples, n_components))
+        # for k, mu in enumerate(means):
+        #     y = np.dot(X, precisions_chol) - np.dot(mu, precisions_chol)
+        #     log_prob[:, k] = np.sum(np.square(y), axis=1)
+
+        ys = []
+        for f in range(n_components):
+            cst = - np.dot(means[f, :], precisions_chol)
+            y = OnnxGemm(X, precisions_chol.astype(dtype),
+                         cst.astype(dtype),
+                         alpha=1., beta=1., op_version=opv)
+            if combined_reducesum:
+                y2s = OnnxReduceSumApi11(OnnxMul(y, y, op_version=opv),
+                                         axes=[1], op_version=opv)
+            else:
+                y2s = OnnxReduceSumSquare(y, axes=[1], op_version=opv)
+            ys.append(y2s)
+        log_prob = OnnxConcat(*ys, axis=1, op_version=opv)
+
+    elif covariance_type == 'diag':
+        # shape(op.means_) = (n_components, n_features)
+        # shape(op.precisions_cholesky_) =
+        #   (n_components, n_features)
+
+        # precisions = precisions_chol ** 2
+        # log_prob = (np.sum((means ** 2 * precisions), 1) -
+        #             2. * np.dot(X, (means * precisions).T) +
+        #             np.dot(X ** 2, precisions.T))
+
+        precisions = (precisions_chol ** 2).astype(dtype)
+        mp = np.sum((means ** 2 * precisions), 1).astype(dtype)
+        zeros = np.zeros((n_components, ), dtype=dtype)
+        xmp = OnnxGemm(
+            X, (means * precisions).T.astype(dtype),
+            zeros, alpha=-2., beta=0., op_version=opv)
+        term = OnnxGemm(OnnxMul(X, X, op_version=opv),
+                        precisions.T.astype(dtype),
+                        zeros, alpha=1., beta=0., op_version=opv)
+        log_prob = OnnxAdd(
+            OnnxAdd(mp.astype(dtype), xmp, op_version=opv),
+            term, op_version=opv)
+
+    elif covariance_type == 'spherical':
+        # shape(op.means_) = (n_components, n_features)
+        # shape(op.precisions_cholesky_) = (n_components, )
+
+        # precisions = precisions_chol ** 2
+        # log_prob = (np.sum(means ** 2, 1) * precisions -
+        #             2 * np.dot(X, means.T * precisions) +
+        #             np.outer(row_norms(X, squared=True), precisions))
+
+        zeros = np.zeros((n_components, ), dtype=dtype)
+        precisions = (precisions_chol ** 2).astype(dtype)
+        if combined_reducesum:
+            normX = OnnxReduceSumApi11(OnnxMul(X, X, op_version=opv),
+                                       axes=[1], op_version=opv)
+        else:
+            normX = OnnxReduceSumSquare(X, axes=[1], op_version=opv)
+        outer = OnnxGemm(
+            normX, precisions[np.newaxis, :].astype(dtype),
+            zeros.astype(dtype), alpha=1., beta=1., op_version=opv)
+        xmp = OnnxGemm(
+            X, (means.T * precisions).astype(dtype),
+            zeros, alpha=-2., beta=0., op_version=opv)
+        mp = (np.sum(means ** 2, 1) * precisions).astype(dtype)
+        log_prob = OnnxAdd(mp, OnnxAdd(xmp, outer, op_version=opv),
+                           op_version=opv)
+    else:
+        raise RuntimeError("Unknown op.covariance_type='{}'. Upgrade "
+                           "to a more recent version of skearn-onnx "
+                           "or raise an issue.".format(covariance_type))
+    # -.5 * (cst + log_prob) + log_det
+    cst = np.array([n_features * np.log(2 * np.pi)]).astype(dtype)
+    add = OnnxAdd(cst, log_prob, op_version=opv)
+    mul = OnnxMul(add, np.array([-0.5], dtype=dtype),
+                  op_version=opv)
+    if isinstance(log_det, (np.float32, np.float64, float)):
+        log_det = np.array([log_det], dtype=dtype)
+
+    return OnnxAdd(mul, log_det.astype(dtype), op_version=opv)
+
+
+def convert_sklearn_gaussian_mixture(scope: Scope, operator: Operator,
+                                     container: ModelComponentContainer):
+    """
+    Converter for *GaussianMixture*,
+    *BayesianGaussianMixture*.
+    """
+    X = operator.inputs[0]
+    dtype = guess_numpy_type(X.type)
+    if dtype != np.float64:
+        dtype = np.float32
+    elif operator.target_opset < 11:
+        raise RuntimeError(
+            "Some needed operators are not available below opset 11"
+            " to convert model %r" % type(operator.raw_operator))
+    out = operator.outputs
+    op = operator.raw_operator
+    n_components = op.means_.shape[0]
+    opv = container.target_opset
+    options = container.get_options(op, dict(score_samples=None))
+    add_score = options.get('score_samples', False)
+    combined_reducesum = not container.is_allowed(
+        {'ReduceLogSumExp', 'ReduceSumSquare'})
+    if add_score and len(out) != 3:
+        raise RuntimeError("3 outputs are expected.")
+
+    if X.type is not None:
+        if X.type.shape[1] != op.means_.shape[1]:
+            raise RuntimeError(
+                "Dimension mismath between expected number of features {} "
+                "and ONNX graphs expectations {}.".format(
+                    op.means_.shape[1], X.type.shape[1]))
+    n_features = op.means_.shape[1]
+
+    # All comments come from scikit-learn code and tells
+    # which functions is being onnxified.
+    # def _estimate_weighted_log_prob(self, X):
+    log_weights = op._estimate_log_weights().astype(dtype)
+
+    log_gauss = _estimate_log_gaussian_prob(
+        X, op.means_, op.precisions_cholesky_, op.covariance_type,
+        dtype, opv, combined_reducesum)
+
+    if isinstance(op, BayesianGaussianMixture):
+        # log_gauss = (_estimate_log_gaussian_prob(
+        #   X, self.means_, self.precisions_cholesky_, self.covariance_type) -
+        #   .5 * n_features * np.log(self.degrees_of_freedom_))
+
+        log_lambda = n_features * np.log(2.) + np.sum(digamma(
+            .5 * (op.degrees_of_freedom_ -
+                  np.arange(0, n_features)[:, np.newaxis])), 0)
+        cst_log_lambda = .5 * (log_lambda - n_features / op.mean_precision_)
+        cst = cst_log_lambda - .5 * n_features * np.log(op.degrees_of_freedom_)
+        if isinstance(cst, np.ndarray):
+            cst_array = cst.astype(dtype)
+        else:
+            cst_array = np.array([cst], dtype=dtype)
+        log_gauss = OnnxAdd(log_gauss, cst_array, op_version=opv)
+    elif not isinstance(op, GaussianMixture):
+        raise RuntimeError(
+            "The converter does not support type {}.".format(
+                type(op)))
+
+    # self._estimate_log_prob(X) + self._estimate_log_weights()
+    weighted_log_prob = OnnxAdd(log_gauss, log_weights, op_version=opv)
+
+    # labels
+    if container.is_allowed('ArgMax'):
+        labels = OnnxArgMax(weighted_log_prob, axis=1,
+                            output_names=out[:1], op_version=opv)
+    else:
+        mxlabels = OnnxReduceMax(weighted_log_prob, axes=[1], op_version=opv)
+        zeros = OnnxEqual(
+            OnnxSub(weighted_log_prob, mxlabels, op_version=opv),
+            np.array([0], dtype=dtype),
+            op_version=opv)
+        toint = OnnxCast(zeros, to=onnx_proto.TensorProto.INT64,
+                         op_version=opv)
+        mulind = OnnxMul(toint,
+                         np.arange(n_components).astype(np.int64),
+                         op_version=opv)
+        labels = OnnxReduceMax(mulind, axes=[1], output_names=out[:1],
+                               op_version=opv)
+
+    # def _estimate_log_prob_resp():
+    # np.exp(log_resp)
+    # weighted_log_prob = self._estimate_weighted_log_prob(X)
+    # log_prob_norm = logsumexp(weighted_log_prob, axis=1)
+    # with np.errstate(under='ignore'):
+    #    log_resp = weighted_log_prob - log_prob_norm[:, np.newaxis]
+    if add_score:
+        outnames = out[2:3]
+    else:
+        outnames = None
+
+    if combined_reducesum:
+        max_weight = OnnxReduceMax(weighted_log_prob, axes=[1], op_version=opv)
+        log_prob_norm_demax = OnnxLog(
+            OnnxReduceSumApi11(
+                OnnxExp(
+                    OnnxSub(weighted_log_prob, max_weight, op_version=opv),
+                    op_version=opv),
+                axes=[1], op_version=opv),
+            op_version=opv)
+        log_prob_norm = OnnxAdd(log_prob_norm_demax, max_weight,
+                                op_version=opv, output_names=outnames)
+    else:
+        log_prob_norm = OnnxReduceLogSumExp(
+            weighted_log_prob, axes=[1], op_version=opv,
+            output_names=outnames)
+    log_resp = OnnxSub(weighted_log_prob, log_prob_norm, op_version=opv)
+
+    # probabilities
+    probs = OnnxExp(log_resp, output_names=out[1:2], op_version=opv)
+
+    # final
+    labels.add_to(scope, container)
+    probs.add_to(scope, container)
+    if add_score:
+        log_prob_norm.add_to(scope, container)
+
+
+register_converter('SklearnGaussianMixture', convert_sklearn_gaussian_mixture,
+                   options={'score_samples': [True, False]})
+register_converter('SklearnBayesianGaussianMixture',
+                   convert_sklearn_gaussian_mixture,
+                   options={'score_samples': [True, False]})
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/gaussian_process.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/gradient_boosting.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/grid_search_cv.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/grid_search_cv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # SPDX-License-Identifier: Apache-2.0
 
-
-from sklearn.base import is_classifier
 from ..common._apply_operation import apply_identity
 from ..common._registration import register_converter
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 from .._supported_operators import sklearn_operator_name_map
 
 
@@ -17,24 +15,19 @@
     opts = scope.get_options(operator.raw_operator)
     grid_search_op = operator.raw_operator
     best_estimator = grid_search_op.best_estimator_
     op_type = sklearn_operator_name_map[type(best_estimator)]
     grid_search_operator = scope.declare_local_operator(
         op_type, best_estimator)
     container.add_options(id(best_estimator), opts)
+    scope.add_options(id(best_estimator), opts)
     grid_search_operator.inputs = operator.inputs
-    label_name = scope.declare_local_variable('label')
-    grid_search_operator.outputs.append(label_name)
-    if is_classifier(best_estimator):
-        proba_name = scope.declare_local_variable(
-            'probability_tensor', operator.inputs[0].type.__class__())
-        grid_search_operator.outputs.append(proba_name)
-    apply_identity(scope, label_name.full_name,
-                   operator.outputs[0].full_name, container)
-    if is_classifier(best_estimator):
-        apply_identity(scope, proba_name.full_name,
-                       operator.outputs[1].full_name, container)
+
+    for i, o in enumerate(operator.outputs):
+        v = scope.declare_local_variable(o.onnx_name, type=o.type)
+        grid_search_operator.outputs.append(v)
+        apply_identity(scope, v.full_name, o.full_name, container)
 
 
 register_converter('SklearnGridSearchCV',
                    convert_sklearn_grid_search_cv,
                    options="passthrough")
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/id_op.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/id_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/imputer_op.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/imputer_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/isolation_forest.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/isolation_forest.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 def convert_sklearn_isolation_forest(
         scope, operator, container, op_type='TreeEnsembleRegressor',
         op_domain='ai.onnx.ml', op_version=1):
     op = operator.raw_operator
     outputs = operator.outputs
     opv = container.target_opset
     opvml = container.target_opset_any_domain('ai.onnx.ml')
+    options = container.get_options(op, dict(score_samples=None))
     if opvml < 2:
         raise RuntimeError(
             "This converter requires at least opset 2 for "
             "domain 'ai.onnx.ml'.")
 
     input_name = operator.inputs[0]
     dtype = guess_numpy_type(operator.inputs[0].type)
@@ -183,21 +184,23 @@
 
     cst = len(op.estimators_) * _average_path_length([op.max_samples_])
     depths = OnnxDiv(OnnxSum(*scores, op_version=opv),
                      np.array([cst], dtype=dtype),
                      op_version=opv)
 
     # decision_function
-    decision = OnnxAdd(
-        OnnxNeg(
+    output_names = outputs[2].full_name if options['score_samples'] else None
+    score_samples = OnnxNeg(
             OnnxPow(np.array([2], dtype=dtype),
                     OnnxNeg(depths, op_version=opv),
                     op_version=opv),
-            op_version=opv),
-        np.array([-op.offset_], dtype=dtype),
+            op_version=opv, output_names=output_names)
+
+    decision = OnnxAdd(
+        score_samples, np.array([-op.offset_], dtype=dtype),
         op_version=opv, output_names=outputs[1].full_name)
     decision.set_onnx_name_prefix('dec')
 
     less = OnnxLess(decision, np.array([0], dtype=dtype),
                     op_version=opv)
     predict = OnnxAdd(
         OnnxMul(
@@ -208,14 +211,16 @@
         np.array([1], dtype=np.int64),
         op_version=opv,
         output_names=outputs[0].full_name)
     predict.set_onnx_name_prefix('predict')
 
     predict.add_to(scope, container)
     less.add_to(scope, container)
+    if options['score_samples']:
+        score_samples.add_to(scope, container)
 
 
 def _build_labels(tree, output):
     def _recursive_build_labels(index, current):
         current[index] = True
         if tree.children_left[index] == -1:
             yield (index, current.copy())
@@ -247,8 +252,9 @@
             paths[leave_index] = spath[leave_index]
     else:
         raise RuntimeError("Unknown method '%s'." % output)
     return paths
 
 
 register_converter('SklearnIsolationForest',
-                   convert_sklearn_isolation_forest)
+                   convert_sklearn_isolation_forest,
+                   options={'score_samples': [True, False]})
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/k_bins_discretiser.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/k_bins_discretiser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/k_means.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/k_means.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..common.data_types import Int64TensorType, guess_numpy_type
 from ..common._registration import register_converter
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 from ..algebra.onnx_ops import (
     OnnxReduceSumSquare, OnnxGemm, OnnxMatMul,
     OnnxAdd, OnnxArgMin, OnnxCast, OnnxSqrt, OnnxMul)
-from ..proto import onnx_proto
 
 
 def convert_sklearn_kmeans(scope: Scope, operator: Operator,
                            container: ModelComponentContainer):
     """
     Computation graph of distances to all centroids for a batch of examples.
     Note that a centriod is just the center of a cluster. We use ``[]`` to
@@ -73,15 +72,15 @@
     C = op.cluster_centers_
     input_name = X
     dtype = guess_numpy_type(X.type)
     if dtype != np.float64:
         dtype = np.float32
 
     if type(X.type) == Int64TensorType:
-        x_cast = OnnxCast(X, to=onnx_proto.TensorProto.FLOAT, op_version=opv)
+        x_cast = OnnxCast(X, to=np.float32, op_version=opv)
         input_name = x_cast
 
     C2 = row_norms(C, squared=True).astype(dtype)
     C = C.astype(dtype)
     rs = OnnxReduceSumSquare(input_name, axes=[1], keepdims=1, op_version=opv)
 
     N = X.get_first_dimension()
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/label_binariser.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/label_binariser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/label_encoder.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/label_encoder.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/linear_classifier.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/linear_classifier.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/linear_regressor.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/linear_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # SPDX-License-Identifier: Apache-2.0
 
-try:
-    import collections.abc as cabc
-except ImportError:
-    import collections as cabc
 import numpy as np
 from ..common._apply_operation import (
     apply_cast, apply_add, apply_sqrt, apply_div, apply_sub,
     apply_reshape)
 from ..common.data_types import (
     BooleanTensorType, Int64TensorType, DoubleTensorType,
     guess_numpy_type, guess_proto_type)
@@ -45,17 +41,15 @@
 
     op_type = 'LinearRegressor'
     dtype = guess_numpy_type(operator.inputs[0].type)
     if dtype not in (np.float32, np.float64):
         dtype = np.float32
     attrs = {'name': scope.get_unique_operator_name(op_type)}
     attrs['coefficients'] = op.coef_.astype(dtype).ravel()
-    attrs['intercepts'] = (op.intercept_.astype(dtype)
-                           if isinstance(op.intercept_, cabc.Iterable)
-                           else np.array([op.intercept_], dtype=dtype))
+    attrs['intercepts'] = np.array([op.intercept_], dtype=dtype).ravel()
     if len(op.coef_.shape) == 2:
         attrs['targets'] = op.coef_.shape[0]
 
     input_name = operator.input_full_names
     if type(operator.inputs[0].type) in (BooleanTensorType, Int64TensorType):
         cast_input_name = scope.get_unique_variable_name('cast_input')
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/multilayer_perceptron.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/multilayer_perceptron.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/multiply_op.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/multiply_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/naive_bayes.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/nearest_neighbours.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/nearest_neighbours.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,40 +74,42 @@
     :param op_version: opset version
     :param keep_distance: returns the distances as well (second position)
     :param optim: implements specific optimisations,
         ``'cdist'`` replaces *Scan* operator by operator *CDist*
     :param kwargs: additional parameters for function @see fn onnx_cdist
     :return: top indices, top distances
     """
+    kwargs_dist = {k: v for k, v in kwargs.items() if k == 'p'}
+    kwargs_topk = {k: v for k, v in kwargs.items() if k != 'p'}
     if optim == 'cdist':
         from skl2onnx.algebra.custom_ops import OnnxCDist
         dist = OnnxCDist(X, Y, metric=metric, op_version=op_version,
-                         **kwargs)
+                         **kwargs_dist)
     elif optim is None:
         dim_in = Y.shape[1] if hasattr(Y, 'shape') else None
         dim_out = Y.shape[0] if hasattr(Y, 'shape') else None
         dist = onnx_cdist(X, Y, metric=metric, dtype=dtype,
                           op_version=op_version,
                           dim_in=dim_in, dim_out=dim_out,
-                          **kwargs)
+                          **kwargs_dist)
     else:
         raise ValueError("Unknown optimisation '{}'.".format(optim))
     if op_version < 10:
         neg_dist = OnnxMul(dist, np.array([-1], dtype=dtype),
                            op_version=op_version)
-        node = OnnxTopK_1(neg_dist, k=k, op_version=1, **kwargs)
+        node = OnnxTopK_1(neg_dist, k=k, op_version=1, **kwargs_topk)
     elif op_version < 11:
         neg_dist = OnnxMul(dist, np.array([-1], dtype=dtype),
                            op_version=op_version)
         node = OnnxTopK_10(neg_dist, np.array([k], dtype=np.int64),
-                           op_version=10, **kwargs)
+                           op_version=10, **kwargs_topk)
     else:
         node = OnnxTopK_11(dist, np.array([k], dtype=np.int64),
                            largest=0, sorted=1,
-                           op_version=11, **kwargs)
+                           op_version=11, **kwargs_topk)
         if keep_distances:
             return (node[1], OnnxMul(
                 node[0], np.array([-1], dtype=dtype), op_version=op_version))
     if keep_distances:
         return (node[1], node[0])
     return node[1]
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/normaliser.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/normaliser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/one_hot_encoder.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/one_vs_rest_classifier.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/one_vs_rest_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..common._registration import register_converter
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 from ..common._apply_operation import apply_normalization
 from ..common._apply_operation import (
     apply_slice, apply_sub, apply_cast, apply_abs, apply_add, apply_div)
 from ..common.utils_classifier import _finalize_converter_classes
-from ..common.data_types import guess_proto_type
+from ..common.data_types import guess_proto_type, Int64TensorType
 from .._supported_operators import sklearn_operator_name_map
 
 
 def convert_one_vs_rest_classifier(scope: Scope, operator: Operator,
                                    container: ModelComponentContainer):
     """
     Converts a *OneVsRestClassifier* into *ONNX* format.
@@ -47,15 +47,18 @@
                 raise RuntimeError("OneVsRestClassifier accepts "
                                    "regressor with only one target.")
             p1 = score_name.onnx_name
         else:
             if container.has_options(estimator, 'raw_scores'):
                 container.add_options(
                     id(estimator), {'raw_scores': use_raw_scores})
-            label_name = scope.declare_local_variable('label_%d' % i)
+                scope.add_options(
+                    id(estimator), {'raw_scores': use_raw_scores})
+            label_name = scope.declare_local_variable(
+                'label_%d' % i, Int64TensorType())
             prob_name = scope.declare_local_variable(
                 'proba_%d' % i, operator.inputs[0].type.__class__())
             this_operator.outputs.append(label_name)
             this_operator.outputs.append(prob_name)
 
             # gets the probability for the class 1
             p1 = scope.get_unique_variable_name('probY_%d' % i)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/ordinal_encoder.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/ordinal_encoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,18 @@
                         "{} input datatype not yet supported. "
                         "You may raise an issue at "
                         "https://github.com/onnx/sklearn-onnx/issues"
                         "".format(type(inp.type)))
 
         apply_concat(scope, input_names,
                      concatenated_input_name, container, axis=1)
+    if len(ordinal_op.categories_) == 0:
+        raise RuntimeError(
+            "No categories found in type=%r, encoder=%r." % (
+                type(ordinal_op), ordinal_op))
     for index, categories in enumerate(ordinal_op.categories_):
         attrs = {'name': scope.get_unique_operator_name('LabelEncoder')}
         if len(categories) > 0:
             if np.issubdtype(categories.dtype, np.floating):
                 attrs['keys_floats'] = categories
             elif np.issubdtype(categories.dtype, np.signedinteger):
                 attrs['keys_int64s'] = categories
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/polynomial_features.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/polynomial_features.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/power_transformer.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/power_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/random_forest.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/random_forest.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/random_projection.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/random_projection.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/ransac_regressor.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/ransac_regressor.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     """
     Converter for RANSACRegressor.
     """
     ransac_op = operator.raw_operator
     op_type = sklearn_operator_name_map[type(ransac_op.estimator_)]
     this_operator = scope.declare_local_operator(op_type, ransac_op.estimator_)
     this_operator.inputs = operator.inputs
-    label_name = scope.declare_local_variable('label')
+    label_name = scope.declare_local_variable(
+        'label', operator.inputs[0].type.__class__())
     this_operator.outputs.append(label_name)
     apply_identity(scope, label_name.full_name,
                    operator.outputs[0].full_name, container)
 
 
 register_converter('SklearnRANSACRegressor',
                    convert_sklearn_ransac_regressor)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/replace_op.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/replace_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/sgd_classifier.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/stacking.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/stacking.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 
 from ..proto import onnx_proto
 from ..common._apply_operation import (
     apply_cast, apply_concat, apply_reshape)
 from ..common._registration import register_converter
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
-from ..common.data_types import guess_proto_type
+from ..common.data_types import guess_proto_type, Int64TensorType
 from .._supported_operators import sklearn_operator_name_map
 
 
 def _fetch_scores(scope, container, model, inputs, raw_scores=False,
                   is_regressor=False):
     op_type = sklearn_operator_name_map[type(model)]
     this_operator = scope.declare_local_operator(op_type, model)
     if container.has_options(model, 'raw_scores'):
         container.add_options(id(model), {'raw_scores': raw_scores})
     this_operator.inputs.append(inputs)
-    label_name = scope.declare_local_variable('label')
-    this_operator.outputs.append(label_name)
     if is_regressor:
-        output_proba = label_name
+        output_proba = scope.declare_local_variable(
+            'variable', inputs.type.__class__())
+        this_operator.outputs.append(output_proba)
     else:
+        label_name = scope.declare_local_variable(
+            'label', Int64TensorType())
+        this_operator.outputs.append(label_name)
         output_proba = scope.declare_local_variable(
             'probability_tensor', inputs.type.__class__())
         this_operator.outputs.append(output_proba)
 
     proto_type = guess_proto_type(inputs.type)
     new_name = scope.get_unique_variable_name(
         output_proba.full_name + '_castio')
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/support_vector_machines.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/support_vector_machines.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,27 +178,32 @@
 
     handles_ovr = False
     svm_attrs['coefficients'] = svm_attrs['coefficients'].astype(np.float32)
     svm_attrs['support_vectors'] = svm_attrs['support_vectors'].astype(
         np.float32)
     svm_attrs['rho'] = svm_attrs['rho'].astype(np.float32)
 
+    options = container.get_options(op, dict(raw_scores=False))
+    use_raw_scores = options['raw_scores']
+
     if operator.type in ['SklearnSVC', 'SklearnNuSVC'] or isinstance(
             op, (SVC, NuSVC)):
-
         if len(op.probA_) > 0:
             svm_attrs['prob_a'] = op.probA_.astype(np.float32)
         else:
             handles_ovr = True
         if len(op.probB_) > 0:
             svm_attrs['prob_b'] = op.probB_.astype(np.float32)
 
         if (hasattr(op, 'decision_function_shape') and
-                op.decision_function_shape == 'ovr') and handles_ovr:
+                op.decision_function_shape == 'ovr' and handles_ovr and
+                len(op.classes_) > 2):
             output_name = scope.get_unique_variable_name('before_ovr')
+        elif len(op.classes_) == 2 and use_raw_scores:
+            output_name = scope.get_unique_variable_name('raw_scores')
         else:
             output_name = operator.outputs[1].full_name
 
         svm_attrs['post_transform'] = 'NONE'
         svm_attrs['vectors_per_class'] = op.n_support_.tolist()
 
         label_name = operator.outputs[0].full_name
@@ -217,20 +222,27 @@
         svm_out = scope.get_unique_variable_name('SVM02')
         container.add_node(
             op_type, operator.inputs[0].full_name,
             [label_name, svm_out],
             op_domain=op_domain, op_version=op_version, **svm_attrs)
         apply_cast(scope, svm_out, probability_tensor_name,
                    container, to=proto_dtype)
+        if len(op.classes_) == 2 and use_raw_scores:
+            minus_one = scope.get_unique_variable_name('minus_one')
+            container.add_initializer(minus_one, proto_dtype, [], [-1])
+            container.add_node(
+                'Mul', [output_name, minus_one], operator.outputs[1].full_name,
+                name=scope.get_unique_operator_name('MulRawScores'))
     else:
         raise ValueError("Unknown support vector machine model type found "
                          "'{0}'.".format(operator.type))
 
     if (hasattr(op, 'decision_function_shape') and
-            op.decision_function_shape == 'ovr' and handles_ovr):
+            op.decision_function_shape == 'ovr' and handles_ovr and
+            len(op.classes_) > 2):
         # Applies _ovr_decision_function.
         # See https://github.com/scikit-learn/scikit-learn/blob/
         # master/sklearn/utils/multiclass.py#L407:
         # ::
         #     _ovr_decision_function(dec < 0, -dec, len(self.classes_))
         #
         #     ...
@@ -352,9 +364,10 @@
             scope, [conc_vote, final], output_name, container, broadcast=0,
             operator_name='AddF1')
 
 
 register_converter('SklearnOneClassSVM', convert_sklearn_svm_regressor)
 register_converter('SklearnSVC', convert_sklearn_svm_classifier,
                    options={'zipmap': [True, False, 'columns'],
-                            'nocl': [True, False]})
+                            'nocl': [True, False],
+                            'raw_scores': [True, False]})
 register_converter('SklearnSVR', convert_sklearn_svm_regressor)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/text_vectoriser.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/text_vectoriser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/tfidf_transformer.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/tfidf_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/tfidf_vectoriser.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/tfidf_vectoriser.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,34 @@
     Converter for scikit-learn's TfidfVectoriser.
     """
     tfidf_op = operator.raw_operator
 
     op_type = sklearn_operator_name_map[CountVectorizer]
     cv_operator = scope.declare_local_operator(op_type, tfidf_op)
     cv_operator.inputs = operator.inputs
-    cv_output_name = scope.declare_local_variable('count_vec_output')
     columns = max(operator.raw_operator.vocabulary_.values()) + 1
     proto_dtype = guess_proto_type(operator.inputs[0].type)
     if proto_dtype != onnx_proto.TensorProto.DOUBLE:
         proto_dtype = onnx_proto.TensorProto.FLOAT
     if proto_dtype == onnx_proto.TensorProto.FLOAT:
         clr = FloatTensorType
     elif proto_dtype == onnx_proto.TensorProto.DOUBLE:
         clr = DoubleTensorType
     else:
         raise RuntimeError(
             "Unexpected dtype '{}'. Float or double expected.".format(
                 proto_dtype))
-    cv_output_name.type = clr([None, columns])
+    cv_output_name = scope.declare_local_variable(
+        'count_vec_output', clr([None, columns]))
     cv_operator.outputs.append(cv_output_name)
 
     op_type = sklearn_operator_name_map[TfidfTransformer]
     tfidf_operator = scope.declare_local_operator(op_type, tfidf_op)
     tfidf_operator.inputs.append(cv_output_name)
-    tfidf_output_name = scope.declare_local_variable('tfidf_output')
+    tfidf_output_name = scope.declare_local_variable('tfidf_output', clr())
     tfidf_operator.outputs.append(tfidf_output_name)
 
     apply_identity(scope, tfidf_output_name.full_name,
                    operator.outputs[0].full_name, container)
 
 
 register_converter('SklearnTfidfVectorizer', convert_sklearn_tfidf_vectoriser,
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/voting_classifier.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/voting_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from onnx.helper import make_tensor
 from ..common._registration import register_converter
 from ..common._topology import Scope, Operator
 from ..common._container import ModelComponentContainer
 from ..common._apply_operation import apply_mul
 from ..common.utils_classifier import _finalize_converter_classes
-from ..common.data_types import guess_proto_type
+from ..common.data_types import guess_proto_type, Int64TensorType
 from .._supported_operators import sklearn_operator_name_map
 from ..proto import onnx_proto
 
 
 def convert_voting_classifier(scope: Scope, operator: Operator,
                               container: ModelComponentContainer):
     """
@@ -47,17 +47,18 @@
             continue
 
         op_type = sklearn_operator_name_map[type(estimator)]
 
         this_operator = scope.declare_local_operator(op_type, estimator)
         this_operator.inputs = operator.inputs
 
-        label_name = scope.declare_local_variable('label_%d' % i)
+        label_name = scope.declare_local_variable(
+            'label_%d' % i, Int64TensorType())
         prob_name = scope.declare_local_variable(
-            'proba_%d' % i, operator.inputs[0].type.__class__())
+            'voting_proba_%d' % i, operator.inputs[0].type.__class__())
         this_operator.outputs.append(label_name)
         this_operator.outputs.append(prob_name)
 
         if op.voting == 'hard':
             if one_name is None:
                 shape_name = scope.get_unique_variable_name('shape')
                 container.add_node(
```

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/voting_regressor.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/voting_regressor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/operator_converters/zip_map.py` & `skl2onnx-1.9.3/skl2onnx/operator_converters/zip_map.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/proto/__init__.py` & `skl2onnx-1.9.3/skl2onnx/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/proto/onnx_helper_modified.py` & `skl2onnx-1.9.3/skl2onnx/proto/onnx_helper_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # Modified file from
 # https://github.com/onnx/onnx/blob/master/onnx/helper.py.
-import collections
 import numbers
 
 from onnx import (
     TensorProto, AttributeProto,
     NodeProto, GraphProto
 )
 from onnx.helper import (  # noqa
@@ -80,15 +79,19 @@
 ):  # type: (...) -> AttributeProto
     """Makes an AttributeProto based on the value type."""
     attr = AttributeProto()
     attr.name = key
     if doc_string:
         attr.doc_string = doc_string
 
-    is_iterable = isinstance(value, collections.abc.Iterable)
+    try:
+        iter(value)
+        is_iterable = True
+    except TypeError:
+        is_iterable = False
     bytes_or_false = _to_bytes_or_false(value)
 
     use_float64 = dtype == np.float64 and domain not in ('', 'ai.onnx.ml')
 
     if isinstance(value, np.float32):
         attr.f = value
         attr.type = AttributeProto.FLOAT
```

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/__init__.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 from . import flatten
 from . import function_transformer
 from . import gaussian_process
 from . import grid_search_cv
 from . import identity
 from . import imputer
 from . import isolation_forest
+from . import kernel_pca
 from . import k_bins_discretiser
 from . import k_means
 from . import label_binariser
 from . import label_encoder
 from . import linear_classifier
 from . import linear_regressor
+from . import local_outlier_factor
 from . import mixture
+from . import multioutput
 from . import nearest_neighbours
 from . import one_hot_encoder
 from . import ordinal_encoder
 from . import one_vs_rest_classifier
+from . import pipelines
 from . import polynomial_features
 from . import power_transformer
 from . import random_projection
 from . import replace_op
 from . import scaler
 from . import svd
 from . import support_vector_machines
@@ -50,25 +54,29 @@
     flatten,
     function_transformer,
     gaussian_process,
     grid_search_cv,
     identity,
     imputer,
     isolation_forest,
+    kernel_pca,
     k_bins_discretiser,
     k_means,
     label_binariser,
     label_encoder,
     linear_classifier,
     linear_regressor,
+    local_outlier_factor,
     mixture,
+    multioutput,
     nearest_neighbours,
     one_hot_encoder,
     ordinal_encoder,
     one_vs_rest_classifier,
+    pipelines,
     polynomial_features,
     power_transformer,
     random_projection,
     replace_op,
     scaler,
     svd,
     support_vector_machines,
```

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/array_feature_extractor.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/cast_op.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/cast_op.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/concat.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/concat.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/cross_decomposition.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/cross_decomposition.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/dict_vectorizer.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/dict_vectorizer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/ensemble_shapes.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/ensemble_shapes.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     check_input_and_output_numbers(operator, input_count_range=1,
                                    output_count_range=[1, 3])
     check_input_and_output_types(operator, good_input_types=[
         BooleanTensorType, DoubleTensorType,
         FloatTensorType, Int64TensorType])
 
     N = operator.inputs[0].get_first_dimension()
+    if operator.outputs[0].type is None:
+        raise RuntimeError(
+            "Output type is unknown for operator %r." % operator)
     operator.outputs[0].type.shape = [N, 1]
 
     # decision_path, decision_leaf
     for n in range(2, len(operator.outputs)):
         if hasattr(operator.raw_operator, 'estimators_'):
             # random forest
             operator.outputs[n].type.shape = [
@@ -47,14 +50,17 @@
 
 def calculate_tree_classifier_output_shapes(operator):
     _calculate_linear_classifier_output_shapes(operator, True, True)
     N = operator.inputs[0].get_first_dimension()
 
     # decision_path, decision_leaf
     for n in range(2, len(operator.outputs)):
+        if operator.outputs[n].type is None:
+            raise RuntimeError(
+                "Output type is unknown for operator %r." % operator)
         if hasattr(operator.raw_operator, 'estimators_'):
             # random forest
             operator.outputs[n].type.shape = [
                 N, len(operator.raw_operator.estimators_)]
         else:
             # single tree
             operator.outputs[n].type.shape = [N, 1]
```

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/flatten.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/flatten.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/function_transformer.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/function_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/gaussian_process.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/grid_search_cv.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/grid_search_cv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # SPDX-License-Identifier: Apache-2.0
 
-
-from ..common._registration import register_shape_calculator
-from ..common.shape_calculator import calculate_linear_classifier_output_shapes
-from ..common.shape_calculator import calculate_linear_regressor_output_shapes
-from .._supported_operators import sklearn_classifier_list
+import logging
+from ..common._registration import (
+    register_shape_calculator,
+    get_shape_calculator)
+from .._supported_operators import sklearn_operator_name_map
 
 
 def convert_sklearn_grid_search_cv(operator):
     grid_search_op = operator.raw_operator
     best_estimator = grid_search_op.best_estimator_
-    if type(best_estimator) in sklearn_classifier_list:
-        calculate_linear_classifier_output_shapes(operator)
-    else:
-        calculate_linear_regressor_output_shapes(operator)
+    name = sklearn_operator_name_map.get(type(best_estimator), None)
+    if name is None:
+        logger = logging.getLogger('skl2onnx')
+        logger.warn("[convert_sklearn_grid_search_cv] failed to find alias "
+                    "to model type %r." % type(best_estimator))
+        return
+    op = operator.new_raw_operator(best_estimator, name)
+    shape_calc = get_shape_calculator(name)
+    shape_calc(op)
+    operator.outputs = op.outputs
 
 
 register_shape_calculator('SklearnGridSearchCV',
                           convert_sklearn_grid_search_cv)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/imputer.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/imputer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/k_bins_discretiser.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/k_bins_discretiser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/k_means.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/k_means.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/label_binariser.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/label_binariser.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/label_encoder.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/label_encoder.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/linear_classifier.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/linear_classifier.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/linear_regressor.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/mixture.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/mixture.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/nearest_neighbours.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/one_hot_encoder.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/ordinal_encoder.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/polynomial_features.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/polynomial_features.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/scaler.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/scaler.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,17 @@
                     for variable in operator.inputs))
                 > 1):
             raise RuntimeError('Batch size must be identical across inputs.')
 
     N = operator.inputs[0].get_first_dimension()
     C = 0
     for variable in operator.inputs:
-        if isinstance(variable.get_first_dimension(), numbers.Integral):
-            C += variable.get_first_dimension()
+        c = variable.get_second_dimension()
+        if isinstance(c, numbers.Integral):
+            C += c
         else:
             C = None
             break
 
     operator.outputs[0].type.shape = [N, C]
```

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/support_vector_machines.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/support_vector_machines.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     elif operator.type in ['SklearnSVR']:
         check_input_and_output_numbers(operator, input_count_range=[1, None],
                                        output_count_range=1)
 
         operator.outputs[0].type.shape = [N, 1]
     else:
         raise RuntimeError(
-            "New kind of SVM, no shape calculer exist for '{}'.".format(
+            "New kind of SVM, no shape calculator exist for '{}'.".format(
                 operator.type))
 
 
 register_shape_calculator(
     'SklearnOneClassSVM', calculate_sklearn_svm_output_shapes)
 register_shape_calculator('SklearnSVC', calculate_sklearn_svm_output_shapes)
 register_shape_calculator('SklearnSVR', calculate_sklearn_svm_output_shapes)
```

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/svd.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/svd.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/text_vectorizer.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/text_vectorizer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/tfidf_transformer.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/tfidf_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/shape_calculators/zip_map.py` & `skl2onnx-1.9.3/skl2onnx/shape_calculators/zip_map.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/sklapi/cast_regressor.py` & `skl2onnx-1.9.3/skl2onnx/sklapi/cast_regressor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/sklapi/cast_transformer.py` & `skl2onnx-1.9.3/skl2onnx/sklapi/cast_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/sklapi/replace_transformer.py` & `skl2onnx-1.9.3/skl2onnx/sklapi/replace_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/tutorial/benchmark.py` & `skl2onnx-1.9.3/skl2onnx/tutorial/benchmark.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx/tutorial/imagenet_classes.py` & `skl2onnx-1.9.3/skl2onnx/tutorial/imagenet_classes.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/skl2onnx.egg-info/PKG-INFO` & `skl2onnx-1.9.3/skl2onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skl2onnx
-Version: 1.9.2
+Version: 1.9.3
 Summary: Convert scikit-learn models to ONNX
 Home-page: https://github.com/onnx/sklearn-onnx
 Author: Microsoft Corporation
 Author-email: onnx@microsoft.com
 License: Apache License v2.0
 Description: ## Introduction
         *sklearn-onnx* converts [scikit-learn](https://scikit-learn.org/stable/) models to [ONNX](https://github.com/onnx/onnx). Once in the ONNX format, you can use tools like [ONNX Runtime](https://github.com/Microsoft/onnxruntime) for high performance scoring.
```

### Comparing `skl2onnx-1.9.2/skl2onnx.egg-info/SOURCES.txt` & `skl2onnx-1.9.3/skl2onnx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,48 +38,56 @@
 docs/examples/plot_custom_model.py
 docs/examples/plot_custom_parser.py
 docs/examples/plot_custom_parser_alternative.py
 docs/examples/plot_errors_onnxruntime.py
 docs/examples/plot_gpr.py
 docs/examples/plot_intermediate_outputs.py
 docs/examples/plot_investigate_pipeline.py
+docs/examples/plot_logging.py
 docs/examples/plot_metadata.py
 docs/examples/plot_nmf.py
 docs/examples/plot_onnx_operators.py
 docs/examples/plot_pipeline.py
 docs/examples/plot_pipeline_lightgbm.py
 docs/examples/plot_pipeline_xgboost.py
 docs/examples/plot_tfidfvectorizer.py
 docs/exts/github_link.py
 docs/exts/sphinx_skl2onnx_extension.py
+docs/exts/__pycache__/github_link.cpython-39.pyc
+docs/exts/__pycache__/sphinx_skl2onnx_extension.cpython-39.pyc
+docs/images/woe.png
 docs/tests/test_documentation_examples.py
 docs/tests/test_documentation_tutorial.py
 docs/tests/test_utils_benchmark.py
 docs/tests/test_utils_classes.py
 docs/tutorial/README.txt
 docs/tutorial/plot_abegin_convert_pipeline.py
 docs/tutorial/plot_bbegin_measure_time.py
+docs/tutorial/plot_catwoe_transformer.py
 docs/tutorial/plot_cbegin_opset.py
 docs/tutorial/plot_dbegin_options.py
 docs/tutorial/plot_dbegin_options_list.py
 docs/tutorial/plot_ebegin_float_double.py
 docs/tutorial/plot_fbegin_investigate.py
+docs/tutorial/plot_gbegin_cst.py
 docs/tutorial/plot_gbegin_dataframe.py
 docs/tutorial/plot_gbegin_transfer_learning.py
 docs/tutorial/plot_gexternal_lightgbm.py
+docs/tutorial/plot_gexternal_lightgbm_reg.py
 docs/tutorial/plot_gexternal_xgboost.py
 docs/tutorial/plot_icustom_converter.py
 docs/tutorial/plot_jcustom_syntax.py
 docs/tutorial/plot_kcustom_converter_wrapper.py
 docs/tutorial/plot_lcustom_options.py
 docs/tutorial/plot_mcustom_parser.py
 docs/tutorial/plot_pextend_python_runtime.py
 docs/tutorial/plot_qextend_onnxruntime.py
 docs/tutorial/plot_usparse_xgboost.py
 docs/tutorial/plot_wext_pyod_forest.py
+docs/tutorial/plot_woe_transformer.py
 skl2onnx/__init__.py
 skl2onnx/_parse.py
 skl2onnx/_supported_operators.py
 skl2onnx/convert.py
 skl2onnx.egg-info/PKG-INFO
 skl2onnx.egg-info/SOURCES.txt
 skl2onnx.egg-info/dependency_links.txt
@@ -100,15 +108,14 @@
 skl2onnx/common/_apply_operation.py
 skl2onnx/common/_container.py
 skl2onnx/common/_onnx_optimisation_common.py
 skl2onnx/common/_registration.py
 skl2onnx/common/_topology.py
 skl2onnx/common/data_types.py
 skl2onnx/common/exceptions.py
-skl2onnx/common/interface.py
 skl2onnx/common/onnx_optimisation_identity.py
 skl2onnx/common/shape_calculator.py
 skl2onnx/common/tree_ensemble.py
 skl2onnx/common/utils.py
 skl2onnx/common/utils_checking.py
 skl2onnx/common/utils_classifier.py
 skl2onnx/common/utils_sklearn.py
@@ -138,26 +145,30 @@
 skl2onnx/operator_converters/gradient_boosting.py
 skl2onnx/operator_converters/grid_search_cv.py
 skl2onnx/operator_converters/id_op.py
 skl2onnx/operator_converters/imputer_op.py
 skl2onnx/operator_converters/isolation_forest.py
 skl2onnx/operator_converters/k_bins_discretiser.py
 skl2onnx/operator_converters/k_means.py
+skl2onnx/operator_converters/kernel_pca.py
 skl2onnx/operator_converters/label_binariser.py
 skl2onnx/operator_converters/label_encoder.py
 skl2onnx/operator_converters/linear_classifier.py
 skl2onnx/operator_converters/linear_regressor.py
+skl2onnx/operator_converters/local_outlier_factor.py
 skl2onnx/operator_converters/multilayer_perceptron.py
+skl2onnx/operator_converters/multioutput.py
 skl2onnx/operator_converters/multiply_op.py
 skl2onnx/operator_converters/naive_bayes.py
 skl2onnx/operator_converters/nearest_neighbours.py
 skl2onnx/operator_converters/normaliser.py
 skl2onnx/operator_converters/one_hot_encoder.py
 skl2onnx/operator_converters/one_vs_rest_classifier.py
 skl2onnx/operator_converters/ordinal_encoder.py
+skl2onnx/operator_converters/pipelines.py
 skl2onnx/operator_converters/polynomial_features.py
 skl2onnx/operator_converters/power_transformer.py
 skl2onnx/operator_converters/random_forest.py
 skl2onnx/operator_converters/random_projection.py
 skl2onnx/operator_converters/ransac_regressor.py
 skl2onnx/operator_converters/replace_op.py
 skl2onnx/operator_converters/scaler_op.py
@@ -184,23 +195,27 @@
 skl2onnx/shape_calculators/gaussian_process.py
 skl2onnx/shape_calculators/grid_search_cv.py
 skl2onnx/shape_calculators/identity.py
 skl2onnx/shape_calculators/imputer.py
 skl2onnx/shape_calculators/isolation_forest.py
 skl2onnx/shape_calculators/k_bins_discretiser.py
 skl2onnx/shape_calculators/k_means.py
+skl2onnx/shape_calculators/kernel_pca.py
 skl2onnx/shape_calculators/label_binariser.py
 skl2onnx/shape_calculators/label_encoder.py
 skl2onnx/shape_calculators/linear_classifier.py
 skl2onnx/shape_calculators/linear_regressor.py
+skl2onnx/shape_calculators/local_outlier_factor.py
 skl2onnx/shape_calculators/mixture.py
+skl2onnx/shape_calculators/multioutput.py
 skl2onnx/shape_calculators/nearest_neighbours.py
 skl2onnx/shape_calculators/one_hot_encoder.py
 skl2onnx/shape_calculators/one_vs_rest_classifier.py
 skl2onnx/shape_calculators/ordinal_encoder.py
+skl2onnx/shape_calculators/pipelines.py
 skl2onnx/shape_calculators/polynomial_features.py
 skl2onnx/shape_calculators/power_transformer.py
 skl2onnx/shape_calculators/random_projection.py
 skl2onnx/shape_calculators/replace_op.py
 skl2onnx/shape_calculators/scaler.py
 skl2onnx/shape_calculators/support_vector_machines.py
 skl2onnx/shape_calculators/svd.py
@@ -208,24 +223,28 @@
 skl2onnx/shape_calculators/tfidf_transformer.py
 skl2onnx/shape_calculators/voting_classifier.py
 skl2onnx/shape_calculators/voting_regressor.py
 skl2onnx/shape_calculators/zip_map.py
 skl2onnx/sklapi/__init__.py
 skl2onnx/sklapi/cast_regressor.py
 skl2onnx/sklapi/cast_transformer.py
+skl2onnx/sklapi/register.py
 skl2onnx/sklapi/replace_transformer.py
+skl2onnx/sklapi/woe_transformer.py
+skl2onnx/sklapi/woe_transformer_onnx.py
 skl2onnx/tutorial/__init__.py
 skl2onnx/tutorial/benchmark.py
 skl2onnx/tutorial/imagenet_classes.py
 tests/benchmark.py
 tests/bug.onnx
 tests/test_algebra_cascade.py
 tests/test_algebra_complex.py
 tests/test_algebra_converters.py
 tests/test_algebra_custom_model.py
+tests/test_algebra_custom_model_sub_estimator.py
 tests/test_algebra_deprecation.py
 tests/test_algebra_double.py
 tests/test_algebra_onnx_doc.py
 tests/test_algebra_onnx_operator_mixin_syntax.py
 tests/test_algebra_onnx_operators.py
 tests/test_algebra_onnx_operators_opset.py
 tests/test_algebra_onnx_operators_scan.py
@@ -233,20 +252,22 @@
 tests/test_algebra_onnx_operators_sub_estimator.py
 tests/test_algebra_onnx_operators_wrapped.py
 tests/test_algebra_symbolic.py
 tests/test_algebra_test_helper.py
 tests/test_algebra_to_onnx.py
 tests/test_applied_functions.py
 tests/test_convert.py
-tests/test_custom_transformer.py
+tests/test_custom_transformer_ordwoe.py
+tests/test_custom_transformer_tsne.py
 tests/test_investigate.py
 tests/test_onnx_helper.py
 tests/test_onnx_rare_helper.py
 tests/test_op10.py
 tests/test_opset13.py
+tests/test_options.py
 tests/test_other_converter_library_pipelines.py
 tests/test_parsing_options.py
 tests/test_raw_name.py
 tests/test_scikit_pandas.py
 tests/test_shapes.py
 tests/test_sklearn_adaboost_converter.py
 tests/test_sklearn_array_feature_extractor.py
@@ -275,17 +296,20 @@
 tests/test_sklearn_glm_regressor_converter.py
 tests/test_sklearn_gradient_boosting_converters.py
 tests/test_sklearn_grid_search_cv_converter.py
 tests/test_sklearn_imputer_converter.py
 tests/test_sklearn_isolation_forest.py
 tests/test_sklearn_k_bins_discretiser_converter.py
 tests/test_sklearn_k_means_converter.py
+tests/test_sklearn_kernel_pca_converter.py
 tests/test_sklearn_label_binariser_converter.py
 tests/test_sklearn_label_encoder_converter.py
+tests/test_sklearn_local_outlier_factor.py
 tests/test_sklearn_mlp_converter.py
+tests/test_sklearn_multi_output.py
 tests/test_sklearn_naive_bayes_converter.py
 tests/test_sklearn_nearest_neighbour_converter.py
 tests/test_sklearn_normalizer_converter.py
 tests/test_sklearn_one_hot_encoder_converter.py
 tests/test_sklearn_one_vs_rest_classifier_converter.py
 tests/test_sklearn_ordinal_encoder.py
 tests/test_sklearn_passive_aggressive_classifier_converter.py
@@ -309,16 +333,18 @@
 tests/test_sklearn_tfidf_vectorizer_converter_char.py
 tests/test_sklearn_tfidf_vectorizer_converter_dataset.py
 tests/test_sklearn_tfidf_vectorizer_converter_pipeline.py
 tests/test_sklearn_tfidf_vectorizer_converter_regex.py
 tests/test_sklearn_truncated_svd.py
 tests/test_sklearn_voting_classifier_converter.py
 tests/test_sklearn_voting_regressor_converter.py
+tests/test_sklearn_woe_transformer.py
 tests/test_supported_converters.py
 tests/test_topology_prune.py
 tests/test_utils_sklearn.py
+tests/test_variable_names.py
 tests/datasets/small_titanic.csv
 tests/test_utils/__init__.py
 tests/test_utils/main.py
 tests/test_utils/tests_helper.py
 tests/test_utils/utils_backend.py
 tests/test_utils/utils_backend_onnxruntime.py
```

### Comparing `skl2onnx-1.9.2/tests/benchmark.py` & `skl2onnx-1.9.3/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/datasets/small_titanic.csv` & `skl2onnx-1.9.3/tests/datasets/small_titanic.csv`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_cascade.py` & `skl2onnx-1.9.3/tests/test_algebra_cascade.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_complex.py` & `skl2onnx-1.9.3/tests/test_algebra_complex.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,27 +28,28 @@
                             (np.complex128, Complex128TensorType, 15)):
             X = np.array([[1-2j, -12j],
                           [-1-2j, 1+2j]]).astype(dt)
 
             for opv in (10, 11, 12, 13, TARGET_OPSET):
                 if opv > TARGET_OPSET:
                     continue
-                out = OnnxAdd('X', np.array([1+2j]), output_names=['Y'],
-                              op_version=opv)
-                onx = out.to_onnx([('X', var((None, 2)))],
-                                  outputs=[('Y', var())],
-                                  target_opset=opv)
-                self.assertIn('elem_type: %d' % pr, str(onx))
+                with self.subTest(dt=dt, opset=opv):
+                    out = OnnxAdd('X', np.array([1+2j], dtype=dt),
+                                  output_names=['Y'], op_version=opv)
+                    onx = out.to_onnx([('X', var((None, 2)))],
+                                      outputs=[('Y', var())],
+                                      target_opset=opv)
+                    self.assertIn('elem_type: %d' % pr, str(onx))
 
-                try:
-                    ort = InferenceSession(onx.SerializeToString())
-                except InvalidGraph as e:
-                    if "Type Error: Type 'tensor(complex" in str(e):
-                        continue
-                    raise e
-                assert ort is not None
-                got = ort.run(None, {'X': X})[0]
-                assert_almost_equal(X + np.array([1+2j]), got)
+                    try:
+                        ort = InferenceSession(onx.SerializeToString())
+                    except InvalidGraph as e:
+                        if "Type Error: Type 'tensor(complex" in str(e):
+                            continue
+                        raise e
+                    assert ort is not None
+                    got = ort.run(None, {'X': X})[0]
+                    assert_almost_equal(X + np.array([1+2j]), got)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `skl2onnx-1.9.2/tests/test_algebra_converters.py` & `skl2onnx-1.9.3/tests/test_algebra_converters.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_custom_model.py` & `skl2onnx-1.9.3/tests/test_algebra_custom_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         self.W_ = np.mean(X, axis=0)
         self.S_ = np.std(X, axis=0)
         return self
 
     def transform(self, X):
         return (X - self.W_) / self.S_
 
-    def to_onnx_operator(self, inputs=None, outputs=('Y', )):
+    def to_onnx_operator(self, inputs=None, outputs=None,
+                         target_opset=None, **kwargs):
         if inputs is None:
             raise RuntimeError("inputs should contain one name")
         i0 = self.get_inputs(inputs, 0)
         W = self.W_.astype(np.float32)
         S = self.S_.astype(np.float32)
         # case if there are multiple output nodes
         return OnnxDiv(OnnxSub(i0, W, op_version=self.op_version), S,
@@ -67,48 +68,44 @@
         model.fit(data)
         try:
             model_onnx = convert_sklearn(model, target_opset=TARGET_OPSET)
             assert model_onnx is not None
         except RuntimeError as e:
             assert "Method enumerate_initial_types is missing" in str(e)
 
+    @unittest.skipIf(StrictVersion(onnx.__version__) <= StrictVersion("1.7.0"),
+                     reason="checm_model crashes")
     def test_custom_scaler(self):
         mat = np.array([[0., 1.], [0., 1.], [2., 2.]])
         tr = CustomOpTransformerShape(op_version=TARGET_OPSET)
         tr.fit(mat)
         z = tr.transform(mat)
         assert z is not None
 
         matf = mat.astype(np.float32)
         model_onnx = tr.to_onnx(matf)
-        # Next instructions fails...
-        # Field 'shape' of type is required but missing.
-        # onnx.checker.check_model(model_onnx)
-
+        onnx.checker.check_model(model_onnx)
         dump_data_and_model(
             mat.astype(np.float32), tr, model_onnx,
             basename="CustomTransformerAlgebra")
 
+    @unittest.skipIf(StrictVersion(onnx.__version__) <= StrictVersion("1.7.0"),
+                     reason="checm_model crashes")
     def test_custom_scaler_pipeline_right(self):
         pipe = make_pipeline(
             StandardScaler(),
             CustomOpTransformerShape(op_version=TARGET_OPSET))
         mat = np.array([[0., 1.], [0., 1.], [2., 2.]])
         pipe.fit(mat)
         z = pipe.transform(mat)
         assert z is not None
 
         matf = mat.astype(np.float32)
         model_onnx = to_onnx(pipe, matf, target_opset=TARGET_OPSET)
-        # Next instructions fails...
-        # Field 'shape' of type is required but missing.
-        # onnx.checker.check_model(model_onnx)
-
-        # use assert_consistent_outputs
-        # calls dump_data_and_model
+        onnx.checker.check_model(model_onnx)
         dump_data_and_model(
             mat.astype(np.float32), pipe, model_onnx,
             basename="CustomTransformerPipelineRightAlgebra")
 
     @unittest.skipIf(StrictVersion(onnx.__version__) <= StrictVersion("1.3.0"),
                      reason="not available")
     def test_custom_scaler_pipeline_left(self):
@@ -120,31 +117,31 @@
         z = pipe.transform(mat)
 
         matf = mat.astype(np.float32)
 
         try:
             model_onnx = to_onnx(pipe, matf, target_opset=TARGET_OPSET)
         except RuntimeError as e:
-            assert "cannot be infered" in str(e)
+            assert "inputs should contain one name" in str(e)
 
         pipe = make_pipeline(
             CustomOpTransformerShape(op_version=TARGET_OPSET),
             StandardScaler())
         mat = np.array([[0., 1.], [0., 1.], [2., 2.]])
         pipe.fit(mat)
         z = pipe.transform(mat)
         assert z is not None
 
         matf = mat.astype(np.float32)
 
         model_onnx = to_onnx(pipe, matf, target_opset=TARGET_OPSET)
 
-        # Next instructions fails...
-        # Field 'shape' of type is required but missing.
-        # onnx.checker.check_model(model_onnx)
+        if StrictVersion(onnx.__version__) >= StrictVersion("1.8.0"):
+            # It fails for older version of onnx.
+            onnx.checker.check_model(model_onnx)
 
         dump_data_and_model(
             mat.astype(np.float32), pipe, model_onnx,
             basename="CustomTransformerPipelineLeftAlgebra")
 
 
 if __name__ == "__main__":
```

### Comparing `skl2onnx-1.9.2/tests/test_algebra_deprecation.py` & `skl2onnx-1.9.3/tests/test_algebra_deprecation.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_double.py` & `skl2onnx-1.9.3/tests/test_algebra_double.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_doc.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_doc.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_operator_mixin_syntax.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_operator_mixin_syntax.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         return (X - self.W_) / self.S_
 
     def onnx_shape_calculator(self):
         def shape_calculator(operator):
             operator.outputs[0].type = operator.inputs[0].type
         return shape_calculator
 
-    def to_onnx_operator(self, inputs=None, outputs=('Y', )):
+    def to_onnx_operator(self, inputs=None, outputs=('Y', ),
+                         target_opset=None, **kwargs):
         if inputs is None:
             raise RuntimeError("inputs should contain one name")
         i0 = self.get_inputs(inputs, 0)
         W = self.W_.astype(np.float32)
         S = self.S_.astype(np.float32)
         return OnnxDiv(
             OnnxSub(
@@ -239,40 +240,49 @@
         except RuntimeError as e:
             if ("Could not find an implementation for the node "
                     "Cl_Clip:Clip(11)" in str(e)):
                 # Not yet implemented in onnxruntime
                 return
             raise e
         X = X.astype(np.float32)
-        got = oinf.run(None, {'X': X})[0]
+        try:
+            got = oinf.run(None, {'X': X})[0]
+        except Exception as e:
+            raise AssertionError(
+                "Cannot run model due to %r\n%r\n%s" % (
+                    e, onx, str(model_def))) from e
         assert_almost_equal(np_fct(X), got, decimal=6)
 
     @unittest.skipIf(onnx.defs.onnx_opset_version() < 10, "irrelevant")
     def test_onnx_clip_10(self):
-        self.common_test_onnxt_runtime_unary(
-            lambda x, output_names=None: OnnxClip_6(
-                x, min=1e-5, max=1e5, output_names=output_names),
-            lambda x: np.clip(x, 1e-5, 1e5),
-            op_version=10)
-        self.common_test_onnxt_runtime_unary(
-            lambda x, output_names=None: OnnxClip(
-                x, min=1e-5, max=1e5, output_names=output_names,
-                op_version=10),
-            lambda x: np.clip(x, 1e-5, 1e5),
-            op_version=10)
-        self.common_test_onnxt_runtime_unary(
-            lambda x, output_names=None: OnnxClip(
-                x, max=1e-5, output_names=output_names,
-                op_version=10),
-            lambda x: np.clip(x, -1e5, 1e-5),
-            op_version=10)
-        self.common_test_onnxt_runtime_unary(
-            lambda x, output_names=None: OnnxClip(
-                x, min=0.1, max=2.1,
-                output_names=output_names,
-                op_version=10),
-            lambda x: np.clip(x, 0.1, 2.1),
-            op_version=10)
+        with self.subTest(name="OnnxClip_6[1e-5, 1e5]"):
+            self.common_test_onnxt_runtime_unary(
+                lambda x, output_names=None: OnnxClip_6(
+                    x, min=1e-5, max=1e5, output_names=output_names),
+                lambda x: np.clip(x, 1e-5, 1e5),
+                op_version=10)
+        with self.subTest(name="OnnxClip-10[1e-5, 1e5]"):
+            self.common_test_onnxt_runtime_unary(
+                lambda x, output_names=None: OnnxClip(
+                    x, min=1e-5, max=1e5, output_names=output_names,
+                    op_version=10),
+                lambda x: np.clip(x, 1e-5, 1e5),
+                op_version=10)
+        with self.subTest(name="OnnxClip-10[-1e5, 1e-5]"):
+            self.common_test_onnxt_runtime_unary(
+                lambda x, output_names=None: OnnxClip(
+                    x, max=1e-5, output_names=output_names,
+                    op_version=10),
+                lambda x: np.clip(x, -1e5, 1e-5),
+                op_version=10)
+        with self.subTest(name="OnnxClip-10[0.1, 2.1]"):
+            self.common_test_onnxt_runtime_unary(
+                lambda x, output_names=None: OnnxClip(
+                    x, min=0.1, max=2.1,
+                    output_names=output_names,
+                    op_version=10),
+                lambda x: np.clip(x, 0.1, 2.1),
+                op_version=10)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_operators.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 from sklearn.cluster import KMeans
 from sklearn.datasets import load_iris
 from sklearn.utils.extmath import row_norms
 from onnxruntime import InferenceSession
 from skl2onnx import convert_sklearn
 from skl2onnx.common._topology import Variable
 from skl2onnx.common.data_types import (
-    FloatTensorType, guess_numpy_type, DoubleTensorType)
+    FloatTensorType, guess_numpy_type)
 from skl2onnx.algebra.onnx_operator import OnnxOperator
 from skl2onnx.algebra.onnx_ops import (
     OnnxSub, OnnxDiv, OnnxReshapeApi13,
     OnnxReduceSumSquare, OnnxGemm,
     OnnxAdd, OnnxArgMin, OnnxSqrt,
     OnnxArrayFeatureExtractor, OnnxMul,
-    OnnxPad, OnnxBatchNormalization)
+    OnnxPad, OnnxBatchNormalization,
+    OnnxConstantOfShape)
 from test_utils import dump_data_and_model, TARGET_OPSET
 
 
 class TestOnnxOperators(unittest.TestCase):
 
     def test_sub(self):
 
@@ -60,22 +61,22 @@
             text = str(container)
             if 'name:"Su_Sub"' not in text:
                 raise AssertionError(
                     "Unnamed operator: '{}'".format(text))
             nin = list(op.enumerate_initial_types())
             nno = list(op.enumerate_nodes())
             nva = list(op.enumerate_variables())
-            assert len(nin) == 1
-            assert nin[0][0] == 'input'
-            assert nin[0][1].shape == [None, 2]
-            assert len(nno) == 1
-            assert nno[0].output_names == ['variable']
-            assert len(nva) == 1
+            self.assertEqual(len(nin), 1)
+            self.assertEqual(nin[0][0], 'input')
+            self.assertEqual(nin[0][1].shape, [None, 2])
+            self.assertEqual(len(nno), 1)
+            self.assertEqual(nno[0].output_names[0].onnx_name, 'variable')
+            self.assertEqual(len(nva), 1)
             assert isinstance(nva[0], tuple)
-            assert nva[0][1] == 0
+            self.assertEqual(nva[0][1], 0)
 
         def shape(operator):
             N = operator.inputs[0].type.shape[0]
             W = operator.raw_operator.W
             operator.outputs[0].type.shape = [N, W.shape[0]]
 
         model_onnx = convert_sklearn(
@@ -199,42 +200,83 @@
         self.assertEqual(var1, "a")
         self.assertEqual(repr(var1), "UnscopedVariable('a')")
 
     def test_constant(self):
         cst = OnnxOperator.ConstantVariable("a")
         self.assertEqual(cst.value, "a")
 
+    def test_constant_of_shape(self):
+        for opset in [TARGET_OPSET, 14, 13, 12, 11, 10, 9]:
+            for value in [np.array([5], dtype=np.float32),
+                          np.array(5, dtype=np.float32)]:
+                if opset > TARGET_OPSET:
+                    continue
+                with self.subTest(opset=opset, value=value):
+                    tensor_value = onnx.helper.make_tensor(
+                        "value", onnx.TensorProto.FLOAT,
+                        [1], [5])
+
+                    cst = OnnxConstantOfShape(
+                        'X', value=tensor_value, op_version=opset,
+                        output_names=['Y'])
+                    shape = np.array([3, 4], dtype=np.int64)
+                    onx = cst.to_onnx(
+                        {'X': shape}, target_opset=opset,
+                        outputs=[('Y', FloatTensorType())])
+                    sess = InferenceSession(onx.SerializeToString())
+                    res = sess.run(None, {'X': shape})
+                    assert_almost_equal(
+                        res[0], np.full(tuple(shape), 5, dtype=np.float32))
+
+                    cst = OnnxConstantOfShape(
+                        'X', value=value, op_version=opset,
+                        output_names=['Y'])
+                    shape = np.array([3, 4], dtype=np.int64)
+                    onx = cst.to_onnx(
+                        {'X': shape}, target_opset=opset,
+                        outputs=[('Y', FloatTensorType())])
+                    sess = InferenceSession(onx.SerializeToString())
+                    res = sess.run(None, {'X': shape})
+                    assert_almost_equal(
+                        res[0], np.full(tuple(shape), 5, dtype=np.float32))
+
+        for opset in [TARGET_OPSET]:
+            for value in [5, np.float32(5)]:
+                with self.subTest(opset=opset, value=value):
+                    with self.assertRaises(TypeError):
+                        OnnxConstantOfShape(
+                            'X', value=value, op_version=opset,
+                            output_names=['Y'])
+
     @unittest.skipIf(StrictVersion(onnx__version__) < StrictVersion("1.4.0"),
                      reason="only available for opset >= 10")
     def test_onnx_reversed_order(self):
         idi = np.identity(2)
         idi2 = np.identity(2) * 2
 
         onx = OnnxAdd(
-            OnnxAdd('X', idi, op_version=TARGET_OPSET),
-            idi2, output_names=['Y'],
+            OnnxAdd('X', idi.astype(np.float32), op_version=TARGET_OPSET),
+            idi2.astype(np.float32), output_names=['Y'],
             op_version=TARGET_OPSET)
         model_def = onx.to_onnx({'X': idi.astype(np.float32)})
         self.assertEqual(len(model_def.graph.output), 1)
         onx = OnnxAdd(
-            idi2,
-            OnnxAdd(
-                'X', idi, op_version=TARGET_OPSET),
-            output_names=['Y'],
-            op_version=TARGET_OPSET)
+            idi2.astype(np.float32),
+            OnnxAdd('X', idi.astype(np.float32), op_version=TARGET_OPSET),
+            output_names=['Y'], op_version=TARGET_OPSET)
         model_def = onx.to_onnx({'X': idi.astype(np.float32)})
         onnx2 = model_def.SerializeToString()
         self.assertIsInstance(onx.outputs, list)
         self.assertEqual(len(onx.outputs), 1)
         self.assertIsInstance(onx.outputs[0], (Variable, tuple))
         if isinstance(onx.outputs[0], tuple):
             self.assertEqual(len(onx.outputs[0]), 2)
-            self.assertIsInstance(onx.outputs[0][1], DoubleTensorType)
+            self.assertIsInstance(onx.outputs[0][1], FloatTensorType)
         else:
-            self.assertIsInstance(onx.outputs[0].type, DoubleTensorType)
+            self.assertIsInstance(onx.outputs[0].type, FloatTensorType)
         # There should be 2 outputs here, bug in ONNX?
         self.assertEqual(len(model_def.graph.output), 1)
         reload = load_model(BytesIO(onnx2))
         self.assertEqual(len(reload.graph.output), 1)
         assert reload is not None
 
     def test_onnx_reversed_order_second(self):
```

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_operators_opset.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_operators_opset.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_operators_scan.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_operators_scan.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_operators_sparse.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_operators_sparse.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,16 +55,17 @@
         data = np.array([1, 1, 1, 1, 1], dtype=np.float32)
         X = coo_matrix((data, (row, col)), shape=(4, 4))
 
         node = OnnxAdd(
             'X', X, output_names=['Y'],
             op_version=TARGET_OPSET)
 
-        model_def = node.to_onnx({'X': X},
-                                 outputs=[('Y', FloatTensorType())])
+        model_def = node.to_onnx(
+            {'X': X}, outputs=[('Y', FloatTensorType())])
+        print(model_def)
 
         try:
             sess = InferenceSession(model_def.SerializeToString())
         except (RuntimeError, OrtInvalidArgument):
             # Sparse tensor is not supported for constant.
             return
         try:
```

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_operators_sub_estimator.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_operators_sub_estimator.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_onnx_operators_wrapped.py` & `skl2onnx-1.9.3/tests/test_algebra_onnx_operators_wrapped.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from numpy.testing import assert_almost_equal
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.datasets import load_iris
 from sklearn.decomposition import PCA
 from onnxruntime import InferenceSession
 from skl2onnx import to_onnx
 from skl2onnx.algebra.onnx_ops import OnnxIdentity
-from skl2onnx.algebra.onnx_operator import OnnxSubEstimator as SubOp
+from skl2onnx.algebra.onnx_operator import OnnxSubEstimator
 from skl2onnx import update_registered_converter
 from onnxruntime import __version__ as ortv
 from test_utils import TARGET_OPSET
 
 
 class DecorrelateTransformer(TransformerMixin, BaseEstimator):
 
@@ -57,25 +57,25 @@
 
 
 def decorrelate_transformer_convertor(scope, operator, container):
     op = operator.raw_operator
     opv = container.target_opset
     out = operator.outputs
     X = operator.inputs[0]
-    subop = SubOp(op.pca_, X, op_version=opv)
+    subop = OnnxSubEstimator(op.pca_, X, op_version=opv)
     Y = OnnxIdentity(subop, op_version=opv, output_names=out[:1])
     Y.add_to(scope, container)
 
 
 def decorrelate_transformer_convertor2(scope, operator, container):
     op = operator.raw_operator
     opv = container.target_opset
     out = operator.outputs
     X = operator.inputs[0]
-    Y = SubOp(op.pca_, X, op_version=opv, output_names=out[:1])
+    Y = OnnxSubEstimator(op.pca_, X, op_version=opv, output_names=out[:1])
     Y.add_to(scope, container)
 
 
 class TestOnnxOperatorsWrapped(unittest.TestCase):
 
     @unittest.skipIf(StrictVersion(ortv) < StrictVersion('0.5.0'),
                      reason="onnxruntime too old")
```

### Comparing `skl2onnx-1.9.2/tests/test_algebra_symbolic.py` & `skl2onnx-1.9.3/tests/test_algebra_symbolic.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_test_helper.py` & `skl2onnx-1.9.3/tests/test_algebra_test_helper.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_algebra_to_onnx.py` & `skl2onnx-1.9.3/tests/test_algebra_to_onnx.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,34 @@
 try:
     from onnxruntime.capi.onnxruntime_pybind11_state import (
         InvalidGraph, Fail, InvalidArgument)
 except ImportError:
     InvalidGraph = RuntimeError
     InvalidArgument = RuntimeError
     Fail = RuntimeError
+try:
+    # scikit-learn >= 0.22
+    from sklearn.utils._testing import ignore_warnings
+except ImportError:
+    # scikit-learn < 0.22
+    from sklearn.utils.testing import ignore_warnings
 from sklearn.linear_model import LinearRegression, LogisticRegression
 from skl2onnx.common.data_types import FloatTensorType, DoubleTensorType
 from skl2onnx.algebra.onnx_ops import (
     OnnxAdd, OnnxLinearRegressor, OnnxIdentity)
 from skl2onnx.algebra.onnx_operator import OnnxSubEstimator
 from skl2onnx.proto import get_latest_tested_opset_version
 from test_utils import TARGET_OPSET
 
 
 class TestOnnxOperatorsToOnnx(unittest.TestCase):
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
     def test_onnx_ml(self):
         def generate_onnx_graph(opv):
             node = OnnxAdd(('X1', FloatTensorType()),
                            np.array([0.1], dtype=np.float32),
                            op_version=opv)
             out = OnnxLinearRegressor(
                 node, coefficients=[0.3, 0.3, 0.4, 0.5, 0.6],
@@ -153,57 +160,63 @@
                 if model == LogisticRegression:
                     self.assertEqual(res.shape, (1, 3))
                 else:
                     self.assertEqual(res.shape, (1, 1))
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
     def test_sub_graph_tuple(self):
         self.common_test_sub_graph(
             ('X1', FloatTensorType()), LinearRegression)
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("1.4.0"),
         reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
     def test_sub_graph_tuple_double(self):
         self.common_test_sub_graph(
             ('X1', DoubleTensorType()), LinearRegression,
             cls_type=DoubleTensorType)
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
     def test_sub_graph_str(self):
         self.common_test_sub_graph('X1', LinearRegression)
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("1.4.0"),
         reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
     def test_sub_graph_str_double(self):
         self.common_test_sub_graph('X1', LinearRegression,
                                    cls_type=DoubleTensorType)
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
     def test_sub_graph_tuple_cls(self):
         self.common_test_sub_graph(
             ('X1', FloatTensorType()), LogisticRegression,
             {'zipmap': False})
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("1.4.0"),
         reason="not available")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("1.10.0"),
         reason="ArgMax not available for double")
+    @ignore_warnings(category=DeprecationWarning)
     def test_sub_graph_tuple_cls_double(self):
         self.common_test_sub_graph(
             ('X1', DoubleTensorType()), LogisticRegression,
             options={'zipmap': False}, cls_type=DoubleTensorType)
 
     @unittest.skipIf(StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
                      reason="not available")
@@ -215,14 +228,15 @@
                      reason="not available")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("1.4.0"),
         reason="not available")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("1.10.0"),
         reason="ArgMax not available for double")
+    @ignore_warnings(category=DeprecationWarning)
     def test_sub_graph_str_cls_double(self):
         self.common_test_sub_graph(
             'X1', LogisticRegression, options={'zipmap': False},
             cls_type=DoubleTensorType)
 
 
 if __name__ == "__main__":
```

### Comparing `skl2onnx-1.9.2/tests/test_convert.py` & `skl2onnx-1.9.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_custom_transformer.py` & `skl2onnx-1.9.3/tests/test_custom_transformer_tsne.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     )
 
     container.add_node("Scaler", [knn_output.onnx_name], [output.full_name],
                        op_domain="ai.onnx.ml",
                        **attrs)
 
 
-class TestCustomTransformer(unittest.TestCase):
+class TestCustomTransformerTSNE(unittest.TestCase):
 
     @unittest.skipIf(StrictVersion(ort.__version__) <= StrictVersion("0.3.0"),
                      reason="TopK is failing.")
     def test_custom_pipeline_scaler(self):
 
         digits = datasets.load_digits(n_class=6)
         Xd = digits.data[:20]
```

### Comparing `skl2onnx-1.9.2/tests/test_investigate.py` & `skl2onnx-1.9.3/tests/test_investigate.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             steps = collect_intermediate_steps(
                 model, "pipeline", [("input", FloatTensorType([None, 2]))],
                 target_opset=opset)
 
             assert len(steps) == 2
             assert len(all_models) == 3
 
-            expected = 'opset_import{domain:""version:%d}' % opset
-            expected1 = 'opset_import{domain:""version:1}'
+            expected = 'version:%d}' % opset
+            expected1 = 'version:1}'
             model.transform(data)
             for step in steps:
                 onnx_step = step['onnx_step']
                 text = str(onnx_step).replace('\n', ' ').replace(' ', '')
                 if expected not in text and expected1 not in text:
                     raise AssertionError(
                         "Unable to find '{}'\n'{}'\n".format(
```

### Comparing `skl2onnx-1.9.2/tests/test_onnx_rare_helper.py` & `skl2onnx-1.9.3/tests/test_onnx_rare_helper.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_op10.py` & `skl2onnx-1.9.3/tests/test_op10.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_opset13.py` & `skl2onnx-1.9.3/tests/test_opset13.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_other_converter_library_pipelines.py` & `skl2onnx-1.9.3/tests/test_other_converter_library_pipelines.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_parsing_options.py` & `skl2onnx-1.9.3/tests/test_parsing_options.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_raw_name.py` & `skl2onnx-1.9.3/tests/test_raw_name.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_scikit_pandas.py` & `skl2onnx-1.9.3/tests/test_scikit_pandas.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_shapes.py` & `skl2onnx-1.9.3/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_adaboost_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_adaboost_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_array_feature_extractor.py` & `skl2onnx-1.9.3/tests/test_sklearn_array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_bagging_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_bagging_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 import unittest
 from distutils.version import StrictVersion
 import onnxruntime
+try:
+    # scikit-learn >= 0.22
+    from sklearn.utils._testing import ignore_warnings
+except ImportError:
+    # scikit-learn < 0.22
+    from sklearn.utils.testing import ignore_warnings
 from sklearn.ensemble import (
     BaggingClassifier,
     BaggingRegressor,
     GradientBoostingClassifier,
-    GradientBoostingRegressor,
-)
+    GradientBoostingRegressor)
 from sklearn.linear_model import SGDClassifier, SGDRegressor
 from skl2onnx import convert_sklearn
 from skl2onnx.common.data_types import (
     BooleanTensorType,
     FloatTensorType,
-    Int64TensorType,
-)
+    Int64TensorType)
 from test_utils import (
     dump_data_and_model,
     fit_classification_model,
     fit_regression_model,
-    TARGET_OPSET
-)
+    TARGET_OPSET)
 
 
 class TestSklearnBaggingConverter(unittest.TestCase):
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_default_binary_int(self):
         model, X = fit_classification_model(
             BaggingClassifier(), 2, is_int=True)
         model_onnx = convert_sklearn(
             model,
             "bagging classifier",
             [("input", Int64TensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
+            target_opset=TARGET_OPSET)
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(
-            X,
-            model,
-            model_onnx,
-            basename="SklearnBaggingClassifierDefaultBinary",
-            allow_failure="StrictVersion(onnxruntime.__version__)"
-            "<= StrictVersion('0.2.1')",
-        )
+            X, model, model_onnx,
+            basename="SklearnBaggingClassifierDefaultBinary")
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_default_multiclass_int(self):
         model, X = fit_classification_model(
             BaggingClassifier(), 4, is_int=True)
         model_onnx = convert_sklearn(
             model,
             "bagging classifier",
             [("input", Int64TensorType([None, X.shape[1]]))],
@@ -60,14 +59,15 @@
             model,
             model_onnx,
             basename="SklearnBaggingClassifierDefaultMulticlass",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_default_binary(self):
         model, X = fit_classification_model(
             BaggingClassifier(), 2)
         model_onnx = convert_sklearn(
             model,
             "bagging classifier",
             [("input", FloatTensorType([None, X.shape[1]]))],
@@ -79,42 +79,45 @@
             model,
             model_onnx,
             basename="SklearnBaggingClassifierDefaultBinary",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_max_features(self):
         model, X = fit_classification_model(
             BaggingClassifier(max_features=0.5), 2)
         model_onnx = convert_sklearn(
             model, "bagging classifier",
             [("input", FloatTensorType([None, X.shape[1]]))],
             target_opset=TARGET_OPSET)
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(
             X, model, model_onnx, verbose=False,
             basename="SklearnBaggingClassifierMaxFeatures",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')")
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_bootstrap_features(self):
         model, X = fit_classification_model(
             BaggingClassifier(bootstrap_features=True), 2)
         model_onnx = convert_sklearn(
             model, "bagging classifier",
             [("input", FloatTensorType([None, X.shape[1]]))],
             target_opset=TARGET_OPSET)
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(
             X[:5], model, model_onnx, verbose=False,
             basename="SklearnBaggingClassifierBootstrapFeatures",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')")
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_default_binary_nozipmap(self):
         model, X = fit_classification_model(
             BaggingClassifier(), 2)
         model_onnx = convert_sklearn(
             model, "bagging classifier",
             [("input", FloatTensorType([None, X.shape[1]]))],
             target_opset=TARGET_OPSET,
@@ -122,14 +125,15 @@
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(
             X, model, model_onnx,
             basename="SklearnBaggingClassifierDefaultBinaryNoZipMap",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')")
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_default_multiclass(self):
         model, X = fit_classification_model(
             BaggingClassifier(), 4)
         model_onnx = convert_sklearn(
             model,
             "bagging classifier",
             [("input", FloatTensorType([None, X.shape[1]]))],
@@ -141,14 +145,15 @@
             model,
             model_onnx,
             basename="SklearnBaggingClassifierDefaultMulticlass",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_sgd_binary(self):
         model, X = fit_classification_model(
             BaggingClassifier(
                 SGDClassifier(loss='modified_huber', random_state=42),
                 random_state=42), 2)
         model_onnx = convert_sklearn(
             model,
@@ -162,14 +167,15 @@
             model,
             model_onnx,
             basename="SklearnBaggingClassifierSGDBinary",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_sgd_binary_decision_function(self):
         model, X = fit_classification_model(
             BaggingClassifier(SGDClassifier(random_state=42),
                               random_state=42), 2)
         options = {id(model): {'raw_scores': True}}
         model_onnx = convert_sklearn(
             model,
@@ -185,14 +191,15 @@
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
             methods=['predict', 'decision_function_binary'])
 
     @unittest.skipIf(StrictVersion(onnxruntime.__version__)
                      <= StrictVersion("0.4.0"),
                      reason="Not implemented.")
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_sgd_multiclass(self):
         model, X = fit_classification_model(
             BaggingClassifier(
                 SGDClassifier(loss='modified_huber', random_state=42),
                 random_state=42), 5)
         model_onnx = convert_sklearn(
             model,
@@ -203,14 +210,15 @@
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(
             X[:5], model, model_onnx,
             basename="SklearnBaggingClassifierSGDMulticlass-Dec3",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')")
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_sgd_multiclass_decision_function(self):
         model, X = fit_classification_model(
             BaggingClassifier(
                 GradientBoostingClassifier(random_state=42, n_estimators=4),
                 random_state=42), 4, n_features=10)
         options = {id(model): {'raw_scores': True}}
         model_onnx = convert_sklearn(
@@ -222,14 +230,15 @@
         dump_data_and_model(
             X[:15], model, model_onnx,
             basename="SklearnBaggingClassifierSGDMultiDecisionFunction-Dec3",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
             methods=['predict', 'decision_function'])
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_gradient_boosting_binary(self):
         model, X = fit_classification_model(
             BaggingClassifier(
                 GradientBoostingClassifier(n_estimators=10)), 2)
         model_onnx = convert_sklearn(
             model,
             "bagging classifier",
@@ -242,14 +251,15 @@
             model,
             model_onnx,
             basename="SklearnBaggingClassifierGradientBoostingBinary",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_classifier_gradient_boosting_multiclass(self):
         model, X = fit_classification_model(
             BaggingClassifier(
                 GradientBoostingClassifier(n_estimators=10)), 3)
         model_onnx = convert_sklearn(
             model,
             "bagging classifier",
@@ -262,14 +272,15 @@
             model,
             model_onnx,
             basename="SklearnBaggingClassifierGradientBoostingMulticlass",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_regressor_default(self):
         model, X = fit_regression_model(
             BaggingRegressor())
         model_onnx = convert_sklearn(
             model,
             "bagging regressor",
             [("input", FloatTensorType([None, X.shape[1]]))],
@@ -281,14 +292,15 @@
             model,
             model_onnx,
             basename="SklearnBaggingRegressorDefault-Dec4",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_regressor_max_features(self):
         model, X = fit_regression_model(
             BaggingRegressor(max_features=0.5, n_estimators=3))
         model_onnx = convert_sklearn(
             model, "bagging regressor",
             [("input", FloatTensorType([None, X.shape[1]]))],
             target_opset=TARGET_OPSET)
@@ -309,14 +321,15 @@
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(
             X, model, model_onnx, verbose=False,
             basename="SklearnBaggingRegressorBootstrapFeatures-Dec4",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')")
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_regressor_sgd(self):
         model, X = fit_regression_model(
             BaggingRegressor(SGDRegressor()))
         model_onnx = convert_sklearn(
             model, "bagging regressor",
             [("input", FloatTensorType([None, X.shape[1]]))],
             target_opset=TARGET_OPSET)
@@ -326,14 +339,15 @@
             model,
             model_onnx,
             basename="SklearnBaggingRegressorSGD-Dec4",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_regressor_gradient_boosting(self):
         model, X = fit_regression_model(
             BaggingRegressor(
                 GradientBoostingRegressor(n_estimators=10)))
         model_onnx = convert_sklearn(
             model, "bagging regressor",
             [("input", FloatTensorType([None, X.shape[1]]))],
@@ -341,14 +355,15 @@
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(
             X, model, model_onnx,
             basename="SklearnBaggingRegressorGradientBoosting-Dec4",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')")
 
+    @ignore_warnings(category=FutureWarning)
     def test_bagging_regressor_bool(self):
         model, X = fit_regression_model(
             BaggingRegressor(), is_bool=True)
         model_onnx = convert_sklearn(
             model,
             "bagging regressor",
             [("input", BooleanTensorType([None, X.shape[1]]))],
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_binarizer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_binarizer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_calibrated_classifier_cv_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_calibrated_classifier_cv_converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,21 +3,30 @@
 """
 Tests scikit-learn's CalibratedClassifierCV converters
 """
 
 import unittest
 from distutils.version import StrictVersion
 import numpy as np
+from numpy.testing import assert_almost_equal
+from onnxruntime import InferenceSession
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.datasets import load_digits, load_iris
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.linear_model import LogisticRegression
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.neighbors import KNeighborsClassifier
-from sklearn.svm import SVC
+from sklearn.svm import SVC, LinearSVC
+from sklearn.exceptions import ConvergenceWarning
+try:
+    # scikit-learn >= 0.22
+    from sklearn.utils._testing import ignore_warnings
+except ImportError:
+    # scikit-learn < 0.22
+    from sklearn.utils.testing import ignore_warnings
 import onnxruntime
 try:
     from skl2onnx.common._apply_operation import apply_less
 except ImportError:
     # onnxconverter-common is too old
     apply_less = None
 from skl2onnx import convert_sklearn
@@ -25,37 +34,34 @@
     FloatTensorType, Int64TensorType, onnx_built_with_ml)
 from test_utils import dump_data_and_model, TARGET_OPSET
 
 
 class TestSklearnCalibratedClassifierCVConverters(unittest.TestCase):
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
     def test_model_calibrated_classifier_cv_float(self):
         data = load_iris()
         X, y = data.data, data.target
         clf = MultinomialNB().fit(X, y)
         model = CalibratedClassifierCV(clf, cv=2, method="sigmoid").fit(X, y)
         model_onnx = convert_sklearn(
-            model,
-            "scikit-learn CalibratedClassifierCVMNB",
+            model, "scikit-learn CalibratedClassifierCVMNB",
             [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
+            target_opset=TARGET_OPSET)
         self.assertTrue(model_onnx is not None)
         dump_data_and_model(
-            X.astype(np.float32),
-            model,
-            model_onnx,
-            basename="SklearnCalibratedClassifierCVFloat",
-            allow_failure="StrictVersion(onnxruntime.__version__)"
-            "<= StrictVersion('0.2.1')",
-        )
+            X.astype(np.float32), model, model_onnx,
+            basename="SklearnCalibratedClassifierCVFloat")
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
     def test_model_calibrated_classifier_cv_float_nozipmap(self):
         data = load_iris()
         X, y = data.data, data.target
         clf = MultinomialNB().fit(X, y)
         model = CalibratedClassifierCV(clf, cv=2, method="sigmoid").fit(X, y)
         model_onnx = convert_sklearn(
             model, "scikit-learn CalibratedClassifierCVMNB",
@@ -67,170 +73,239 @@
             X.astype(np.float32), model, model_onnx,
             basename="SklearnCalibratedClassifierCVFloatNoZipMap",
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')")
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=FutureWarning)
     def test_model_calibrated_classifier_cv_int(self):
         data = load_digits()
         X, y = data.data, data.target
         clf = MultinomialNB().fit(X, y)
         model = CalibratedClassifierCV(clf, cv=2, method="sigmoid").fit(X, y)
         model_onnx = convert_sklearn(
-            model,
-            "scikit-learn CalibratedClassifierCVMNB",
+            model, "scikit-learn CalibratedClassifierCVMNB",
             [("input", Int64TensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
+            target_opset=TARGET_OPSET)
         self.assertTrue(model_onnx is not None)
         dump_data_and_model(
-            X.astype(np.int64),
-            model,
-            model_onnx,
-            basename="SklearnCalibratedClassifierCVInt-Dec4",
-            allow_failure="StrictVersion(onnxruntime.__version__)"
-            "<= StrictVersion('0.2.1')",
-        )
+            X.astype(np.int64), model, model_onnx,
+            basename="SklearnCalibratedClassifierCVInt-Dec4")
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
         reason="not available")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
     def test_model_calibrated_classifier_cv_isotonic_float(self):
         data = load_iris()
         X, y = data.data, data.target
         clf = KNeighborsClassifier().fit(X, y)
         model = CalibratedClassifierCV(clf, cv=2, method="isotonic").fit(X, y)
         model_onnx = convert_sklearn(
-            model,
-            "scikit-learn CalibratedClassifierCVKNN",
+            model, "scikit-learn CalibratedClassifierCVKNN",
             [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
-        self.assertTrue(model_onnx is not None)
+            target_opset=TARGET_OPSET)
         try:
             dump_data_and_model(
-                X.astype(np.float32),
-                model,
-                model_onnx,
+                X.astype(np.float32), model, model_onnx,
                 basename="SklearnCalibratedClassifierCVIsotonicFloat")
         except Exception as e:
             raise AssertionError("Issue with model\n{}".format(
                 model_onnx)) from e
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
-    def test_model_calibrated_classifier_cv_binary(self):
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
+    def test_model_calibrated_classifier_cv_binary_mnb(self):
         data = load_iris()
         X, y = data.data, data.target
         y[y > 1] = 1
         clf = MultinomialNB().fit(X, y)
         model = CalibratedClassifierCV(clf, cv=2, method="sigmoid").fit(X, y)
         model_onnx = convert_sklearn(
-            model,
-            "scikit-learn CalibratedClassifierCV",
+            model, "scikit-learn CalibratedClassifierCV",
             [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
+            target_opset=TARGET_OPSET)
         self.assertTrue(model_onnx is not None)
         dump_data_and_model(
-            X.astype(np.float32),
-            model,
-            model_onnx,
-            basename="SklearnCalibratedClassifierCVBinaryMNB",
-            allow_failure="StrictVersion(onnxruntime.__version__)"
-            "<= StrictVersion('0.2.1')",
-        )
+            X.astype(np.float32), model, model_onnx,
+            basename="SklearnCalibratedClassifierCVBinaryMNB")
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
         reason="not available")
-    def test_model_calibrated_classifier_cv_isotonic_binary(self):
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
+    def test_model_calibrated_classifier_cv_isotonic_binary_knn(self):
         data = load_iris()
         X, y = data.data, data.target
         y[y > 1] = 1
         clf = KNeighborsClassifier().fit(X, y)
         model = CalibratedClassifierCV(clf, cv=2, method="isotonic").fit(X, y)
         model_onnx = convert_sklearn(
-            model,
-            "scikit-learn CalibratedClassifierCV",
+            model, "scikit-learn CalibratedClassifierCV",
             [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
+            target_opset=TARGET_OPSET)
         self.assertTrue(model_onnx is not None)
         dump_data_and_model(
-            X.astype(np.float32),
-            model,
-            model_onnx,
+            X.astype(np.float32), model, model_onnx,
             basename="SklearnCalibratedClassifierCVIsotonicBinaryKNN")
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
         reason="not available")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
     def test_model_calibrated_classifier_cv_logistic_regression(self):
         data = load_iris()
         X, y = data.data, data.target
         y[y > 1] = 1
         model = CalibratedClassifierCV(
             base_estimator=LogisticRegression(), method='sigmoid').fit(X, y)
         model_onnx = convert_sklearn(
             model, "unused",
             [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
-        self.assertTrue(model_onnx is not None)
+            target_opset=TARGET_OPSET)
         dump_data_and_model(
-            X.astype(np.float32),
-            model,
-            model_onnx,
-            basename="SklearnCalibratedClassifierCVBinaryLogReg",
-            allow_failure="StrictVersion(onnxruntime.__version__)"
-            "<= StrictVersion('0.2.1')",
-        )
+            X.astype(np.float32), model, model_onnx,
+            basename="SklearnCalibratedClassifierCVBinaryLogReg")
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
         reason="not available")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
     def test_model_calibrated_classifier_cv_rf(self):
         data = load_iris()
         X, y = data.data, data.target
         y[y > 1] = 1
         model = CalibratedClassifierCV(
             base_estimator=RandomForestClassifier(n_estimators=2),
             method='sigmoid').fit(X, y)
         try:
             convert_sklearn(
                 model, "unused",
-                [("input", FloatTensorType([None, X.shape[1]]))])
+                [("input", FloatTensorType([None, X.shape[1]]))],
+                target_opset=TARGET_OPSET)
             raise AssertionError(
                 "RandomForestClassifier has no decision_function")
         except RuntimeError as e:
             assert "cannot implement decision_function" in str(e)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(
         StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
         reason="not available")
     @unittest.skipIf(apply_less is None, reason="onnxconverter-common old")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
     def test_model_calibrated_classifier_cv_svc(self):
         data = load_iris()
         X, y = data.data, data.target
         model = CalibratedClassifierCV(
             base_estimator=SVC(),
             method='sigmoid').fit(X, y)
         model_onnx = convert_sklearn(
             model, "unused",
-            [("input", FloatTensorType([None, X.shape[1]]))])
-        assert model_onnx is not None
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(np.float32), model, model_onnx,
+            basename="SklearnCalibratedClassifierSVC")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(apply_less is None, reason="onnxconverter-common old")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
+    def test_model_calibrated_classifier_cv_linearsvc(self):
+        data = load_iris()
+        X, y = data.data, data.target
+        model = CalibratedClassifierCV(
+            base_estimator=LinearSVC(),
+            method='sigmoid').fit(X, y)
+        model_onnx = convert_sklearn(
+            model, "unused",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(np.float32), model, model_onnx,
+            basename="SklearnCalibratedClassifierLinearSVC")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(apply_less is None, reason="onnxconverter-common old")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
+    def test_model_calibrated_classifier_cv_linearsvc2(self):
+        data = load_iris()
+        X, y = data.data, data.target
+        y[y == 2] = 0
+        self.assertEqual(len(set(y)), 2)
+        model = CalibratedClassifierCV(
+            base_estimator=LinearSVC(),
+            method='sigmoid').fit(X, y)
+        model_onnx = convert_sklearn(
+            model, "unused",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(np.float32), model, model_onnx,
+            basename="SklearnCalibratedClassifierLinearSVC2")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(apply_less is None, reason="onnxconverter-common old")
+    @ignore_warnings(
+        category=(FutureWarning, ConvergenceWarning, DeprecationWarning))
+    def test_model_calibrated_classifier_cv_svc2_binary(self):
+        data = load_iris()
+        X, y = data.data, data.target
+        X = X[:90]
+        y = y[:90]
+        self.assertEqual(len(set(y)), 2)
+
+        for model_sub in [LogisticRegression(), SVC(probability=False)]:
+            model_sub.fit(X, y)
+            with self.subTest(model=model_sub):
+                model = CalibratedClassifierCV(
+                    base_estimator=model_sub, cv=2,
+                    method='sigmoid').fit(X, y)
+                model_onnx = convert_sklearn(
+                    model, "unused",
+                    [("input", FloatTensorType([None, X.shape[1]]))],
+                    target_opset=TARGET_OPSET,
+                    options={id(model): {'zipmap': False}})
+
+                sess = InferenceSession(model_onnx.SerializeToString())
+                res = sess.run(None, {'input': X[:5].astype(np.float32)})
+                assert_almost_equal(model.predict_proba(X[:5]), res[1])
+                assert_almost_equal(model.predict(X[:5]), res[0])
+
+                dump_data_and_model(
+                    X.astype(np.float32)[:10], model, model_onnx,
+                    basename="SklearnCalibratedClassifierSVC2")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_cast_regressor.py` & `skl2onnx-1.9.3/tests/test_sklearn_cast_regressor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_cast_transformer.py` & `skl2onnx-1.9.3/tests/test_sklearn_cast_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_concat.py` & `skl2onnx-1.9.3/tests/test_sklearn_concat.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_count_vectorizer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_count_vectorizer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_count_vectorizer_converter_bug.py` & `skl2onnx-1.9.3/tests/test_sklearn_count_vectorizer_converter_bug.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_custom_nmf.py` & `skl2onnx-1.9.3/tests/test_sklearn_custom_nmf.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_decision_tree_converters.py` & `skl2onnx-1.9.3/tests/test_sklearn_decision_tree_converters.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_dict_vectorizer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_dict_vectorizer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_documentation.py` & `skl2onnx-1.9.3/tests/test_sklearn_documentation.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_double_tensor_type_cls.py` & `skl2onnx-1.9.3/tests/test_sklearn_double_tensor_type_cls.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_double_tensor_type_reg.py` & `skl2onnx-1.9.3/tests/test_sklearn_double_tensor_type_reg.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_double_tensor_type_tr.py` & `skl2onnx-1.9.3/tests/test_sklearn_double_tensor_type_tr.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_feature_selection_converters.py` & `skl2onnx-1.9.3/tests/test_sklearn_feature_selection_converters.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_feature_union.py` & `skl2onnx-1.9.3/tests/test_sklearn_feature_union.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_function_transformer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_function_transformer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_gaussian_mixture_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_gaussian_mixture_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import unittest
 import numpy as np
 from sklearn.datasets import load_iris
 from sklearn.mixture import GaussianMixture, BayesianGaussianMixture
+try:
+    # scikit-learn >= 0.22
+    from sklearn.utils._testing import ignore_warnings
+except ImportError:
+    # scikit-learn < 0.22
+    from sklearn.utils.testing import ignore_warnings
 from onnxruntime import InferenceSession
 try:
     from onnxruntime.capi.onnxruntime_pybind11_state import Fail as OrtFail
 except ImportError:
     OrtFail = RuntimeError
 from skl2onnx import convert_sklearn, to_onnx
 from skl2onnx.common.data_types import FloatTensorType
@@ -50,14 +56,15 @@
         np.testing.assert_almost_equal(
             exp.ravel(), got[2].ravel(), decimal=decimal)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(TARGET_OPSET < 11,
                      reason="Missing Gemm (11)")
+    @ignore_warnings(category=UserWarning)
     def test_model_gaussian_mixture_binary_classification(self):
         model, X = self._fit_model_binary_classification(
             GaussianMixture(), load_iris())
         for tg in range(min(9, TARGET_OPSET), TARGET_OPSET + 1):
             with self.subTest(target_opset=tg):
                 model_onnx = convert_sklearn(
                     model, "gaussian_mixture",
@@ -67,14 +74,15 @@
                 dump_data_and_model(
                     X, model, model_onnx,
                     basename="SklearnBinGaussianMixture",
                     allow_failure="StrictVersion(onnxruntime.__version__)"
                     "<= StrictVersion('0.2.1')")
                 self._test_score(model, X, tg)
 
+    @ignore_warnings(category=UserWarning)
     def test_model_bayesian_mixture_binary_classification(self):
         for cov in ["full", "tied", "diag", "spherical"]:
             with self.subTest(cov=cov):
                 model, X = self._fit_model_binary_classification(
                     BayesianGaussianMixture(), load_iris(),
                     covariance_type=cov)
                 model_onnx = convert_sklearn(
@@ -92,14 +100,15 @@
                     allow_failure="StrictVersion(onnxruntime.__version__)"
                     "<= StrictVersion('0.2.1')",
                 )
                 self._test_score(model, X, TARGET_OPSET)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=UserWarning)
     def test_model_gaussian_mixture_multiclass(self):
         model, X = self._fit_model_multiclass_classification(
             GaussianMixture(), load_iris())
         model_onnx = convert_sklearn(
             model,
             "gaussian_mixture",
             [("input", FloatTensorType([None, X.shape[1]]))],
@@ -114,14 +123,15 @@
             allow_failure="StrictVersion(onnxruntime.__version__)"
             "<= StrictVersion('0.2.1')",
         )
         self._test_score(model, X, TARGET_OPSET)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_comp2(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=2)
         model.fit(X)
         model_onnx = convert_sklearn(model, "GM",
                                      [("input", FloatTensorType([None, 4]))],
@@ -137,14 +147,15 @@
             allow_failure="StrictVersion(onnx.__version__)"
                           " < StrictVersion('1.2')",
         )
         self._test_score(model, X, TARGET_OPSET)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_full(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=2, covariance_type='full')
         model.fit(X)
         model_onnx = convert_sklearn(model, "GM",
                                      [("input", FloatTensorType([None, 4]))],
@@ -160,14 +171,15 @@
             allow_failure="StrictVersion(onnx.__version__)"
                           " < StrictVersion('1.2')",
         )
         self._test_score(model, X, TARGET_OPSET)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_tied(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=2, covariance_type='tied')
         model.fit(X)
         model_onnx = convert_sklearn(model, "GM",
                                      [("input", FloatTensorType([None, 4]))],
@@ -183,14 +195,15 @@
             allow_failure="StrictVersion(onnx.__version__)"
                           " < StrictVersion('1.2')",
         )
         self._test_score(model, X, TARGET_OPSET)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_diag(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=2, covariance_type='diag')
         model.fit(X)
         model_onnx = convert_sklearn(model, "GM",
                                      [("input", FloatTensorType([None, 4]))],
@@ -207,14 +220,15 @@
             allow_failure="StrictVersion(onnx.__version__)"
                           " < StrictVersion('1.2')",
         )
         self._test_score(model, X, TARGET_OPSET, decimal=4)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_spherical(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=2, covariance_type='spherical')
         model.fit(X)
         model_onnx = convert_sklearn(
             model, "GM", [("input", FloatTensorType([None, 4]))],
@@ -228,14 +242,15 @@
             # Operator gemm is not implemented in onnxruntime
             allow_failure="StrictVersion(onnx.__version__)"
                           " < StrictVersion('1.2')")
         self._test_score(model, X, TARGET_OPSET, decimal=4)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_full_black_op(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=2, covariance_type='full')
         model.fit(X)
         with self.assertRaises(RuntimeError):
             convert_sklearn(
@@ -258,14 +273,15 @@
         )
         self._test_score(model, X, TARGET_OPSET)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(TARGET_OPSET < 11,
                      reason="OnnxEqual does not support float")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_full_black_op_noargmax(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=2, covariance_type='full')
         model.fit(X)
         with self.assertRaises(RuntimeError):
             convert_sklearn(
@@ -288,14 +304,15 @@
         )
         self._test_score(model, X, TARGET_OPSET)
 
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(TARGET_OPSET < 11,
                      reason="OnnxEqual does not support float")
+    @ignore_warnings(category=UserWarning)
     def test_gaussian_mixture_full_black_op_noargmax_inf(self):
         data = load_iris()
         X = data.data
         model = GaussianMixture(n_components=10, covariance_type='full')
         model.fit(X)
         model_onnx1 = convert_sklearn(
             model, "GM", [("input", FloatTensorType([None, 4]))],
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_gaussian_process_classifier.py` & `skl2onnx-1.9.3/tests/test_sklearn_gaussian_process_classifier.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_gaussian_process_regressor.py` & `skl2onnx-1.9.3/tests/test_sklearn_gaussian_process_regressor.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_glm_classifier_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_glm_classifier_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_glm_regressor_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_glm_regressor_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_gradient_boosting_converters.py` & `skl2onnx-1.9.3/tests/test_sklearn_gradient_boosting_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 from distutils.version import StrictVersion
-from logging import getLogger
 import unittest
 import numpy as np
 from pandas import DataFrame
 from sklearn.datasets import make_classification
 from sklearn.ensemble import (
     GradientBoostingClassifier,
     GradientBoostingRegressor
@@ -25,18 +24,14 @@
 from test_utils import dump_data_and_model, fit_regression_model
 
 THRESHOLD = "0.2.1"
 
 
 class TestSklearnGradientBoostingModels(unittest.TestCase):
 
-    def setUp(self):
-        log = getLogger('skl2onnx')
-        log.disabled = True
-
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     @unittest.skipIf(
         StrictVersion(__version__) <= StrictVersion(THRESHOLD),
         reason="Depends on PR #1015 onnxruntime.")
     def test_gradient_boosting_classifier1Deviance(self):
         model = GradientBoostingClassifier(n_estimators=1, max_depth=2)
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_grid_search_cv_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_grid_search_cv_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 import unittest
 import numpy as np
 import onnx
 from onnxruntime import __version__ as ort_version
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.linear_model import Lasso, LassoLars, LogisticRegression
 from sklearn.model_selection import GridSearchCV
+from sklearn.cluster import KMeans
 from sklearn.svm import SVC
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import load_iris
 from skl2onnx import convert_sklearn, to_onnx
 from skl2onnx.common.data_types import (
     DoubleTensorType, FloatTensorType, Int64TensorType)
 from skl2onnx.common.data_types import onnx_built_with_ml
 from test_utils import (
     dump_data_and_model, fit_classification_model,
+    fit_clustering_model,
     fit_regression_model, TARGET_OPSET)
 
 
 class TestSklearnGridSearchCVModels(unittest.TestCase):
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     def test_grid_search_binary_float(self):
@@ -216,10 +218,26 @@
             return X_test, clf, convert_to_onnx(clf, X_test, onnx_model_name)
 
         x_test, model, model_onnx = run()
         dump_data_and_model(
             x_test.astype(np.float32), model, model_onnx,
             basename="SklearnGridSearchSVC-Out0")
 
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    def test_grid_search_binary_kmeans(self):
+        tuned_parameters = [{'n_clusters': [2, 3]}]
+        clf = GridSearchCV(KMeans(), tuned_parameters, cv=5)
+        model, X = fit_clustering_model(clf, n_classes=2)
+        X = X.astype(np.float32)
+        model_onnx = convert_sklearn(
+            model, "GridSearchCV",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X, model.best_estimator_, model_onnx,
+            basename="SklearnGridSearchKMeans")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_imputer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_imputer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_isolation_forest.py` & `skl2onnx-1.9.3/tests/test_sklearn_isolation_forest.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 """
 Test scikit-learn's IsolationForest.
 """
 import unittest
 from distutils.version import StrictVersion
 import numpy as np
+from numpy.testing import assert_almost_equal
+from onnxruntime import InferenceSession
 from sklearn import __version__ as sklv
 try:
     from sklearn.ensemble import IsolationForest
 except ImportError:
     IsolationForest = None
 from skl2onnx import to_onnx
 from test_utils import dump_data_and_model, TARGET_OPSET
@@ -36,14 +38,36 @@
         self.assertIsNotNone(model_onnx)
         dump_data_and_model(data, model, model_onnx,
                             basename="IsolationForest")
 
     @unittest.skipIf(IsolationForest is None, reason="old scikit-learn")
     @unittest.skipIf(StrictVersion(sklv2) < StrictVersion('0.22.0'),
                      reason="tree structure is different.")
+    def test_isolation_forest_score_samples(self):
+        isol = IsolationForest(n_estimators=3, random_state=0)
+        data = np.array([[-1.1, -1.2], [0.3, 0.2],
+                         [0.5, 0.4], [100., 99.]], dtype=np.float32)
+        model = isol.fit(data)
+        model_onnx = to_onnx(model, data, target_opset=TARGET_OPSET,
+                             options={'score_samples': True})
+        sess = InferenceSession(model_onnx.SerializeToString())
+        names = [o.name for o in sess.get_outputs()]
+        self.assertEqual(names, ['label', 'scores', 'score_samples'])
+        got = sess.run(None, {'X': data})
+        self.assertEqual(len(got), 3)
+        expected_label = isol.predict(data)
+        expected_decif = isol.decision_function(data)
+        expected_score = isol.score_samples(data)
+        assert_almost_equal(expected_label, got[0].ravel())
+        assert_almost_equal(expected_decif, got[1].ravel())
+        assert_almost_equal(expected_score, got[2].ravel())
+
+    @unittest.skipIf(IsolationForest is None, reason="old scikit-learn")
+    @unittest.skipIf(StrictVersion(sklv2) < StrictVersion('0.22.0'),
+                     reason="tree structure is different.")
     def test_isolation_forest_op1(self):
         isol = IsolationForest(n_estimators=3, random_state=0)
         data = np.array([[-1.1, -1.2], [0.3, 0.2],
                          [0.5, 0.4], [100., 99.]], dtype=np.float32)
         model = isol.fit(data)
         with self.assertRaises(RuntimeError):
             to_onnx(model, data,
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_k_bins_discretiser_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_k_bins_discretiser_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_k_means_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_k_means_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_label_binariser_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_label_binariser_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_label_encoder_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_label_encoder_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_mlp_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_mlp_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_naive_bayes_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_naive_bayes_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_nearest_neighbour_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_nearest_neighbour_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1001 +1,1004 @@
-# SPDX-License-Identifier: Apache-2.0
-
-"""
-Tests scikit-learn's KNeighbours Classifier and Regressor converters.
-"""
-import sys
-import warnings
-import unittest
-import functools
-from distutils.version import StrictVersion
-import numpy
-from numpy.testing import assert_almost_equal
-import onnx
-import onnxruntime
-from onnxruntime import InferenceSession
-from pandas import DataFrame
-try:
-    from sklearn.utils._testing import ignore_warnings
-except ImportError:
-    # older versions of scikit-learn
-    from sklearn.utils.testing import ignore_warnings
-from sklearn import datasets
-from sklearn.model_selection import train_test_split
-from sklearn.neighbors import (
-    KNeighborsRegressor, RadiusNeighborsRegressor,
-    KNeighborsClassifier, RadiusNeighborsClassifier,
-    NearestNeighbors)
-try:
-    from sklearn.impute import KNNImputer
-    from sklearn.neighbors import (
-        KNeighborsTransformer,
-        NeighborhoodComponentsAnalysis)
-except ImportError:
-    # New in 0.22
-    KNNImputer = None
-    KNeighborsTransformer = None
-    NeighborhoodComponentsAnalysis = None
-from sklearn.pipeline import make_pipeline
-from sklearn.preprocessing import StandardScaler
-try:
-    from onnxruntime.capi.onnxruntime_pybind11_state import (
-        NotImplemented as OrtImpl)
-except ImportError:
-    OrtImpl = RuntimeError
-from skl2onnx import convert_sklearn, to_onnx
-from skl2onnx.common.data_types import (
-    DoubleTensorType,
-    FloatTensorType,
-    Int64TensorType,
-)
-from skl2onnx.common.data_types import onnx_built_with_ml
-from skl2onnx.helpers.onnx_helper import (
-    enumerate_model_node_outputs, select_model_inputs_outputs)
-from test_utils import (
-    dump_data_and_model,
-    fit_classification_model,
-    fit_multilabel_classification_model,
-    TARGET_OPSET)
-
-
-def dont_test_radius():
-    return (
-        StrictVersion(onnxruntime.__version__) <= StrictVersion("1.3.0") or
-        StrictVersion(onnx.__version__) <= StrictVersion("1.6.0"))
-
-
-class TestNearestNeighbourConverter(unittest.TestCase):
-
-    @functools.lru_cache(maxsize=1)
-    def _get_iris(self):
-        iris = datasets.load_iris()
-        X = iris.data[::2, :3]
-        y = iris.target[::2]
-        return X, y
-
-    def _fit_model_binary_classification(self, model):
-        X, y = self._get_iris()
-        y[y == 2] = 1
-        model.fit(X, y)
-        return model, X
-
-    def _fit_model_multiclass_classification(self, model, use_string=False):
-        X, y = self._get_iris()
-        if use_string:
-            y = numpy.array(["cl%d" % _ for _ in y])
-        model.fit(X, y)
-        return model, X
-
-    @functools.lru_cache(maxsize=20)
-    def _get_reg_data(self, n, n_features, n_targets, n_informative=10):
-        X, y = datasets.make_regression(
-            n, n_features=n_features, random_state=0,
-            n_targets=n_targets, n_informative=n_informative)
-        return X, y
-
-    def _fit_model(self, model, n_targets=1, label_int=False,
-                   n_informative=10):
-        X, y = self._get_reg_data(20, 4, n_targets, n_informative)
-        if label_int:
-            y = y.astype(numpy.int64)
-        model.fit(X, y)
-        return model, X
-
-    def _fit_model_simple(self, model, n_targets=1, label_int=False,
-                          n_informative=3):
-        X, y = self._get_reg_data(20, 2, n_targets, n_informative)
-        y /= 100
-        if label_int:
-            y = y.astype(numpy.int64)
-        model.fit(X, y)
-        return model, X
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor(self):
-        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=2))
-        model_onnx = convert_sklearn(model, "KNN regressor",
-                                     [("input", FloatTensorType([None, 4]))],
-                                     target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressor-Dec4")
-        dump_data_and_model(
-            (X + 0.1).astype(numpy.float32)[:7],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressor-Dec4")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("1.8.0"),
-        reason="produces nan values")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_radius(self):
-        model, X = self._fit_model(RadiusNeighborsRegressor())
-        model_onnx = convert_sklearn(model, "KNN regressor",
-                                     [("input", FloatTensorType([None, 4]))],
-                                     target_opset=TARGET_OPSET,
-                                     options={id(model): {'optim': 'cdist'}})
-        sess = InferenceSession(model_onnx.SerializeToString())
-        X = X[:5]
-        got = sess.run(None, {'input': X.astype(numpy.float32)})[0]
-        exp = model.predict(X.astype(numpy.float32))
-        if any(numpy.isnan(got.ravel())):
-            # The model is unexpectedly producing nan values
-            # not on all platforms.
-            rows = ['--EXP--', str(exp), '--GOT--', str(got),
-                    '--EVERY-OUTPUT--']
-            for out in enumerate_model_node_outputs(
-                    model_onnx, add_node=False):
-                onx = select_model_inputs_outputs(model_onnx, out)
-                sess = InferenceSession(onx.SerializeToString())
-                res = sess.run(
-                    None, {'input': X.astype(numpy.float32)})
-                rows.append('--{}--'.format(out))
-                rows.append(str(res))
-            if (StrictVersion(onnxruntime.__version__) <
-                    StrictVersion("1.4.0")):
-                return
-            raise AssertionError('\n'.join(rows))
-        assert_almost_equal(exp.ravel(), got.ravel(), decimal=3)
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @unittest.skipIf(
-        StrictVersion(onnx.__version__) < StrictVersion("1.6.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_double(self):
-        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=2))
-        model_onnx = convert_sklearn(
-            model, "KNN regressor",
-            [("input", DoubleTensorType([None, 4]))],
-            target_opset=TARGET_OPSET,
-            options={id(model): {'optim': 'cdist'}})
-        self.assertIsNotNone(model_onnx)
-        try:
-            InferenceSession(model_onnx.SerializeToString())
-        except OrtImpl as e:
-            if ("Could not find an implementation for the node "
-                    "To_TopK:TopK(11)") in str(e):
-                # onnxruntime does not declare TopK(11) for double
-                return
-            raise e
-        dump_data_and_model(
-            X.astype(numpy.float64)[:7],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressor64")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_double_radius(self):
-        model, X = self._fit_model(RadiusNeighborsRegressor())
-        model_onnx = convert_sklearn(
-            model, "KNN regressor",
-            [("input", DoubleTensorType([None, 4]))],
-            target_opset=TARGET_OPSET,
-            options={id(model): {'optim': 'cdist'}})
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float64)[:7],
-            model, model_onnx,
-            basename="SklearnRadiusNeighborsRegressor64")
-        dump_data_and_model(
-            (X + 0.1).astype(numpy.float64)[:7],
-            model, model_onnx,
-            basename="SklearnRadiusNeighborsRegressor64")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_yint(self):
-        model, X = self._fit_model(
-            KNeighborsRegressor(n_neighbors=2), label_int=True)
-        model_onnx = convert_sklearn(model, "KNN regressor",
-                                     [("input", FloatTensorType([None, 4]))],
-                                     target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressorYInt")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_yint_radius(self):
-        model, X = self._fit_model(
-            RadiusNeighborsRegressor(), label_int=True)
-        model_onnx = convert_sklearn(model, "KNN regressor",
-                                     [("input", FloatTensorType([None, 4]))],
-                                     target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7],
-            model, model_onnx,
-            basename="SklearnRadiusNeighborsRegressorYInt")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor2_1(self):
-        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=1),
-                                   n_targets=2)
-        model_onnx = convert_sklearn(model, "KNN regressor",
-                                     [("input", FloatTensorType([None, 4]))],
-                                     target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:3],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressor2")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor2_1_radius(self):
-        model, X = self._fit_model_simple(
-            RadiusNeighborsRegressor(algorithm="brute"),
-            n_targets=2)
-        X = X[:-1]
-        model_onnx = convert_sklearn(
-            model, "KNN regressor",
-            [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        sess = InferenceSession(model_onnx.SerializeToString())
-        got = sess.run(None, {'input': X.astype(numpy.float32)})[0]
-        exp = model.predict(X.astype(numpy.float32))
-        if any(numpy.isnan(got.ravel())):
-            # The model is unexpectedly producing nan values
-            # not on all platforms.
-            # It happens when two matrices are multiplied,
-            # one is (2, 20, 20), second is (20, 20)
-            # and contains only 0 or 1 values.
-            # The output contains nan values on the first row
-            # but not on the second one.
-            rows = ['--EXP--', str(exp), '--GOT--', str(got),
-                    '--EVERY-OUTPUT--']
-            for out in enumerate_model_node_outputs(
-                    model_onnx, add_node=False):
-                onx = select_model_inputs_outputs(model_onnx, out)
-                sess = InferenceSession(onx.SerializeToString())
-                res = sess.run(
-                    None, {'input': X.astype(numpy.float32)})
-                rows.append('--{}--'.format(out))
-                rows.append(str(res))
-            if (onnxruntime.__version__.startswith('1.4.') or
-                    onnxruntime.__version__.startswith('1.5.')):
-                # TODO: investigate the regression in onnxruntime 1.4
-                # One broadcasted multiplication unexpectedly produces nan.
-                whole = '\n'.join(rows)
-                if "[        nan" in whole:
-                    warnings.warn(whole)
-                    return
-                raise AssertionError(whole)
-            if (onnxruntime.__version__.startswith('1.3.') and
-                    sys.platform == 'win32'):
-                # Same error but different line number for further
-                # investigation.
-                raise AssertionError(whole)
-            raise AssertionError('\n'.join(rows))
-        assert_almost_equal(exp, got, decimal=5)
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @unittest.skipIf(
-        StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor2_1_opset(self):
-        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=1),
-                                   n_targets=2)
-        for op in [TARGET_OPSET, 12, 11, 10, 9]:
-            if op > TARGET_OPSET:
-                continue
-            with self.subTest(opset=op):
-                model_onnx = convert_sklearn(
-                    model, "KNN regressor",
-                    [("input", FloatTensorType([None, 4]))],
-                    target_opset=op)
-                self.assertIsNotNone(model_onnx)
-                dump_data_and_model(
-                    X.astype(numpy.float32)[:3],
-                    model, model_onnx,
-                    basename="SklearnKNeighborsRegressor2%d" % op)
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor2_2(self):
-        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=2),
-                                   n_targets=2)
-        model_onnx = convert_sklearn(model, "KNN regressor",
-                                     [("input", FloatTensorType([None, 4]))],
-                                     target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:2],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressor2")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @unittest.skipIf(TARGET_OPSET < 9,
-                     reason="needs higher target_opset")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_weights_distance_11(self):
-        model, X = self._fit_model(
-            KNeighborsRegressor(
-                weights="distance", algorithm="brute", n_neighbors=1))
-        for op in sorted(set([9, 10, 11, 12, TARGET_OPSET])):
-            if op > TARGET_OPSET:
-                continue
-            with self.subTest(opset=op):
-                model_onnx = convert_sklearn(
-                    model, "KNN regressor",
-                    [("input", FloatTensorType([None, 4]))],
-                    target_opset=op)
-                if op < 12 and model_onnx.ir_version > 6:
-                    raise AssertionError(
-                        "ir_version ({}, op={}) must be <= 6.".format(
-                            model_onnx.ir_version, op))
-                if op < 11 and model_onnx.ir_version > 5:
-                    raise AssertionError(
-                        "ir_version ({}, op={}) must be <= 5.".format(
-                            model_onnx.ir_version, op))
-                if op < 10 and model_onnx.ir_version > 4:
-                    raise AssertionError(
-                        "ir_version ({}, op={}) must be <= 4.".format(
-                            model_onnx.ir_version, op))
-                self.assertIsNotNone(model_onnx)
-                dump_data_and_model(
-                    X.astype(numpy.float32)[:3],
-                    model, model_onnx,
-                    basename="SklearnKNeighborsRegressorWDist%d-Dec3" % op)
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_weights_distance_11_radius(self):
-        model, X = self._fit_model_simple(
-            RadiusNeighborsRegressor(
-                weights="distance", algorithm="brute", radius=100))
-        for op in sorted(set([TARGET_OPSET, 12, 11])):
-            if op > TARGET_OPSET:
-                continue
-            with self.subTest(opset=op):
-                model_onnx = convert_sklearn(
-                    model, "KNN regressor",
-                    [("input", FloatTensorType([None, X.shape[1]]))],
-                    target_opset=op)
-                self.assertIsNotNone(model_onnx)
-                sess = InferenceSession(model_onnx.SerializeToString())
-                got = sess.run(None, {'input': X.astype(numpy.float32)})[0]
-                exp = model.predict(X.astype(numpy.float32))
-                assert_almost_equal(exp, got.ravel(), decimal=3)
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_metric_cityblock(self):
-        model, X = self._fit_model(KNeighborsRegressor(metric="cityblock"))
-        model_onnx = convert_sklearn(model, "KNN regressor",
-                                     [("input", FloatTensorType([None, 4]))],
-                                     target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressorMetricCityblock")
-
-    @unittest.skipIf(not onnx_built_with_ml(),
-                     reason="Requires ONNX-ML extension.")
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @unittest.skipIf(TARGET_OPSET < TARGET_OPSET,
-                     reason="needs higher target_opset")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_binary_class(self):
-        model, X = self._fit_model_binary_classification(
-            KNeighborsClassifier())
-        model_onnx = convert_sklearn(
-            model,
-            "KNN classifier binary",
-            [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32),
-            model, model_onnx,
-            basename="SklearnKNeighborsClassifierBinary")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @unittest.skipIf(TARGET_OPSET < 12,
-                     reason="needs higher target_opset")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_binary_class_radius(self):
-        model, X = self._fit_model_binary_classification(
-            RadiusNeighborsClassifier())
-        model_onnx = convert_sklearn(
-            model, "KNN classifier binary",
-            [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32),
-            model, model_onnx,
-            basename="SklearnRadiusNeighborsClassifierBinary")
-
-    @unittest.skipIf(not onnx_built_with_ml(),
-                     reason="Requires ONNX-ML extension.")
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_multi_class(self):
-        model, X = self._fit_model_multiclass_classification(
-            KNeighborsClassifier())
-        model_onnx = convert_sklearn(
-            model,
-            "KNN classifier multi-class",
-            [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET
-        )
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32),
-            model, model_onnx,
-            basename="SklearnKNeighborsClassifierMulti")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @unittest.skipIf(TARGET_OPSET < 12,
-                     reason="needs higher target_opset")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_multi_class_radius(self):
-        model, X = self._fit_model_multiclass_classification(
-            RadiusNeighborsClassifier())
-        model_onnx = convert_sklearn(
-            model, "KNN classifier multi-class",
-            [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET,
-            options={id(model): {'optim': 'cdist'}})
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:5],
-            model, model_onnx,
-            basename="SklearnRadiusNeighborsClassifierMulti")
-
-    @unittest.skipIf(not onnx_built_with_ml(),
-                     reason="Requires ONNX-ML extension.")
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_multi_class_string(self):
-        model, X = self._fit_model_multiclass_classification(
-            KNeighborsClassifier(), use_string=True)
-        model_onnx = convert_sklearn(
-            model,
-            "KNN classifier multi-class",
-            [("input", FloatTensorType([None, 3]))],
-            target_opset=TARGET_OPSET
-        )
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32),
-            model, model_onnx,
-            basename="SklearnKNeighborsClassifierMulti")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_weights_distance(self):
-        model, X = self._fit_model_multiclass_classification(
-            KNeighborsClassifier(weights='distance'))
-        model_onnx = convert_sklearn(
-            model, 'KNN classifier', [('input', FloatTensorType([None, 3]))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7], model, model_onnx,
-            basename="SklearnKNeighborsClassifierWeightsDistance")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_metric_cityblock(self):
-        model, X = self._fit_model_multiclass_classification(
-            KNeighborsClassifier(metric='cityblock'))
-        model_onnx = convert_sklearn(
-            model, 'KNN classifier', [('input', FloatTensorType([None, 3]))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7], model, model_onnx,
-            basename="SklearnKNeighborsClassifierMetricCityblock")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_classifier_multilabel(self):
-        model, X_test = fit_multilabel_classification_model(
-            KNeighborsClassifier(), n_classes=7, n_labels=3,
-            n_samples=100, n_features=10)
-        options = {id(model): {'zipmap': False}}
-        model_onnx = convert_sklearn(
-            model,
-            "scikit-learn KNN Classifier",
-            [("input", FloatTensorType([None, X_test.shape[1]]))],
-            options=options,
-            target_opset=TARGET_OPSET
-        )
-        self.assertTrue(model_onnx is not None)
-        assert 'zipmap' not in str(model_onnx).lower()
-        dump_data_and_model(
-            X_test,
-            model,
-            model_onnx,
-            basename="SklearnKNNClassifierMultiLabel-Out0",
-            allow_failure="StrictVersion("
-            "onnxruntime.__version__) <= StrictVersion('0.2.1')",
-        )
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_int(self):
-        model, X = self._fit_model(KNeighborsRegressor())
-        X = X.astype(numpy.int64)
-        model_onnx = convert_sklearn(
-            model,
-            "KNN regressor",
-            [("input", Int64TensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X,
-            model,
-            model_onnx,
-            basename="SklearnKNNRegressorInt-Dec4"
-        )
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor_equal(self):
-        X, y = datasets.make_regression(
-            n_samples=1000, n_features=100, random_state=42)
-        X = X.astype(numpy.int64)
-        X_train, X_test, y_train, y_test = train_test_split(
-            X, y, test_size=0.5, random_state=42)
-        model = KNeighborsRegressor(
-            algorithm='brute', metric='manhattan').fit(X_train, y_train)
-        model_onnx = convert_sklearn(
-            model, 'knn',
-            [('input', Int64TensorType([None, X_test.shape[1]]))],
-            target_opset=TARGET_OPSET)
-        exp = model.predict(X_test)
-
-        sess = InferenceSession(model_onnx.SerializeToString())
-        res = sess.run(None, {'input': numpy.array(X_test)})[0].ravel()
-
-        # The conversion has discrepencies when
-        # neighbours are at the exact same distance.
-        maxd = 1000
-        accb = numpy.abs(exp - res) > maxd
-        ind = [i for i, a in enumerate(accb) if a == 1]
-        assert len(ind) == 0
-
-        accp = numpy.abs(exp - res) < maxd
-        acc = numpy.sum(accp)
-        ratio = acc * 1.0 / res.shape[0]
-        assert ratio >= 0.7
-        # assert_almost_equal(exp, res)
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_multi_class_nocl(self):
-        model, X = fit_classification_model(
-            KNeighborsClassifier(),
-            2, label_string=True)
-        model_onnx = convert_sklearn(
-            model, "KNN multi-class nocl",
-            [("input", FloatTensorType([None, X.shape[1]]))],
-            options={id(model): {'nocl': True}},
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        sonx = str(model_onnx)
-        assert 'classlabels_strings' not in sonx
-        assert 'cl0' not in sonx
-        dump_data_and_model(
-            X, model, model_onnx, classes=model.classes_,
-            basename="SklearnKNNMultiNoCl", verbose=False,
-            allow_failure="StrictVersion(onnx.__version__)"
-                          " < StrictVersion('1.2') or "
-                          "StrictVersion(onnxruntime.__version__)"
-                          " <= StrictVersion('0.2.1')")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_regressor2_2_pipee(self):
-        pipe = make_pipeline(StandardScaler(),
-                             KNeighborsClassifier())
-        model, X = self._fit_model_binary_classification(pipe)
-        model_onnx = convert_sklearn(
-            model, "KNN pipe",
-            [("input", FloatTensorType([None, X.shape[1]]))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:2],
-            model, model_onnx,
-            basename="SklearnKNeighborsRegressorPipe2")
-
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_onnx_test_knn_transform(self):
-        iris = datasets.load_iris()
-        X, _ = iris.data, iris.target
-
-        X_train, X_test = train_test_split(X, random_state=11)
-        clr = NearestNeighbors(n_neighbors=3, radius=None)
-        clr.fit(X_train)
-
-        for to in (9, 10, 11):
-            if to > TARGET_OPSET:
-                break
-            model_def = to_onnx(clr, X_train.astype(numpy.float32),
-                                target_opset=to)
-            oinf = InferenceSession(model_def.SerializeToString())
-
-            X_test = X_test[:3]
-            y = oinf.run(None, {'X': X_test.astype(numpy.float32)})
-            dist, ind = clr.kneighbors(X_test)
-
-            assert_almost_equal(dist, DataFrame(y[1]).values, decimal=5)
-            assert_almost_equal(ind, y[0])
-
-    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
-                     reason="new in 0.22")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_nca_default(self):
-        model, X_test = fit_classification_model(
-            NeighborhoodComponentsAnalysis(random_state=42), 3)
-        model_onnx = convert_sklearn(
-            model,
-            "NCA",
-            [("input", FloatTensorType((None, X_test.shape[1])))],
-        )
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X_test,
-            model,
-            model_onnx,
-            basename="SklearnNCADefault",
-        )
-
-    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
-                     reason="new in 0.22")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_nca_identity(self):
-        model, X_test = fit_classification_model(
-            NeighborhoodComponentsAnalysis(
-                init='identity', max_iter=4, random_state=42), 3)
-        model_onnx = convert_sklearn(
-            model,
-            "NCA",
-            [("input", FloatTensorType((None, X_test.shape[1])))],
-        )
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X_test,
-            model,
-            model_onnx,
-            basename="SklearnNCAIdentity",
-        )
-
-    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
-                     reason="new in 0.22")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_nca_double(self):
-        model, X_test = fit_classification_model(
-            NeighborhoodComponentsAnalysis(
-                n_components=2, max_iter=4, random_state=42), 3)
-        X_test = X_test.astype(numpy.float64)
-        model_onnx = convert_sklearn(
-            model,
-            "NCA",
-            [("input", DoubleTensorType((None, X_test.shape[1])))],
-        )
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X_test,
-            model,
-            model_onnx,
-            basename="SklearnNCADouble",
-        )
-
-    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
-                     reason="new in 0.22")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_nca_int(self):
-        model, X_test = fit_classification_model(
-            NeighborhoodComponentsAnalysis(
-                init='pca', max_iter=4, random_state=42), 3, is_int=True)
-        model_onnx = convert_sklearn(
-            model,
-            "NCA",
-            [("input", Int64TensorType((None, X_test.shape[1])))],
-        )
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X_test,
-            model,
-            model_onnx,
-            basename="SklearnNCAInt",
-        )
-
-    @unittest.skipIf(KNeighborsTransformer is None,
-                     reason="new in 0.22")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_k_neighbours_transformer_distance(self):
-        model, X_test = fit_classification_model(
-            KNeighborsTransformer(
-                n_neighbors=4, mode='distance'), 2)
-        model_onnx = convert_sklearn(
-            model,
-            "KNN transformer",
-            [("input", FloatTensorType((None, X_test.shape[1])))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X_test,
-            model,
-            model_onnx,
-            basename="SklearnKNNTransformerDistance",
-        )
-
-    @unittest.skipIf(KNeighborsTransformer is None,
-                     reason="new in 0.22")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_k_neighbours_transformer_connectivity(self):
-        model, X_test = fit_classification_model(
-            KNeighborsTransformer(
-                n_neighbors=3, mode='connectivity'), 3)
-        model_onnx = convert_sklearn(
-            model,
-            "KNN transformer",
-            [("input", FloatTensorType((None, X_test.shape[1])))],
-            target_opset=TARGET_OPSET)
-        self.assertIsNotNone(model_onnx)
-        dump_data_and_model(
-            X_test,
-            model,
-            model_onnx,
-            basename="SklearnKNNTransformerConnectivity",
-        )
-
-    @unittest.skipIf(KNNImputer is None,
-                     reason="new in 0.22")
-    @unittest.skipIf((StrictVersion(onnx.__version__) <
-                      StrictVersion("1.4.1")),
-                     reason="ConstantOfShape op not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_knn_imputer(self):
-        x_train = numpy.array(
-            [[1, 2, numpy.nan, 12], [3, numpy.nan, 3, 13],
-             [1, 4, numpy.nan, 1], [numpy.nan, 4, 3, 12]], dtype=numpy.float32)
-        x_test = numpy.array(
-            [[1.3, 2.4, numpy.nan, 1], [-1.3, numpy.nan, 3.1, numpy.nan]],
-            dtype=numpy.float32)
-        model = KNNImputer(n_neighbors=3, metric='nan_euclidean').fit(x_train)
-        for opset in [TARGET_OPSET, 9, 10, 11, 12]:
-            if opset > TARGET_OPSET:
-                continue
-            model_onnx = convert_sklearn(
-                model, "KNN imputer",
-                [("input", FloatTensorType((None, x_test.shape[1])))],
-                target_opset=opset)
-            self.assertIsNotNone(model_onnx)
-            dump_data_and_model(
-                x_test, model, model_onnx,
-                basename="SklearnKNNImputer%d" % opset)
-
-    @unittest.skipIf(KNNImputer is None,
-                     reason="new in 0.22")
-    @unittest.skipIf((StrictVersion(onnx.__version__) <
-                      StrictVersion("1.4.1")),
-                     reason="ConstantOfShape op not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_sklearn_knn_imputer_cdist(self):
-        x_train = numpy.array(
-            [[1, 2, numpy.nan, 12], [3, numpy.nan, 3, 13],
-             [1, 4, numpy.nan, 1], [numpy.nan, 4, 3, 12]], dtype=numpy.float32)
-        x_test = numpy.array(
-            [[1.3, 2.4, numpy.nan, 1], [-1.3, numpy.nan, 3.1, numpy.nan]],
-            dtype=numpy.float32)
-        model = KNNImputer(n_neighbors=3, metric='nan_euclidean').fit(x_train)
-
-        with self.assertRaises(NameError):
-            convert_sklearn(
-                model, "KNN imputer",
-                [("input", FloatTensorType((None, x_test.shape[1])))],
-                target_opset=TARGET_OPSET,
-                options={id(model): {'optim2': 'cdist'}})
-
-        for opset in [TARGET_OPSET, 12, 11, 10, 9]:
-            if opset > TARGET_OPSET:
-                continue
-            model_onnx = convert_sklearn(
-                model, "KNN imputer",
-                [("input", FloatTensorType((None, x_test.shape[1])))],
-                target_opset=opset,
-                options={id(model): {'optim': 'cdist'}})
-            self.assertIsNotNone(model_onnx)
-            self.assertIn('op_type: "cdist"', str(model_onnx).lower())
-            self.assertNotIn('scan', str(model_onnx).lower())
-            dump_data_and_model(
-                x_test, model, model_onnx,
-                basename="SklearnKNNImputer%dcdist" % opset)
-
-    @unittest.skipIf(not onnx_built_with_ml(),
-                     reason="Requires ONNX-ML extension.")
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @unittest.skipIf(TARGET_OPSET < 11,
-                     reason="needs higher target_opset")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_iris_regressor_multi_reg(self):
-        iris = datasets.load_iris()
-        X = iris.data.astype(numpy.float32)
-        y = iris.target.astype(numpy.float32)
-        y = numpy.vstack([y, 1 - y, y + 10]).T
-        model = KNeighborsRegressor(
-            algorithm='brute', weights='distance', n_neighbors=7)
-        model.fit(X[:13], y[:13])
-        onx = to_onnx(model, X[:1],
-                      options={id(model): {'optim': 'cdist'}},
-                      target_opset=TARGET_OPSET)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7],
-            model, onx,
-            basename="SklearnKNeighborsRegressorMReg")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_iris_regressor_multi_reg_radius(self):
-        iris = datasets.load_iris()
-        X = iris.data.astype(numpy.float32)
-        y = iris.target.astype(numpy.float32)
-        y = numpy.vstack([y, 1 - y, y + 10]).T
-        model = KNeighborsRegressor(
-            algorithm='brute', weights='distance')
-        model.fit(X[:13], y[:13])
-        onx = to_onnx(model, X[:1],
-                      options={id(model): {'optim': 'cdist'}},
-                      target_opset=TARGET_OPSET)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:7],
-            model, onx,
-            basename="SklearnRadiusNeighborsRegressorMReg")
-        dump_data_and_model(
-            (X + 0.1).astype(numpy.float32)[:7],
-            model, onx,
-            basename="SklearnRadiusNeighborsRegressorMReg")
-
-    @unittest.skipIf(not onnx_built_with_ml(),
-                     reason="Requires ONNX-ML extension.")
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @unittest.skipIf(TARGET_OPSET < 11,
-                     reason="needs higher target_opset")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_iris_classifier_multi_reg2_weight(self):
-        iris = datasets.load_iris()
-        X = iris.data.astype(numpy.float32)
-        y = iris.target.astype(numpy.int64)
-        y = numpy.vstack([(y + 1) % 2, y % 2]).T
-        model = KNeighborsClassifier(
-            algorithm='brute', weights='distance', n_neighbors=7)
-        model.fit(X[:13], y[:13])
-        onx = to_onnx(model, X[:1],
-                      options={id(model): {'optim': 'cdist',
-                                           'zipmap': False}},
-                      target_opset=TARGET_OPSET)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:11],
-            model, onx,
-            basename="SklearnKNeighborsClassifierMReg2-Out0")
-
-    @unittest.skipIf(dont_test_radius(), reason="not available")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_iris_classifier_multi_reg2_weight_radius(self):
-        iris = datasets.load_iris()
-        X = iris.data.astype(numpy.float32)
-        y = iris.target.astype(numpy.int64)
-        y = numpy.vstack([(y + 1) % 2, y % 2]).T
-        model = RadiusNeighborsClassifier(
-            algorithm='brute', weights='distance')
-        model.fit(X[:13], y[:13])
-        onx = to_onnx(model, X[:1],
-                      options={id(model): {'optim': 'cdist',
-                                           'zipmap': False}},
-                      target_opset=TARGET_OPSET)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:11],
-            model, onx,
-            basename="SklearnRadiusNeighborsClassifierMReg2-Out0")
-
-    @unittest.skipIf(not onnx_built_with_ml(),
-                     reason="Requires ONNX-ML extension.")
-    @unittest.skipIf(
-        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
-        reason="not available")
-    @unittest.skipIf(TARGET_OPSET < 11,
-                     reason="needs higher target_opset")
-    @ignore_warnings(category=DeprecationWarning)
-    def test_model_knn_iris_classifier_multi_reg3_weight(self):
-        iris = datasets.load_iris()
-        X = iris.data.astype(numpy.float32)
-        y = iris.target.astype(numpy.int64)
-        y = numpy.vstack([y % 2, y % 2, (y+1) % 2]).T
-        model = KNeighborsClassifier(
-            algorithm='brute', weights='distance',
-            n_neighbors=7)
-        model.fit(X[:13], y[:13])
-        onx = to_onnx(model, X[:1],
-                      options={id(model): {'optim': 'cdist',
-                                           'zipmap': False}},
-                      target_opset=TARGET_OPSET)
-        dump_data_and_model(
-            X.astype(numpy.float32)[:11],
-            model, onx,
-            basename="SklearnKNeighborsClassifierMReg3-Out0")
-
-
-if __name__ == "__main__":
-    unittest.main()
+# SPDX-License-Identifier: Apache-2.0
+
+"""
+Tests scikit-learn's KNeighbours Classifier and Regressor converters.
+"""
+import sys
+import warnings
+import unittest
+import functools
+from distutils.version import StrictVersion
+import numpy
+from numpy.testing import assert_almost_equal
+import onnx
+import onnxruntime
+from onnxruntime import InferenceSession
+from pandas import DataFrame
+try:
+    from sklearn.utils._testing import ignore_warnings
+except ImportError:
+    # older versions of scikit-learn
+    from sklearn.utils.testing import ignore_warnings
+from sklearn import datasets
+from sklearn.model_selection import train_test_split
+from sklearn.neighbors import (
+    KNeighborsRegressor, RadiusNeighborsRegressor,
+    KNeighborsClassifier, RadiusNeighborsClassifier,
+    NearestNeighbors)
+try:
+    from sklearn.impute import KNNImputer
+    from sklearn.neighbors import (
+        KNeighborsTransformer,
+        NeighborhoodComponentsAnalysis)
+except ImportError:
+    # New in 0.22
+    KNNImputer = None
+    KNeighborsTransformer = None
+    NeighborhoodComponentsAnalysis = None
+from sklearn.pipeline import make_pipeline
+from sklearn.preprocessing import StandardScaler
+try:
+    from onnxruntime.capi.onnxruntime_pybind11_state import (
+        NotImplemented as OrtImpl)
+except ImportError:
+    OrtImpl = RuntimeError
+from skl2onnx import convert_sklearn, to_onnx
+from skl2onnx.common.data_types import (
+    DoubleTensorType,
+    FloatTensorType,
+    Int64TensorType,
+)
+from skl2onnx.common.data_types import onnx_built_with_ml
+from skl2onnx.helpers.onnx_helper import (
+    enumerate_model_node_outputs, select_model_inputs_outputs)
+from test_utils import (
+    dump_data_and_model,
+    fit_classification_model,
+    fit_multilabel_classification_model,
+    TARGET_OPSET)
+
+
+def dont_test_radius():
+    return (
+        StrictVersion(onnxruntime.__version__) <= StrictVersion("1.3.0") or
+        StrictVersion(onnx.__version__) <= StrictVersion("1.6.0"))
+
+
+class TestNearestNeighbourConverter(unittest.TestCase):
+
+    @functools.lru_cache(maxsize=1)
+    def _get_iris(self):
+        iris = datasets.load_iris()
+        X = iris.data[::2, :3]
+        y = iris.target[::2]
+        return X, y
+
+    def _fit_model_binary_classification(self, model):
+        X, y = self._get_iris()
+        y[y == 2] = 1
+        model.fit(X, y)
+        return model, X
+
+    def _fit_model_multiclass_classification(self, model, use_string=False):
+        X, y = self._get_iris()
+        if use_string:
+            y = numpy.array(["cl%d" % _ for _ in y])
+        model.fit(X, y)
+        return model, X
+
+    @functools.lru_cache(maxsize=20)
+    def _get_reg_data(self, n, n_features, n_targets, n_informative=10):
+        X, y = datasets.make_regression(
+            n, n_features=n_features, random_state=0,
+            n_targets=n_targets, n_informative=n_informative)
+        return X, y
+
+    def _fit_model(self, model, n_targets=1, label_int=False,
+                   n_informative=10):
+        X, y = self._get_reg_data(20, 4, n_targets, n_informative)
+        if label_int:
+            y = y.astype(numpy.int64)
+        model.fit(X, y)
+        return model, X
+
+    def _fit_model_simple(self, model, n_targets=1, label_int=False,
+                          n_informative=3):
+        X, y = self._get_reg_data(20, 2, n_targets, n_informative)
+        y /= 100
+        if label_int:
+            y = y.astype(numpy.int64)
+        model.fit(X, y)
+        return model, X
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor(self):
+        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=2))
+        model_onnx = convert_sklearn(model, "KNN regressor",
+                                     [("input", FloatTensorType([None, 4]))],
+                                     target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressor-Dec4")
+        dump_data_and_model(
+            (X + 0.1).astype(numpy.float32)[:7],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressor-Dec4")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("1.8.0"),
+        reason="produces nan values")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_radius(self):
+        model, X = self._fit_model(RadiusNeighborsRegressor())
+        model_onnx = convert_sklearn(model, "KNN regressor",
+                                     [("input", FloatTensorType([None, 4]))],
+                                     target_opset=TARGET_OPSET,
+                                     options={id(model): {'optim': 'cdist'}})
+        sess = InferenceSession(model_onnx.SerializeToString())
+        X = X[:5]
+        got = sess.run(None, {'input': X.astype(numpy.float32)})[0]
+        exp = model.predict(X.astype(numpy.float32))
+        if any(numpy.isnan(got.ravel())):
+            # The model is unexpectedly producing nan values
+            # not on all platforms.
+            rows = ['--EXP--', str(exp), '--GOT--', str(got),
+                    '--EVERY-OUTPUT--']
+            for out in enumerate_model_node_outputs(
+                    model_onnx, add_node=False):
+                onx = select_model_inputs_outputs(model_onnx, out)
+                sess = InferenceSession(onx.SerializeToString())
+                res = sess.run(
+                    None, {'input': X.astype(numpy.float32)})
+                rows.append('--{}--'.format(out))
+                rows.append(str(res))
+            if (StrictVersion(onnxruntime.__version__) <
+                    StrictVersion("1.4.0")):
+                return
+            raise AssertionError('\n'.join(rows))
+        assert_almost_equal(exp.ravel(), got.ravel(), decimal=3)
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(
+        StrictVersion(onnx.__version__) < StrictVersion("1.6.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_double(self):
+        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=2))
+        model_onnx = convert_sklearn(
+            model, "KNN regressor",
+            [("input", DoubleTensorType([None, 4]))],
+            target_opset=TARGET_OPSET,
+            options={id(model): {'optim': 'cdist'}})
+        self.assertIsNotNone(model_onnx)
+        try:
+            InferenceSession(model_onnx.SerializeToString())
+        except OrtImpl as e:
+            if ("Could not find an implementation for the node "
+                    "To_TopK:TopK(11)") in str(e):
+                # onnxruntime does not declare TopK(11) for double
+                return
+            raise e
+        dump_data_and_model(
+            X.astype(numpy.float64)[:7],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressor64")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("1.7.0"),
+        reason="nan may happen during computation")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_double_radius(self):
+        model, X = self._fit_model(RadiusNeighborsRegressor())
+        model_onnx = convert_sklearn(
+            model, "KNN regressor",
+            [("input", DoubleTensorType([None, 4]))],
+            target_opset=TARGET_OPSET,
+            options={id(model): {'optim': 'cdist'}})
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float64)[:7],
+            model, model_onnx,
+            basename="SklearnRadiusNeighborsRegressor64")
+        dump_data_and_model(
+            (X + 10.).astype(numpy.float64)[:7],
+            model, model_onnx,
+            basename="SklearnRadiusNeighborsRegressor64")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_yint(self):
+        model, X = self._fit_model(
+            KNeighborsRegressor(n_neighbors=2), label_int=True)
+        model_onnx = convert_sklearn(model, "KNN regressor",
+                                     [("input", FloatTensorType([None, 4]))],
+                                     target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressorYInt")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_yint_radius(self):
+        model, X = self._fit_model(
+            RadiusNeighborsRegressor(), label_int=True)
+        model_onnx = convert_sklearn(model, "KNN regressor",
+                                     [("input", FloatTensorType([None, 4]))],
+                                     target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7],
+            model, model_onnx,
+            basename="SklearnRadiusNeighborsRegressorYInt")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor2_1(self):
+        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=1),
+                                   n_targets=2)
+        model_onnx = convert_sklearn(model, "KNN regressor",
+                                     [("input", FloatTensorType([None, 4]))],
+                                     target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:3],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressor2")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor2_1_radius(self):
+        model, X = self._fit_model_simple(
+            RadiusNeighborsRegressor(algorithm="brute"),
+            n_targets=2)
+        X = X[:-1]
+        model_onnx = convert_sklearn(
+            model, "KNN regressor",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        sess = InferenceSession(model_onnx.SerializeToString())
+        got = sess.run(None, {'input': X.astype(numpy.float32)})[0]
+        exp = model.predict(X.astype(numpy.float32))
+        if any(numpy.isnan(got.ravel())):
+            # The model is unexpectedly producing nan values
+            # not on all platforms.
+            # It happens when two matrices are multiplied,
+            # one is (2, 20, 20), second is (20, 20)
+            # and contains only 0 or 1 values.
+            # The output contains nan values on the first row
+            # but not on the second one.
+            rows = ['--EXP--', str(exp), '--GOT--', str(got),
+                    '--EVERY-OUTPUT--']
+            for out in enumerate_model_node_outputs(
+                    model_onnx, add_node=False):
+                onx = select_model_inputs_outputs(model_onnx, out)
+                sess = InferenceSession(onx.SerializeToString())
+                res = sess.run(
+                    None, {'input': X.astype(numpy.float32)})
+                rows.append('--{}--'.format(out))
+                rows.append(str(res))
+            if (onnxruntime.__version__.startswith('1.4.') or
+                    onnxruntime.__version__.startswith('1.5.')):
+                # TODO: investigate the regression in onnxruntime 1.4
+                # One broadcasted multiplication unexpectedly produces nan.
+                whole = '\n'.join(rows)
+                if "[        nan" in whole:
+                    warnings.warn(whole)
+                    return
+                raise AssertionError(whole)
+            if (onnxruntime.__version__.startswith('1.3.') and
+                    sys.platform == 'win32'):
+                # Same error but different line number for further
+                # investigation.
+                raise AssertionError(whole)
+            raise AssertionError('\n'.join(rows))
+        assert_almost_equal(exp, got, decimal=5)
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(
+        StrictVersion(onnx.__version__) < StrictVersion("1.4.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor2_1_opset(self):
+        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=1),
+                                   n_targets=2)
+        for op in [TARGET_OPSET, 12, 11, 10, 9]:
+            if op > TARGET_OPSET:
+                continue
+            with self.subTest(opset=op):
+                model_onnx = convert_sklearn(
+                    model, "KNN regressor",
+                    [("input", FloatTensorType([None, 4]))],
+                    target_opset=op)
+                self.assertIsNotNone(model_onnx)
+                dump_data_and_model(
+                    X.astype(numpy.float32)[:3],
+                    model, model_onnx,
+                    basename="SklearnKNeighborsRegressor2%d" % op)
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor2_2(self):
+        model, X = self._fit_model(KNeighborsRegressor(n_neighbors=2),
+                                   n_targets=2)
+        model_onnx = convert_sklearn(model, "KNN regressor",
+                                     [("input", FloatTensorType([None, 4]))],
+                                     target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:2],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressor2")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(TARGET_OPSET < 9,
+                     reason="needs higher target_opset")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_weights_distance_11(self):
+        model, X = self._fit_model(
+            KNeighborsRegressor(
+                weights="distance", algorithm="brute", n_neighbors=1))
+        for op in sorted(set([9, 10, 11, 12, TARGET_OPSET])):
+            if op > TARGET_OPSET:
+                continue
+            with self.subTest(opset=op):
+                model_onnx = convert_sklearn(
+                    model, "KNN regressor",
+                    [("input", FloatTensorType([None, 4]))],
+                    target_opset=op)
+                if op < 12 and model_onnx.ir_version > 6:
+                    raise AssertionError(
+                        "ir_version ({}, op={}) must be <= 6.".format(
+                            model_onnx.ir_version, op))
+                if op < 11 and model_onnx.ir_version > 5:
+                    raise AssertionError(
+                        "ir_version ({}, op={}) must be <= 5.".format(
+                            model_onnx.ir_version, op))
+                if op < 10 and model_onnx.ir_version > 4:
+                    raise AssertionError(
+                        "ir_version ({}, op={}) must be <= 4.".format(
+                            model_onnx.ir_version, op))
+                self.assertIsNotNone(model_onnx)
+                dump_data_and_model(
+                    X.astype(numpy.float32)[:3],
+                    model, model_onnx,
+                    basename="SklearnKNeighborsRegressorWDist%d-Dec3" % op)
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_weights_distance_11_radius(self):
+        model, X = self._fit_model_simple(
+            RadiusNeighborsRegressor(
+                weights="distance", algorithm="brute", radius=100))
+        for op in sorted(set([TARGET_OPSET, 12, 11])):
+            if op > TARGET_OPSET:
+                continue
+            with self.subTest(opset=op):
+                model_onnx = convert_sklearn(
+                    model, "KNN regressor",
+                    [("input", FloatTensorType([None, X.shape[1]]))],
+                    target_opset=op)
+                self.assertIsNotNone(model_onnx)
+                sess = InferenceSession(model_onnx.SerializeToString())
+                got = sess.run(None, {'input': X.astype(numpy.float32)})[0]
+                exp = model.predict(X.astype(numpy.float32))
+                assert_almost_equal(exp, got.ravel(), decimal=3)
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_metric_cityblock(self):
+        model, X = self._fit_model(KNeighborsRegressor(metric="cityblock"))
+        model_onnx = convert_sklearn(model, "KNN regressor",
+                                     [("input", FloatTensorType([None, 4]))],
+                                     target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressorMetricCityblock")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(TARGET_OPSET < TARGET_OPSET,
+                     reason="needs higher target_opset")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_binary_class(self):
+        model, X = self._fit_model_binary_classification(
+            KNeighborsClassifier())
+        model_onnx = convert_sklearn(
+            model,
+            "KNN classifier binary",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET
+        )
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32),
+            model, model_onnx,
+            basename="SklearnKNeighborsClassifierBinary")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @unittest.skipIf(TARGET_OPSET < 12,
+                     reason="needs higher target_opset")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_binary_class_radius(self):
+        model, X = self._fit_model_binary_classification(
+            RadiusNeighborsClassifier())
+        model_onnx = convert_sklearn(
+            model, "KNN classifier binary",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32),
+            model, model_onnx,
+            basename="SklearnRadiusNeighborsClassifierBinary")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_multi_class(self):
+        model, X = self._fit_model_multiclass_classification(
+            KNeighborsClassifier())
+        model_onnx = convert_sklearn(
+            model,
+            "KNN classifier multi-class",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET
+        )
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32),
+            model, model_onnx,
+            basename="SklearnKNeighborsClassifierMulti")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @unittest.skipIf(TARGET_OPSET < 12,
+                     reason="needs higher target_opset")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_multi_class_radius(self):
+        model, X = self._fit_model_multiclass_classification(
+            RadiusNeighborsClassifier())
+        model_onnx = convert_sklearn(
+            model, "KNN classifier multi-class",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET,
+            options={id(model): {'optim': 'cdist'}})
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:5],
+            model, model_onnx,
+            basename="SklearnRadiusNeighborsClassifierMulti")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_multi_class_string(self):
+        model, X = self._fit_model_multiclass_classification(
+            KNeighborsClassifier(), use_string=True)
+        model_onnx = convert_sklearn(
+            model,
+            "KNN classifier multi-class",
+            [("input", FloatTensorType([None, 3]))],
+            target_opset=TARGET_OPSET
+        )
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32),
+            model, model_onnx,
+            basename="SklearnKNeighborsClassifierMulti")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_weights_distance(self):
+        model, X = self._fit_model_multiclass_classification(
+            KNeighborsClassifier(weights='distance'))
+        model_onnx = convert_sklearn(
+            model, 'KNN classifier', [('input', FloatTensorType([None, 3]))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7], model, model_onnx,
+            basename="SklearnKNeighborsClassifierWeightsDistance")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_metric_cityblock(self):
+        model, X = self._fit_model_multiclass_classification(
+            KNeighborsClassifier(metric='cityblock'))
+        model_onnx = convert_sklearn(
+            model, 'KNN classifier', [('input', FloatTensorType([None, 3]))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7], model, model_onnx,
+            basename="SklearnKNeighborsClassifierMetricCityblock")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_classifier_multilabel(self):
+        model, X_test = fit_multilabel_classification_model(
+            KNeighborsClassifier(), n_classes=7, n_labels=3,
+            n_samples=100, n_features=10)
+        options = {id(model): {'zipmap': False}}
+        model_onnx = convert_sklearn(
+            model,
+            "scikit-learn KNN Classifier",
+            [("input", FloatTensorType([None, X_test.shape[1]]))],
+            options=options,
+            target_opset=TARGET_OPSET
+        )
+        self.assertTrue(model_onnx is not None)
+        assert 'zipmap' not in str(model_onnx).lower()
+        dump_data_and_model(
+            X_test,
+            model,
+            model_onnx,
+            basename="SklearnKNNClassifierMultiLabel-Out0",
+            allow_failure="StrictVersion("
+            "onnxruntime.__version__) <= StrictVersion('0.2.1')",
+        )
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_int(self):
+        model, X = self._fit_model(KNeighborsRegressor())
+        X = X.astype(numpy.int64)
+        model_onnx = convert_sklearn(
+            model,
+            "KNN regressor",
+            [("input", Int64TensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X,
+            model,
+            model_onnx,
+            basename="SklearnKNNRegressorInt-Dec4"
+        )
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor_equal(self):
+        X, y = datasets.make_regression(
+            n_samples=1000, n_features=100, random_state=42)
+        X = X.astype(numpy.int64)
+        X_train, X_test, y_train, y_test = train_test_split(
+            X, y, test_size=0.5, random_state=42)
+        model = KNeighborsRegressor(
+            algorithm='brute', metric='manhattan').fit(X_train, y_train)
+        model_onnx = convert_sklearn(
+            model, 'knn',
+            [('input', Int64TensorType([None, X_test.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        exp = model.predict(X_test)
+
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': numpy.array(X_test)})[0].ravel()
+
+        # The conversion has discrepencies when
+        # neighbours are at the exact same distance.
+        maxd = 1000
+        accb = numpy.abs(exp - res) > maxd
+        ind = [i for i, a in enumerate(accb) if a == 1]
+        assert len(ind) == 0
+
+        accp = numpy.abs(exp - res) < maxd
+        acc = numpy.sum(accp)
+        ratio = acc * 1.0 / res.shape[0]
+        assert ratio >= 0.7
+        # assert_almost_equal(exp, res)
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_multi_class_nocl(self):
+        model, X = fit_classification_model(
+            KNeighborsClassifier(),
+            2, label_string=True)
+        model_onnx = convert_sklearn(
+            model, "KNN multi-class nocl",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            options={id(model): {'nocl': True}},
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        sonx = str(model_onnx)
+        assert 'classlabels_strings' not in sonx
+        assert 'cl0' not in sonx
+        dump_data_and_model(
+            X, model, model_onnx, classes=model.classes_,
+            basename="SklearnKNNMultiNoCl", verbose=False,
+            allow_failure="StrictVersion(onnx.__version__)"
+                          " < StrictVersion('1.2') or "
+                          "StrictVersion(onnxruntime.__version__)"
+                          " <= StrictVersion('0.2.1')")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_regressor2_2_pipee(self):
+        pipe = make_pipeline(StandardScaler(),
+                             KNeighborsClassifier())
+        model, X = self._fit_model_binary_classification(pipe)
+        model_onnx = convert_sklearn(
+            model, "KNN pipe",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:2],
+            model, model_onnx,
+            basename="SklearnKNeighborsRegressorPipe2")
+
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_onnx_test_knn_transform(self):
+        iris = datasets.load_iris()
+        X, _ = iris.data, iris.target
+
+        X_train, X_test = train_test_split(X, random_state=11)
+        clr = NearestNeighbors(n_neighbors=3, radius=None)
+        clr.fit(X_train)
+
+        for to in (9, 10, 11):
+            if to > TARGET_OPSET:
+                break
+            model_def = to_onnx(clr, X_train.astype(numpy.float32),
+                                target_opset=to)
+            oinf = InferenceSession(model_def.SerializeToString())
+
+            X_test = X_test[:3]
+            y = oinf.run(None, {'X': X_test.astype(numpy.float32)})
+            dist, ind = clr.kneighbors(X_test)
+
+            assert_almost_equal(dist, DataFrame(y[1]).values, decimal=5)
+            assert_almost_equal(ind, y[0])
+
+    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
+                     reason="new in 0.22")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_nca_default(self):
+        model, X_test = fit_classification_model(
+            NeighborhoodComponentsAnalysis(random_state=42), 3)
+        model_onnx = convert_sklearn(
+            model,
+            "NCA",
+            [("input", FloatTensorType((None, X_test.shape[1])))],
+        )
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X_test,
+            model,
+            model_onnx,
+            basename="SklearnNCADefault",
+        )
+
+    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
+                     reason="new in 0.22")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_nca_identity(self):
+        model, X_test = fit_classification_model(
+            NeighborhoodComponentsAnalysis(
+                init='identity', max_iter=4, random_state=42), 3)
+        model_onnx = convert_sklearn(
+            model,
+            "NCA",
+            [("input", FloatTensorType((None, X_test.shape[1])))],
+        )
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X_test,
+            model,
+            model_onnx,
+            basename="SklearnNCAIdentity",
+        )
+
+    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
+                     reason="new in 0.22")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_nca_double(self):
+        model, X_test = fit_classification_model(
+            NeighborhoodComponentsAnalysis(
+                n_components=2, max_iter=4, random_state=42), 3)
+        X_test = X_test.astype(numpy.float64)
+        model_onnx = convert_sklearn(
+            model,
+            "NCA",
+            [("input", DoubleTensorType((None, X_test.shape[1])))],
+        )
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X_test,
+            model,
+            model_onnx,
+            basename="SklearnNCADouble",
+        )
+
+    @unittest.skipIf(NeighborhoodComponentsAnalysis is None,
+                     reason="new in 0.22")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_nca_int(self):
+        model, X_test = fit_classification_model(
+            NeighborhoodComponentsAnalysis(
+                init='pca', max_iter=4, random_state=42), 3, is_int=True)
+        model_onnx = convert_sklearn(
+            model,
+            "NCA",
+            [("input", Int64TensorType((None, X_test.shape[1])))],
+        )
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X_test,
+            model,
+            model_onnx,
+            basename="SklearnNCAInt",
+        )
+
+    @unittest.skipIf(KNeighborsTransformer is None,
+                     reason="new in 0.22")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_k_neighbours_transformer_distance(self):
+        model, X_test = fit_classification_model(
+            KNeighborsTransformer(
+                n_neighbors=4, mode='distance'), 2)
+        model_onnx = convert_sklearn(
+            model,
+            "KNN transformer",
+            [("input", FloatTensorType((None, X_test.shape[1])))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X_test,
+            model,
+            model_onnx,
+            basename="SklearnKNNTransformerDistance",
+        )
+
+    @unittest.skipIf(KNeighborsTransformer is None,
+                     reason="new in 0.22")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_k_neighbours_transformer_connectivity(self):
+        model, X_test = fit_classification_model(
+            KNeighborsTransformer(
+                n_neighbors=3, mode='connectivity'), 3)
+        model_onnx = convert_sklearn(
+            model,
+            "KNN transformer",
+            [("input", FloatTensorType((None, X_test.shape[1])))],
+            target_opset=TARGET_OPSET)
+        self.assertIsNotNone(model_onnx)
+        dump_data_and_model(
+            X_test,
+            model,
+            model_onnx,
+            basename="SklearnKNNTransformerConnectivity",
+        )
+
+    @unittest.skipIf(KNNImputer is None,
+                     reason="new in 0.22")
+    @unittest.skipIf((StrictVersion(onnx.__version__) <
+                      StrictVersion("1.4.1")),
+                     reason="ConstantOfShape op not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_knn_imputer(self):
+        x_train = numpy.array(
+            [[1, 2, numpy.nan, 12], [3, numpy.nan, 3, 13],
+             [1, 4, numpy.nan, 1], [numpy.nan, 4, 3, 12]], dtype=numpy.float32)
+        x_test = numpy.array(
+            [[1.3, 2.4, numpy.nan, 1], [-1.3, numpy.nan, 3.1, numpy.nan]],
+            dtype=numpy.float32)
+        model = KNNImputer(n_neighbors=3, metric='nan_euclidean').fit(x_train)
+        for opset in [TARGET_OPSET, 9, 10, 11, 12]:
+            if opset > TARGET_OPSET:
+                continue
+            model_onnx = convert_sklearn(
+                model, "KNN imputer",
+                [("input", FloatTensorType((None, x_test.shape[1])))],
+                target_opset=opset)
+            self.assertIsNotNone(model_onnx)
+            dump_data_and_model(
+                x_test, model, model_onnx,
+                basename="SklearnKNNImputer%d" % opset)
+
+    @unittest.skipIf(KNNImputer is None,
+                     reason="new in 0.22")
+    @unittest.skipIf((StrictVersion(onnx.__version__) <
+                      StrictVersion("1.4.1")),
+                     reason="ConstantOfShape op not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_sklearn_knn_imputer_cdist(self):
+        x_train = numpy.array(
+            [[1, 2, numpy.nan, 12], [3, numpy.nan, 3, 13],
+             [1, 4, numpy.nan, 1], [numpy.nan, 4, 3, 12]], dtype=numpy.float32)
+        x_test = numpy.array(
+            [[1.3, 2.4, numpy.nan, 1], [-1.3, numpy.nan, 3.1, numpy.nan]],
+            dtype=numpy.float32)
+        model = KNNImputer(n_neighbors=3, metric='nan_euclidean').fit(x_train)
+
+        with self.assertRaises(NameError):
+            convert_sklearn(
+                model, "KNN imputer",
+                [("input", FloatTensorType((None, x_test.shape[1])))],
+                target_opset=TARGET_OPSET,
+                options={id(model): {'optim2': 'cdist'}})
+
+        for opset in [TARGET_OPSET, 12, 11, 10, 9]:
+            if opset > TARGET_OPSET:
+                continue
+            model_onnx = convert_sklearn(
+                model, "KNN imputer",
+                [("input", FloatTensorType((None, x_test.shape[1])))],
+                target_opset=opset,
+                options={id(model): {'optim': 'cdist'}})
+            self.assertIsNotNone(model_onnx)
+            self.assertIn('op_type: "cdist"', str(model_onnx).lower())
+            self.assertNotIn('scan', str(model_onnx).lower())
+            dump_data_and_model(
+                x_test, model, model_onnx,
+                basename="SklearnKNNImputer%dcdist" % opset)
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(TARGET_OPSET < 11,
+                     reason="needs higher target_opset")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_iris_regressor_multi_reg(self):
+        iris = datasets.load_iris()
+        X = iris.data.astype(numpy.float32)
+        y = iris.target.astype(numpy.float32)
+        y = numpy.vstack([y, 1 - y, y + 10]).T
+        model = KNeighborsRegressor(
+            algorithm='brute', weights='distance', n_neighbors=7)
+        model.fit(X[:13], y[:13])
+        onx = to_onnx(model, X[:1],
+                      options={id(model): {'optim': 'cdist'}},
+                      target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7],
+            model, onx,
+            basename="SklearnKNeighborsRegressorMReg")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_iris_regressor_multi_reg_radius(self):
+        iris = datasets.load_iris()
+        X = iris.data.astype(numpy.float32)
+        y = iris.target.astype(numpy.float32)
+        y = numpy.vstack([y, 1 - y, y + 10]).T
+        model = KNeighborsRegressor(
+            algorithm='brute', weights='distance')
+        model.fit(X[:13], y[:13])
+        onx = to_onnx(model, X[:1],
+                      options={id(model): {'optim': 'cdist'}},
+                      target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:7],
+            model, onx,
+            basename="SklearnRadiusNeighborsRegressorMReg")
+        dump_data_and_model(
+            (X + 0.1).astype(numpy.float32)[:7],
+            model, onx,
+            basename="SklearnRadiusNeighborsRegressorMReg")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(TARGET_OPSET < 11,
+                     reason="needs higher target_opset")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_iris_classifier_multi_reg2_weight(self):
+        iris = datasets.load_iris()
+        X = iris.data.astype(numpy.float32)
+        y = iris.target.astype(numpy.int64)
+        y = numpy.vstack([(y + 1) % 2, y % 2]).T
+        model = KNeighborsClassifier(
+            algorithm='brute', weights='distance', n_neighbors=7)
+        model.fit(X[:13], y[:13])
+        onx = to_onnx(model, X[:1],
+                      options={id(model): {'optim': 'cdist',
+                                           'zipmap': False}},
+                      target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:11],
+            model, onx,
+            basename="SklearnKNeighborsClassifierMReg2-Out0")
+
+    @unittest.skipIf(dont_test_radius(), reason="not available")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_iris_classifier_multi_reg2_weight_radius(self):
+        iris = datasets.load_iris()
+        X = iris.data.astype(numpy.float32)
+        y = iris.target.astype(numpy.int64)
+        y = numpy.vstack([(y + 1) % 2, y % 2]).T
+        model = RadiusNeighborsClassifier(
+            algorithm='brute', weights='distance')
+        model.fit(X[:13], y[:13])
+        onx = to_onnx(model, X[:1],
+                      options={id(model): {'optim': 'cdist',
+                                           'zipmap': False}},
+                      target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:11],
+            model, onx,
+            basename="SklearnRadiusNeighborsClassifierMReg2-Out0")
+
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    @unittest.skipIf(
+        StrictVersion(onnxruntime.__version__) < StrictVersion("0.5.0"),
+        reason="not available")
+    @unittest.skipIf(TARGET_OPSET < 11,
+                     reason="needs higher target_opset")
+    @ignore_warnings(category=DeprecationWarning)
+    def test_model_knn_iris_classifier_multi_reg3_weight(self):
+        iris = datasets.load_iris()
+        X = iris.data.astype(numpy.float32)
+        y = iris.target.astype(numpy.int64)
+        y = numpy.vstack([y % 2, y % 2, (y+1) % 2]).T
+        model = KNeighborsClassifier(
+            algorithm='brute', weights='distance',
+            n_neighbors=7)
+        model.fit(X[:13], y[:13])
+        onx = to_onnx(model, X[:1],
+                      options={id(model): {'optim': 'cdist',
+                                           'zipmap': False}},
+                      target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X.astype(numpy.float32)[:11],
+            model, onx,
+            basename="SklearnKNeighborsClassifierMReg3-Out0")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_normalizer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_normalizer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_one_hot_encoder_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_one_hot_encoder_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_one_vs_rest_classifier_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_one_vs_rest_classifier_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_ordinal_encoder.py` & `skl2onnx-1.9.3/tests/test_sklearn_ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_passive_aggressive_classifier_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_passive_aggressive_classifier_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_pca_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_pca_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_perceptron_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_perceptron_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_pipeline_within_pipeline.py` & `skl2onnx-1.9.3/tests/test_sklearn_pipeline_within_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Tests pipeline within pipelines.
 """
-
-import numpy as np
+from textwrap import dedent
 import unittest
+from io import StringIO
+import numpy as np
+import pandas
 try:
     from sklearn.compose import ColumnTransformer
 except ImportError:
     # not available in 0.19
     ColumnTransformer = None
 try:
     from sklearn.impute import SimpleImputer
 except ImportError:
     from sklearn.preprocessing import Imputer as SimpleImputer
 from sklearn.decomposition import PCA
 from sklearn.linear_model import LogisticRegression
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.pipeline import Pipeline
-from sklearn.preprocessing import MinMaxScaler
-from sklearn.preprocessing import RobustScaler, StandardScaler
-from skl2onnx import convert_sklearn
-from skl2onnx.common.data_types import FloatTensorType
+from sklearn.preprocessing import (
+    MinMaxScaler, RobustScaler, StandardScaler, OneHotEncoder)
+from sklearn.feature_extraction.text import CountVectorizer
+from skl2onnx import convert_sklearn, to_onnx
+from skl2onnx.common.data_types import FloatTensorType, StringTensorType
 from skl2onnx.common.data_types import onnx_built_with_ml
 from test_utils import dump_data_and_model, TARGET_OPSET
 
 
 class TestSklearnPipelineWithinPipeline(unittest.TestCase):
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
@@ -264,16 +267,15 @@
             basename="SklearnPipelinePcaPipelineMinMaxNBNone",
             allow_failure="StrictVersion(onnxruntime.__version__)"
                           " <= StrictVersion('0.2.1')",
         )
 
     @unittest.skipIf(
         ColumnTransformer is None,
-        reason="ColumnTransformer not available in 0.19",
-    )
+        reason="ColumnTransformer not available in 0.19")
     @unittest.skipIf(not onnx_built_with_ml(),
                      reason="Requires ONNX-ML extension.")
     def test_pipeline_column_transformer_pipeline_imputer_scaler_lr(self):
         X = np.array([[1, 2], [3, np.nan], [3, 0]], dtype=np.float32)
         y = np.array([1, 0, 1])
         model = Pipeline([
             (
@@ -312,10 +314,56 @@
             model,
             model_onnx,
             basename="SklearnPipelineCTPipelineImputerScalerLR",
             allow_failure="StrictVersion(onnxruntime.__version__)"
                           " <= StrictVersion('0.2.1')",
         )
 
+    @unittest.skipIf(
+        ColumnTransformer is None,
+        reason="ColumnTransformer not available in 0.19")
+    @unittest.skipIf(not onnx_built_with_ml(),
+                     reason="Requires ONNX-ML extension.")
+    def test_complex_pipeline(self):
+
+        df = pandas.read_csv(StringIO(dedent("""
+            CAT1,CAT2,TEXT
+            A,M,clean
+            B,N,text
+            A,M,cleaning
+            B,N,normalizing""")))
+
+        X_train = df
+        y_train = np.array([[1, 0, 1, 0], [1, 0, 1, 0]]).T
+
+        categorical_features = ['CAT1', 'CAT2']
+        textual_feature = 'TEXT'
+
+        preprocessor = ColumnTransformer(
+            transformers=[
+                ('cat_transform', OneHotEncoder(handle_unknown='ignore'),
+                 categorical_features),
+                ('count_vector', Pipeline(steps=[
+                    ('count_vect', CountVectorizer(
+                        max_df=0.8, min_df=0.05, max_features=1000))]),
+                 textual_feature)])
+
+        preprocessor.fit(X_train, y_train)
+        initial_type = [('CAT1', StringTensorType([None, 1])),
+                        ('CAT2', StringTensorType([None, 1])),
+                        ('TEXTs', StringTensorType([None, 1]))]
+        with self.assertRaises(RuntimeError):
+            to_onnx(preprocessor, initial_types=initial_type,
+                    target_opset=TARGET_OPSET)
+
+        initial_type = [('CAT1', StringTensorType([None, 1])),
+                        ('CAT2', StringTensorType([None, 1])),
+                        ('TEXT', StringTensorType([None, 1]))]
+        onx = to_onnx(preprocessor, initial_types=initial_type,
+                      target_opset=TARGET_OPSET)
+        dump_data_and_model(
+            X_train, preprocessor, onx,
+            basename="SklearnPipelineComplex")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_pls_regression.py` & `skl2onnx-1.9.3/tests/test_sklearn_pls_regression.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_polynomial_features_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_polynomial_features_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_power_transformer.py` & `skl2onnx-1.9.3/tests/test_sklearn_power_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_random_forest_converters.py` & `skl2onnx-1.9.3/tests/test_sklearn_random_forest_converters.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_random_projection.py` & `skl2onnx-1.9.3/tests/test_sklearn_random_projection.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_replace_transformer.py` & `skl2onnx-1.9.3/tests/test_sklearn_replace_transformer.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_scaler_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_scaler_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_sgd_classifier_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_sgd_classifier_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_stacking.py` & `skl2onnx-1.9.3/tests/test_sklearn_stacking.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_svm_converters.py` & `skl2onnx-1.9.3/tests/test_sklearn_svm_converters.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 """
 Tests scikit-linear converter.
 """
 import unittest
 from distutils.version import StrictVersion
 import numpy
+from numpy.testing import assert_almost_equal
+from onnxruntime import InferenceSession
 from sklearn.datasets import load_iris
-from sklearn.svm import SVC, SVR, NuSVC, NuSVR, OneClassSVM
+from sklearn.svm import SVC, SVR, NuSVC, NuSVR, OneClassSVM, LinearSVC
 try:
     from skl2onnx.common._apply_operation import apply_less
 except ImportError:
     # onnxconverter-common is too old
     apply_less = None
 from skl2onnx import convert_sklearn
 from skl2onnx.common.data_types import (
@@ -538,10 +540,141 @@
             X,
             model,
             model_onnx,
             basename="SklearnBinOneClassSVM",
             allow_failure="StrictVersion(onnxruntime.__version__)"
                           " < StrictVersion('0.5.0')")
 
+    def test_model_linear_svc_binary_class(self):
+        model, X = self._fit_binary_classification(LinearSVC(max_iter=10000))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))])
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.decision_function(X)
+        assert_almost_equal(proba, res[1].ravel(), decimal=5)
+        assert_almost_equal(label, res[0])
+
+    def test_model_linear_svc_multi_class(self):
+        model, X = self._fit_multi_classification(LinearSVC(max_iter=10000))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))])
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.decision_function(X)
+        assert_almost_equal(proba, res[1], decimal=5)
+        assert_almost_equal(label, res[0])
+
+    def test_model_svc_binary_class_false(self):
+        model, X = self._fit_binary_classification(SVC(max_iter=10000))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))])
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.decision_function(X)
+        assert_almost_equal(proba, res[1][:, 0], decimal=5)
+        assert_almost_equal(label, res[0])
+
+    @unittest.skipIf(TARGET_OPSET < 12, reason="operator Less")
+    def test_model_svc_multi_class_false(self):
+        model, X = self._fit_multi_classification(SVC(max_iter=10000))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))])
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.decision_function(X)
+        assert_almost_equal(proba, res[1], decimal=5)
+        assert_almost_equal(label, res[0])
+
+    def test_model_svc_binary_class_true(self):
+        model, X = self._fit_binary_classification(
+            SVC(max_iter=10000, probability=True))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            options={'zipmap': False})
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.predict_proba(X)
+        assert_almost_equal(proba, res[1], decimal=5)
+        assert_almost_equal(label, res[0])
+
+    def test_model_svc_multi_class_true(self):
+        model, X = self._fit_multi_classification(
+            SVC(max_iter=10000, probability=True))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            options={'zipmap': False})
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.predict_proba(X)
+        assert_almost_equal(proba, res[1], decimal=5)
+        assert_almost_equal(label, res[0])
+
+    def test_model_nusvc_binary_class_false(self):
+        model, X = self._fit_binary_classification(NuSVC(max_iter=10000))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))])
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.decision_function(X)
+        assert_almost_equal(proba, res[1][:, 0], decimal=5)
+        assert_almost_equal(label, res[0])
+
+    @unittest.skipIf(TARGET_OPSET < 12, reason="operator Less")
+    def test_model_nusvc_multi_class_false(self):
+        model, X = self._fit_multi_classification(
+            NuSVC(max_iter=10000, nu=0.1))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))])
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.decision_function(X)
+        assert_almost_equal(proba, res[1], decimal=4)
+        assert_almost_equal(label, res[0])
+
+    def test_model_nusvc_binary_class_true(self):
+        model, X = self._fit_binary_classification(
+            NuSVC(max_iter=10000, probability=True))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            options={'zipmap': False})
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.predict_proba(X)
+        assert_almost_equal(proba, res[1], decimal=5)
+        assert_almost_equal(label, res[0])
+
+    def test_model_nusvc_multi_class_true(self):
+        model, X = self._fit_multi_classification(
+            NuSVC(max_iter=10000, probability=True, nu=0.1))
+        model_onnx = convert_sklearn(
+            model, "linear SVC",
+            [("input", FloatTensorType([None, X.shape[1]]))],
+            options={'zipmap': False})
+        sess = InferenceSession(model_onnx.SerializeToString())
+        res = sess.run(None, {'input': X})
+        label = model.predict(X)
+        proba = model.predict_proba(X)
+        assert_almost_equal(proba, res[1], decimal=3)
+        assert_almost_equal(label, res[0])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_tfidf_transformer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_tfidf_transformer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_tfidf_transformer_converter_sparse.py` & `skl2onnx-1.9.3/tests/test_sklearn_tfidf_transformer_converter_sparse.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_char.py` & `skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_char.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_dataset.py` & `skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_dataset.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_pipeline.py` & `skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_pipeline.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_tfidf_vectorizer_converter_regex.py` & `skl2onnx-1.9.3/tests/test_sklearn_tfidf_vectorizer_converter_regex.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_truncated_svd.py` & `skl2onnx-1.9.3/tests/test_sklearn_truncated_svd.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_voting_classifier_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_voting_classifier_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_sklearn_voting_regressor_converter.py` & `skl2onnx-1.9.3/tests/test_sklearn_voting_regressor_converter.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_supported_converters.py` & `skl2onnx-1.9.3/tests/test_supported_converters.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_utils/__init__.py` & `skl2onnx-1.9.3/tests/test_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     dump_multiple_classification)
 from .tests_helper import (  # noqa
     dump_multiple_regression,
     dump_single_regression,
     convert_model,
     fit_classification_model,
     fit_multilabel_classification_model,
+    fit_clustering_model,
     fit_regression_model,
     binary_array_to_string,
     path_to_leaf
 )
 
 
 def create_tensor(N, C, H=None, W=None):
```

### Comparing `skl2onnx-1.9.2/tests/test_utils/main.py` & `skl2onnx-1.9.3/tests/test_utils/main.py`

 * *Files identical despite different names*

### Comparing `skl2onnx-1.9.2/tests/test_utils/tests_helper.py` & `skl2onnx-1.9.3/tests/test_utils/tests_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,36 @@
         X = X.astype(bool)
     X_train, X_test, y_train, _ = train_test_split(X, y, test_size=0.5,
                                                    random_state=42)
     model.fit(X_train, y_train)
     return model, X_test
 
 
+def fit_clustering_model(model, n_classes, is_int=False,
+                         pos_features=False, label_string=False,
+                         random_state=42, is_bool=False,
+                         n_features=20, n_redundant=None,
+                         n_repeated=None):
+    X, y = make_classification(
+        n_classes=n_classes, n_features=n_features, n_samples=250,
+        random_state=random_state, n_informative=min(7, n_features),
+        n_redundant=n_redundant or min(2, n_features - min(7, n_features)),
+        n_repeated=n_repeated or 0)
+    if label_string:
+        y = numpy.array(['cl%d' % cl for cl in y])
+    X = X.astype(numpy.int64) if is_int or is_bool else X.astype(numpy.float32)
+    if pos_features:
+        X = numpy.abs(X)
+    if is_bool:
+        X = X.astype(bool)
+    X_train, X_test = train_test_split(X, test_size=0.5, random_state=42)
+    model.fit(X_train)
+    return model, X_test
+
+
 def fit_multilabel_classification_model(model, n_classes=5, n_labels=2,
                                         n_samples=200, n_features=20,
                                         is_int=False):
     X, y = make_multilabel_classification(
         n_classes=n_classes, n_labels=n_labels, n_features=n_features,
         n_samples=n_samples, random_state=42)
     X = X.astype(numpy.int64) if is_int else X.astype(numpy.float32)
@@ -317,27 +339,28 @@
         pickle.dump(prediction, f)
 
     dest = os.path.join(folder, basename + ".data.pkl")
     names.append(dest)
     with open(dest, "wb") as f:
         pickle.dump(data, f)
 
-    if hasattr(model, "save"):
-        dest = os.path.join(folder, basename + ".model.keras")
-        names.append(dest)
-        model.save(dest)
-    else:
-        dest = os.path.join(folder, basename + ".model.pkl")
-        names.append(dest)
-        with open(dest, "wb") as f:
-            try:
-                pickle.dump(model, f)
-            except AttributeError as e:
-                print("[dump_data_and_model] cannot pickle model '{}'"
-                      " due to {}.".format(dest, e))
+    dest = os.path.join(folder, basename + ".model.pkl")
+    names.append(dest)
+    load_pickle = True
+    with open(dest, "wb") as f:
+        try:
+            pickle.dump(model, f)
+        except AttributeError as e:
+            print("[dump_data_and_model] cannot pickle model '{}'"
+                  " due to {}.".format(dest, e))
+            load_pickle = False
+    if load_pickle and os.path.exists(dest):
+        # Test unpickle works.
+        with open(dest, "rb") as f:
+            pickle.load(f)
 
     if dump_error_log:
         error_dump = os.path.join(folder, basename + ".err")
 
     if onnx is None:
         array = numpy.array(data)
         if inputs is None:
@@ -873,14 +896,15 @@
     import onnxruntime
     import cpuinfo
 
     res = {}
     benched = 0
     files = os.listdir(folder)
     for name in files:
+        print(name)
         if name.endswith(".expected.pkl"):
             model = name.split(".")[0]
             if model not in res:
                 res[model] = {}
             res[model]["_tested"] = True
         elif ".backend." in name:
             bk = name.split(".backend.")[-1].split(".")[0]
```

### Comparing `skl2onnx-1.9.2/tests/test_utils/utils_backend.py` & `skl2onnx-1.9.3/tests/test_utils/utils_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 class OnnxRuntimeAssertionError(AssertionError):
     """
     Expected failure.
     """
 
     def __init__(self, msg):
-        new_msg = "{}\nonnx=={} onnxruntime=={}".format(
-            msg, onnx.__version__, onnxruntime.__version__)
+        from . import TARGET_OPSET
+        new_msg = "{}\nonnx=={} onnxruntime=={} TARGET_OPSET={}".format(
+            msg, onnx.__version__, onnxruntime.__version__, TARGET_OPSET)
         AssertionError.__init__(self, new_msg)
 
 
 class OnnxRuntimeMissingNewOnnxOperatorException(OnnxRuntimeAssertionError):
     """
     Raised when onnxruntime does not implement a new operator
     defined in the latest onnx.
```

### Comparing `skl2onnx-1.9.2/tests/test_utils/utils_backend_onnxruntime.py` & `skl2onnx-1.9.3/tests/test_utils/utils_backend_onnxruntime.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,18 +478,14 @@
     if isinstance(expected, list):
         if isinstance(output, list):
             if 'Out0' in kwargs:
                 expected = expected[:1]
                 output = output[:1]
                 del kwargs['Out0']
             elif 'Out1' in kwargs:
-                print('----------')
-                print(expected)
-                print(output)
-                print('----------')
                 expected = expected[1:2]
                 output = output[1:2]
                 del kwargs['Out1']
             if 'Reshape' in kwargs:
                 del kwargs['Reshape']
                 output = numpy.hstack(output).ravel()
                 output = output.reshape(
```

### Comparing `skl2onnx-1.9.2/tests/test_utils_sklearn.py` & `skl2onnx-1.9.3/tests/test_utils_sklearn.py`

 * *Files identical despite different names*

