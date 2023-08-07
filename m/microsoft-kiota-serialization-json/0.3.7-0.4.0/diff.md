# Comparing `tmp/microsoft_kiota_serialization_json-0.3.7.tar.gz` & `tmp/microsoft_kiota_serialization_json-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_serialization_json-0.3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_serialization_json-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_serialization_json-0.3.7.tar` & `microsoft_kiota_serialization_json-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0       82 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1874 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.gitignore
--rw-r--r--   0        0        0    15976 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.pylintrc
--rw-r--r--   0        0        0     1362 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/LICENSE
--rw-r--r--   0        0        0     1146 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/Pipfile
--rw-r--r--   0        0        0    71082 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/Pipfile.lock
--rw-r--r--   0        0        0     2545 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/README.md
--rw-r--r--   0        0        0     2757 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    11570 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1433 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    16603 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1344 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      909 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/__init__.py
--rw-r--r--   0        0        0      119 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1569 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/entity.py
--rw-r--r--   0        0        0     2692 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/intersection_type.py
--rw-r--r--   0        0        0       94 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/office_location.py
--rw-r--r--   0        0        0     3077 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/union_type.py
--rw-r--r--   0        0        0     3133 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/user.py
--rw-r--r--   0        0        0     2151 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/user2.py
--rw-r--r--   0        0        0        0 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/__init__.py
--rw-r--r--   0        0        0     1554 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/conftest.py
--rw-r--r--   0        0        0     5236 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_intersection_wrapper.py
--rw-r--r--   0        0        0     4123 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1679 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0     7188 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1018 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     5873 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_union_wrapper.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1787 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.gitignore
+-rw-r--r--   0        0        0    15976 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/.pylintrc
+-rw-r--r--   0        0        0     1443 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/LICENSE
+-rw-r--r--   0        0        0    71086 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/README.md
+-rw-r--r--   0        0        0     2757 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2023-08-07 11:21:37.750280 microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    12030 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1433 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    17120 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1344 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      798 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      119 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1569 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/helpers/entity.py
+-rw-r--r--   0        0        0     2692 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/helpers/intersection_type.py
+-rw-r--r--   0        0        0       94 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     3077 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/helpers/union_type.py
+-rw-r--r--   0        0        0     3133 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/helpers/user.py
+-rw-r--r--   0        0        0     2151 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/helpers/user2.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1554 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     5236 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/test_intersection_wrapper.py
+-rw-r--r--   0        0        0     4123 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1679 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0     7188 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1018 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     5873 2023-08-07 11:21:37.754280 microsoft_kiota_serialization_json-0.4.0/tests/unit/test_union_wrapper.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.4.0/PKG-INFO
```

### Comparing `microsoft_kiota_serialization_json-0.3.7/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_serialization_json-0.4.0/.github/workflows/auto-merge-dependabot.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/.github/workflows/build_publish.yml` & `microsoft_kiota_serialization_json-0.4.0/.github/workflows/build_publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -19,31 +19,30 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pipenv
-          pipenv install -r requirements-dev.txt
+          pip install -r requirements-dev.txt
       - name: Check code format
         run: |
-          pipenv run yapf -dr kiota_serialization_json
+          yapf -dr kiota_serialization_json
       - name: Check import order
         run: |
-          pipenv run isort kiota_serialization_json
+          isort kiota_serialization_json
       - name: Lint with Pylint
         run: |
-          pipenv run pylint kiota_serialization_json --disable=W --rcfile=.pylintrc
+          pylint kiota_serialization_json --disable=W --rcfile=.pylintrc
       - name: Static type checking with Mypy
         run: |
-          pipenv run mypy kiota_serialization_json
+          mypy kiota_serialization_json
       - name: Run tests with Pytest
         run: |
-          pipenv run pytest
+          pytest
 
   publish:
     name: Publish distribution to PyPI
     if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
     runs-on: ubuntu-latest
     environment: pypi_prod
     needs: [build]
```

### Comparing `microsoft_kiota_serialization_json-0.3.7/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_serialization_json-0.4.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_serialization_json-0.4.0/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/.gitignore` & `microsoft_kiota_serialization_json-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/.pylintrc` & `microsoft_kiota_serialization_json-0.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/CHANGELOG.md` & `microsoft_kiota_serialization_json-0.4.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] - 2023-07-27
+
+### Added
+
+### Changed
+- Enabled backing store support
+
 ## [0.3.7] - 2023-07-04
 
 ### Added
 
 ### Changed
 - Fixes the key assignment to the writer in write_bytes_value.
```

### Comparing `microsoft_kiota_serialization_json-0.3.7/LICENSE` & `microsoft_kiota_serialization_json-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/Pipfile.lock` & `microsoft_kiota_serialization_json-0.4.0/Pipfile.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9709353146853146%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'ab95a5e17fc4dbf62dc0e1490a711ce8ac82f479fa805b649580be8815a61a26'}}",*

 * * "'default'": "{'astroid': {'hashes': "*

 * *              "['sha256:389656ca57b6108f939cf5d2f9a2a825a3be50ba9d589670f393236e0a03b91c', "*

 * *              "'sha256:903f024859b7c7687d7a7f3a3f73b17301f8e42dfd9cc9df9d4418172d3e2dbd'], "*

 * *              "'version': '==2.15.6'}, 'certifi': {'hashes': "*

 * *              "['sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082', "*

 * *            […]*

```diff
@@ -1,119 +1,119 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "b144c90232a6fe4dc73700fa35a8a3c4ed0bdc58cab58f6af5559a8aa99fcd01"
+            "sha256": "ab95a5e17fc4dbf62dc0e1490a711ce8ac82f479fa805b649580be8815a61a26"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "astroid": {
             "hashes": [
-                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
-                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
+                "sha256:389656ca57b6108f939cf5d2f9a2a825a3be50ba9d589670f393236e0a03b91c",
+                "sha256:903f024859b7c7687d7a7f3a3f73b17301f8e42dfd9cc9df9d4418172d3e2dbd"
             ],
             "index": "pypi",
-            "version": "==2.15.5"
+            "version": "==2.15.6"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "index": "pypi",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "index": "pypi",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "index": "pypi",
@@ -186,19 +186,19 @@
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
             "version": "==7.2.7"
         },
         "dill": {
             "hashes": [
-                "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
-                "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
+                "sha256:76b122c08ef4ce2eedcd4d1abd8e641114bfc6c2867f49f3c41facf65bf19f5e",
+                "sha256:cc1c8b182eb3013e24bd475ff2e9295af86c1a38eb1aff128dac8962a9ce3c03"
             ],
             "index": "pypi",
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "docutils": {
             "hashes": [
                 "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "index": "pypi",
@@ -234,19 +234,19 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "index": "pypi",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
-                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
+                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==6.7.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==6.8.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "index": "pypi",
@@ -364,35 +364,35 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "index": "pypi",
             "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
-                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
+                "sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d",
+                "sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d"
             ],
             "index": "pypi",
-            "version": "==3.8.0"
+            "version": "==3.10.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "index": "pypi",
             "version": "==1.2.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
-                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
+                "sha256:73995fb8216d3bed149c8d51bba25b2c52a8251a2c8ac846ec668ce38fab5413",
+                "sha256:f7b601cbc06fef7e62a754e2b41294c2aa31f1cb659624b9a85bcba29eaf8252"
             ],
             "index": "pypi",
-            "version": "==2.17.4"
+            "version": "==2.17.5"
         },
         "pytest": {
             "hashes": [
                 "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
                 "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
@@ -452,27 +452,27 @@
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "index": "pypi",
             "version": "==1.0.0"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
-                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
+                "sha256:38e1ff8edb991273ec9f6181244a6a391ac30e9f5098e7535640ea6be97a7c86",
+                "sha256:712cbd236609acc6a3e2e97253dfc52d4c2082982a88f61b640ecf0817eab899"
             ],
             "index": "pypi",
-            "version": "==0.11.8"
+            "version": "==0.12.1"
         },
         "types-python-dateutil": {
             "hashes": [
-                "sha256:09a0275f95ee31ce68196710ed2c3d1b9dc42e0b61cc43acc369a42cb939134f",
-                "sha256:0b0e7c68e7043b0354b26a1e0225cb1baea7abb1b324d02b50e2d08f1221043f"
+                "sha256:1f4f10ac98bb8b16ade9dbee3518d9ace017821d94b057a425b069f834737f4b",
+                "sha256:f977b8de27787639986b4e28963263fd0e5158942b3ecef91b9335c130cb1ce9"
             ],
             "index": "pypi",
-            "version": "==2.8.19.13"
+            "version": "==2.8.19.14"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
                 "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "index": "pypi",
@@ -484,19 +484,19 @@
                 "sha256:830c08b8d99bdd312ea4ead05994a38e8936266f84b9a7878232db50b044e02e"
             ],
             "index": "pypi",
             "version": "==4.1.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
-                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
+                "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
+                "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
             "index": "pypi",
-            "version": "==2.0.3"
+            "version": "==2.0.4"
         },
         "wrapt": {
             "hashes": [
                 "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
                 "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
                 "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
                 "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
@@ -581,118 +581,118 @@
                 "sha256:b8bfc1f280949153e795181768ca14ef43d7312629a06c43e7abd279323af313"
             ],
             "index": "pypi",
             "version": "==0.40.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.2"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
-                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
+                "sha256:389656ca57b6108f939cf5d2f9a2a825a3be50ba9d589670f393236e0a03b91c",
+                "sha256:903f024859b7c7687d7a7f3a3f73b17301f8e42dfd9cc9df9d4418172d3e2dbd"
             ],
             "index": "pypi",
-            "version": "==2.15.5"
+            "version": "==2.15.6"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "index": "pypi",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "index": "pypi",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
                 "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
@@ -757,19 +757,19 @@
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
             "version": "==7.2.7"
         },
         "dill": {
             "hashes": [
-                "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
-                "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
+                "sha256:76b122c08ef4ce2eedcd4d1abd8e641114bfc6c2867f49f3c41facf65bf19f5e",
+                "sha256:cc1c8b182eb3013e24bd475ff2e9295af86c1a38eb1aff128dac8962a9ce3c03"
             ],
             "index": "pypi",
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "docutils": {
             "hashes": [
                 "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "index": "pypi",
@@ -797,19 +797,19 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "index": "pypi",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
-                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
+                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==6.7.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==6.8.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "index": "pypi",
@@ -919,35 +919,35 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "index": "pypi",
             "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
-                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
+                "sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d",
+                "sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d"
             ],
             "index": "pypi",
-            "version": "==3.8.0"
+            "version": "==3.10.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "index": "pypi",
             "version": "==1.2.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
-                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
+                "sha256:73995fb8216d3bed149c8d51bba25b2c52a8251a2c8ac846ec668ce38fab5413",
+                "sha256:f7b601cbc06fef7e62a754e2b41294c2aa31f1cb659624b9a85bcba29eaf8252"
             ],
             "index": "pypi",
-            "version": "==2.17.4"
+            "version": "==2.17.5"
         },
         "pytest": {
             "hashes": [
                 "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
                 "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
@@ -991,43 +991,43 @@
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "index": "pypi",
             "version": "==1.0.0"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
-                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
+                "sha256:38e1ff8edb991273ec9f6181244a6a391ac30e9f5098e7535640ea6be97a7c86",
+                "sha256:712cbd236609acc6a3e2e97253dfc52d4c2082982a88f61b640ecf0817eab899"
             ],
             "index": "pypi",
-            "version": "==0.11.8"
+            "version": "==0.12.1"
         },
         "types-python-dateutil": {
             "hashes": [
-                "sha256:09a0275f95ee31ce68196710ed2c3d1b9dc42e0b61cc43acc369a42cb939134f",
-                "sha256:0b0e7c68e7043b0354b26a1e0225cb1baea7abb1b324d02b50e2d08f1221043f"
+                "sha256:1f4f10ac98bb8b16ade9dbee3518d9ace017821d94b057a425b069f834737f4b",
+                "sha256:f977b8de27787639986b4e28963263fd0e5158942b3ecef91b9335c130cb1ce9"
             ],
             "index": "pypi",
-            "version": "==2.8.19.13"
+            "version": "==2.8.19.14"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
                 "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "index": "pypi",
             "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
-                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
+                "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
+                "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
             "index": "pypi",
-            "version": "==2.0.3"
+            "version": "==2.0.4"
         },
         "wrapt": {
             "hashes": [
                 "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
                 "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
                 "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
                 "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
@@ -1112,15 +1112,15 @@
                 "sha256:b8bfc1f280949153e795181768ca14ef43d7312629a06c43e7abd279323af313"
             ],
             "index": "pypi",
             "version": "==0.40.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.2"
         }
     }
 }
```

### Comparing `microsoft_kiota_serialization_json-0.3.7/README.md` & `microsoft_kiota_serialization_json-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/SECURITY.md` & `microsoft_kiota_serialization_json-0.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/SUPPORT.md` & `microsoft_kiota_serialization_json-0.4.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node.py` & `microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_parse_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,37 +15,36 @@
 U = TypeVar("U", bound=Parsable)
 
 K = TypeVar("K", bound=Enum)
 
 
 class JsonParseNode(ParseNode, Generic[T, U]):
 
-    on_before_assign_field_values: Optional[Callable[[Parsable], None]] = None
-    on_after_assign_field_values: Optional[Callable[[Parsable], None]] = None
-
     def __init__(self, node: Any) -> None:
         """
         Args:
             node (Any): The JsonElement\
                 to initialize the node with
         """
         self._json_node = node
+        self._on_before_assign_field_values: Optional[Callable[[Parsable], None]] = None
+        self._on_after_assign_field_values: Optional[Callable[[Parsable], None]] = None
 
     def get_child_node(self, identifier: str) -> Optional[ParseNode]:
         """Gets a new parse node for the given identifier
         Args:
             identifier (str): The identifier of the current node property
         Returns:
             Optional[ParseNode]: A new parse node for the given identifier
         """
         if not identifier:
             raise ValueError("identifier cannot be None or empty.")
 
         if isinstance(node := self._json_node, dict) and identifier in node:
-            return JsonParseNode(node[identifier])
+            return self._create_new_node(node[identifier])
         return None
 
     def get_str_value(self) -> Optional[str]:
         """Gets the string value from the json node
         Returns:
             str: The string value of the node
         """
@@ -138,15 +137,15 @@
             List[T]: The collection of primitive values
         """
 
         primitive_types = {bool, str, int, float, UUID, datetime, timedelta, date, time, bytes}
 
         def func(item):
             generic_type = primitive_type if primitive_type else type(item)
-            current_parse_node = JsonParseNode(item)
+            current_parse_node = self._create_new_node(item)
             if generic_type in primitive_types:
                 method = getattr(current_parse_node, f'get_{generic_type.__name__.lower()}_value')
                 return method()
             raise Exception(f"Encountered an unknown type during deserialization {generic_type}")
 
         if isinstance(self._json_node, str):
             return list(map(func, json.loads(self._json_node)))
@@ -156,27 +155,29 @@
         """Gets the collection of type U values from the json node
         Returns:
             List[U]: The collection of model object values of the node
         """
         if isinstance(self._json_node, list):
             return list(
                 map(
-                    lambda x: JsonParseNode(x).get_object_value(factory),  # type: ignore
+                    lambda x: self._create_new_node(x).get_object_value(factory),  # type: ignore
                     self._json_node,
                 )
             )
         return []
 
     def get_collection_of_enum_values(self, enum_class: K) -> List[Optional[K]]:
         """Gets the collection of enum values of the json node
         Returns:
             List[K]: The collection of enum values
         """
         if isinstance(self._json_node, list):
-            return list(map(lambda x: JsonParseNode(x).get_enum_value(enum_class), self._json_node))
+            return list(
+                map(lambda x: self._create_new_node(x).get_enum_value(enum_class), self._json_node)
+            )
         return []
 
     def get_enum_value(self, enum_class: K) -> Optional[K]:
         """Gets the enum value of the node
         Returns:
             Optional[K]: The enum value of the node
         """
@@ -199,60 +200,64 @@
     def get_object_value(self, factory: ParsableFactory) -> U:
         """Gets the model object value of the node
         Returns:
             Parsable: The model object value of the node
         """
 
         result = factory.create_from_discriminator_value(self)
-        if self.on_before_assign_field_values:
-            self.on_before_assign_field_values(result)
+        if on_before := self.on_before_assign_field_values:
+            on_before(result)
         self._assign_field_values(result)
-        if self.on_after_assign_field_values:
-            self.on_after_assign_field_values(result)
+        if on_after := self.on_after_assign_field_values:
+            on_after(result)
         return result
 
     def get_bytes_value(self) -> Optional[bytes]:
         """Get a bytearray value from the nodes
         Returns:
             bytearray: The bytearray value from the nodes
         """
         base64_string = str(self._json_node)
         if not base64_string:
             return None
         return base64_string.encode("utf-8")
 
-    def get_on_before_assign_field_values(self) -> Optional[Callable[[Parsable], None]]:
-        """Gets the callback called before the node is deserialized.
-        Returns:
-            Callable[[Parsable], None]: the callback called before the node is deserialized.
-        """
-        return self.on_before_assign_field_values
-
-    def get_on_after_assign_field_values(self) -> Optional[Callable[[Parsable], None]]:
+    @property
+    def on_before_assign_field_values(self) -> Optional[Callable[[Parsable], None]]:
         """Gets the callback called before the node is deserialized.
         Returns:
             Callable[[Parsable], None]: the callback called before the node is deserialized.
         """
-        return self.on_after_assign_field_values
+        return self._on_before_assign_field_values
 
-    def set_on_before_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
+    @on_before_assign_field_values.setter
+    def on_before_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
         """Sets the callback called before the node is deserialized.
         Args:
             value (Callable[[Parsable], None]): the callback called before the node is
             deserialized.
         """
-        self.on_before_assign_field_values = value
+        self._on_before_assign_field_values = value
 
-    def set_on_after_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
+    @property
+    def on_after_assign_field_values(self) -> Optional[Callable[[Parsable], None]]:
+        """Gets the callback called before the node is deserialized.
+        Returns:
+            Callable[[Parsable], None]: the callback called before the node is deserialized.
+        """
+        return self._on_after_assign_field_values
+
+    @on_after_assign_field_values.setter
+    def on_after_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
         """Sets the callback called after the node is deserialized.
         Args:
             value (Callable[[Parsable], None]): the callback called after the node is
             deserialized.
         """
-        self.on_after_assign_field_values = value
+        self._on_after_assign_field_values = value
 
     def _assign_field_values(self, item: U) -> None:
         """Assigns the field values to the model object"""
 
         # if object is null
         if not isinstance(self._json_node, dict):
             return
@@ -302,7 +307,13 @@
                 pass
             try:
                 return UUID(value)
             except ValueError:
                 pass
             return value
         raise ValueError(f"Unexpected additional value type {type(value)} during deserialization.")
+
+    def _create_new_node(self, node: Any) -> JsonParseNode:
+        new_node: JsonParseNode = JsonParseNode(node)
+        new_node.on_before_assign_field_values = self.on_before_assign_field_values
+        new_node.on_after_assign_field_values = self.on_after_assign_field_values
+        return new_node
```

### Comparing `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_serialization_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 U = TypeVar("U", bound=Parsable)
 
 
 class JsonSerializationWriter(SerializationWriter):
 
     PROPERTY_SEPARATOR: str = ','
 
-    _on_start_object_serialization: Optional[Callable[[Parsable, SerializationWriter], None]] = None
-
-    _on_before_object_serialization: Optional[Callable[[Parsable], None]] = None
-
-    _on_after_object_serialization: Optional[Callable[[Parsable], None]] = None
-
     def __init__(self) -> None:
         self.writer: Dict = {}
         self.value: Any = None
 
+        self._on_start_object_serialization: Optional[Callable[[Parsable, SerializationWriter],
+                                                               None]] = None
+        self._on_before_object_serialization: Optional[Callable[[Parsable], None]] = None
+        self._on_after_object_serialization: Optional[Callable[[Parsable], None]] = None
+
     def write_str_value(self, key: Optional[str], value: Optional[str]) -> None:
         """Writes the specified string value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[str]): The string value to be written.
         """
         if isinstance(value, str):
@@ -143,15 +142,15 @@
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             values (Optional[List[T]]): The collection of primitive values to be written.
         """
         if isinstance(values, list):
             result = []
             for val in values:
-                temp_writer = JsonSerializationWriter()
+                temp_writer = self._create_new_writer()
                 temp_writer.write_any_value(None, val)
                 result.append(temp_writer.value)
 
             if key:
                 self.writer[key] = result
             else:
                 self.value = result
@@ -164,15 +163,15 @@
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             values (Optional[List[U]]): The collection of model objects to be written.
         """
         if isinstance(values, list):
             obj_list = []
             for val in values:
-                temp_writer = JsonSerializationWriter()
+                temp_writer = self._create_new_writer()
                 temp_writer.write_object_value(None, val)
                 obj_list.append(temp_writer.value)
 
             if key:
                 self.writer[key] = obj_list
             else:
                 self.value = obj_list
@@ -184,15 +183,15 @@
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             values Optional[List[Enum]): The enum values to be written.
         """
         if isinstance(values, list):
             result = []
             for val in values:
-                temp_writer = JsonSerializationWriter()
+                temp_writer = self._create_new_writer()
                 temp_writer.write_enum_value(None, val)
                 result.append(temp_writer.value)
 
             if key:
                 self.writer[key] = result
             else:
                 self.value = result
@@ -219,24 +218,24 @@
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Parsable): The model object to be written.
             additional_values_to_merge (tuple[Parsable]): The additional values to merge to the
             main value when serializing an intersection wrapper.
         """
         if value or additional_values_to_merge:
-            temp_writer = JsonSerializationWriter()
+            temp_writer = self._create_new_writer()
 
             if value:
                 self._serialize_value(temp_writer, value)
 
             if additional_values_to_merge:
                 for additional_value in filter(lambda x: x is not None, additional_values_to_merge):
                     self._serialize_value(temp_writer, additional_value)
-                    if self._on_after_object_serialization:
-                        self._on_after_object_serialization(additional_value)
+                    if on_after := self.on_after_object_serialization:
+                        on_after(additional_value)
 
             if value and self._on_after_object_serialization:
                 self._on_after_object_serialization(value)
 
             if key:
                 self.writer[key] = temp_writer.writer
             else:
@@ -274,76 +273,78 @@
                 self.writer[key] = val
 
     def get_serialized_content(self) -> bytes:
         """Gets the value of the serialized content.
         Returns:
             bytes: The value of the serialized content.
         """
-        if self.writer and self.value is not None:
+        if self.writer and self.value:
             # Json output is invalid if it has a mix of values
             # and key-value pairs.
             raise ValueError("Invalid Json output")
 
         if self.value:
             json_string = json.dumps(self.value)
             self.value = None
         else:
             json_string = json.dumps(self.writer)
             self.writer.clear()
 
         stream = json_string.encode('utf-8')
         return stream
 
-    def get_on_before_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
+    @property
+    def on_before_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
         """Gets the callback called before the object gets serialized.
         Returns:
             Optional[Callable[[Parsable], None]]:the callback called before the object
             gets serialized.
         """
         return self._on_before_object_serialization
 
-    def get_on_after_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
+    @on_before_object_serialization.setter
+    def on_before_object_serialization(self, value: Optional[Callable[[Parsable], None]]) -> None:
+        """Sets the callback called before the objects gets serialized.
+        Args:
+            value (Optional[Callable[[Parsable], None]]): the callback called before the objects
+            gets serialized.
+        """
+        self._on_before_object_serialization = value
+
+    @property
+    def on_after_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
         """Gets the callback called after the object gets serialized.
         Returns:
             Optional[Optional[Callable[[Parsable], None]]]: the callback called after the object
             gets serialized.
         """
         return self._on_after_object_serialization
 
-    def get_on_start_object_serialization(
+    @on_after_object_serialization.setter
+    def on_after_object_serialization(self, value: Optional[Callable[[Parsable], None]]) -> None:
+        """Sets the callback called after the objects gets serialized.
+        Args:
+            value (Optional[Callable[[Parsable], None]]): the callback called after the objects
+            gets serialized.
+        """
+        self._on_after_object_serialization = value
+
+    @property
+    def on_start_object_serialization(
         self
     ) -> Optional[Callable[[Parsable, SerializationWriter], None]]:
         """Gets the callback called right after the serialization process starts.
         Returns:
             Optional[Callable[[Parsable, SerializationWriter], None]]: the callback called
             right after the serialization process starts.
         """
         return self._on_start_object_serialization
 
-    def set_on_before_object_serialization(
-        self, value: Optional[Callable[[Parsable], None]]
-    ) -> None:
-        """Sets the callback called before the objects gets serialized.
-        Args:
-            value (Optional[Callable[[Parsable], None]]): the callback called before the objects
-            gets serialized.
-        """
-        self._on_before_object_serialization = value
-
-    def set_on_after_object_serialization(
-        self, value: Optional[Callable[[Parsable], None]]
-    ) -> None:
-        """Sets the callback called after the objects gets serialized.
-        Args:
-            value (Optional[Callable[[Parsable], None]]): the callback called after the objects
-            gets serialized.
-        """
-        self._on_after_object_serialization = value
-
-    def set_on_start_object_serialization(
+    @on_start_object_serialization.setter
+    def on_start_object_serialization(
         self, value: Optional[Callable[[Parsable, SerializationWriter], None]]
     ) -> None:
         """Sets the callback called right after the serialization process starts.
         Args:
             value (Optional[Callable[[Parsable, SerializationWriter], None]]): the callback
             called right after the serialization process starts.
         """
@@ -393,12 +394,19 @@
                     self.write_non_parsable_object_value(None, value)
                 else:
                     raise TypeError(
                         f"Encountered an unknown type during serialization {value_type}"
                     )
 
     def _serialize_value(self, temp_writer: JsonSerializationWriter, value: U):
-        if self._on_before_object_serialization:
-            self._on_before_object_serialization(value)
-        if self._on_start_object_serialization:
-            self._on_start_object_serialization(value, self)
+        if on_before := self.on_before_object_serialization:
+            on_before(value)
+        if on_start := self.on_start_object_serialization:
+            on_start(value, self)
         value.serialize(temp_writer)
+
+    def _create_new_writer(self) -> SerializationWriter:
+        writer = JsonSerializationWriter()
+        writer.on_before_object_serialization = self.on_before_object_serialization
+        writer.on_after_object_serialization = self.on_after_object_serialization
+        writer.on_start_object_serialization = self.on_start_object_serialization
+        return writer
```

### Comparing `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.4.0/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/pyproject.toml` & `microsoft_kiota_serialization_json-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/helpers/entity.py` & `microsoft_kiota_serialization_json-0.4.0/tests/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/helpers/intersection_type.py` & `microsoft_kiota_serialization_json-0.4.0/tests/helpers/intersection_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/helpers/union_type.py` & `microsoft_kiota_serialization_json-0.4.0/tests/helpers/union_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/helpers/user.py` & `microsoft_kiota_serialization_json-0.4.0/tests/helpers/user.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/helpers/user2.py` & `microsoft_kiota_serialization_json-0.4.0/tests/helpers/user2.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/unit/conftest.py` & `microsoft_kiota_serialization_json-0.4.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_intersection_wrapper.py` & `microsoft_kiota_serialization_json-0.4.0/tests/unit/test_intersection_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node.py` & `microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.4.0/tests/unit/test_json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_union_wrapper.py` & `microsoft_kiota_serialization_json-0.4.0/tests/unit/test_union_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.7/PKG-INFO` & `microsoft_kiota_serialization_json-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 0.3.7
+Version: 0.4.0
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

