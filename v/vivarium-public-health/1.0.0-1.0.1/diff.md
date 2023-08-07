# Comparing `tmp/vivarium_public_health-1.0.0.tar.gz` & `tmp/vivarium_public_health-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium_public_health-1.0.0.tar", last modified: Wed Aug  2 21:41:03 2023, max compression
+gzip compressed data, was "vivarium_public_health-1.0.1.tar", last modified: Mon Aug  7 19:28:10 2023, max compression
```

## Comparing `vivarium_public_health-1.0.0.tar` & `vivarium_public_health-1.0.1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/api_reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/api_reference/disease/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/special_disease.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/state.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/transition.rst
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/disability.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/disease.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/mortality.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/risk.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/stratification.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/delay.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/disease.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/intervention.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/magic_wand_components.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/observer.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/population.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/population/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/add_new_birth_cohorts.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/base_population.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/data_transformations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/mortality.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/risks/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/base_risk.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/data_transformations.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/distributions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/effect.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/risks/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/implementations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/implementations/low_birth_weight_and_short_gestation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/testing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/testing/mock_artifact.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/testing/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/magic_wand.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/scale_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/therapeutic_inertia.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/tutorials/risk_exposure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.766962 vivarium_public_health-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/src/vivarium_public_health/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14156 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/special_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/transition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.782962 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/disability.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/disease.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/mortality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/stratification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.782962 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/disease.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/magic_wand_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/population.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.782962 vivarium_public_health-1.0.0/src/vivarium_public_health/population/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/add_new_birth_cohorts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/base_population.py
--rw-r--r--   0 runner    (1001) docker     (123)    21804 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/data_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/mortality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/base_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/data_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/effect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/implementations/low_birth_weight_and_short_gestation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/mock_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/magic_wand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/scale_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/therapeutic_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/tests/disease/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/disease/test_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/disease/test_special_disease.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.790962 vivarium_public_health-1.0.0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_categorical_risk_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_disability.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_disability_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_disease_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_mortality_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_stratification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.794962 vivarium_public_health-1.0.0/tests/population/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/test_add_new_birth_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/test_base_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/test_data_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/tests/risks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_base_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_data_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20333 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/tests/treatment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/treatment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.822623 vivarium_public_health-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-07 19:28:10.822623 vivarium_public_health-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/docs/source/api_reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/disease/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/disease/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/disease/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/disease/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/disease/special_disease.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/disease/state.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/disease/transition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/metrics/disability.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/metrics/disease.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/metrics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/metrics/mortality.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/metrics/risk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/metrics/stratification.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/delay.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/disease.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/intervention.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/magic_wand_components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/observer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/mslt/population.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/population/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/population/add_new_birth_cohorts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/population/base_population.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/population/data_transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/population/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/population/mortality.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/risks/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/risks/base_risk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/risks/data_transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/risks/distributions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/risks/effect.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/risks/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/risks/implementations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/risks/implementations/low_birth_weight_and_short_gestation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/risks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/testing/mock_artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/testing/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/api_reference/treatment/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/treatment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/treatment/magic_wand.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/treatment/scale_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/treatment/therapeutic_inertia.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/api_reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/docs/source/tutorials/risk_exposure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:28:10.822623 vivarium_public_health-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.810623 vivarium_public_health-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/src/vivarium_public_health/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 19:28:10.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/disease/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/disease/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/disease/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14156 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/disease/special_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19738 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/disease/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/disease/transition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/disability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/mortality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/stratification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/magic_wand_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/population/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/population/add_new_birth_cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/population/base_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21804 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/population/data_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/population/mortality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/base_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/data_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/effect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/risks/implementations/low_birth_weight_and_short_gestation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/testing/mock_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/magic_wand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/scale_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/therapeutic_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/src/vivarium_public_health/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.814623 vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-07 19:28:10.000000 vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-08-07 19:28:10.000000 vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:28:10.000000 vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:28:10.000000 vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 19:28:10.000000 vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 19:28:10.000000 vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/tests/disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/disease/test_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/disease/test_special_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.818623 vivarium_public_health-1.0.1/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/metrics/test_categorical_risk_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/metrics/test_disability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/metrics/test_disability_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/metrics/test_disease_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/metrics/test_mortality_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/metrics/test_stratification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.822623 vivarium_public_health-1.0.1/tests/population/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/population/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/population/test_add_new_birth_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/population/test_base_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/population/test_data_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.822623 vivarium_public_health-1.0.1/tests/risks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/risks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/risks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/risks/test_base_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/risks/test_data_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/risks/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20333 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/risks/test_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:10.822623 vivarium_public_health-1.0.1/tests/treatment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tests/treatment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-07 19:27:59.000000 vivarium_public_health-1.0.1/tox.ini
```

### Comparing `vivarium_public_health-1.0.0/.github/pull_request_template.md` & `vivarium_public_health-1.0.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/.github/workflows/build.yml` & `vivarium_public_health-1.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/.github/workflows/deploy.yml` & `vivarium_public_health-1.0.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/.gitignore` & `vivarium_public_health-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/.zenodo.json` & `vivarium_public_health-1.0.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/CHANGELOG.rst` & `vivarium_public_health-1.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**1.0.1 - 08/07/23**
+
+- Minor bugfix to improve handling of excess mortality rate data
+
 **1.0.0 - 08/02/23**
 
  - Performance and architectural improvements to results manager, including observers
  - Updates versioning to use setuptools_scm
  - Other bugfixes
 
 **0.11.0 - 06/01/23**
```

### Comparing `vivarium_public_health-1.0.0/CODE_OF_CONDUCT.rst` & `vivarium_public_health-1.0.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/CONTRIBUTING.rst` & `vivarium_public_health-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/LICENSE.txt` & `vivarium_public_health-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/PKG-INFO` & `vivarium_public_health-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium_public_health
-Version: 1.0.0
+Version: 1.0.1
 Summary: Components for modelling diseases, risks, and interventions with ``vivarium``
 Home-page: https://github.com/ihmeuw/vivarium_public_health
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `vivarium_public_health-1.0.0/README.rst` & `vivarium_public_health-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/docs/Makefile` & `vivarium_public_health-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/docs/source/conf.py` & `vivarium_public_health-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/docs/source/tutorials/risk_exposure.rst` & `vivarium_public_health-1.0.1/docs/source/tutorials/risk_exposure.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/setup.py` & `vivarium_public_health-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/disease/model.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/disease/model.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/disease/models.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/disease/models.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/disease/special_disease.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/disease/special_disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/disease/state.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/disease/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,18 +495,17 @@
 
         if isinstance(disability_weight, pd.DataFrame) and len(disability_weight) == 1:
             disability_weight = disability_weight.value[0]  # sequela only have single value
 
         return disability_weight
 
     def load_excess_mortality_rate_data(self, builder):
-        only_morbid = builder.data.load(f"cause.{self._model}.restrictions")["yld_only"]
         if "excess_mortality_rate" in self._get_data_functions:
             return self._get_data_functions["excess_mortality_rate"](builder, self.cause)
-        elif only_morbid:
+        elif builder.data.load(f"cause.{self._model}.restrictions")["yld_only"]:
             return 0
         else:
             return builder.data.load(f"{self.cause_type}.{self.cause}.excess_mortality_rate")
 
     def __repr__(self):
         return "DiseaseState({})".format(self.state_id)
```

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/disease/transition.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/disease/transition.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/disability.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/disability.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/disease.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/mortality.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/mortality.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/risk.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/risk.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/stratification.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/metrics/stratification.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/delay.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/delay.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/disease.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/intervention.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/intervention.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/magic_wand_components.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/magic_wand_components.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/observer.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/observer.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/population.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/mslt/population.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/population/add_new_birth_cohorts.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/population/add_new_birth_cohorts.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/population/base_population.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/population/base_population.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/population/data_transformations.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/population/data_transformations.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/population/mortality.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/population/mortality.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/base_risk.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/risks/base_risk.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/data_transformations.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/risks/data_transformations.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/distributions.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/risks/distributions.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/effect.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/risks/effect.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/implementations/low_birth_weight_and_short_gestation.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/risks/implementations/low_birth_weight_and_short_gestation.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/testing/mock_artifact.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/testing/mock_artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/testing/utils.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/testing/utils.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/magic_wand.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/magic_wand.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/scale_up.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/scale_up.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/therapeutic_inertia.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/treatment/therapeutic_inertia.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health/utilities.py` & `vivarium_public_health-1.0.1/src/vivarium_public_health/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/PKG-INFO` & `vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-public-health
-Version: 1.0.0
+Version: 1.0.1
 Summary: Components for modelling diseases, risks, and interventions with ``vivarium``
 Home-page: https://github.com/ihmeuw/vivarium_public_health
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/SOURCES.txt` & `vivarium_public_health-1.0.1/src/vivarium_public_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/conftest.py` & `vivarium_public_health-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/disease/test_disease.py` & `vivarium_public_health-1.0.1/tests/disease/test_disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/disease/test_special_disease.py` & `vivarium_public_health-1.0.1/tests/disease/test_special_disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/metrics/test_categorical_risk_observer.py` & `vivarium_public_health-1.0.1/tests/metrics/test_categorical_risk_observer.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/metrics/test_disability.py` & `vivarium_public_health-1.0.1/tests/metrics/test_disability.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/metrics/test_disability_observer.py` & `vivarium_public_health-1.0.1/tests/metrics/test_disability_observer.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/metrics/test_disease_observer.py` & `vivarium_public_health-1.0.1/tests/metrics/test_disease_observer.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/metrics/test_mortality_observer.py` & `vivarium_public_health-1.0.1/tests/metrics/test_mortality_observer.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/metrics/test_stratification.py` & `vivarium_public_health-1.0.1/tests/metrics/test_stratification.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/population/test_add_new_birth_cohort.py` & `vivarium_public_health-1.0.1/tests/population/test_add_new_birth_cohort.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/population/test_base_population.py` & `vivarium_public_health-1.0.1/tests/population/test_base_population.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/population/test_data_transformations.py` & `vivarium_public_health-1.0.1/tests/population/test_data_transformations.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/risks/conftest.py` & `vivarium_public_health-1.0.1/tests/risks/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/risks/test_base_risk.py` & `vivarium_public_health-1.0.1/tests/risks/test_base_risk.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/risks/test_data_transformations.py` & `vivarium_public_health-1.0.1/tests/risks/test_data_transformations.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/risks/test_distributions.py` & `vivarium_public_health-1.0.1/tests/risks/test_distributions.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/risks/test_effect.py` & `vivarium_public_health-1.0.1/tests/risks/test_effect.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-1.0.0/tests/test_utilities.py` & `vivarium_public_health-1.0.1/tests/test_utilities.py`

 * *Files identical despite different names*

