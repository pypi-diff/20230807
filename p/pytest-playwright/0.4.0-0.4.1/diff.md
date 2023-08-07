# Comparing `tmp/pytest-playwright-0.4.0.tar.gz` & `tmp/pytest-playwright-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-0.4.0.tar", last modified: Mon Aug  7 09:02:44 2023, max compression
+gzip compressed data, was "pytest-playwright-0.4.1.tar", last modified: Mon Aug  7 09:13:15 2023, max compression
```

## Comparing `pytest-playwright-0.4.0.tar` & `pytest-playwright-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.209586 pytest-playwright-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.209586 pytest-playwright-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/local-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/pytest_playwright/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/pytest_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright/_repo_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/pytest_playwright/pytest_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/pytest_playwright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.209586 pytest-playwright-0.4.0/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/tests/assets/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/assets/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/assets/django/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/assets/django/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/test_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.197479 pytest-playwright-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/local-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/pytest_playwright/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/pytest_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 09:13:15.000000 pytest-playwright-0.4.1/pytest_playwright/_repo_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/pytest_playwright/pytest_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/pytest_playwright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-07 09:13:15.000000 pytest-playwright-0.4.1/pytest_playwright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-07 09:13:15.000000 pytest-playwright-0.4.1/pytest_playwright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:13:15.000000 pytest-playwright-0.4.1/pytest_playwright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 09:13:15.000000 pytest-playwright-0.4.1/pytest_playwright.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 09:13:15.000000 pytest-playwright-0.4.1/pytest_playwright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 09:13:15.000000 pytest-playwright-0.4.1/pytest_playwright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.197479 pytest-playwright-0.4.1/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:13:15.201479 pytest-playwright-0.4.1/tests/assets/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/tests/assets/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/tests/assets/django/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/tests/assets/django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-08-07 09:12:52.000000 pytest-playwright-0.4.1/tests/test_playwright.py
```

### Comparing `pytest-playwright-0.4.0/.github/workflows/ci.yml` & `pytest-playwright-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/.github/workflows/python-publish.yml` & `pytest-playwright-0.4.1/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -43,8 +43,8 @@
       - name: Prepare
         run: conda install anaconda-client conda-build conda-verify
       - name: Build and Upload
         env:
           ANACONDA_API_TOKEN: ${{ secrets.ANACONDA_API_TOKEN }}
         run: |
           conda config --set anaconda_upload yes
-          conda build --user microsoft . -c microsoft -c conda-forge
+          conda build --user microsoft . -c microsoft
```

### Comparing `pytest-playwright-0.4.0/.gitignore` & `pytest-playwright-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/.pre-commit-config.yaml` & `pytest-playwright-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/CONTRIBUTING.md` & `pytest-playwright-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/LICENSE` & `pytest-playwright-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/PKG-INFO` & `pytest-playwright-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.4.0
+Version: 0.4.1
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-playwright-0.4.0/README.md` & `pytest-playwright-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/SECURITY.md` & `pytest-playwright-0.4.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/meta.yaml` & `pytest-playwright-0.4.1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/pytest_playwright/pytest_playwright.py` & `pytest-playwright-0.4.1/pytest_playwright/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/pytest_playwright.egg-info/PKG-INFO` & `pytest-playwright-0.4.1/pytest_playwright.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.4.0
+Version: 0.4.1
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-playwright-0.4.0/pytest_playwright.egg-info/SOURCES.txt` & `pytest-playwright-0.4.1/pytest_playwright.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/setup.py` & `pytest-playwright-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/tests/assets/django/settings.py` & `pytest-playwright-0.4.1/tests/assets/django/settings.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/tests/conftest.py` & `pytest-playwright-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.0/tests/test_playwright.py` & `pytest-playwright-0.4.1/tests/test_playwright.py`

 * *Files identical despite different names*

