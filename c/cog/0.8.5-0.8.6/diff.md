# Comparing `tmp/cog-0.8.5-py3-none-any.whl.zip` & `tmp/cog-0.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,99 +1,100 @@
-Zip file size: 79104 bytes, number of entries: 97
--rw-r--r--  2.0 unx       13 b- defN 23-Aug-01 23:24 cog/.gitignore
--rw-r--r--  2.0 unx      362 b- defN 23-Aug-01 23:24 cog/__init__.py
--rw-r--r--  2.0 unx      160 b- defN 23-Aug-01 23:25 cog/_version.py
--rw-r--r--  2.0 unx      286 b- defN 23-Aug-01 23:24 cog/errors.py
--rw-r--r--  2.0 unx     2082 b- defN 23-Aug-01 23:24 cog/files.py
--rw-r--r--  2.0 unx     1992 b- defN 23-Aug-01 23:24 cog/json.py
--rw-r--r--  2.0 unx     3171 b- defN 23-Aug-01 23:24 cog/logging.py
--rw-r--r--  2.0 unx    11239 b- defN 23-Aug-01 23:24 cog/predictor.py
--rw-r--r--  2.0 unx     2385 b- defN 23-Aug-01 23:24 cog/schema.py
--rw-r--r--  2.0 unx      645 b- defN 23-Aug-01 23:24 cog/suppress_output.py
--rw-r--r--  2.0 unx     8562 b- defN 23-Aug-01 23:24 cog/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 23:24 cog/command/__init__.py
--rw-r--r--  2.0 unx      761 b- defN 23-Aug-01 23:24 cog/command/openapi_schema.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 23:24 cog/server/__init__.py
--rw-r--r--  2.0 unx      593 b- defN 23-Aug-01 23:24 cog/server/eventtypes.py
--rw-r--r--  2.0 unx      149 b- defN 23-Aug-01 23:24 cog/server/exceptions.py
--rw-r--r--  2.0 unx     5349 b- defN 23-Aug-01 23:24 cog/server/helpers.py
--rw-r--r--  2.0 unx    12055 b- defN 23-Aug-01 23:24 cog/server/http.py
--rw-r--r--  2.0 unx      957 b- defN 23-Aug-01 23:24 cog/server/probes.py
--rw-r--r--  2.0 unx      650 b- defN 23-Aug-01 23:24 cog/server/response_throttler.py
--rw-r--r--  2.0 unx    14284 b- defN 23-Aug-01 23:24 cog/server/runner.py
--rw-r--r--  2.0 unx     3092 b- defN 23-Aug-01 23:24 cog/server/webhook.py
--rw-r--r--  2.0 unx     7970 b- defN 23-Aug-01 23:24 cog/server/worker.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 23:24 tests/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 23-Aug-01 23:24 tests/conftest.py
--rw-r--r--  2.0 unx     1733 b- defN 23-Aug-01 23:24 tests/test_json.py
--rw-r--r--  2.0 unx      486 b- defN 23-Aug-01 23:24 tests/test_predictor.py
--rw-r--r--  2.0 unx     4690 b- defN 23-Aug-01 23:24 tests/test_types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 23:24 tests/server/__init__.py
--rw-r--r--  2.0 unx     2056 b- defN 23-Aug-01 23:24 tests/server/conftest.py
--rw-r--r--  2.0 unx     4692 b- defN 23-Aug-01 23:24 tests/server/test_helpers.py
--rw-r--r--  2.0 unx    15179 b- defN 23-Aug-01 23:24 tests/server/test_http.py
--rw-r--r--  2.0 unx     6957 b- defN 23-Aug-01 23:24 tests/server/test_http_input.py
--rw-r--r--  2.0 unx     4020 b- defN 23-Aug-01 23:24 tests/server/test_http_output.py
--rw-r--r--  2.0 unx     1334 b- defN 23-Aug-01 23:24 tests/server/test_probes.py
--rw-r--r--  2.0 unx     1210 b- defN 23-Aug-01 23:24 tests/server/test_response_throttler.py
--rw-r--r--  2.0 unx    10943 b- defN 23-Aug-01 23:24 tests/server/test_runner.py
--rw-r--r--  2.0 unx     3225 b- defN 23-Aug-01 23:24 tests/server/test_webhook.py
--rw-r--r--  2.0 unx    16095 b- defN 23-Aug-01 23:24 tests/server/test_worker.py
--rw-r--r--  2.0 unx      198 b- defN 23-Aug-01 23:24 tests/server/fixtures/catch_in_predict.py
--rw-r--r--  2.0 unx      232 b- defN 23-Aug-01 23:24 tests/server/fixtures/complex_output.py
--rw-r--r--  2.0 unx      131 b- defN 23-Aug-01 23:24 tests/server/fixtures/count_up.py
--rw-r--r--  2.0 unx      136 b- defN 23-Aug-01 23:24 tests/server/fixtures/exc_in_predict.py
--rw-r--r--  2.0 unx      133 b- defN 23-Aug-01 23:24 tests/server/fixtures/exc_in_setup.py
--rw-r--r--  2.0 unx      151 b- defN 23-Aug-01 23:24 tests/server/fixtures/exc_in_setup_and_predict.py
--rw-r--r--  2.0 unx       56 b- defN 23-Aug-01 23:24 tests/server/fixtures/exc_on_import.py
--rw-r--r--  2.0 unx      122 b- defN 23-Aug-01 23:24 tests/server/fixtures/exit_in_predict.py
--rw-r--r--  2.0 unx      124 b- defN 23-Aug-01 23:24 tests/server/fixtures/exit_in_setup.py
--rw-r--r--  2.0 unx       23 b- defN 23-Aug-01 23:24 tests/server/fixtures/exit_on_import.py
--rw-r--r--  2.0 unx       58 b- defN 23-Aug-01 23:24 tests/server/fixtures/function.py
--rw-r--r--  2.0 unx      159 b- defN 23-Aug-01 23:24 tests/server/fixtures/hello_world.py
--rw-r--r--  2.0 unx      197 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_choices.py
--rw-r--r--  2.0 unx      153 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_choices_integer.py
--rw-r--r--  2.0 unx      139 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_file.py
--rw-r--r--  2.0 unx      160 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_ge_le.py
--rw-r--r--  2.0 unx      126 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_integer.py
--rw-r--r--  2.0 unx      152 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_integer_default.py
--rw-r--r--  2.0 unx      317 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_multiple.py
--rw-r--r--  2.0 unx      118 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_none.py
--rw-r--r--  2.0 unx      236 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_path.py
--rw-r--r--  2.0 unx      137 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_path_2.py
--rw-r--r--  2.0 unx      125 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_string.py
--rw-r--r--  2.0 unx      205 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_unsupported_type.py
--rw-r--r--  2.0 unx      122 b- defN 23-Aug-01 23:24 tests/server/fixtures/input_untyped.py
--rw-r--r--  2.0 unx      160 b- defN 23-Aug-01 23:24 tests/server/fixtures/killed_in_predict.py
--rw-r--r--  2.0 unx      882 b- defN 23-Aug-01 23:24 tests/server/fixtures/logging.py
--rw-r--r--  2.0 unx      109 b- defN 23-Aug-01 23:24 tests/server/fixtures/missing_predict.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 23:24 tests/server/fixtures/missing_predictor.py
--rw-r--r--  2.0 unx      481 b- defN 23-Aug-01 23:24 tests/server/fixtures/openapi_complex_input.py
--rw-r--r--  2.0 unx      332 b- defN 23-Aug-01 23:24 tests/server/fixtures/openapi_custom_output_type.py
--rw-r--r--  2.0 unx      169 b- defN 23-Aug-01 23:24 tests/server/fixtures/openapi_input_int_choices.py
--rw-r--r--  2.0 unx      153 b- defN 23-Aug-01 23:24 tests/server/fixtures/openapi_output_list.py
--rw-r--r--  2.0 unx      374 b- defN 23-Aug-01 23:24 tests/server/fixtures/openapi_output_type.py
--rw-r--r--  2.0 unx      161 b- defN 23-Aug-01 23:24 tests/server/fixtures/openapi_output_yield.py
--rw-r--r--  2.0 unx      264 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_complex.py
--rw-r--r--  2.0 unx      148 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_file.py
--rw-r--r--  2.0 unx      192 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_file_named.py
--rw-r--r--  2.0 unx      257 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_iterator_complex.py
--rw-r--r--  2.0 unx      151 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_numpy.py
--rw-r--r--  2.0 unx      355 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_path_image.py
--rw-r--r--  2.0 unx      323 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_path_text.py
--rw-r--r--  2.0 unx      115 b- defN 23-Aug-01 23:24 tests/server/fixtures/output_wrong_type.py
--rw-r--r--  2.0 unx      175 b- defN 23-Aug-01 23:24 tests/server/fixtures/setup.py
--rw-r--r--  2.0 unx      167 b- defN 23-Aug-01 23:24 tests/server/fixtures/setup_weights.py
--rw-r--r--  2.0 unx      118 b- defN 23-Aug-01 23:24 tests/server/fixtures/simple.py
--rw-r--r--  2.0 unx      193 b- defN 23-Aug-01 23:24 tests/server/fixtures/sleep.py
--rw-r--r--  2.0 unx      219 b- defN 23-Aug-01 23:24 tests/server/fixtures/slow_predict.py
--rw-r--r--  2.0 unx      290 b- defN 23-Aug-01 23:24 tests/server/fixtures/steps.py
--rw-r--r--  2.0 unx      263 b- defN 23-Aug-01 23:24 tests/server/fixtures/yield_concatenate_iterator.py
--rw-r--r--  2.0 unx      506 b- defN 23-Aug-01 23:24 tests/server/fixtures/yield_files.py
--rw-r--r--  2.0 unx      245 b- defN 23-Aug-01 23:24 tests/server/fixtures/yield_strings.py
--rw-r--r--  2.0 unx      339 b- defN 23-Aug-01 23:24 tests/server/fixtures/yield_strings_file_input.py
--rw-r--r--  2.0 unx    11347 b- defN 23-Aug-01 23:25 cog-0.8.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    35131 b- defN 23-Aug-01 23:25 cog-0.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 23:25 cog-0.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Aug-01 23:25 cog-0.8.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8474 b- defN 23-Aug-01 23:25 cog-0.8.5.dist-info/RECORD
-97 files, 215818 bytes uncompressed, 65554 bytes compressed:  69.6%
+Zip file size: 83627 bytes, number of entries: 98
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-07 21:51 cog/.gitignore
+-rw-r--r--  2.0 unx      362 b- defN 23-Aug-07 21:51 cog/__init__.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Aug-07 21:52 cog/_version.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Aug-07 21:51 cog/errors.py
+-rw-r--r--  2.0 unx     2082 b- defN 23-Aug-07 21:51 cog/files.py
+-rw-r--r--  2.0 unx     1992 b- defN 23-Aug-07 21:51 cog/json.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Aug-07 21:51 cog/logging.py
+-rw-r--r--  2.0 unx    11239 b- defN 23-Aug-07 21:51 cog/predictor.py
+-rw-r--r--  2.0 unx     2618 b- defN 23-Aug-07 21:51 cog/schema.py
+-rw-r--r--  2.0 unx      645 b- defN 23-Aug-07 21:51 cog/suppress_output.py
+-rw-r--r--  2.0 unx     8590 b- defN 23-Aug-07 21:51 cog/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 21:51 cog/command/__init__.py
+-rw-r--r--  2.0 unx    17318 b- defN 23-Aug-07 21:51 cog/command/ast_openapi_schema.py
+-rw-r--r--  2.0 unx      761 b- defN 23-Aug-07 21:51 cog/command/openapi_schema.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 21:51 cog/server/__init__.py
+-rw-r--r--  2.0 unx      593 b- defN 23-Aug-07 21:51 cog/server/eventtypes.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Aug-07 21:51 cog/server/exceptions.py
+-rw-r--r--  2.0 unx     5349 b- defN 23-Aug-07 21:51 cog/server/helpers.py
+-rw-r--r--  2.0 unx    12055 b- defN 23-Aug-07 21:51 cog/server/http.py
+-rw-r--r--  2.0 unx      957 b- defN 23-Aug-07 21:51 cog/server/probes.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Aug-07 21:51 cog/server/response_throttler.py
+-rw-r--r--  2.0 unx    14284 b- defN 23-Aug-07 21:51 cog/server/runner.py
+-rw-r--r--  2.0 unx     3092 b- defN 23-Aug-07 21:51 cog/server/webhook.py
+-rw-r--r--  2.0 unx     7970 b- defN 23-Aug-07 21:51 cog/server/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 21:51 tests/__init__.py
+-rw-r--r--  2.0 unx      536 b- defN 23-Aug-07 21:51 tests/conftest.py
+-rw-r--r--  2.0 unx     1733 b- defN 23-Aug-07 21:51 tests/test_json.py
+-rw-r--r--  2.0 unx      486 b- defN 23-Aug-07 21:51 tests/test_predictor.py
+-rw-r--r--  2.0 unx     4689 b- defN 23-Aug-07 21:51 tests/test_types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 21:51 tests/server/__init__.py
+-rw-r--r--  2.0 unx     2312 b- defN 23-Aug-07 21:51 tests/server/conftest.py
+-rw-r--r--  2.0 unx     4692 b- defN 23-Aug-07 21:51 tests/server/test_helpers.py
+-rw-r--r--  2.0 unx    15623 b- defN 23-Aug-07 21:51 tests/server/test_http.py
+-rw-r--r--  2.0 unx     6957 b- defN 23-Aug-07 21:51 tests/server/test_http_input.py
+-rw-r--r--  2.0 unx     4020 b- defN 23-Aug-07 21:51 tests/server/test_http_output.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-Aug-07 21:51 tests/server/test_probes.py
+-rw-r--r--  2.0 unx     1210 b- defN 23-Aug-07 21:51 tests/server/test_response_throttler.py
+-rw-r--r--  2.0 unx    10943 b- defN 23-Aug-07 21:51 tests/server/test_runner.py
+-rw-r--r--  2.0 unx     3225 b- defN 23-Aug-07 21:51 tests/server/test_webhook.py
+-rw-r--r--  2.0 unx    16095 b- defN 23-Aug-07 21:51 tests/server/test_worker.py
+-rw-r--r--  2.0 unx      198 b- defN 23-Aug-07 21:51 tests/server/fixtures/catch_in_predict.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Aug-07 21:51 tests/server/fixtures/complex_output.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Aug-07 21:51 tests/server/fixtures/count_up.py
+-rw-r--r--  2.0 unx      136 b- defN 23-Aug-07 21:51 tests/server/fixtures/exc_in_predict.py
+-rw-r--r--  2.0 unx      133 b- defN 23-Aug-07 21:51 tests/server/fixtures/exc_in_setup.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Aug-07 21:51 tests/server/fixtures/exc_in_setup_and_predict.py
+-rw-r--r--  2.0 unx       56 b- defN 23-Aug-07 21:51 tests/server/fixtures/exc_on_import.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Aug-07 21:51 tests/server/fixtures/exit_in_predict.py
+-rw-r--r--  2.0 unx      124 b- defN 23-Aug-07 21:51 tests/server/fixtures/exit_in_setup.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Aug-07 21:51 tests/server/fixtures/exit_on_import.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Aug-07 21:51 tests/server/fixtures/function.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Aug-07 21:51 tests/server/fixtures/hello_world.py
+-rw-r--r--  2.0 unx      197 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_choices_integer.py
+-rw-r--r--  2.0 unx      139 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_file.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_ge_le.py
+-rw-r--r--  2.0 unx      126 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_integer.py
+-rw-r--r--  2.0 unx      152 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_integer_default.py
+-rw-r--r--  2.0 unx      317 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_multiple.py
+-rw-r--r--  2.0 unx      118 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_none.py
+-rw-r--r--  2.0 unx      236 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_path.py
+-rw-r--r--  2.0 unx      137 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_path_2.py
+-rw-r--r--  2.0 unx      125 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_string.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_unsupported_type.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Aug-07 21:51 tests/server/fixtures/input_untyped.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Aug-07 21:51 tests/server/fixtures/killed_in_predict.py
+-rw-r--r--  2.0 unx      882 b- defN 23-Aug-07 21:51 tests/server/fixtures/logging.py
+-rw-r--r--  2.0 unx      109 b- defN 23-Aug-07 21:51 tests/server/fixtures/missing_predict.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 21:51 tests/server/fixtures/missing_predictor.py
+-rw-r--r--  2.0 unx      481 b- defN 23-Aug-07 21:51 tests/server/fixtures/openapi_complex_input.py
+-rw-r--r--  2.0 unx      332 b- defN 23-Aug-07 21:51 tests/server/fixtures/openapi_custom_output_type.py
+-rw-r--r--  2.0 unx      169 b- defN 23-Aug-07 21:51 tests/server/fixtures/openapi_input_int_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Aug-07 21:51 tests/server/fixtures/openapi_output_list.py
+-rw-r--r--  2.0 unx      374 b- defN 23-Aug-07 21:51 tests/server/fixtures/openapi_output_type.py
+-rw-r--r--  2.0 unx      161 b- defN 23-Aug-07 21:51 tests/server/fixtures/openapi_output_yield.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_complex.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_file.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_file_named.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_iterator_complex.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_numpy.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_path_image.py
+-rw-r--r--  2.0 unx      323 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_path_text.py
+-rw-r--r--  2.0 unx      115 b- defN 23-Aug-07 21:51 tests/server/fixtures/output_wrong_type.py
+-rw-r--r--  2.0 unx      175 b- defN 23-Aug-07 21:51 tests/server/fixtures/setup.py
+-rw-r--r--  2.0 unx      167 b- defN 23-Aug-07 21:51 tests/server/fixtures/setup_weights.py
+-rw-r--r--  2.0 unx      118 b- defN 23-Aug-07 21:51 tests/server/fixtures/simple.py
+-rw-r--r--  2.0 unx      193 b- defN 23-Aug-07 21:51 tests/server/fixtures/sleep.py
+-rw-r--r--  2.0 unx      219 b- defN 23-Aug-07 21:51 tests/server/fixtures/slow_predict.py
+-rw-r--r--  2.0 unx      290 b- defN 23-Aug-07 21:51 tests/server/fixtures/steps.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Aug-07 21:51 tests/server/fixtures/yield_concatenate_iterator.py
+-rw-r--r--  2.0 unx      506 b- defN 23-Aug-07 21:51 tests/server/fixtures/yield_files.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Aug-07 21:51 tests/server/fixtures/yield_strings.py
+-rw-r--r--  2.0 unx      339 b- defN 23-Aug-07 21:51 tests/server/fixtures/yield_strings_file_input.py
+-rw-r--r--  2.0 unx    11347 b- defN 23-Aug-07 21:52 cog-0.8.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    35113 b- defN 23-Aug-07 21:52 cog-0.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 21:52 cog-0.8.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-07 21:52 cog-0.8.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8565 b- defN 23-Aug-07 21:52 cog-0.8.6.dist-info/RECORD
+98 files, 234169 bytes uncompressed, 69935 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -30,14 +30,17 @@
 
 Filename: cog/types.py
 Comment: 
 
 Filename: cog/command/__init__.py
 Comment: 
 
+Filename: cog/command/ast_openapi_schema.py
+Comment: 
+
 Filename: cog/command/openapi_schema.py
 Comment: 
 
 Filename: cog/server/__init__.py
 Comment: 
 
 Filename: cog/server/eventtypes.py
@@ -270,23 +273,23 @@
 
 Filename: tests/server/fixtures/yield_strings.py
 Comment: 
 
 Filename: tests/server/fixtures/yield_strings_file_input.py
 Comment: 
 
-Filename: cog-0.8.5.dist-info/LICENSE
+Filename: cog-0.8.6.dist-info/LICENSE
 Comment: 
 
-Filename: cog-0.8.5.dist-info/METADATA
+Filename: cog-0.8.6.dist-info/METADATA
 Comment: 
 
-Filename: cog-0.8.5.dist-info/WHEEL
+Filename: cog-0.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: cog-0.8.5.dist-info/top_level.txt
+Filename: cog-0.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: cog-0.8.5.dist-info/RECORD
+Filename: cog-0.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cog/_version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '0.8.5'
-__version_tuple__ = version_tuple = (0, 8, 5)
+__version__ = version = '0.8.6'
+__version_tuple__ = version_tuple = (0, 8, 6)
```

## cog/schema.py

```diff
@@ -20,16 +20,19 @@
 class WebhookEvent(str, Enum):
     START = "start"
     OUTPUT = "output"
     LOGS = "logs"
     COMPLETED = "completed"
 
     @classmethod
-    def default_events(cls) -> t.Set["WebhookEvent"]:
-        return {cls.START, cls.OUTPUT, cls.LOGS, cls.COMPLETED}
+    def default_events(cls) -> t.List["WebhookEvent"]:
+        # if this is a set, it gets serialized to an array with an unstable ordering
+        # so even though it's logically a set, have it as a list for deterministic schemas
+        # note: this change removes "uniqueItems":true
+        return [cls.START, cls.OUTPUT, cls.LOGS, cls.COMPLETED]
 
 
 class PredictionBaseModel(pydantic.BaseModel, extra=pydantic.Extra.allow):
     input: t.Dict[str, t.Any]
 
 
 class PredictionRequest(PredictionBaseModel):
@@ -37,15 +40,15 @@
     created_at: t.Optional[datetime]
 
     # TODO: deprecate this
     output_file_prefix: t.Optional[str]
 
     webhook: t.Optional[pydantic.AnyHttpUrl]
     webhook_events_filter: t.Optional[
-        t.Set[WebhookEvent]
+        t.List[WebhookEvent]
     ] = WebhookEvent.default_events()
 
     @classmethod
     def with_types(cls, input_type: t.Type) -> t.Any:
         # [compat] Input is implicitly optional -- previous versions of the
         # Cog HTTP API allowed input to be omitted (e.g. for models that don't
         # have any inputs). We should consider changing this in future.
```

## cog/types.py

```diff
@@ -1,8 +1,7 @@
-import base64
 import io
 import mimetypes
 import os
 import pathlib
 import shutil
 import tempfile
 import urllib
@@ -52,15 +51,15 @@
     @classmethod
     def validate(cls, value: Any) -> io.IOBase:
         if isinstance(value, io.IOBase):
             return value
 
         parsed_url = urllib.parse.urlparse(value)
         if parsed_url.scheme == "data":
-            res = urllib.request.urlopen(value)
+            res = urllib.request.urlopen(value)  # noqa: S310
             return io.BytesIO(res.read())
         elif parsed_url.scheme == "http" or parsed_url.scheme == "https":
             return URLFile(value)
         else:
             raise ValueError(
                 f"'{parsed_url.scheme}' is not a valid URL scheme. 'data', 'http', or 'https' is supported."
             )
@@ -207,15 +206,15 @@
             )
 
 
 def get_filename(url: str) -> str:
     parsed_url = urllib.parse.urlparse(url)
 
     if parsed_url.scheme == "data":
-        resp = urllib.request.urlopen(url)
+        resp = urllib.request.urlopen(url)  # noqa: S310
         mime_type = resp.headers.get_content_type()
         extension = mimetypes.guess_extension(mime_type)
         if extension is None:
             return "file"
         return "file" + extension
 
     basename = os.path.basename(parsed_url.path)
@@ -257,19 +256,19 @@
         yield cls.validate
 
     @classmethod
     def validate(cls, value: Any) -> Iterator:
         return value
 
 
-def _len_bytes(s, encoding="utf-8"):
+def _len_bytes(s, encoding="utf-8") -> int:
     return len(s.encode(encoding))
 
 
-def _truncate_filename_bytes(s, length, encoding="utf-8"):
+def _truncate_filename_bytes(s, length, encoding="utf-8") -> str:
     """
     Truncate a filename to at most `length` bytes, preserving file extension
     and avoiding text encoding corruption from truncation.
     """
     root, ext = os.path.splitext(s.encode(encoding))
     root = root[: length - len(ext) - 1]
     return root.decode(encoding, "ignore") + "~" + ext.decode(encoding)
```

## tests/test_types.py

```diff
@@ -1,13 +1,12 @@
 import io
 import pickle
 
 import pytest
 import responses
-
 from cog.types import URLFile, get_filename
 
 
 @responses.activate
 def test_urlfile_acts_like_response():
     responses.get(
         "https://example.com/some/url",
```

## tests/server/conftest.py

```diff
@@ -3,14 +3,15 @@
 import time
 from contextlib import ExitStack
 from typing import Any, Dict, Optional
 from unittest import mock
 
 import pytest
 from attrs import define
+from cog.command import ast_openapi_schema
 from cog.server.http import create_app
 from fastapi.testclient import TestClient
 
 
 @define
 class AppConfig:
     predictor_fixture: str
@@ -70,8 +71,16 @@
             stack.enter_context(mock.patch.dict(os.environ, options["env"]))
             del options["env"]
 
         # Use context manager to trigger setup/shutdown events.
         c = make_client(fixture_name=fixture_name, **options)
         stack.enter_context(c)
         wait_for_setup(c)
+        c.ref = fixture_name
         yield c
+
+
+@pytest.fixture
+def static_schema(client) -> dict:
+    ref = _fixture_path(client.ref)
+    module_path = ref.split(":", 1)[0]
+    return ast_openapi_schema.extract_file(module_path)
```

## tests/server/test_http.py

```diff
@@ -21,19 +21,20 @@
 def test_predict_works_with_functions(client, match):
     resp = client.post("/predictions", json={"input": {"text": "baz"}})
     assert resp.status_code == 200
     assert resp.json() == match({"status": "succeeded", "output": "hello baz"})
 
 
 @uses_predictor("openapi_complex_input")
-def test_openapi_specification(client):
+def test_openapi_specification(client, static_schema):
     resp = client.get("/openapi.json")
     assert resp.status_code == 200
 
     schema = resp.json()
+    assert schema == static_schema
     assert schema["openapi"] == "3.0.2"
     assert schema["info"] == {"title": "Cog", "version": "0.1.0"}
     assert schema["paths"]["/"] == {
         "get": {
             "summary": "Root",
             "operationId": "root__get",
             "responses": {
@@ -186,19 +187,22 @@
         "enum": [3, 4, 5],
         "title": "int_choices",
         "type": "integer",
     }
 
 
 @uses_predictor("openapi_custom_output_type")
-def test_openapi_specification_with_custom_user_defined_output_type(client):
+def test_openapi_specification_with_custom_user_defined_output_type(
+    client, static_schema
+):
     resp = client.get("/openapi.json")
     assert resp.status_code == 200
 
     schema = resp.json()
+    assert schema == static_schema
     assert schema["components"]["schemas"]["Output"] == {
         "$ref": "#/components/schemas/MyOutput",
         "title": "Output",
     }
     assert schema["components"]["schemas"]["MyOutput"] == {
         "title": "MyOutput",
         "type": "object",
@@ -215,19 +219,20 @@
             },
         },
     }
 
 
 @uses_predictor("openapi_output_type")
 def test_openapi_specification_with_custom_user_defined_output_type_called_output(
-    client,
+    client, static_schema
 ):
     resp = client.get("/openapi.json")
     assert resp.status_code == 200
-
+    schema = resp.json()
+    assert schema == static_schema
     assert resp.json()["components"]["schemas"]["Output"] == {
         "properties": {
             "foo_number": {"default": "42", "title": "Foo Number", "type": "integer"},
             "foo_string": {
                 "default": "meaning of life",
                 "title": "Foo String",
                 "type": "string",
@@ -235,64 +240,72 @@
         },
         "title": "Output",
         "type": "object",
     }
 
 
 @uses_predictor("openapi_output_yield")
-def test_openapi_specification_with_yield(client):
+def test_openapi_specification_with_yield(client, static_schema):
     resp = client.get("/openapi.json")
     assert resp.status_code == 200
-
-    assert resp.json()["components"]["schemas"]["Output"] == {
+    schema = resp.json()
+    assert schema == static_schema
+    assert schema["components"]["schemas"]["Output"] == {
         "title": "Output",
         "type": "array",
         "items": {
             "type": "string",
         },
         "x-cog-array-type": "iterator",
     }
 
 
 @uses_predictor("yield_concatenate_iterator")
-def test_openapi_specification_with_yield_with_concatenate_iterator(client):
+def test_openapi_specification_with_yield_with_concatenate_iterator(
+    client, static_schema
+):
     resp = client.get("/openapi.json")
     assert resp.status_code == 200
 
-    assert resp.json()["components"]["schemas"]["Output"] == {
+    schema = resp.json()
+    assert schema == static_schema
+    assert schema["components"]["schemas"]["Output"] == {
         "title": "Output",
         "type": "array",
         "items": {
             "type": "string",
         },
         "x-cog-array-type": "iterator",
         "x-cog-array-display": "concatenate",
     }
 
 
 @uses_predictor("openapi_output_list")
-def test_openapi_specification_with_list(client):
+def test_openapi_specification_with_list(client, static_schema):
     resp = client.get("/openapi.json")
     assert resp.status_code == 200
 
-    assert resp.json()["components"]["schemas"]["Output"] == {
+    schema = resp.json()
+    assert schema == static_schema
+    assert schema["components"]["schemas"]["Output"] == {
         "title": "Output",
         "type": "array",
         "items": {
             "type": "string",
         },
     }
 
 
 @uses_predictor("openapi_input_int_choices")
-def test_openapi_specification_with_int_choices(client):
+def test_openapi_specification_with_int_choices(client, static_schema):
     resp = client.get("/openapi.json")
     assert resp.status_code == 200
 
     schema = resp.json()
+    assert schema == static_schema
     schemas = schema["components"]["schemas"]
 
     assert schemas["Input"]["properties"]["pick_a_number_any_number"] == {
         "allOf": [{"$ref": "#/components/schemas/pick_a_number_any_number"}],
         "x-order": 0,
     }
     assert schemas["pick_a_number_any_number"] == {
```

## Comparing `cog-0.8.5.dist-info/LICENSE` & `cog-0.8.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cog-0.8.5.dist-info/METADATA` & `cog-0.8.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog
-Version: 0.8.5
+Version: 0.8.6
 Summary: Containers for machine learning
 Author-email: Replicate <team@replicate.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,37 +206,37 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Source, https://github.com/replicate/cog
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: attrs (<24,>=20.1)
-Requires-Dist: fastapi (<0.99.0,>=0.75.2)
-Requires-Dist: pydantic (<2,>=1.9)
+Requires-Dist: attrs <24,>=20.1
+Requires-Dist: fastapi <0.99.0,>=0.75.2
+Requires-Dist: pydantic <2,>=1.9
 Requires-Dist: PyYAML
-Requires-Dist: requests (<3,>=2)
-Requires-Dist: structlog (<24,>=20)
-Requires-Dist: typing-extensions (>=4.1.0)
-Requires-Dist: uvicorn[standard] (<1,>=0.12)
+Requires-Dist: requests <3,>=2
+Requires-Dist: structlog <24,>=20
+Requires-Dist: typing-extensions >=4.1.0
+Requires-Dist: uvicorn[standard] <1,>=0.12
 Requires-Dist: typing-compat ; python_version < "3.8"
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: build ; extra == 'dev'
 Requires-Dist: httpx ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: pillow ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-httpserver ; extra == 'dev'
 Requires-Dist: pytest-rerunfailures ; extra == 'dev'
 Requires-Dist: pytest-xdist ; extra == 'dev'
 Requires-Dist: responses ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
-Requires-Dist: hypothesis (<6.80.0) ; (python_version < "3.8") and extra == 'dev'
-Requires-Dist: numpy (<1.22.0) ; (python_version < "3.8") and extra == 'dev'
+Requires-Dist: hypothesis <6.80.0 ; (python_version < "3.8") and extra == 'dev'
+Requires-Dist: numpy <1.22.0 ; (python_version < "3.8") and extra == 'dev'
 Requires-Dist: hypothesis ; (python_version >= "3.8") and extra == 'dev'
 Requires-Dist: numpy ; (python_version >= "3.8") and extra == 'dev'
 
 # Cog: Containers for machine learning
 
 Cog is an open-source tool that lets you package machine learning models in a standard, production-ready container.
```

## Comparing `cog-0.8.5.dist-info/RECORD` & `cog-0.8.6.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 cog/.gitignore,sha256=OIzCsCr9oYv3wBtJU_TppxWi-OhuDmwCBrrUqcE6kfY,13
 cog/__init__.py,sha256=qDIBBVsf5tfoaCGu49zQyYQb_AWtCwIxQrp9RLZlbbI,362
-cog/_version.py,sha256=_yTFHIaycw2gu_KorhTVKABA78x3tEzdUAQVvpcM4xw,160
+cog/_version.py,sha256=tnPaGZc_1U1yYoze8SrI5NCDv7PExNqxFYt9JZajs10,160
 cog/errors.py,sha256=pB29TjzvXmyqbqi3zPOlLobFJnVWb6GJ9WsLE-77TIQ,286
 cog/files.py,sha256=HC8Z9yrM4g5jQy8Ohin_RR5f2VtPeqbzyNa6lOjNO1I,2082
 cog/json.py,sha256=c7yTci8VdhnVknXYX7G0gcDDCg9PSXS3Ni0-Xlttvns,1992
 cog/logging.py,sha256=3I7jOG1HKU5oh6-xJF1dh_qFMJMBrjo9Z60zM6sr3qU,3171
 cog/predictor.py,sha256=l6x0JcKbXpvo17gPzrC2zcTMnB0vv7PFZCax1lQ_rsw,11239
-cog/schema.py,sha256=RgjgTyU4vrBNR8NQ5HxZW8GQJsDhh6zqoe5X2HBWNqk,2385
+cog/schema.py,sha256=LS3jAiWmJPpPDiASP1YQVSspJ6ZVH_FQNK_IzOtkly8,2618
 cog/suppress_output.py,sha256=HHSNGR9j4rkyLL4mGnkluxzSQAYYIUcEWGdNCtYfwZc,645
-cog/types.py,sha256=p_OZM3d0Fg8Urz2xUr8jAjgq3VBPtvnGGYi3S8IeQJA,8562
+cog/types.py,sha256=ahiHjlp-7GIw72E70S91V7zfKtp6q3iIxZR0sHT5nlc,8590
 cog/command/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cog/command/ast_openapi_schema.py,sha256=sRI2tRRimErvmCeTnLCsDYrQ-V1yu_0LEcrHaXSBcWw,17318
 cog/command/openapi_schema.py,sha256=_gOGeACOBIm3mhztyc3d2R-5bWptvWGST_7IhzU8gWg,761
 cog/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cog/server/eventtypes.py,sha256=s2iJKjiXFG_cRIS_a4VQE_wVQosoyppRqTJfevBD_XI,593
 cog/server/exceptions.py,sha256=HknokO6g7gIlbIAMBM8685gE4Xgb8lykC-gTF6SLEYM,149
 cog/server/helpers.py,sha256=Z0mRZJOonbqc7Kir3JiGSbg-0svmtJCVpp3IaET3MlM,5349
 cog/server/http.py,sha256=s4yDvxVsbd2AGyn_vqR7i419SafXi4D1-WCzPnrHxkk,12055
 cog/server/probes.py,sha256=LxdHFrRCVbEimbuCHRCcDxLa97_7cSadacd0tj9Jhj4,957
@@ -21,19 +22,19 @@
 cog/server/runner.py,sha256=XomJNS4biXNKLQ4pWCa4RBjfsMav6TrcfA7b8HsK8Wo,14284
 cog/server/webhook.py,sha256=HVtuNG9KtQVqV9zC7dZPnH7tru-UKVXZsIBUDuxZviY,3092
 cog/server/worker.py,sha256=zrJ-xlUNOYTm_ROC9xmymFnxdBS5LtLITPyaBrE07zc,7970
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=KbeqWWshZoqqT6aLcZGB3_zLMe1G0IQ61BhoKQU1Xro,536
 tests/test_json.py,sha256=IvDxu8sjt5Ys4JeG8EQf2DfMujMXIt4NtwhBTg-Nke0,1733
 tests/test_predictor.py,sha256=pFBY6ON155CZN8FLEU2TbH7fN1FxWOP6eiZkTYVOz8c,486
-tests/test_types.py,sha256=MQvB34i9NJLzOgnErjwHpt_sFA0erbYdzLFKCG1e-yA,4690
+tests/test_types.py,sha256=Okt_mbTcsVQapR5su0CIQEhMV-5xuFpXjzxKldFgR_Q,4689
 tests/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/server/conftest.py,sha256=ZY5aihB1C2ckRDv8hWxtqQMJYNSEZzl9APL0seMIMTc,2056
+tests/server/conftest.py,sha256=68Lhj-gHGNsOyvgJioVqPP0XvgrJVBILHSWO-D-LNaI,2312
 tests/server/test_helpers.py,sha256=XVpcv42AYwUmo1wAoR73FMdN4tOoRYkqaTjduKE_aDA,4692
-tests/server/test_http.py,sha256=0TbZmCs4Dkkjp7wImuZoDOukAsZTCdn3AYTeZ-M4vLE,15179
+tests/server/test_http.py,sha256=fO4pGWaBmppXXYtvOGxKa91Y_j75hsEf5xWvuLL6n78,15623
 tests/server/test_http_input.py,sha256=uYrQfOvRyuj6ySKaR86VWhQXgUFx-9a0HzYC7pxfQpk,6957
 tests/server/test_http_output.py,sha256=AViMdeDEoSNfNtkftmtvyYG2A4DCP0ViGrmnZjYXuy4,4020
 tests/server/test_probes.py,sha256=L1ncJKDELevnxFq_Nr4hiZtNrLhkbClzbvAIGJ-RTzA,1334
 tests/server/test_response_throttler.py,sha256=5Dfslni4ioDrNbMJ2xNt-3La4K1SBm6LlV1UTosTlbg,1210
 tests/server/test_runner.py,sha256=cKx4jaDZMWhfHZBL6aF9o3dGE1dv5auyp4f4LwJW5r0,10943
 tests/server/test_webhook.py,sha256=gt8XfJ-gizqKd__K2sCKTNkWJ1iYm29h1YDIYxxJo3Y,3225
 tests/server/test_worker.py,sha256=lBc_XHm29vz20qZGAuPPsc7iaqh2pegkJf4ej_CZCJw,16095
@@ -86,12 +87,12 @@
 tests/server/fixtures/sleep.py,sha256=68T_2NweSlVsV-yhSgSyYNJxjfU1u-3KZZhZ06HMidw,193
 tests/server/fixtures/slow_predict.py,sha256=-jVSMLD_IRQY56Yf9XvTLXtLMNH5uGihcZkamH0wPLQ,219
 tests/server/fixtures/steps.py,sha256=WbD27CUVQE8Zj_SVOtOqtleG3Y8meSJVAn-vkhpKst8,290
 tests/server/fixtures/yield_concatenate_iterator.py,sha256=2X582IGdiprIALwIs5e-EZO4i1eBUdM7CI4FCPf-CAo,263
 tests/server/fixtures/yield_files.py,sha256=QpIl1SOFsaakNZJlShl_XkjBGyB_MyuQgv5-J2Vm75U,506
 tests/server/fixtures/yield_strings.py,sha256=7Y9cTGZ7WE0iKlr-ZQmhkeg30mXt-fEpY9U0AQ0QMAQ,245
 tests/server/fixtures/yield_strings_file_input.py,sha256=rNxZHFXLhzqkNiG35JfcyihSA4Lx6s3bp86YRGPztX8,339
-cog-0.8.5.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
-cog-0.8.5.dist-info/METADATA,sha256=UBOKkZ47LqqPTbd8HDgqMshECxL1M3Hgy9jtCLL7XjA,35131
-cog-0.8.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-cog-0.8.5.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
-cog-0.8.5.dist-info/RECORD,,
+cog-0.8.6.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
+cog-0.8.6.dist-info/METADATA,sha256=5lsx-HJqGlZty-P03kKEhN2ZZ4ZpFC-Vju7SGW_kUGE,35113
+cog-0.8.6.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+cog-0.8.6.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
+cog-0.8.6.dist-info/RECORD,,
```

