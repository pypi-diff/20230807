# Comparing `tmp/pop_create-8.1.0.tar.gz` & `tmp/pop_create-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop_create-8.1.0.tar", last modified: Mon Jul 31 18:19:13 2023, max compression
+gzip compressed data, was "pop_create-8.1.1.tar", last modified: Mon Aug  7 12:10:33 2023, max compression
```

## Comparing `pop_create-8.1.0.tar` & `pop_create-8.1.1.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 18:18:58.000000 pop_create-8.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-31 18:18:58.000000 pop_create-8.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4372 2023-07-31 18:19:13.567263 pop_create-8.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3278 2023-07-31 18:18:58.000000 pop_create-8.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.559263 pop_create-8.1.0/pop_create/pop_create/cicd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1322 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     5546 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
--rw-r--r--   0 root         (0) root         (0)    13448 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/
--rw-r--r--   0 root         (0) root         (0)      220 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/modindex-note.rst
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/reference-toc-template.rst
--rw-r--r--   0 root         (0) root         (0)    11003 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      881 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      194 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/py-modindex.rst
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/sitevars.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/license.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/example.rst
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)     4809 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/hooks/
--rw-r--r--   0 root         (0) root         (0)      473 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2459 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore
--rw-r--r--   0 root         (0) root         (0)      366 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    10301 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    11375 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/run.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)     1243 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/scripts.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      908 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.559263 pop_create-8.1.0/pop_create/pop_create/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)      899 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/hooks/post_gen_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/tests.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.559263 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)      881 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      166 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/test_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      766 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      305 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/test_init.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/tool/
--rw-r--r--   0 root         (0) root         (0)     2119 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/tool/path.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4372 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3355 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 18:19:13.567263 pop_create-8.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2814 2023-07-31 18:18:58.000000 pop_create-8.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-07 12:10:19.000000 pop_create-8.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-08-07 12:10:19.000000 pop_create-8.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-08-07 12:10:33.949828 pop_create-8.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-08-07 12:10:19.000000 pop_create-8.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/cicd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)      112 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.brokignore
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     5546 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
+-rw-r--r--   0 root         (0) root         (0)    13512 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/docs/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/modindex-note.rst
+-rw-r--r--   0 root         (0) root         (0)      112 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/reference-toc-template.rst
+-rw-r--r--   0 root         (0) root         (0)    11003 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      881 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      194 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/py-modindex.rst
+-rw-r--r--   0 root         (0) root         (0)       64 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/sitevars.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      227 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/license.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/example.rst
+-rw-r--r--   0 root         (0) root         (0)       76 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)      139 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)     4809 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/seed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/seed/hooks/
+-rw-r--r--   0 root         (0) root         (0)      473 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      366 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    10301 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    11375 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/run.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py
+-rw-r--r--   0 root         (0) root         (0)      188 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/scripts.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      908 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)      899 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/tests/hooks/post_gen_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)      881 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      166 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/test_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      766 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/test_init.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.949828 pop_create-8.1.1/pop_create/tool/
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-08-07 12:10:19.000000 pop_create-8.1.1/pop_create/tool/path.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-07 12:10:33.000000 pop_create-8.1.1/pop_create/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:10:33.945829 pop_create-8.1.1/pop_create.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-08-07 12:10:33.000000 pop_create-8.1.1/pop_create.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-08-07 12:10:33.000000 pop_create-8.1.1/pop_create.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 12:10:33.000000 pop_create-8.1.1/pop_create.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-07 12:10:33.000000 pop_create-8.1.1/pop_create.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-08-07 12:10:33.000000 pop_create-8.1.1/pop_create.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-07 12:10:33.000000 pop_create-8.1.1/pop_create.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-07 12:10:33.949828 pop_create-8.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-08-07 12:10:19.000000 pop_create-8.1.1/setup.py
```

### Comparing `pop_create-8.1.0/LICENSE` & `pop_create-8.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/PKG-INFO` & `pop_create-8.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop_create
-Version: 8.1.0
+Version: 8.1.1
 Summary: Create new pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-create/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-create
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-create/issues
```

### Comparing `pop_create-8.1.0/README.rst` & `pop_create-8.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/conf.py` & `pop_create-8.1.1/pop_create/conf.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc` & `pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml` & `pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,25 @@
   - pre-commit
   - test-suite
   - pkg
   - pop-release
 
 include:
   - project: saltstack/pop/cicd/ci-templates
+    file: /docswork/url-tester-brok.yml
+  - project: saltstack/pop/cicd/ci-templates
     file: /lint/pre-commit-run-all.yml
   - project: saltstack/pop/cicd/ci-templates
     file: /release/pop_release.yml
+  - project: saltstack/pop/cicd/ci-templates
+    file: /docswork/build-docs-html-nox.yml
+  - project: saltstack/pop/cicd/ci-templates
+    file: /docswork/publish-docs-gitlab.yml
+  - project: saltstack/pop/cicd/ci-templates
+    file: /docswork/publish-docs-release.yml
 
 variables:
   # TODO If your upstream gitlab url is "gitlab.com/my/upstream/path"
   # Then your CICD_UPSTREAM_PATH would be my/upstream/path"
   # Set this variable for the bot to release this project on Pypi on tag
   CICD_UPSTREAM_PATH: ""
```

### Comparing `pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml` & `pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py` & `pop_create-8.1.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
             sub_dirs = [
                 f.path
                 for f in os.scandir(f"{base_modules_dir}/{dir_target}")
                 if f.is_dir()
             ]
 
             # Include all functions that might be defined in the base directory
+            sub_dirs.append(f"{base_modules_dir}/{dir_target}")
             sub_dirs.append(f"{base_modules_dir}/{dir_type}")
 
             # Generate docs/ref dir tree
             for sub_dir in sub_dirs:
                 module_dir = sub_dir.split("/")[-1]
                 if module_dir in skip_dir_config:
                     continue
```

### Comparing `pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py` & `pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst` & `pop_create-8.1.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 .. toctree::
    :maxdepth: 2
    :glob:
    :hidden:
 
    tutorial/index
 
+.. include:: /_includes/reference-toc.rst
+
 .. toctree::
    :caption: Get Involved
    :maxdepth: 2
    :glob:
    :hidden:
 
    topics/contributing
    topics/license
 
-.. include:: /_includes/reference-toc.rst
-
 .. todo:: Validate Project Repository URL
    Project Repository <https://gitlab.com/{{cookiecutter.author}}/{{cookiecutter.project_name}}/>
 
 .. toctree::
    :caption: Links
    :hidden:
```

### Comparing `pop_create-8.1.0/pop_create/pop_create/init.py` & `pop_create-8.1.1/pop_create/pop_create/init.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore` & `pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst` & `pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE` & `pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst` & `pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py` & `pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py` & `pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py` & `pop_create-8.1.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/tests/hooks/post_gen_project.py` & `pop_create-8.1.1/pop_create/pop_create/tests/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop_create-8.1.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create/tool/path.py` & `pop_create-8.1.1/pop_create/tool/path.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.1.0/pop_create.egg-info/PKG-INFO` & `pop_create-8.1.1/pop_create.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create
-Version: 8.1.0
+Version: 8.1.1
 Summary: Create new pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-create/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-create
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-create/issues
```

### Comparing `pop_create-8.1.0/pop_create.egg-info/SOURCES.txt` & `pop_create-8.1.1/pop_create.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pop_create.egg-info/PKG-INFO
 pop_create.egg-info/SOURCES.txt
 pop_create.egg-info/dependency_links.txt
 pop_create.egg-info/entry_points.txt
 pop_create.egg-info/requires.txt
 pop_create.egg-info/top_level.txt
 pop_create/pop_create/init.py
+pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.brokignore
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
 pop_create/pop_create/docs/init.py
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
```

### Comparing `pop_create-8.1.0/setup.py` & `pop_create-8.1.1/setup.py`

 * *Files identical despite different names*

