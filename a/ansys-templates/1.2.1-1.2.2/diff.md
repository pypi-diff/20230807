# Comparing `tmp/ansys_templates-1.2.1.tar.gz` & `tmp/ansys_templates-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_templates-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_templates-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_templates-1.2.1.tar` & `ansys_templates-1.2.2.tar`

### file list

```diff
@@ -1,276 +1,276 @@
--rw-r--r--   0        0        0     1091 2023-07-24 09:35:43.373373 ansys_templates-1.2.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9947 2023-07-24 09:35:43.373373 ansys_templates-1.2.1/README.rst
--rw-r--r--   0        0        0     3122 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2266 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     3803 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3894 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      418 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3713 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2779 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      764 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      379 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
--rw-r--r--   0        0        0       11 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      105 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
--rw-r--r--   0        0        0      282 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0     1026 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      969 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       63 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rwxr-xr-x   0        0        0     4076 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3414 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       27 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       81 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2377 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1087 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2046 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3238 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1187 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      825 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1434 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/cookiecutter.json
--rw-r--r--   0        0        0     7431 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      175 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2147 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2944 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      199 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
--rw-r--r--   0        0        0     3897 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    38166 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      421 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       50 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0     3919 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py
--rw-r--r--   0        0        0       47 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      959 2023-07-24 09:35:43.377373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
--rw-r--r--   0        0        0      725 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      248 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
--rw-r--r--   0        0        0    14653 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
--rw-r--r--   0        0        0      922 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       41 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0     9913 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0     2579 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
--rw-r--r--   0        0        0     3687 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
--rw-r--r--   0        0        0     3177 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
--rw-r--r--   0        0        0     5284 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
--rw-r--r--   0        0        0     1837 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
--rw-r--r--   0        0        0     2482 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
--rw-r--r--   0        0        0     5649 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
--rw-r--r--   0        0        0     1753 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
--rw-r--r--   0        0        0     4962 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
--rw-r--r--   0        0        0     7522 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0    15892 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
--rw-r--r--   0        0        0     3165 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
--rw-r--r--   0        0        0     3676 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
--rw-r--r--   0        0        0      960 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
--rw-r--r--   0        0        0     3626 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
--rw-r--r--   0        0        0      618 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
--rw-r--r--   0        0        0      983 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
--rw-r--r--   0        0        0     1372 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
--rw-r--r--   0        0        0      296 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
--rw-r--r--   0        0        0      714 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
--rw-r--r--   0        0        0      660 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
--rw-r--r--   0        0        0      793 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
--rw-r--r--   0        0        0      574 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
--rw-r--r--   0        0        0       20 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2941 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      800 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      111 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3108 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      763 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       58 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      104 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3093 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      951 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       44 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      116 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2869 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      860 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-07-24 09:35:43.381373 ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1148 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3398 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2657 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6537 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1048 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1857 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1073 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3170 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1063 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     3319 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      175 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1710 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2739 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1567 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
--rw-r--r--   0        0        0      655 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3557 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    38166 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      583 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       52 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       51 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0       52 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      803 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      570 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0      274 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
--rw-r--r--   0        0        0      263 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      922 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       18 2023-07-24 09:35:43.385373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0   749872 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
--rw-r--r--   0        0        0     9913 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0       18 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
--rw-r--r--   0        0        0     3490 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
--rw-r--r--   0        0        0     4700 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
--rw-r--r--   0        0        0     5244 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0      593 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
--rw-r--r--   0        0        0       20 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     6698 2023-07-24 09:35:43.389373 ansys_templates-1.2.1/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    11425 1970-01-01 00:00:00.000000 ansys_templates-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-08-07 09:52:52.262883 ansys_templates-1.2.2/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     9680 2023-08-07 09:52:52.262883 ansys_templates-1.2.2/README.rst
+-rw-r--r--   0        0        0     3128 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2266 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3803 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3894 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3713 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      379 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
+-rw-r--r--   0        0        0       11 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      105 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      282 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4076 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1434 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/cookiecutter.json
+-rw-r--r--   0        0        0     7431 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      175 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2147 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2944 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      199 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
+-rw-r--r--   0        0        0     3897 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      421 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       50 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0     3919 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py
+-rw-r--r--   0        0        0       47 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      959 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
+-rw-r--r--   0        0        0      725 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      248 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
+-rw-r--r--   0        0        0    14653 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
+-rw-r--r--   0        0        0      922 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       41 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0     9913 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0     2579 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
+-rw-r--r--   0        0        0     3687 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
+-rw-r--r--   0        0        0     3177 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
+-rw-r--r--   0        0        0     5284 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
+-rw-r--r--   0        0        0     1837 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
+-rw-r--r--   0        0        0     2482 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
+-rw-r--r--   0        0        0     5649 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
+-rw-r--r--   0        0        0     1753 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
+-rw-r--r--   0        0        0     4962 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
+-rw-r--r--   0        0        0     7522 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0    15892 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
+-rw-r--r--   0        0        0     3165 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
+-rw-r--r--   0        0        0     3676 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
+-rw-r--r--   0        0        0      960 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
+-rw-r--r--   0        0        0     3626 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
+-rw-r--r--   0        0        0      618 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
+-rw-r--r--   0        0        0      983 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
+-rw-r--r--   0        0        0     1372 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
+-rw-r--r--   0        0        0      296 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
+-rw-r--r--   0        0        0      714 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
+-rw-r--r--   0        0        0      660 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
+-rw-r--r--   0        0        0      793 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
+-rw-r--r--   0        0        0      574 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
+-rw-r--r--   0        0        0       20 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2941 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3108 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3093 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2869 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1148 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2657 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1048 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1073 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1063 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     3319 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      175 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1710 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2739 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1567 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
+-rw-r--r--   0        0        0      655 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3557 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       51 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       52 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      922 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       18 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0   749872 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
+-rw-r--r--   0        0        0     9913 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0       18 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
+-rw-r--r--   0        0        0     3490 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
+-rw-r--r--   0        0        0     4700 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
+-rw-r--r--   0        0        0     5244 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0      593 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
+-rw-r--r--   0        0        0       20 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11164 1970-01-01 00:00:00.000000 ansys_templates-1.2.2/PKG-INFO
```

### Comparing `ansys_templates-1.2.1/LICENSES/MIT.txt` & `ansys_templates-1.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/README.rst` & `ansys_templates-1.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,14 @@
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. |implemented| image:: <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24"><path d="M21.03 5.72a.75.75 0 0 1 0 1.06l-11.5 11.5a.747.747 0 0 1-1.072-.012l-5.5-5.75a.75.75 0 1 1 1.084-1.036l4.97 5.195L19.97 5.72a.75.75 0 0 1 1.06 0Z"></path></svg>
-
 
 The ``ansys-templates`` repository holds a collection of useful templates compliant
 with PyAnsys guidelines. It also provides the ``ansys-templates`` command line tool
 for interactively generating new projects based on previous templates.
 
 The main advantages of using this tool are:
 
@@ -82,15 +80,15 @@
 
     python -m pip install ansys-templates
 
 The usage of `pipx`_ is encouraged too. See `installing ansys-templates using
 pipx`_.
 
 .. _pipx: https://pypa.github.io/pipx/
-.. _installing ansys-templates using pipx: https://templates.pyansys.com/getting_started/index.html#installing-pipx
+.. _installing ansys-templates using pipx: https://templates.ansys.com/version/stable/getting_started/index.html#installing-pipx
 
 
 Basic commands
 --------------
 The following commands are provided with ``ansys-templates``:
 
 - ``ansys-templates --help``: lists information about the tool.
```

### Comparing `ansys_templates-1.2.1/pyproject.toml` & `ansys_templates-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-templates"
-version = "1.2.1"
+version = "1.2.2"
 description = "Creates Python projects according to PyAnsys guidelines"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSES/MIT.txt"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -48,25 +48,25 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "importlib-metadata >=4.0",
     "click>=7.0,<9.0.0",
-    "cookiecutter>=2.1.0",
+    "cookiecutter>=2.1.0,<2.3.0",
     "isort>=5.10.1",
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.4.0",
     "pytest-cov==4.1.0",
 ]
 doc = [
-    "ansys-sphinx-theme==0.9.9",
+    "ansys-sphinx-theme==0.10",
     "numpydoc==1.5.0",
     "sphinx==7.0.1",
     "sphinx-copybutton==0.5.2",
 ]
 
 [tool.flit.module]
 name = "ansys.templates"
```

### Comparing `ansys_templates-1.2.1/src/ansys/templates/__init__.py` & `ansys_templates-1.2.2/src/ansys/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/__main__.py` & `ansys_templates-1.2.2/src/ansys/templates/__main__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/cli.py` & `ansys_templates-1.2.2/src/ansys/templates/cli.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/licenses/LICENSE_MIT` & `ansys_templates-1.2.2/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/paths.py` & `ansys_templates-1.2.2/src/ansys/templates/paths.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/cookiecutter.json` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/hooks/post_gen_project.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/testing.py` & `ansys_templates-1.2.2/src/ansys/templates/testing.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/src/ansys/templates/utils.py` & `ansys_templates-1.2.2/src/ansys/templates/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.1/PKG-INFO` & `ansys_templates-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 1.2.1
+Version: 1.2.2
 Summary: Creates Python projects according to PyAnsys guidelines
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
 Requires-Dist: click>=7.0,<9.0.0
-Requires-Dist: cookiecutter>=2.1.0
+Requires-Dist: cookiecutter>=2.1.0,<2.3.0
 Requires-Dist: isort>=5.10.1
-Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.10 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Project-URL: Documentation, https://templates.ansys.com/
 Project-URL: Homepage, https://templates.ansys.com/
@@ -82,16 +82,14 @@
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. |implemented| image:: <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24"><path d="M21.03 5.72a.75.75 0 0 1 0 1.06l-11.5 11.5a.747.747 0 0 1-1.072-.012l-5.5-5.75a.75.75 0 1 1 1.084-1.036l4.97 5.195L19.97 5.72a.75.75 0 0 1 1.06 0Z"></path></svg>
-
 
 The ``ansys-templates`` repository holds a collection of useful templates compliant
 with PyAnsys guidelines. It also provides the ``ansys-templates`` command line tool
 for interactively generating new projects based on previous templates.
 
 The main advantages of using this tool are:
 
@@ -116,15 +114,15 @@
 
     python -m pip install ansys-templates
 
 The usage of `pipx`_ is encouraged too. See `installing ansys-templates using
 pipx`_.
 
 .. _pipx: https://pypa.github.io/pipx/
-.. _installing ansys-templates using pipx: https://templates.pyansys.com/getting_started/index.html#installing-pipx
+.. _installing ansys-templates using pipx: https://templates.ansys.com/version/stable/getting_started/index.html#installing-pipx
 
 
 Basic commands
 --------------
 The following commands are provided with ``ansys-templates``:
 
 - ``ansys-templates --help``: lists information about the tool.
```

