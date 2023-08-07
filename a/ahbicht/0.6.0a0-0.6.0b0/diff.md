# Comparing `tmp/ahbicht-0.6.0a0.tar.gz` & `tmp/ahbicht-0.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahbicht-0.6.0a0.tar", last modified: Mon Jan 16 09:49:52 2023, max compression
+gzip compressed data, was "ahbicht-0.6.0b0.tar", last modified: Mon Jan 16 12:27:23 2023, max compression
```

## Comparing `ahbicht-0.6.0a0.tar` & `ahbicht-0.6.0b0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.840021 ahbicht-0.6.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.824020 ahbicht-0.6.0a0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.824020 ahbicht-0.6.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/json_schemas.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/typescript_from_json_schemas.yml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-01-16 09:49:52.840021 ahbicht-0.6.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54198 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/definition-of-terms.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.824020 ahbicht-0.6.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.828020 ahbicht-0.6.0a0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/_static/ahbicht-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)  2076200 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/_static/ahbicht-logo-raw.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/_static/ahbicht-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/_static/ahbicht-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)  2025509 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/_static/ahbicht_uml.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/_static/wim_ahb_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.828020 ahbicht-0.6.0a0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/api/ahbicht.content_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/api/ahbicht.expressions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/api/ahbicht.json_serialization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/api/ahbicht.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/api/ahbicht.validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.832020 ahbicht-0.6.0a0/json_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/AhbExpressionEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/CategorizedKeyExtractSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/ConditionKeyConditionTextMappingSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/ContentEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/EvaluatedFormatConstraintSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/FormatConstraintEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/PackageKeyConditionExpressionMappingSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/RequirementConstraintEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/TokenSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/json_schemas/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/minimal_working_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-16 09:49:52.840021 ahbicht-0.6.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.820020 ahbicht-0.6.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.832020 ahbicht-0.6.0a0/src/ahbicht/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/condition_node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/condition_node_distinction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.832020 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)   136061 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/EvaluatingConditions.png
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/categorized_key_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/content_evaluation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/evaluationdatatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/evaluator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/fc_evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/rc_evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/content_evaluation/token_logic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/evaluation_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.836020 ahbicht-0.6.0a0/src/ahbicht/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/ahb_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/ahb_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/condition_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/condition_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)   171830 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/expression_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/expression_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/format_constraint_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/hints_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/package_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.836020 ahbicht-0.6.0a0/src/ahbicht/json_serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/json_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/json_serialization/concise_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/json_serialization/tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/mapping_results.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.836020 ahbicht-0.6.0a0/src/ahbicht/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22516 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/validation/validation_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/src/ahbicht/validation/validation_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.832020 ahbicht-0.6.0a0/src/ahbicht.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-01-16 09:49:52.000000 ahbicht-0.6.0a0/src/ahbicht.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-01-16 09:49:52.000000 ahbicht-0.6.0a0/src/ahbicht.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 09:49:52.000000 ahbicht-0.6.0a0/src/ahbicht.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 09:49:52.000000 ahbicht-0.6.0a0/src/ahbicht.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-16 09:49:52.000000 ahbicht-0.6.0a0/src/ahbicht.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-16 09:49:52.000000 ahbicht-0.6.0a0/src/ahbicht.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.840021 ahbicht-0.6.0a0/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.840021 ahbicht-0.6.0a0/unittests/content_evaluation_result_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/content_evaluation_result_generation/example0.json
--rw-r--r--   0 runner    (1001) docker     (123)    42249 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/content_evaluation_result_generation/example1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 09:49:52.840021 ahbicht-0.6.0a0/unittests/provider_test_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/provider_test_files/example_hints_file.json
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/provider_test_files/example_package_mapping_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/provider_test_files/example_package_mapping_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_ahb_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_ahb_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_categorized_key_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_cer_based_fc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_cer_based_hints_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_cer_based_package_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_cer_based_rc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_condition_node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_condition_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_condition_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_dict_based_fc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_dict_based_rc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_evaluator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_evaluator_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_expression_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_expression_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_format_constraint_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_format_constraints_context_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_hints_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_integration_mwe.py
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_json_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_mixed_sync_async_rc_fc_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_package_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_requirement_constraint_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_requirement_constraint_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_time_condition_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_tree_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    47895 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_validation_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_validity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-16 09:49:41.000000 ahbicht-0.6.0a0/unittests/test_warning_when_using_inject_attr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/json_schemas.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/typescript_from_json_schemas.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54198 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/definition-of-terms.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.291481 ahbicht-0.6.0b0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2076200 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-logo-raw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  2025509 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht_uml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/wim_ahb_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.content_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.expressions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.json_serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.validation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/json_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/AhbExpressionEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/CategorizedKeyExtractSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/ConditionKeyConditionTextMappingSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/ContentEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/EvaluatedFormatConstraintSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/FormatConstraintEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/PackageKeyConditionExpressionMappingSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/RequirementConstraintEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/TokenSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/minimal_working_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/src/ahbicht/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/condition_node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/condition_node_distinction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)   136061 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/EvaluatingConditions.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/categorized_key_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/content_evaluation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluationdatatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/fc_evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/rc_evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/token_logic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/evaluation_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.299481 ahbicht-0.6.0b0/src/ahbicht/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/condition_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/condition_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171830 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/expression_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/expression_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/format_constraint_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/hints_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/package_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.299481 ahbicht-0.6.0b0/src/ahbicht/json_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/mapping_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.299481 ahbicht-0.6.0b0/src/ahbicht/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22516 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/validation_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/validation_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/src/ahbicht.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42249 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/unittests/provider_test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/provider_test_files/example_hints_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/provider_test_files/example_package_mapping_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/provider_test_files/example_package_mapping_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_ahb_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_ahb_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_categorized_key_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_fc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_hints_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_package_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_rc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_condition_node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_condition_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_condition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_dict_based_fc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_dict_based_rc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_evaluator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_evaluator_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_expression_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_expression_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_format_constraint_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_format_constraints_context_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_german_strom_and_gas_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_hints_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_integration_mwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_json_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_mixed_sync_async_rc_fc_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_package_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_requirement_constraint_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_requirement_constraint_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_time_condition_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_tree_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47895 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_validation_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_validity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_warning_when_using_inject_attr.py
```

### Comparing `ahbicht-0.6.0a0/.github/dependabot.yml` & `ahbicht-0.6.0b0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/codeql-analysis.yml` & `ahbicht-0.6.0b0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/coverage.yml` & `ahbicht-0.6.0b0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/docs.yml` & `ahbicht-0.6.0b0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/json_schemas.yml` & `ahbicht-0.6.0b0/.github/workflows/json_schemas.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/packaging_test.yml` & `ahbicht-0.6.0b0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/python-publish.yml` & `ahbicht-0.6.0b0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/pythonlint.yml` & `ahbicht-0.6.0b0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/typescript_from_json_schemas.yml` & `ahbicht-0.6.0b0/.github/workflows/typescript_from_json_schemas.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.github/workflows/unittests.yml` & `ahbicht-0.6.0b0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.gitignore` & `ahbicht-0.6.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.pre-commit-config.yaml` & `ahbicht-0.6.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/.readthedocs.yaml` & `ahbicht-0.6.0b0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/LICENSE` & `ahbicht-0.6.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/PKG-INFO` & `ahbicht-0.6.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahbicht
-Version: 0.6.0a0
+Version: 0.6.0b0
 Summary: Python Library to parse AHB expressions.
 Home-page: https://github.com/Hochfrequenz/ahbicht
 Author: Annika Schlögl
 Author-email: annika.schloegl@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://ahbicht.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/ahbicht/
```

### Comparing `ahbicht-0.6.0a0/README.rst` & `ahbicht-0.6.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/definition-of-terms.csv` & `ahbicht-0.6.0b0/definition-of-terms.csv`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/Makefile` & `ahbicht-0.6.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/_static/ahbicht-favicon.png` & `ahbicht-0.6.0b0/docs/_static/ahbicht-favicon.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/_static/ahbicht-logo-raw.svg` & `ahbicht-0.6.0b0/docs/_static/ahbicht-logo-raw.svg`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/_static/ahbicht-logo.png` & `ahbicht-0.6.0b0/docs/_static/ahbicht-logo.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/_static/ahbicht-logo.svg` & `ahbicht-0.6.0b0/docs/_static/ahbicht-logo.svg`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/_static/ahbicht_uml.svg` & `ahbicht-0.6.0b0/docs/_static/ahbicht_uml.svg`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/_static/wim_ahb_screenshot.png` & `ahbicht-0.6.0b0/docs/_static/wim_ahb_screenshot.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/api/ahbicht.content_evaluation.rst` & `ahbicht-0.6.0b0/docs/api/ahbicht.content_evaluation.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/api/ahbicht.expressions.rst` & `ahbicht-0.6.0b0/docs/api/ahbicht.expressions.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/api/ahbicht.json_serialization.rst` & `ahbicht-0.6.0b0/docs/api/ahbicht.json_serialization.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/api/ahbicht.rst` & `ahbicht-0.6.0b0/docs/api/ahbicht.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/api/ahbicht.validation.rst` & `ahbicht-0.6.0b0/docs/api/ahbicht.validation.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/conf.py` & `ahbicht-0.6.0b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/docs/make.bat` & `ahbicht-0.6.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/AhbExpressionEvaluationResultSchema.json` & `ahbicht-0.6.0b0/json_schemas/AhbExpressionEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/CategorizedKeyExtractSchema.json` & `ahbicht-0.6.0b0/json_schemas/CategorizedKeyExtractSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/ConditionKeyConditionTextMappingSchema.json` & `ahbicht-0.6.0b0/json_schemas/ConditionKeyConditionTextMappingSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/ContentEvaluationResultSchema.json` & `ahbicht-0.6.0b0/json_schemas/ContentEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/EvaluatedFormatConstraintSchema.json` & `ahbicht-0.6.0b0/json_schemas/EvaluatedFormatConstraintSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/FormatConstraintEvaluationResultSchema.json` & `ahbicht-0.6.0b0/json_schemas/FormatConstraintEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/PackageKeyConditionExpressionMappingSchema.json` & `ahbicht-0.6.0b0/json_schemas/PackageKeyConditionExpressionMappingSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/README.md` & `ahbicht-0.6.0b0/json_schemas/README.md`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/RequirementConstraintEvaluationResultSchema.json` & `ahbicht-0.6.0b0/json_schemas/RequirementConstraintEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/TokenSchema.json` & `ahbicht-0.6.0b0/json_schemas/TokenSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/json_schemas/generate_json_schemas.py` & `ahbicht-0.6.0b0/json_schemas/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/minimal_working_example.ipynb` & `ahbicht-0.6.0b0/minimal_working_example.ipynb`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/pyproject.toml` & `ahbicht-0.6.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/requirements.txt` & `ahbicht-0.6.0b0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/setup.cfg` & `ahbicht-0.6.0b0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 python_requires = >=3.8
 install_requires = 
 	attrs>=21.4.0
 	lark>=1.1.4
 	inject
 	marshmallow
 	marshmallow_enum
-	maus>=0.1.24
+	maus>=0.3.1a
 	pytz
 
 [options.packages.find]
 where = src
 exclude = 
 	unittests
```

### Comparing `ahbicht-0.6.0a0/src/ahbicht/__init__.py` & `ahbicht-0.6.0b0/src/ahbicht/__init__.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/condition_node_builder.py` & `ahbicht-0.6.0b0/src/ahbicht/condition_node_builder.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/condition_node_distinction.py` & `ahbicht-0.6.0b0/src/ahbicht/condition_node_distinction.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/EvaluatingConditions.png` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/EvaluatingConditions.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/__init__.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/categorized_key_extract.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/categorized_key_extract.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/content_evaluation_result.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/content_evaluation_result.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/evaluationdatatypes.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluationdatatypes.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/evaluator_factory.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluator_factory.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/evaluators.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluators.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/fc_evaluators.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/fc_evaluators.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/rc_evaluators.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/rc_evaluators.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/content_evaluation/token_logic_provider.py` & `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/token_logic_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/evaluation_results.py` & `ahbicht-0.6.0b0/src/ahbicht/evaluation_results.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/__init__.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/ahb_expression_evaluation.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/ahb_expression_parser.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/base_transformer.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/base_transformer.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/condition_expression_parser.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/condition_expression_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/condition_nodes.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/condition_nodes.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png` & `ahbicht-0.6.0b0/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/enums.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/enums.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/expression_builder.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/expression_builder.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/expression_resolver.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/expression_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/format_constraint_expression_evaluation.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/format_constraint_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/hints_provider.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/hints_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/package_expansion.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/package_expansion.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py` & `ahbicht-0.6.0b0/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py` & `ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/json_serialization/concise_tree_schema.py` & `ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_tree_schema.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/json_serialization/tree_schema.py` & `ahbicht-0.6.0b0/src/ahbicht/json_serialization/tree_schema.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/mapping_results.py` & `ahbicht-0.6.0b0/src/ahbicht/mapping_results.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/utility_functions.py` & `ahbicht-0.6.0b0/src/ahbicht/utility_functions.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/validation/validation.py` & `ahbicht-0.6.0b0/src/ahbicht/validation/validation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht/validation/validation_results.py` & `ahbicht-0.6.0b0/src/ahbicht/validation/validation_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,14 +221,28 @@
 
     def filter_for_boneycomb_path_results(self) -> None:
         """
         Filters the list of validation results for those that have a boneycomb path as discriminator
         """
         self.validation_results = list(filter(self._is_boneycomb_path_result, self.validation_results))
 
+    @staticmethod
+    def _is_not_absender_or_empfaenger_path_result(validation_result_in_context: ValidationResultInContext) -> bool:
+        return (
+            validation_result_in_context.discriminator is not None
+            and "absender" not in validation_result_in_context.discriminator
+            and "empfaenger" not in validation_result_in_context.discriminator
+        )
+
+    def remove_absender_and_empfaenger_path_results(self) -> None:
+        """
+        Removes all paths containing Absender oder Empfaenger
+        """
+        self.validation_results = list(filter(self._is_not_absender_or_empfaenger_path_result, self.validation_results))
+
 
 class ListOfValidationResultInContextSchema(Schema):
     """
     A schema to deserialize ListOfValidationResultInContext
     """
 
     validation_results = fields.List(fields.Nested(ValidationResultInContextSchema))
```

### Comparing `ahbicht-0.6.0a0/src/ahbicht/validation/validation_values.py` & `ahbicht-0.6.0b0/src/ahbicht/validation/validation_values.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/src/ahbicht.egg-info/PKG-INFO` & `ahbicht-0.6.0b0/src/ahbicht.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahbicht
-Version: 0.6.0a0
+Version: 0.6.0b0
 Summary: Python Library to parse AHB expressions.
 Home-page: https://github.com/Hochfrequenz/ahbicht
 Author: Annika Schlögl
 Author-email: annika.schloegl@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://ahbicht.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/ahbicht/
```

### Comparing `ahbicht-0.6.0a0/src/ahbicht.egg-info/SOURCES.txt` & `ahbicht-0.6.0b0/src/ahbicht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/tox.ini` & `ahbicht-0.6.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/conftest.py` & `ahbicht-0.6.0b0/unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/content_evaluation_result_generation/example0.json` & `ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example0.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/content_evaluation_result_generation/example1.json` & `ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example1.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/defaults.py` & `ahbicht-0.6.0b0/unittests/defaults.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/provider_test_files/example_hints_file.json` & `ahbicht-0.6.0b0/unittests/provider_test_files/example_hints_file.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_ahb_expression_evaluation.py` & `ahbicht-0.6.0b0/unittests/test_ahb_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_ahb_expression_parser.py` & `ahbicht-0.6.0b0/unittests/test_ahb_expression_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_caching.py` & `ahbicht-0.6.0b0/unittests/test_caching.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_categorized_key_extraction.py` & `ahbicht-0.6.0b0/unittests/test_categorized_key_extraction.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_cer_based_fc_evaluator.py` & `ahbicht-0.6.0b0/unittests/test_cer_based_fc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_cer_based_hints_provider.py` & `ahbicht-0.6.0b0/unittests/test_cer_based_hints_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_cer_based_package_resolver.py` & `ahbicht-0.6.0b0/unittests/test_cer_based_package_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_cer_based_rc_evaluator.py` & `ahbicht-0.6.0b0/unittests/test_cer_based_rc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_condition_node_builder.py` & `ahbicht-0.6.0b0/unittests/test_condition_node_builder.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_condition_nodes.py` & `ahbicht-0.6.0b0/unittests/test_condition_nodes.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_condition_parser.py` & `ahbicht-0.6.0b0/unittests/test_condition_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_dict_based_fc_evaluator.py` & `ahbicht-0.6.0b0/unittests/test_dict_based_fc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_dict_based_rc_evaluator.py` & `ahbicht-0.6.0b0/unittests/test_dict_based_rc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_evaluator_factory.py` & `ahbicht-0.6.0b0/unittests/test_evaluator_factory.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_evaluator_provider.py` & `ahbicht-0.6.0b0/unittests/test_evaluator_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_expression_builder.py` & `ahbicht-0.6.0b0/unittests/test_expression_builder.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_expression_resolver.py` & `ahbicht-0.6.0b0/unittests/test_expression_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_format_constraint_expression_evaluation.py` & `ahbicht-0.6.0b0/unittests/test_format_constraint_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_format_constraints_context_var.py` & `ahbicht-0.6.0b0/unittests/test_format_constraints_context_var.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_german_strom_and_gas_tag.py` & `ahbicht-0.6.0b0/unittests/test_german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_hints_provider.py` & `ahbicht-0.6.0b0/unittests/test_hints_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_integration_mwe.py` & `ahbicht-0.6.0b0/unittests/test_integration_mwe.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_json_serialization.py` & `ahbicht-0.6.0b0/unittests/test_json_serialization.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_mixed_sync_async_rc_fc_evaluation.py` & `ahbicht-0.6.0b0/unittests/test_mixed_sync_async_rc_fc_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_package_resolver.py` & `ahbicht-0.6.0b0/unittests/test_package_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_requirement_constraint_evaluation.py` & `ahbicht-0.6.0b0/unittests/test_requirement_constraint_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_requirement_constraint_expression_evaluation.py` & `ahbicht-0.6.0b0/unittests/test_requirement_constraint_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_time_condition_resolver.py` & `ahbicht-0.6.0b0/unittests/test_time_condition_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_tree_schemas.py` & `ahbicht-0.6.0b0/unittests/test_tree_schemas.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_utility_functions.py` & `ahbicht-0.6.0b0/unittests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_validation.py` & `ahbicht-0.6.0b0/unittests/test_validation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_validity_check.py` & `ahbicht-0.6.0b0/unittests/test_validity_check.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0a0/unittests/test_warning_when_using_inject_attr.py` & `ahbicht-0.6.0b0/unittests/test_warning_when_using_inject_attr.py`

 * *Files identical despite different names*

