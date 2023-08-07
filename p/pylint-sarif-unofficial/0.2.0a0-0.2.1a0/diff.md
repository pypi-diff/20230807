# Comparing `tmp/pylint_sarif_unofficial-0.2.0a0.tar.gz` & `tmp/pylint_sarif_unofficial-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_sarif_unofficial-0.2.0a0.tar", max compression
+gzip compressed data, was "pylint_sarif_unofficial-0.2.1a0.tar", max compression
```

## Comparing `pylint_sarif_unofficial-0.2.0a0.tar` & `pylint_sarif_unofficial-0.2.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0a0/LICENSE
--rw-r--r--   0        0        0     2597 2023-07-16 05:19:07.265949 pylint_sarif_unofficial-0.2.0a0/README.md
--rw-r--r--   0        0        0     1121 2023-07-16 05:19:07.265949 pylint_sarif_unofficial-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0   110930 2023-07-15 23:25:17.669142 pylint_sarif_unofficial-0.2.0a0/sarif-schema.json
--rwxr-xr-x   0        0        0     4060 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0a0/src/pylint2cso.py
--rwxr-xr-x   0        0        0    13050 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0a0/src/pylint2sarif.py
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 pylint_sarif_unofficial-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.1a0/LICENSE
+-rw-r--r--   0        0        0     2699 2023-08-07 03:57:39.206625 pylint_sarif_unofficial-0.2.1a0/README.md
+-rw-r--r--   0        0        0     1098 2023-08-07 03:57:39.206625 pylint_sarif_unofficial-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0   110930 2023-07-15 23:25:17.669142 pylint_sarif_unofficial-0.2.1a0/sarif-schema.json
+-rwxr-xr-x   0        0        0     4060 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.1a0/src/pylint2cso.py
+-rwxr-xr-x   0        0        0    13050 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.1a0/src/pylint2sarif.py
+-rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 pylint_sarif_unofficial-0.2.1a0/PKG-INFO
```

### Comparing `pylint_sarif_unofficial-0.2.0a0/LICENSE` & `pylint_sarif_unofficial-0.2.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0a0/README.md` & `pylint_sarif_unofficial-0.2.1a0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 [the `pylint-sarif` project](https://github.com/GrammaTech/pylint-sarif).** Most
 code here was written by the original GrammaTech developers, but they are not
 responsible for any bugs.
 
 This is on PyPI as
 [`pylint-sarif-unofficial`](https://pypi.org/project/pylint-sarif-unofficial/).
 
-This does not currently support
-[jsonschema](https://github.com/python-jsonschema/jsonschema) 4.18
-([bug #19](https://github.com/EliahKagan/pylint-sarif/issues/19)). To avoid
-holding your project's `jsonschema` version (if it uses it) back, I suggest
-installing `pylint-sarif-unofficial` using `pipx` instead of listing it in
-your project's manifest file. You can put a command like this in your pylint CI
-workflow:
+This uses
+[python-jsonschema-objects](http://python-jsonschema-objects.readthedocs.org/),
+which [does not currently
+support](https://github.com/cwacek/python-jsonschema-objects/issues/235)
+version 4.18 of [jsonschema](https://github.com/python-jsonschema/jsonschema).
+To avoid holding your project's `jsonschema` version (if it uses it) back, I
+suggest installing `pylint-sarif-unofficial` using `pipx` instead of listing it
+in your project's manifest file. You can put a command like this in your pylint
+CI workflow:
 
 ```bash
 pipx install pylint-sarif-unofficial
 ```
 
 Or with the specific version you want, for example:
 
 ```bash
-pipx install pylint-sarif-unofficial==0.2.0
+pipx install pylint-sarif-unofficial==0.2.1
 ```
 
 Your project can still install `pylint` itself as a development dependency.
 
 The [`LICENSE`](https://github.com/EliahKagan/pylint-sarif/blob/develop/LICENSE)
 is the same as in the upstream project. The original project readme follows
 below.
```

### Comparing `pylint_sarif_unofficial-0.2.0a0/pyproject.toml` & `pylint_sarif_unofficial-0.2.1a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-sarif-unofficial"
-version = "0.2.0a0"
+version = "0.2.1a0"
 description = "Pylint output as SARIF"
 authors = []
 maintainers = ["Eliah Kagan <degeneracypressure@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/EliahKagan/pylint-sarif"
 repository = "https://github.com/EliahKagan/pylint-sarif"
@@ -19,19 +19,18 @@
     { include = "pylint2cso.py", from = "src" },
     { include = "pylint2sarif.py", from = "src" },
 ]
 include = ["sarif-schema.json"]  # TODO: Do this better (maybe via data_files).
 
 [tool.poetry.dependencies]
 python = "^3.7"
-jsonschema = "~4.17.3"
-python-jsonschema-objects = "^0.4.2"
+python-jsonschema-objects = "^0.4.4"
 
 [tool.poetry.group.dev.dependencies]
-pylint = { version = "^2.17.4", python = ">=3.7.2,<4.0" }
+pylint = { version = "^2.17.5", python = ">=3.7.2,<4.0" }
 
 [tool.poetry.scripts]
 pylint2cso = "pylint2cso:main"
 pylint2sarif = "pylint2sarif:main"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pylint_sarif_unofficial-0.2.0a0/sarif-schema.json` & `pylint_sarif_unofficial-0.2.1a0/sarif-schema.json`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0a0/src/pylint2cso.py` & `pylint_sarif_unofficial-0.2.1a0/src/pylint2cso.py`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0a0/src/pylint2sarif.py` & `pylint_sarif_unofficial-0.2.1a0/src/pylint2sarif.py`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0a0/PKG-INFO` & `pylint_sarif_unofficial-0.2.1a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-sarif-unofficial
-Version: 0.2.0a0
+Version: 0.2.1a0
 Summary: Pylint output as SARIF
 Home-page: https://github.com/EliahKagan/pylint-sarif
 License: MIT
 Keywords: pylint,sarif
 Maintainer: Eliah Kagan
 Maintainer-email: degeneracypressure@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -15,43 +15,44 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Dist: jsonschema (>=4.17.3,<4.18.0)
-Requires-Dist: python-jsonschema-objects (>=0.4.2,<0.5.0)
+Requires-Dist: python-jsonschema-objects (>=0.4.4,<0.5.0)
 Project-URL: Repository, https://github.com/EliahKagan/pylint-sarif
 Description-Content-Type: text/markdown
 
 **This is [an unofficial fork](https://github.com/EliahKagan/pylint-sarif) of
 [the `pylint-sarif` project](https://github.com/GrammaTech/pylint-sarif).** Most
 code here was written by the original GrammaTech developers, but they are not
 responsible for any bugs.
 
 This is on PyPI as
 [`pylint-sarif-unofficial`](https://pypi.org/project/pylint-sarif-unofficial/).
 
-This does not currently support
-[jsonschema](https://github.com/python-jsonschema/jsonschema) 4.18
-([bug #19](https://github.com/EliahKagan/pylint-sarif/issues/19)). To avoid
-holding your project's `jsonschema` version (if it uses it) back, I suggest
-installing `pylint-sarif-unofficial` using `pipx` instead of listing it in
-your project's manifest file. You can put a command like this in your pylint CI
-workflow:
+This uses
+[python-jsonschema-objects](http://python-jsonschema-objects.readthedocs.org/),
+which [does not currently
+support](https://github.com/cwacek/python-jsonschema-objects/issues/235)
+version 4.18 of [jsonschema](https://github.com/python-jsonschema/jsonschema).
+To avoid holding your project's `jsonschema` version (if it uses it) back, I
+suggest installing `pylint-sarif-unofficial` using `pipx` instead of listing it
+in your project's manifest file. You can put a command like this in your pylint
+CI workflow:
 
 ```bash
 pipx install pylint-sarif-unofficial
 ```
 
 Or with the specific version you want, for example:
 
 ```bash
-pipx install pylint-sarif-unofficial==0.2.0
+pipx install pylint-sarif-unofficial==0.2.1
 ```
 
 Your project can still install `pylint` itself as a development dependency.
 
 The [`LICENSE`](https://github.com/EliahKagan/pylint-sarif/blob/develop/LICENSE)
 is the same as in the upstream project. The original project readme follows
 below.
```

