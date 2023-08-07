# Comparing `tmp/ansys_templates-1.2.2.tar.gz` & `tmp/ansys_templates-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_templates-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_templates-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_templates-1.2.2.tar` & `ansys_templates-1.3.0.tar`

### file list

```diff
@@ -1,276 +1,286 @@
--rw-r--r--   0        0        0     1091 2023-08-07 09:52:52.262883 ansys_templates-1.2.2/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9680 2023-08-07 09:52:52.262883 ansys_templates-1.2.2/README.rst
--rw-r--r--   0        0        0     3128 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2266 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     3803 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3894 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      418 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3713 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2779 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      764 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      379 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
--rw-r--r--   0        0        0       11 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      105 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
--rw-r--r--   0        0        0      282 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0     1026 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      969 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       63 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rwxr-xr-x   0        0        0     4076 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3414 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       27 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       81 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2377 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1087 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2046 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3238 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1187 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      825 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1434 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/cookiecutter.json
--rw-r--r--   0        0        0     7431 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      175 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2147 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2944 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-08-07 09:52:52.266883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      199 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
--rw-r--r--   0        0        0     3897 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    38166 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      421 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       50 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0     3919 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py
--rw-r--r--   0        0        0       47 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      959 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
--rw-r--r--   0        0        0      725 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      248 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
--rw-r--r--   0        0        0    14653 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
--rw-r--r--   0        0        0      922 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       41 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0     9913 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0     2579 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
--rw-r--r--   0        0        0     3687 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
--rw-r--r--   0        0        0     3177 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
--rw-r--r--   0        0        0     5284 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
--rw-r--r--   0        0        0     1837 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
--rw-r--r--   0        0        0     2482 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
--rw-r--r--   0        0        0     5649 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
--rw-r--r--   0        0        0     1753 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
--rw-r--r--   0        0        0     4962 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
--rw-r--r--   0        0        0     7522 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0    15892 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
--rw-r--r--   0        0        0     3165 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
--rw-r--r--   0        0        0     3676 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
--rw-r--r--   0        0        0      960 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
--rw-r--r--   0        0        0     3626 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
--rw-r--r--   0        0        0      618 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
--rw-r--r--   0        0        0      983 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
--rw-r--r--   0        0        0     1372 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
--rw-r--r--   0        0        0      296 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
--rw-r--r--   0        0        0      714 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
--rw-r--r--   0        0        0      660 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
--rw-r--r--   0        0        0      793 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
--rw-r--r--   0        0        0      574 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
--rw-r--r--   0        0        0       20 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2941 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      800 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      111 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3108 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      763 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       58 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      104 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-08-07 09:52:52.270883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3093 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      951 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       44 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      116 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2869 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      860 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1148 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3398 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2657 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6537 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1048 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1857 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1073 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3170 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1063 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     3319 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      175 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1710 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2739 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1567 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
--rw-r--r--   0        0        0      655 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3557 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    38166 2023-08-07 09:52:52.274883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      583 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       52 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       51 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0       52 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      803 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      570 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0      274 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
--rw-r--r--   0        0        0      263 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      922 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       18 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0   749872 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
--rw-r--r--   0        0        0     9913 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0       18 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
--rw-r--r--   0        0        0     3490 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
--rw-r--r--   0        0        0     4700 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
--rw-r--r--   0        0        0     5244 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0      593 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
--rw-r--r--   0        0        0       20 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     6698 2023-08-07 09:52:52.278883 ansys_templates-1.2.2/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    11164 1970-01-01 00:00:00.000000 ansys_templates-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-08-07 11:18:39.527581 ansys_templates-1.3.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     9680 2023-08-07 11:18:39.527581 ansys_templates-1.3.0/README.rst
+-rw-r--r--   0        0        0     3129 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2266 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3803 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3894 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3713 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      379 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
+-rw-r--r--   0        0        0       11 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      105 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      282 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4076 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1434 2023-08-07 11:18:39.531581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/cookiecutter.json
+-rw-r--r--   0        0        0     7551 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      175 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2147 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2944 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   222116 2023-08-07 11:18:39.535581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0   222261 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
+-rw-r--r--   0        0        0     3897 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      421 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       50 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0     2923 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/optislang/install.py
+-rw-r--r--   0        0        0     5037 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/optislang/project_tree.py
+-rw-r--r--   0        0        0       47 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      959 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
+-rw-r--r--   0        0        0      725 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      248 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
+-rw-r--r--   0        0        0    16262 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
+-rw-r--r--   0        0        0      946 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       41 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0     9913 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0     2579 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
+-rw-r--r--   0        0        0     3687 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
+-rw-r--r--   0        0        0     3177 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
+-rw-r--r--   0        0        0     5284 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
+-rw-r--r--   0        0        0     1837 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
+-rw-r--r--   0        0        0     2482 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
+-rw-r--r--   0        0        0     5649 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
+-rw-r--r--   0        0        0     1753 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
+-rw-r--r--   0        0        0     4215 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
+-rw-r--r--   0        0        0     7824 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0    14842 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
+-rw-r--r--   0        0        0     2724 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
+-rw-r--r--   0        0        0     3849 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
+-rw-r--r--   0        0        0     2072 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
+-rw-r--r--   0        0        0      565 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
+-rw-r--r--   0        0        0      618 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
+-rw-r--r--   0        0        0     2734 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
+-rw-r--r--   0        0        0     2728 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
+-rw-r--r--   0        0        0      410 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
+-rw-r--r--   0        0        0      876 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
+-rw-r--r--   0        0        0      822 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
+-rw-r--r--   0        0        0     2432 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
+-rw-r--r--   0        0        0      752 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
+-rw-r--r--   0        0        0       20 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2941 2023-08-07 11:18:39.539581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3108 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3093 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2869 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1148 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2657 2023-08-07 11:18:39.543581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1048 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1073 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1063 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     3855 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      175 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1710 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2739 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3557 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       51 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       52 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      922 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       18 2023-08-07 11:18:39.547581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0   749872 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
+-rw-r--r--   0        0        0     9913 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0       18 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
+-rw-r--r--   0        0        0     3490 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
+-rw-r--r--   0        0        0     4700 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
+-rw-r--r--   0        0        0     5244 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0      593 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
+-rw-r--r--   0        0        0     1351 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/collector/otel-collector-config.yaml
+-rw-r--r--   0        0        0     4160 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboard.json
+-rw-r--r--   0        0        0      265 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboards.yml
+-rw-r--r--   0        0        0     1478 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-datasources.yml
+-rw-r--r--   0        0        0      267 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana.ini
+-rw-r--r--   0        0        0      482 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/loki/loki.yml
+-rw-r--r--   0        0        0      412 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/prometheus/prometheus.yml
+-rw-r--r--   0        0        0     2826 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/compose.yaml
+-rw-r--r--   0        0        0     1567 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/tracelens/compose.yaml
+-rw-r--r--   0        0        0       20 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-08-07 11:18:39.551581 ansys_templates-1.3.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11165 1970-01-01 00:00:00.000000 ansys_templates-1.3.0/PKG-INFO
```

### Comparing `ansys_templates-1.2.2/LICENSES/MIT.txt` & `ansys_templates-1.3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/README.rst` & `ansys_templates-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/pyproject.toml` & `ansys_templates-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-templates"
-version = "1.2.2"
+version = "1.3.0"
 description = "Creates Python projects according to PyAnsys guidelines"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSES/MIT.txt"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -58,15 +58,15 @@
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.4.0",
     "pytest-cov==4.1.0",
 ]
 doc = [
-    "ansys-sphinx-theme==0.10",
+    "ansys-sphinx-theme==0.9.9",
     "numpydoc==1.5.0",
     "sphinx==7.0.1",
     "sphinx-copybutton==0.5.2",
 ]
 
 [tool.flit.module]
 name = "ansys.templates"
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/__init__.py` & `ansys_templates-1.3.0/src/ansys/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/__main__.py` & `ansys_templates-1.3.0/src/ansys/templates/__main__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/cli.py` & `ansys_templates-1.3.0/src/ansys/templates/cli.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/licenses/LICENSE_MIT` & `ansys_templates-1.3.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/paths.py` & `ansys_templates-1.3.0/src/ansys/templates/paths.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.3.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.3.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     "doc/styles/.gitignore",
     "doc/.vale.ini",
     "doc/make.bat",
     "doc/Makefile",
     "examples/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/assets/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/scripts/README.md",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/osl_project_tree.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/optislang/project_tree.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/optislang/install.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/utils.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/definition.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/monitoring_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/problem_setup_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/css/style.css",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/images/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/logos/ansys-solutions-horizontal-logo.png",
@@ -70,14 +71,15 @@
     "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CODEOWNERS",
     "CONTRIBUTING.md",
     "CONTRIBUTORS.md",
     "LICENSE.rst",
+    "poetry.lock",
     "pyproject.toml",
     "README.rst",
     "setup_environment.py",
     "tox.ini"
 ]
 """A list holding all desired files to be included in the project."""
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
 ansys-optislang-core = "^0.3.0"
 ansys-saf-glow = {version = "0.3.0", source = "solutions-private-pypi"}
 ansys-saf-portal = {version = "0.4.1", source = "solutions-private-pypi"}
-ansys-solutions-dash-lib = {version = "0.4.3", source = "solutions-private-pypi"}
+ansys-solutions-dash-lib = {version = "0.4.4", source = "solutions-private-pypi"}
 ansys-solutions-products-ecosystem = {version = "^0.1.dev0", source = "solutions-private-pypi"}
-ansys-solutions-optislang-frontend-components = {version = "^0.1.dev7", source = "solutions-private-pypi"}
+ansys-solutions-optislang-frontend-components = {version = "^0.1.dev9", source = "solutions-private-pypi"}
 optislang-dash-lib = {version = "^0.2.1", source = "solutions-private-pypi"}
 dash = "^2.6"
 dash_bootstrap_components = "^1.2"
 dash-extensions = "^0.1"
 dash-iconify = "^0.1"
 dash-loading-spinners = "^1.0.0"
 dash-uploader = "^0.6"
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/optislang/project_tree.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import os
 from pathlib import Path
 import shutil
 from typing import Union
 
 from ansys.optislang.core import Optislang
+from ansys.optislang.core.nodes import System
 
 
 def dump_project_state(project_file: Path, project_state_file: Path) -> None:
     """Start PyOptiSLang and dump project state file."""
 
     working_directory = project_file.parent
     temporary_directory = working_directory / "extract_project_tree.tmp"
@@ -132,7 +133,41 @@
     """Return the list of nodes in the optiSLang project file."""
 
     return [
         node_info
         for node_info in project_tree["project_tree"]
         if node_info["key"] not in ["problem_setup_step"]
     ]
+
+
+def get_node_by_uid(osl: Optislang, actor_uid: str):
+    """Get node by walking throughout the root system recursively."""
+
+    def recursive_search(nodes, actor_uid):
+
+        for node in nodes:
+            if node.uid == actor_uid:
+                return node
+            if isinstance(node, System):
+                result = recursive_search(node.get_nodes(), actor_uid)
+                if result:
+                    return result
+
+    for node in osl.project.root_system.get_nodes():
+        if node.uid == actor_uid:
+            return node
+        if isinstance(node, System):
+            result = recursive_search(node.get_nodes(), actor_uid)
+            if result:
+                return result
+
+
+def get_node_hids(osl: Optislang, actor_uid: str) -> list:
+    """Return the hirearchical ID (hid) of the actor."""
+
+    actor_states = osl.get_osl_server().get_actor_states(actor_uid)
+
+    if "states" in actor_states.keys():
+        if len(actor_states["states"]):
+            return [state["hid"] for state in actor_states["states"]]
+    else:
+        return []
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,30 +13,35 @@
 
 from ansys.optislang.core import Optislang, logging
 from ansys.saf.glow.solution import FileReference, FileGroupReference, StepModel, StepSpec, long_running, transaction
 from ansys.solutions.optislang.frontend_components.project_properties import ProjectProperties, write_properties_file, apply_placeholders_to_properties_file
 from ansys.solutions.products_ecosystem.controller import AnsysProductsEcosystemController
 from ansys.solutions.products_ecosystem.utils import convert_to_long_version
 
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.model.osl_project_tree import dump_project_state, get_project_tree, get_node_list, get_step_list
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.monitoring import _get_actor_hids, read_optislang_logs
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.model.optislang.project_tree import dump_project_state, get_project_tree, get_node_list, get_step_list, get_node_hids
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.model.optislang.install import get_available_optislang_installations
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.monitoring import read_log_file
 
 
 class ProblemSetupStep(StepModel):
     """Step model of the problem setup step."""
 
     # Parameters ------------------------------------------------------------------------------------------------------
 
     # Frontend persistence
     ansys_ecosystem_ready: bool = False
-    optislang_solve_status: str = "initial"  # initial, processing, finished, stopped, aborted, idle
     ui_placeholders: dict = {}
     app_metadata: dict = {}
-    analysis_running: bool = False
     analysis_locked: bool = True
+    project_locked: bool = False
+    treeview_locked: bool = True
+    selected_actor_from_treeview: str = None
+    selected_command: str = None
+    selected_actor_from_command: str = None
+    commands_locked: bool = False
 
     # Backend data model
     tcp_server_host: str = "127.0.0.1"
     tcp_server_port: int = None
     ansys_ecosystem: dict = {
         "optislang": {
             "authorized_versions": ["2022.2", "2023.1"],
@@ -55,15 +60,39 @@
     settings: dict = {}
     parameter_manager: dict = {}
     criteria: dict = {}
     project_status_info: dict = {}
     actors_info: dict = {}
     actors_status_info: dict = {}
     results_files: dict = {}
-    tcp_server_stopped_states = ["idle", "finished", "stopped", "aborted"]
+    project_state: str = "NOT STARTED"
+    osl_project_states: list = [
+        "IDLE",
+        "PROCESSING",
+        "PAUSED",
+        "PAUSE_REQUESTED",
+        "STOPPED",
+        "STOP_REQUESTED",
+        "GENTLY_STOPPED",
+        "GENTLE_STOP_REQUESTED",
+        "FINISHED"
+    ]
+    osl_actor_states: list = [
+        "Idle",
+        "Succeeded",
+        "Failed",
+        "Running",
+        "Aborted",
+        "Predecessor failed",
+        "Skipped",
+        "Incomplete",
+        "Processing done",
+        "Stopped",
+        "Gently stopped"
+    ]
     optislang_logs: list = []
     optislang_log_level: str = "INFO"
     project_initialized: bool = False
     has_project_state: bool = False
 
     # File storage ----------------------------------------------------------------------------------------------------
 
@@ -133,38 +162,53 @@
 
         original_metadata_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "metadata.json"
         self.metadata_file.write_bytes(original_metadata_file.read_bytes())
 
         original_project_state_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "project_state.json"
         self.project_state_file.write_bytes(original_project_state_file.read_bytes())
 
-
     @transaction(self=StepSpec(download=["properties_file"], upload=["placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
     def get_default_placeholder_values(self):
         """Get placeholder values and definitions using the ProjectProperties class."""
         pp = ProjectProperties()
         pp.read_file(self.properties_file.path)
         self.placeholders = pp._placeholders
         self.registered_files = pp._registered_files
         self.settings = pp._settings
         self.parameter_manager = pp._parameter_manager
         self.criteria = pp._criteria
 
-    @transaction(self=StepSpec(download=["properties_file", "ui_placeholders"], upload=["working_properties_file", "placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
+    @transaction(
+        self=StepSpec(
+            download=["properties_file", "ui_placeholders"],
+            upload=[
+                "working_properties_file",
+                "placeholders",
+                "registered_files",
+                "settings",
+                "parameter_manager",
+                "criteria",
+            ],
+        )
+    )
     def write_updated_properties_file(self) -> None:
         properties = apply_placeholders_to_properties_file(self.ui_placeholders, self.properties_file.path)
         self.placeholders = properties["placeholders"]
         self.registered_files = properties["registered_files"]
         self.settings = properties["settings"]
         self.parameter_manager = properties["parameter_manager"]
         self.criteria = properties["criteria"]
         write_properties_file(properties, Path(self.working_properties_file.path))
 
-
-    @transaction(self=StepSpec(download=["properties_file", "ui_placeholders"], upload=["placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
+    @transaction(
+        self=StepSpec(
+            download=["properties_file", "ui_placeholders"],
+            upload=["placeholders", "registered_files", "settings", "parameter_manager", "criteria"],
+        )
+    )
     def update_osl_placeholders_with_ui_values(self) -> None:
         properties = apply_placeholders_to_properties_file(self.ui_placeholders, self.properties_file.path)
         self.placeholders = properties["placeholders"]
         self.registered_files = properties["registered_files"]
         self.settings = properties["settings"]
         self.parameter_manager = properties["parameter_manager"]
         self.criteria = properties["criteria"]
@@ -175,27 +219,39 @@
         )
     )
     def check_ansys_ecosystem(self) -> None:
         """Check if Ansys Products are installed and if the appropriate versions are available."""
 
         self.ansys_ecosystem_ready = True
 
-        controller = AnsysProductsEcosystemController()
+        # Collect optiSLang installations
+        self.ansys_ecosystem["optislang"]["installed_versions"] = get_available_optislang_installations(
+            output_format="long"
+        )
+        self.ansys_ecosystem["optislang"]["compatible_versions"] = [
+            product_version
+            for product_version in self.ansys_ecosystem["optislang"]["installed_versions"]
+            if product_version in self.ansys_ecosystem["optislang"]["authorized_versions"]
+        ]
 
+        # Collect additonnal Ansys products installations
+        controller = AnsysProductsEcosystemController()
         for product_name in self.ansys_ecosystem.keys():
+            if product_name != "optislang":
+                self.ansys_ecosystem[product_name]["installed_versions"] = controller.get_installed_versions(
+                    product_name, output_format="long"
+                )
+                self.ansys_ecosystem[product_name]["compatible_versions"] = [
+                    product_version
+                    for product_version in self.ansys_ecosystem[product_name]["installed_versions"]
+                    if product_version in self.ansys_ecosystem[product_name]["authorized_versions"]
+                ]
 
-            self.ansys_ecosystem[product_name]["installed_versions"] = controller.get_installed_versions(
-                product_name, outout_format="long"
-            )
-            self.ansys_ecosystem[product_name]["compatible_versions"] = [
-                product_version
-                for product_version in self.ansys_ecosystem[product_name]["installed_versions"]
-                if product_version in self.ansys_ecosystem[product_name]["authorized_versions"]
-            ]
-
+        # Check ecosystem
+        for product_name in self.ansys_ecosystem.keys():
             if len(self.ansys_ecosystem[product_name]["installed_versions"]) == 0:
                 alert_message = f"No installation of {product_name.title()} found in the machine {platform.node()}."
                 alert_color = "danger"
                 self.ansys_ecosystem_ready = False
             elif len(self.ansys_ecosystem[product_name]["compatible_versions"]) == 0:
                 alert_message = (
                     f"None of the authorized versions of {product_name.title()} "
@@ -220,15 +276,14 @@
                     alert_message += f" {convert_to_long_version(compatible_version)}"
                 alert_message += ".\n"
                 alert_message += "Selected version is %s." % (self.ansys_ecosystem[product_name]["selected_version"])
                 alert_color = "success"
             self.ansys_ecosystem[product_name]["alert_message"] = alert_message
             self.ansys_ecosystem[product_name]["alert_color"] = alert_color
 
-
     @transaction(
         self=StepSpec(
             download=["metadata_file"],
             upload=["app_metadata"]
         )
     )
     def get_app_metadata(self) -> None:
@@ -236,49 +291,53 @@
 
         with open(self.metadata_file.path) as f:
             self.app_metadata = json.load(f)
 
     @transaction(
         self=StepSpec(
             download=[
+                "input_files",
+                "node_list",
+                "optislang_log_level",
                 "project_file",
                 "working_properties_file",
-                "tcp_server_stopped_states",
-                "optislang_log_level",
-                "node_list",
             ],
             upload=[
-                "optislang_solve_status",
-                "server_info_file",
                 "actors_info",
                 "actors_status_info",
-                "tcp_server_port",
+                "optislang_logs",
+                "optislang_log_file",
+                "project_state",
                 "project_status_info",
                 "results_files",
-                "optislang_log_file",
-                "optislang_logs",
+                "server_info_file",
+                "tcp_server_port",
+                "treeview_locked",
             ],
         )
     )
     @long_running
-    def start_analysis(self) -> None:
+    def start(self) -> None:
         """Start optiSLang and run the project."""
 
+        self.treeview_locked = False
+        self.transaction.upload(["treeview_locked"])
+
         osl_logger = logging.OslLogger(
             loglevel=self.optislang_log_level,
             log_to_file=True,
             logfile_name=self.optislang_log_file.path,
             log_to_stdout=True,
         )
 
         osl = Optislang(
             project_path=self.project_file.path,
             loglevel=self.optislang_log_level,
             reset=True,
-            shutdown_on_finished=True,
+            shutdown_on_finished=False,
             import_project_properties_file=self.working_properties_file.path,
             additional_args=[f"--write-server-info={self.server_info_file.path}"],
             ini_timeout=300,  # might need to be adjusted
         )
 
         osl.__logger = osl_logger.add_instance_logger(osl.name, osl, self.optislang_log_level)
 
@@ -288,41 +347,40 @@
                     lines = [line.rstrip("\n") for line in file.readlines()]
                 for line in lines:
                     if line.startswith("server_port="):
                         self.tcp_server_port = int(line.split("=")[1])
                         break
             else:
                 raise Exception("No server info file detected. Unable to retrieve TCP port number.")
+            self.transaction.upload(["tcp_server_port"])
 
         osl.start(wait_for_started=True, wait_for_finished=False)
 
         while True:
+            # Get project state
+            self.project_state = osl.project.get_status()
+            osl.log.info(f"Analysis status: {self.project_state}")
             # Get project status info
             self.project_status_info = osl.get_osl_server().get_full_project_status_info()
             # Read pyoptislang logs
-            self.optislang_logs = read_optislang_logs(self.optislang_log_file.path)
+            self.optislang_logs = read_log_file(self.optislang_log_file.path)
             # Get actor status info
             for node_info in self.node_list:
                 self.actors_info[node_info["uid"]] = osl.get_osl_server().get_actor_info(node_info["uid"])
-                node_hids = _get_actor_hids(osl.get_osl_server().get_actor_states(node_info["uid"]))
+                node_hids = get_node_hids(osl, node_info["uid"])
                 if len(node_hids):
                     self.actors_status_info[node_info["uid"]] = []
                     for hid in node_hids:
                         self.actors_status_info[node_info["uid"]].append(
                             osl.get_osl_server().get_actor_status_info(node_info["uid"], hid)
                         )
-            # Get status
-            self.optislang_solve_status = osl.project.get_status().lower()
-            osl.log.info(f"Analysis status: {self.optislang_solve_status}")
-            # Upload fields
-            self.transaction.upload(["optislang_solve_status"])
+             # Upload fields
+            self.transaction.upload(["project_state"])
             self.transaction.upload(["project_status_info"])
             self.transaction.upload(["actors_info"])
             self.transaction.upload(["actors_status_info"])
             self.transaction.upload(["optislang_logs"])
-            # Check if analysis stopped
-            if self.optislang_solve_status in self.tcp_server_stopped_states:
+            if self.project_state == "FINISHED":
                 break
             time.sleep(3)
 
         osl.dispose()
-
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,51 +6,47 @@
 import dash_bootstrap_components as dbc
 from dash_extensions.enrich import Input, Output, State, callback, dcc, html
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import {{ cookiecutter.__solution_definition_name }}
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.monitoring_step import MonitoringStep
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.problem_setup_step import ProblemSetupStep
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.components.logs_table import LogsTable
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.alerts import update_monitoring_alert
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.common_functions import update_list_of_tabs
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.views import (
     design_table_page,
     project_summary_page,
     result_files_page,
     scenery_page,
     status_overview_page,
     summary_page,
     visualization_page,
 )
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.common_functions import extract_dict_by_key
 
 
-def layout(problem_setup_step: ProblemSetupStep, monitoring_step: MonitoringStep, node_info: dict) -> html.Div:
+def layout(problem_setup_step: ProblemSetupStep) -> html.Div:
 
-    list_of_tabs = update_list_of_tabs(node_info)
+    actor_info = extract_dict_by_key(problem_setup_step.step_list, "uid", problem_setup_step.selected_actor_from_treeview, expect_unique=True, return_index=False)
+    list_of_tabs = update_list_of_tabs(actor_info)
 
     return html.Div(
         [
-            html.Div(
-                id="monitoring_alert",
-                children=update_monitoring_alert(problem_setup_step),
-            ),
             dbc.Tabs(
                 list_of_tabs,
                 id="monitoring_tabs",
                 active_tab=list_of_tabs[0].tab_id,
                 style={
                     "color": "#000000",
                     "background-color": "#FFFFFF",
                     "text-color": "#000000",
                 },
             ),
             html.Div(
                 id="monitoring_page_content",
             ),
-            dcc.Store(id="node_info", data=node_info),
             html.Br(),
             html.Div(
                 [
                     dbc.Button(
                         "optiSLang logs",
                         id="fade_button",
                         className="mb-3",
@@ -59,58 +55,44 @@
                     ),
                     dbc.Fade(
                         id="fade",
                         is_in=False,
                         appear=False,
                     ),
                 ]
-            ),
-            dcc.Interval(
-                id="update_data_interval",
-                interval=1 * 3000,  # in milliseconds
-                n_intervals=0,
-            ),
+            )
         ]
     )
 
 
 @callback(
     Output("monitoring_page_content", "children"),
     Input("monitoring_tabs", "active_tab"),
-    Input("update_data_interval", "n_intervals"),
     Input("url", "pathname"),
-    State("node_info", "data"),
 )
-def update_page_content(active_tab, n_intervals, pathname, node_info):
+def update_page_content(active_tab, pathname):
     """Update the page content according to the selected tab."""
 
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
 
     if active_tab == "project_summary_tab":
-        return project_summary_page.layout(problem_setup_step.project_status_info)
+        return project_summary_page.layout(problem_setup_step)
     elif active_tab == "summary_tab":
-        return summary_page.layout(
-            problem_setup_step.actors_info,
-            problem_setup_step.actors_status_info,
-            problem_setup_step.results_files,
-            node_info["uid"],
-        )
+        return summary_page.layout(problem_setup_step)
     elif active_tab == "result_files_tab":
-        return result_files_page.layout(problem_setup_step.project_status_info, node_info["uid"])
+        return result_files_page.layout(problem_setup_step)
     elif active_tab == "scenery_tab":
-        return scenery_page.layout(problem_setup_step.project_status_info)
+        return scenery_page.layout(problem_setup_step)
     elif active_tab == "design_table_tab":
-        return design_table_page.layout(
-            problem_setup_step.actors_info, problem_setup_step.actors_status_info, node_info["uid"]
-        )
+        return design_table_page.layout(problem_setup_step)
     elif active_tab == "visualization_tab":
-        return visualization_page.layout(problem_setup_step.project_status_info, node_info["uid"])
+        return visualization_page.layout(problem_setup_step)
     elif active_tab == "status_overview_tab":
-        return status_overview_page.layout(problem_setup_step.project_status_info)
+        return status_overview_page.layout(problem_setup_step)
 
 
 @callback(
     Output("fade", "children"),
     Output("fade", "is_in"),
     Input("fade_button", "n_clicks"),
     Input("url", "pathname"),
@@ -124,8 +106,7 @@
     if not n_clicks:
         # Button has never been clicked
         return None, False
 
     table = LogsTable(problem_setup_step.optislang_logs)
 
     return table.render(), not is_in
-
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,189 +9,205 @@
 from dash.exceptions import PreventUpdate
 from dash_iconify import DashIconify
 import dash_loading_spinners as dls
 from pathlib import Path
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import {{ cookiecutter.__solution_definition_name }}
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages import monitoring_page, problem_setup_page
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.common_functions import extract_dict_by_key, read_system_hierarchy
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.common_functions import extract_dict_by_key
 
 
 layout = html.Div(
     [
-        dcc.Location(id="url", refresh=False),  # represents the browser address bar and doesn't render anything
-        dls.Pulse(
-            color="#FFB71B",
-            speed_multiplier=0.4,
-            margin=4,
-            width=57,
-            fullscreen=True,
-            fullscreen_style={
-                "background-color": "rgba(255, 255, 255, 0)",
-                "position": "relative"
-            },
-            children=html.Div(id="wait_app_initialization"),
+        dcc.Location(id="url", refresh=False), # represents the browser address bar and doesn't render anything
+        dbc.Stack(
+            [
+                html.Div(
+                    [
+                        html.Img(
+                        src = r"/assets/logos/ansys-solutions-horizontal-logo.png",
+                        style={'width': '80%'}
+                    )
+                    ],
+                ),
+                html.Div(
+                    [
+                        dbc.Button(
+                            "Project Name:",
+                            id = "project_name",
+                            disabled = True,
+                            style={
+                                "color": "rgba(0, 0, 0, 1)",
+                                "background-color": "rgba(255, 255, 255, 1)",
+                                "border-color": "rgba(0, 0, 0, 1)"
+                            },
+                        )
+                    ],
+                    className="ms-auto",
+                ),
+                html.Div(id="return_to_portal"),
+            ],
+            direction = "horizontal",
+            gap = 3,
         ),
-        html.Div(
-            id="page_content",
+        html.Br(),
+        dbc.Row(
+            [
+                dbc.Col(
+                    AnsysDashTreeview(
+                        id="navigation_tree",
+                        items=[
+                            {
+                                "key": "problem_setup_step",
+                                "text": "Problem Setup",
+                                "depth": 0,
+                                "uid": None,
+                                "type": None,
+                                "kind": None,
+                                "is_root": False,
+                            },
+                        ],
+                        children=[
+                            DashIconify(icon="bi:caret-right-square-fill"),
+                            DashIconify(icon="bi:caret-down-square-fill"),
+                        ],
+                        style={"showButtons": True, "focusColor": "#ffb71b", "itemHeight": "32"},  # Ansys gold
+                    ),
+                    width=2,
+                    style={"background-color": "rgba(242, 242, 242, 0.6)"},  # Ansys grey
+                ),
+                dbc.Col(
+                    html.Div(
+                        id="page_content",
+                        style={"padding-right": "1%"}
+                    ),
+                    width=10
+                ),
+            ],
         ),
-        dbc.Button(
+        dcc.Store(id='project_initialized'),
+         dbc.Button(
             id="dummy_button",
             style={"display": "none"},
             n_clicks=0,
             color="dark"
         ),
     ]
 )
 
 
 @callback(
-    Output("return_to_portal", "children"),
-    Input("url", "pathname"),
-)
-def return_to_portal(pathname):
-    """Display Solution Portal when back-to-portal button gets selected."""
-    portal_ui_url = DashClient.get_portal_ui_url()
-    children = (
-        []
-        if portal_ui_url is None
-        else [
-            dbc.Button(
-                "Back to Projects",
-                id="return_to_portal",
-                className="me-2",
-                n_clicks=0,
-                href=portal_ui_url,
-                style={"background-color": "rgba(0, 0, 0, 1)", "border-color": "rgba(0, 0, 0, 1)"},
-            )
-        ]
-    )
-    return children
-
-
-@callback(
-    Output("page_content", "children"),
     Output("dummy_button", "n_clicks"),
-    Output("wait_app_initialization", "children"),
     Input("url", "pathname"),
     State("dummy_button", "n_clicks")
 )
-def project_initialization(pathname, n_clicks):
+def initialization(pathname, n_clicks):
+    """Display current project name."""
 
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
 
     if not project.steps.problem_setup_step.project_initialized:
         # Solution-specific code
         project_tree_path = Path(__file__).absolute().parent.parent.parent / "model" / "assets" / "project_state.json"
         if not project_tree_path.exists():
             project.steps.problem_setup_step.generate_project_state()
         # Project-specific code
-        project.steps.problem_setup_step.upload_bulk_files_to_project_directory()
+        project.steps.problem_setup_step.upload_bulk_files_to_project_directory() # to be replaced by AssetFileReference
         project.steps.problem_setup_step.read_project_tree()
         project.steps.problem_setup_step.get_app_metadata()
-        project.steps.problem_setup_step.check_ansys_ecosystem()
-        return [
-            dbc.Stack(
-                [
-                    html.Div(
-                        [html.Img(src=r"/assets/logos/ansys-solutions-horizontal-logo.png", style={"width": "80%"})],
-                    ),
-                    html.Div(
-                        [
-                            dbc.Button(
-                                f"Project Name: {project.project_display_name}",
-                                id="project-name",
-                                disabled=True,
-                                style={
-                                    "color": "rgba(0, 0, 0, 1)",
-                                    "background-color": "rgba(255, 255, 255, 1)",
-                                    "border-color": "rgba(0, 0, 0, 1)",
-                                },
-                            )
-                        ],
-                        className="ms-auto",
-                    ),
-                    html.Div(id="return_to_portal"),
-                ],
-                direction="horizontal",
-                gap=3,
-            ),
-            html.Br(),
-            dbc.Row(
-                [
-                    dbc.Col(
-                        AnsysDashTreeview(
-                            id="navigation_tree",
-                            items=[
-                                {
-                                    "key": "problem_setup_step",
-                                    "text": "Problem Setup",
-                                    "depth": 0,
-                                    "uid": None,
-                                    "type": None,
-                                    "kind": None,
-                                    "is_root": False,
-                                },
-                            ],
-                            children=[
-                                DashIconify(icon="bi:caret-right-square-fill"),
-                                DashIconify(icon="bi:caret-down-square-fill"),
-                            ],
-                            style={"showButtons": True, "focusColor": "#ffb71b", "itemHeight": "32"},  # Ansys gold
-                        ),
-                        width=2,
-                        style={"background-color": "rgba(242, 242, 242, 0.6)"},  # Ansys grey
-                    ),
-                    dbc.Col(html.Div(id="page_body", style={"padding-right": "1%"}), width=10),
-                ],
-            ),
-        ], n_clicks + 1, True
-    else:
-        raise PreventUpdate
+        project.steps.problem_setup_step.get_default_placeholder_values()
+        project.steps.problem_setup_step.project_initialized = True
+
+    return n_clicks + 1
+
+
+@callback(
+    Output("project_name", "children"),
+    Input("url", "pathname"),
+)
+def display_poject_name(pathname):
+    """Display current project name."""
+
+    project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
+
+    return f"Project Name: {project.project_display_name}"
 
 
 @callback(
     Output("navigation_tree", "items"),
     Input("dummy_button", "n_clicks"),
-    Input("url", "pathname"),
+    State("url", "pathname"),
 )
-def display_step_list(n_clicks, pathname):
+def display_tree_view(n_clicks, pathname):
     """Display current project name."""
+
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
 
-    return project.steps.problem_setup_step.step_list
+    if project.steps.problem_setup_step.project_initialized:
+        return project.steps.problem_setup_step.step_list
+    else:
+        raise PreventUpdate
 
 
 @callback(
-    Output("page_body", "children"),
-    [
-        Input("url", "pathname"),
-        Input("navigation_tree", "focus"),
-        Input("dummy_button", "n_clicks"),
-    ],
+    Output("page_content", "children"),
+    Input("navigation_tree", "focus"),
+    Input("dummy_button", "n_clicks"),
+    State("url", "pathname"),
     prevent_initial_call=True,
 )
-def display_page_body(pathname, value, n_clicks):
+def display_page_content(value, n_clicks, pathname):
     """
     Display page content.
 
     this callback is essential for initializing the step based on the persisted
     state of the project when the browser first displays the project to the user
     given the project's URL
     """
 
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
-    triggered_id = callback_context.triggered[0]["prop_id"].split(".")[0]
 
-    if triggered_id == "url" or triggered_id == "dummy_button":
-        return problem_setup_page.layout(project.steps.problem_setup_step)
-    if triggered_id == "navigation_tree":
-        if value is None:
-            page_layout = html.H1("Welcome!")
-        elif value == "problem_setup_step":
-            page_layout = problem_setup_page.layout(project.steps.problem_setup_step)
-        else:
-            node_info = extract_dict_by_key(project.steps.problem_setup_step.step_list, "key", value, expect_unique=True)
-            page_layout = monitoring_page.layout(
-                project.steps.problem_setup_step, project.steps.monitoring_step, node_info
+    problem_setup_step = project.steps.problem_setup_step
+
+    if problem_setup_step.project_initialized:
+        triggered_id = callback_context.triggered[0]["prop_id"].split(".")[0]
+        if triggered_id == "url" or triggered_id == "dummy_button":
+            return problem_setup_page.layout(problem_setup_step)
+        if triggered_id == "navigation_tree":
+            if value is None:
+                page_layout = html.H1("Welcome!")
+            elif value == "problem_setup_step":
+                page_layout = problem_setup_page.layout(problem_setup_step)
+            else:
+                if not problem_setup_step.treeview_locked:
+                    problem_setup_step.selected_actor_from_treeview = extract_dict_by_key(problem_setup_step.step_list, "key", value, expect_unique=True, return_index=False)["uid"]
+                    page_layout = monitoring_page.layout(problem_setup_step)
+                else:
+                    page_layout = problem_setup_page.layout(problem_setup_step)
+            return page_layout
+    else:
+        raise PreventUpdate
+
+
+@callback(
+    Output("return_to_portal", "children"),
+    Input("url", "pathname"),
+)
+def return_to_portal(pathname):
+    """Display Solution Portal when back-to-portal button gets selected."""
+
+    portal_ui_url = DashClient.get_portal_ui_url()
+    children = (
+        []
+        if portal_ui_url is None
+        else [
+            dbc.Button(
+                "Back to Projects",
+                id = "return_to_portal",
+                className = "me-2",
+                n_clicks = 0,
+                href = portal_ui_url,
+                style = {"background-color": "rgba(0, 0, 0, 1)", "border-color": "rgba(0, 0, 0, 1)"},
             )
-        return page_layout
+        ]
+    )
+    return children
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 from ansys.saf.glow.client.dashclient import DashClient
 from ansys.solutions.dash_components.table import InputRow
 from ansys.solutions.optislang.frontend_components.load_sections import to_dash_sections
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import {{ cookiecutter.__solution_definition_name }}
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.problem_setup_step import ProblemSetupStep
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.alerts import update_alerts
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.common_functions import check_empty_strings
+
 
 
 def layout(problem_setup_step: ProblemSetupStep) -> html.Div:
     """Layout of the problem setup step."""
 
-    # Upload placeholders and assets
-    if problem_setup_step.placeholders == {}:
-        problem_setup_step.get_default_placeholder_values()
-    project_properties_sections = to_dash_sections(problem_setup_step.placeholders, problem_setup_step.registered_files)
+    project_properties_sections = to_dash_sections(
+            problem_setup_step.placeholders, problem_setup_step.registered_files, problem_setup_step.project_locked
+        )
 
     return html.Div(
         [
             # Header
             html.H1(
                 problem_setup_step.app_metadata["title"].strip().title(),
                 className="display-3",
@@ -39,14 +40,24 @@
                 className="lead",
                 style={"font-size": "25px"},
             ),
             html.Hr(className="my-2"),
             html.Br(),
             # Alerts
             dbc.Row(
+                id="project-locked-alert",
+                children=[
+                    dbc.Alert(
+                        "The selected inputs are locked. To set new inputs, create a new project.",
+                        color="info",
+                    )
+                ],
+                style={"display": "block"} if problem_setup_step.project_locked else {"display": "none"},
+            ),
+            dbc.Row(
                 [
                     dbc.Col(
                         [
                             dbc.Stack(
                                 update_alerts(problem_setup_step),
                                 id="alert_messages",
                                 direction="horizontal",
@@ -62,35 +73,14 @@
             dbc.Row(id="osl-dash-sections",children=project_properties_sections),
             dbc.Row(
                 [
                     dbc.Accordion(
                         [
                             dbc.AccordionItem(
                                 [
-                                    # InputRow(
-                                    #     "button",
-                                    #     "check_ansys_ecosystem",
-                                    #     "Check Ansys ecosystem",
-                                    #     disabled=False,
-                                    #     label_width=2,
-                                    #     value_width=4,
-                                    #     unit_width=1,
-                                    #     description_width=4,
-                                    #     class_name="button",
-                                    # ).get(),
-                                    # dcc.Loading(
-                                    #     type="circle",
-                                    #     fullscreen=True,
-                                    #     color="#ffb71b",
-                                    #     style={
-                                    #         "background-color": "rgba(55, 58, 54, 0.1)",
-                                    #     },
-                                    #     children=html.Div(id="wait_ecosystem_ckeck"),
-                                    # ),
-                                    # html.Br(),
                                     InputRow(
                                         "button",
                                         "start_analysis",
                                         "Start analysis",
                                         disabled=problem_setup_step.analysis_locked,
                                         label_width=2,
                                         value_width=4,
@@ -139,86 +129,84 @@
     )
     def toggle_popover(n_clicks, is_open):
         if n_clicks:
             return not is_open
         return is_open
 
 
-# @callback(
-#     Output("alert_messages", "children"),
-#     Output("wait_ecosystem_ckeck", "children"),
-#     Output("start_analysis", "disabled"),
-#     Input("check_ansys_ecosystem", "n_clicks"),
-#     State("url", "pathname"),
-#     prevent_initial_call=True,
-# )
-# def check_ansys_ecosystem(n_clicks, pathname):
-#     """Start optiSLang and run the simulation. Wait for the process to complete."""
-
-#     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
-#     problem_setup_step = project.steps.problem_setup_step
-
-#     if n_clicks:
-#         problem_setup_step.check_ansys_ecosystem()
-#         return update_alerts(problem_setup_step), True, False if problem_setup_step.ansys_ecosystem_ready else True
-#     else:
-#         raise PreventUpdate
-
-
 @callback(
     Output("alert_messages", "children"),
     Output("wait_start_analysis", "children"),
     Output("start_analysis", "disabled"),
+    Output("osl-dash-sections", "children"),
+    Output("project-locked-alert", "style"),
     Input("start_analysis", "n_clicks"),
     State("url", "pathname"),
     prevent_initial_call=True,
 )
 def start_analysis(n_clicks, pathname):
     """Start optiSLang and run the simulation. Wait for the process to complete."""
 
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
 
     if n_clicks:
-        ui_data=problem_setup_step.ui_placeholders
+        ui_data = problem_setup_step.ui_placeholders
         ui_data.update({"start_analysis_requested": True})
-        problem_setup_step.ui_placeholders=ui_data
-        # Update project properties file prior to the solve
-        problem_setup_step.write_updated_properties_file()
-        # Start analysis
-        problem_setup_step.start_analysis()
-        # Lock start analysis
-        problem_setup_step.analysis_locked = True
-        # Wait until the analysis effectively starts
-        while problem_setup_step.optislang_solve_status == "initial":
-            time.sleep(1)
-        return update_alerts(problem_setup_step), True, True
+        problem_setup_step.ui_placeholders = ui_data
+        # Check if Ansys products are available
+        project.steps.problem_setup_step.check_ansys_ecosystem()
+        if problem_setup_step.ansys_ecosystem_ready:
+            # Update project properties file prior to the solve
+            problem_setup_step.write_updated_properties_file()
+            # Start analysis
+            problem_setup_step.start()
+            # Lock start analysis and ui data
+            problem_setup_step.analysis_locked = True
+            problem_setup_step.project_locked = True
+            # Wait until the analysis effectively starts
+            while problem_setup_step.project_state == "NOT STARTED":
+                time.sleep(1)
+            return (
+                update_alerts(problem_setup_step),
+                True,
+                True,
+                to_dash_sections(
+                    problem_setup_step.placeholders, problem_setup_step.registered_files, problem_setup_step.project_locked
+                ),
+                {"display": "block"},
+            )
+        else:
+            return (
+                update_alerts(problem_setup_step),
+                True,
+                False,
+                to_dash_sections(
+                    problem_setup_step.placeholders, problem_setup_step.registered_files, problem_setup_step.project_locked
+                ),
+                {"display": "block"},
+            )
     else:
         raise PreventUpdate
 
 
 @callback(
     Output("alert_messages", "children"),
-    Output("start_analysis", "disabled"),
     Input("solve_interval_component", "n_intervals"),
     Input("start_analysis", "n_clicks"),
     State("url", "pathname"),
 )
 def update_alert_messages(n_intervals, n_clicks, pathname):
     """Display status badges."""
 
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
 
     if problem_setup_step.ansys_ecosystem_ready:
-        status = problem_setup_step.get_long_running_method_state("start_analysis").status
-        if status == MethodStatus.Running:
-            problem_setup_step.analysis_running = True
-            problem_setup_step.analysis_locked = True
-        return update_alerts(problem_setup_step), problem_setup_step.analysis_locked
+        return update_alerts(problem_setup_step)
     else:
         raise PreventUpdate
 
 
 @callback(
     Output("start_analysis", "disabled"),
     Input("dummy_button_2", "n_clicks"),
@@ -232,15 +220,15 @@
 def initialize_dictionary_of_ui_placeholders(n_clicks, data, ids, input_file_ids, dummy_clicks, pathname):
     """This initializes the dictionary of ui placeholders using only the values in the Placeholders section."""
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
     designs = {}
     parameters = {}
     if problem_setup_step.ui_placeholders == {}:
-        ui_data=problem_setup_step.ui_placeholders
+        ui_data = problem_setup_step.ui_placeholders
         for index in range(len(data)):
             if ids[index]["placeholder"].startswith("StartDesigns"):
                 split_values = ids[index]["placeholder"].split("##")
                 values = split_values[1:]
                 rowId = values[0].split("#")[1]
                 key = values[1].split("#")[1]
                 value = values[2].split("#")[1]
@@ -249,25 +237,25 @@
                 else:
                     designs[rowId] = {key: value}
             elif "ParameterManager" in ids[index]["placeholder"]:
                 split_values = ids[index]["placeholder"].split("#")
                 pm_name = split_values[0]
                 key = split_values[1]
                 parameters[key] = data[index]
-                ui_data.update({pm_name:parameters})
-            elif "Bool" in ids[index]["placeholder"] and type(data[index])==list:
-                value=data[index]
+                ui_data.update({pm_name: parameters})
+            elif "Bool" in ids[index]["placeholder"] and type(data[index]) == list:
+                value = data[index]
                 if True in value:
                     new_value = True
                 else:
                     new_value = False
                 ui_data.update({ids[index]["placeholder"]: new_value})
             else:
-                ui_data.update({ids[index]["placeholder"]:data[index]})
-            ui_data.update({"StartDesigns":designs})
+                ui_data.update({ids[index]["placeholder"]: data[index]})
+            ui_data.update({"StartDesigns": designs})
             ui_data["start_analysis_requested"] = False
         if input_file_ids:
             problem_setup_step.analysis_locked = True
         else:
             problem_setup_step.analysis_locked = False
         for index in range(len(input_file_ids)):
             ui_data.update({input_file_ids[index]["placeholder"]: ""})
@@ -285,79 +273,79 @@
     State("url", "pathname"),
     prevent_initial_call=True,
 )
 def update_ui_placeholders(value, id, pathname):
     """This updates the dictionary of ui placeholders each time the ui data changes in the Placeholders section"""
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
-    name=id["placeholder"]
-    ui_data=problem_setup_step.ui_placeholders
+    name = id["placeholder"]
+    ui_data = problem_setup_step.ui_placeholders
     if name.startswith("StartDesigns"):
         split_values = id["placeholder"].split("##")
         values = split_values[1:]
         rowId = values[0].split("#")[1]
         key = values[1].split("#")[1]
-        ui_data["StartDesigns"][rowId][key]=value
+        ui_data["StartDesigns"][rowId][key] = value
     elif "ParameterManager" in name:
         split_values = id["placeholder"].split("#")
         pm_name = split_values[0]
         key = split_values[1]
-        ui_data[pm_name][key]=value
-    elif "Bool" in name and type(value)==list:
+        ui_data[pm_name][key] = value
+    elif "Bool" in name and type(value) == list:
         if True in value:
             value = True
         else:
             value = False
         ui_data.update({name: value})
     else:
         ui_data.update({name: value})
-    problem_setup_step.ui_placeholders=ui_data
+    problem_setup_step.ui_placeholders = ui_data
     problem_setup_step.update_osl_placeholders_with_ui_values()
 
     return no_update
 
 
 @callback(
     Output({"type": "upload", "placeholder": MATCH}, "children"),
     Input({"type": "upload", "placeholder": MATCH}, "isCompleted"),
     State({"type": "upload", "placeholder": MATCH}, "fileNames"),
     State({"type": "upload", "placeholder": MATCH}, "upload_id"),
     State({"type": "upload", "placeholder": MATCH}, "id"),
     State("url", "pathname"),
     prevent_initial_call=True,
 )
-def upload(is_completed, filenames, upload_id, component_id, pathname):
+def upload_input_files_to_project_and_update_ui_placeholders(is_completed, filenames, upload_id, component_id, pathname):
     """This uploads an Input file to the project directory and updates the dictionary of ui placeholders every time
     the ui data changes in the Input files section."""
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
 
     name = component_id["placeholder"]
     if is_completed and filenames and len(filenames):
         filename = filenames[0]
         filepath = os.path.join(problem_setup_step.upload_directory, upload_id, filename)
         file_data = open(filepath, mode="rb")
 
         project.upload_file(f"Problem_Setup/Input_Files/{filename}", file_data)
-        ui_data=problem_setup_step.ui_placeholders
+        ui_data = problem_setup_step.ui_placeholders
         ui_data.update({name: filename})
         problem_setup_step.ui_placeholders = ui_data
 
         return no_update
     else:
         raise PreventUpdate
 
 
 @callback(
     Output("start_analysis", "disabled"),
     Input({"type": "upload", "placeholder": ALL}, "isCompleted"),
     State({"type": "upload", "placeholder": ALL}, "fileNames"),
     State("url", "pathname"),
     prevent_initial_call=True,
-    )
+)
 def update_status_of_start_analysis_button(is_completed, filenames, pathname):
     """This enables the start analysis button if a file has been uploaded for all input files."""
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
     if all(filenames):
         problem_setup_step.analysis_locked = False
     else:
@@ -371,15 +359,7 @@
 @callback(
     Output("dummy_button_2", "n_clicks"),
     Input("url", "pathname"),
     State("dummy_button_2", "n_clicks"),
 )
 def on_page_load_initialize_dictionary_of_ui_placeholder_values(pathname, n_clicks):
     return n_clicks + 1
-
-
-def check_empty_strings(lst):
-    for sublist in lst:
-        for item in sublist:
-            if not item.strip():  # Using strip() to remove leading/trailing whitespaces
-                return False
-    return True
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 import dash_bootstrap_components as dbc
 from dash_extensions.enrich import html
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.problem_setup_step import ProblemSetupStep
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.constants import PROJECT_STATES
 
 
 def update_alerts(problem_setup_step: ProblemSetupStep) -> list:
     """Update all Alerts."""
 
     alerts = []
 
@@ -33,26 +34,18 @@
                         is_open=False,
                     ),
                 ]
             ),
         )
 
     # optiSLang solve alert
-    if problem_setup_step.optislang_solve_status == "initial":
-        solve_message, solve_color = "optiSLang simulation not started.", "warning"
-    elif problem_setup_step.optislang_solve_status == "processing":
-        solve_message, solve_color = "optiSLang simulation in progress.", "primary"
-    elif problem_setup_step.optislang_solve_status == "stopped":
-        solve_message, solve_color = "optiSLang simulation stopped.", "danger"
-    elif problem_setup_step.optislang_solve_status == "aborted":
-        solve_message, solve_color = "optiSLang simulation aborted.", "danger"
-    elif problem_setup_step.optislang_solve_status == "finished":
-        solve_message, solve_color = "optiSLang simulation completed successfully.", "success"
+    if problem_setup_step.project_state in PROJECT_STATES.keys():
+        solve_message, solve_color = PROJECT_STATES[problem_setup_step.project_state]["alert"], PROJECT_STATES[problem_setup_step.project_state]["color"]
     else:
-        raise ValueError(f"Unknown optiSLang status: {problem_setup_step.optislang_solve_status}.")
+        raise ValueError(f"Unknown optiSLang state: {problem_setup_step.project_state}.")
 
     alerts.append(
         html.Div(
             [
                 dbc.Button(
                     "optiSLang Solve",
                     id="popover_optislang_solve_target",
@@ -74,12 +67,12 @@
     )
 
     return alerts
 
 
 def update_monitoring_alert(problem_setup_step: ProblemSetupStep) -> dbc.Alert:
 
-    if problem_setup_step.optislang_solve_status == "initial":
+    if problem_setup_step.project_state == "NOT STARTED":
         return dbc.Alert(
             "No analysis started. No data to display.",
             color="warning",
         )
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Frontend of the scenery view."""
 
 from dash_extensions.enrich import html
 import optislang_dash_lib
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.problem_setup_step import ProblemSetupStep
 
 
-def layout(project_status_info: dict) -> html.Div:
+def layout(problem_setup_step: ProblemSetupStep) -> html.Div:
     """Layout of the scenery view."""
 
-    if project_status_info:
+    if problem_setup_step.project_status_info:
         return html.Div(
             [
                 html.Br(),
                 html.Div(
                     [
                         optislang_dash_lib.SceneryComponent(
                             id="input",
-                            project_state=project_status_info,
+                            project_state=problem_setup_step.project_status_info,
                         ),
                     ]
                 ),
             ]
         )
     else:
         return html.Div([])
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys_templates-1.3.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.3.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/cookiecutter.json` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/tracelens/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.3.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import dash_bootstrap_components as dbc
 from dash_extensions.enrich import DashProxy, MultiplexerTransform, NoOutputTransform, TriggerTransform
 import dash_uploader as du
 
 
 app = DashProxy(
     __name__,
-    external_stylesheets=[dbc.themes.BOOTSTRAP],
+    external_stylesheets=[dbc.themes.BOOTSTRAP, dbc.icons.FONT_AWESOME],
     suppress_callback_exceptions=True,
     transforms=[NoOutputTransform(), TriggerTransform(), MultiplexerTransform()],
 )
 
 # If folder doesn't exist, it will be created later
 UPLOAD_DIRECTORY = os.path.join(tempfile.gettempdir(), "GLOW")
 du.configure_upload(app, UPLOAD_DIRECTORY)
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Frontend of the first step."""
 
 
-from ansys.saf.glow.client.dashclient import DashClient
-from dash_extensions.enrich import Input, Output, State, callback, dcc, html
+from ansys.saf.glow.client.dashclient import DashClient, callback
+from dash_extensions.enrich import Input, Output, State, dcc, html
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import {{cookiecutter.__solution_definition_name}}
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.first_step import FirstStep
 from ansys.solutions.dash_components.table import InputRow,OutputRow
 
 
 def layout(step: FirstStep):
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Initialization of the frontend layout across all the steps."""
 
 
-from ansys.saf.glow.client.dashclient import DashClient
+from ansys.saf.glow.client.dashclient import DashClient, callback
 from ansys_dash_treeview import AnsysDashTreeview
 import dash_bootstrap_components as dbc
-from dash_extensions.enrich import Input, Output, callback, callback_context, dcc, html
+from dash_extensions.enrich import Input, Output, callback_context, dcc, html
 from dash_iconify import DashIconify
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import (
     {{ cookiecutter.__solution_definition_name }},
 )
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages import intro_page, first_page, second_page
```

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.3.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/testing.py` & `ansys_templates-1.3.0/src/ansys/templates/testing.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/src/ansys/templates/utils.py` & `ansys_templates-1.3.0/src/ansys/templates/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.2.2/PKG-INFO` & `ansys_templates-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 1.2.2
+Version: 1.3.0
 Summary: Creates Python projects according to PyAnsys guidelines
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
 Requires-Dist: click>=7.0,<9.0.0
 Requires-Dist: cookiecutter>=2.1.0,<2.3.0
 Requires-Dist: isort>=5.10.1
-Requires-Dist: ansys-sphinx-theme==0.10 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Project-URL: Documentation, https://templates.ansys.com/
 Project-URL: Homepage, https://templates.ansys.com/
```

