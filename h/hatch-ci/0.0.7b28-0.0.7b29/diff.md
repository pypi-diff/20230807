# Comparing `tmp/hatch_ci-0.0.7b28.tar.gz` & `tmp/hatch_ci-0.0.7b29.tar.gz`

## Comparing `hatch_ci-0.0.7b28.tar` & `hatch_ci-0.0.7b29.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/.gitattributes
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/.pre-commit-config.yaml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/Makefile
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/.github/workflows/beta.yml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/.github/workflows/master.yml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/.github/workflows/tags.yml
--rw-r--r--   0        0        0    27490 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage.xml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
--rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
--rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
--rw-r--r--   0        0        0    49436 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
--rw-r--r--   0        0        0   115699 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
--rw-r--r--   0        0        0    22969 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/favicon_32.png
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/style.css
--rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/junit/junit.html
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/junit/junit.xml
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/index.html
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/mypy-html.css
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
--rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
--rw-r--r--   0        0        0    30321 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
--rw-r--r--   0        0        0    68104 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
--rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/cli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/script.py
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/tests/test_scm.py
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/LICENSE.txt
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/README.md
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/pyproject.toml
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b28/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/.gitattributes
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/Makefile
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/.github/workflows/master.yml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    49436 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
+-rw-r--r--   0        0        0   115699 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    22969 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    30321 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
+-rw-r--r--   0        0        0    68104 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/script.py
+-rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/tests/test_scm.py
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/LICENSE.txt
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/README.md
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/pyproject.toml
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b29/PKG-INFO
```

### Comparing `hatch_ci-0.0.7b28/.github/workflows/beta.yml` & `hatch_ci-0.0.7b29/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/.github/workflows/master.yml` & `hatch_ci-0.0.7b29/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/.github/workflows/tags.yml` & `hatch_ci-0.0.7b29/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage.xml`

 * *Files 5% similar despite different names*

#### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1691387798509" lines-valid="550" lines-covered="328" line-rate="0.5964" branches-valid="214" branches-covered="130" branch-rate="0.6075" complexity="0">
+<coverage version="7.2.7" timestamp="1691389672354" lines-valid="550" lines-covered="328" line-rate="0.5964" branches-valid="188" branches-covered="112" branch-rate="0.5957" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/hatch-ci/hatch-ci</source>
   </sources>
   <packages>
-    <package name="src.hatch_ci" line-rate="0.5964" branch-rate="0.6075" complexity="0">
+    <package name="src.hatch_ci" line-rate="0.5964" branch-rate="0.5957" complexity="0">
       <classes>
         <class name="__init__.py" filename="src/hatch_ci/__init__.py" complexity="0" line-rate="1" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
           </lines>
@@ -26,15 +26,15 @@
             <line number="7" hits="0"/>
             <line number="9" hits="0"/>
             <line number="12" hits="0"/>
             <line number="13" hits="0"/>
             <line number="14" hits="0"/>
             <line number="17" hits="0"/>
             <line number="18" hits="0"/>
-            <line number="19" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="18,25"/>
+            <line number="19" hits="0"/>
             <line number="20" hits="0"/>
             <line number="21" hits="0"/>
             <line number="22" hits="0"/>
             <line number="23" hits="0"/>
             <line number="25" hits="0"/>
             <line number="32" hits="0"/>
             <line number="33" hits="0"/>
@@ -59,17 +59,17 @@
             <line number="65" hits="0"/>
             <line number="68" hits="0"/>
             <line number="75" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="78,79"/>
             <line number="78" hits="0"/>
             <line number="79" hits="0"/>
             <line number="82" hits="0"/>
             <line number="88" hits="0"/>
-            <line number="89" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="88,136"/>
+            <line number="89" hits="0"/>
             <line number="90" hits="0"/>
-            <line number="91" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="90,134"/>
+            <line number="91" hits="0"/>
             <line number="92" hits="0"/>
             <line number="94" hits="0"/>
             <line number="98" hits="0"/>
             <line number="100" hits="0"/>
             <line number="101" hits="0"/>
             <line number="106" hits="0"/>
             <line number="107" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="108,110"/>
@@ -94,25 +94,25 @@
         </class>
         <class name="common.py" filename="src/hatch_ci/common.py" complexity="0" line-rate="0" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
           </lines>
         </class>
-        <class name="hooks.py" filename="src/hatch_ci/hooks.py" complexity="0" line-rate="0" branch-rate="0">
+        <class name="hooks.py" filename="src/hatch_ci/hooks.py" complexity="0" line-rate="0" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
             <line number="3" hits="0"/>
             <line number="6" hits="0"/>
-            <line number="7" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,6"/>
+            <line number="7" hits="0"/>
             <line number="8" hits="0"/>
           </lines>
         </class>
-        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8333" branch-rate="0.8065">
+        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8333" branch-rate="0.7692">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -148,15 +148,15 @@
             <line number="61" hits="1"/>
             <line number="62" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="63" hits="1"/>
             <line number="64" hits="1"/>
             <line number="66" hits="1"/>
             <line number="67" hits="1"/>
             <line number="69" hits="1"/>
-            <line number="70" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="70" hits="1"/>
             <line number="71" hits="0"/>
             <line number="74" hits="1"/>
             <line number="75" hits="1"/>
             <line number="76" hits="1"/>
             <line number="77" hits="1"/>
             <line number="78" hits="1"/>
             <line number="80" hits="1"/>
@@ -178,30 +178,30 @@
             <line number="106" hits="1"/>
             <line number="107" hits="1"/>
             <line number="109" hits="1"/>
             <line number="110" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="111" hits="1"/>
             <line number="114" hits="1"/>
             <line number="115" hits="1"/>
-            <line number="116" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="116" hits="1"/>
             <line number="117" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="118,119"/>
             <line number="118" hits="0"/>
             <line number="119" hits="0"/>
             <line number="121" hits="0"/>
             <line number="122" hits="0"/>
             <line number="124" hits="0"/>
             <line number="125" hits="0"/>
             <line number="127" hits="0"/>
             <line number="128" hits="0"/>
             <line number="136" hits="0"/>
             <line number="138" hits="1"/>
             <line number="139" hits="1"/>
             <line number="140" hits="1"/>
             <line number="142" hits="1"/>
-            <line number="143" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="143" hits="1"/>
             <line number="144" hits="1"/>
             <line number="145" hits="1"/>
             <line number="146" hits="1"/>
             <line number="147" hits="0"/>
             <line number="148" hits="0"/>
             <line number="149" hits="1"/>
             <line number="151" hits="1"/>
@@ -233,27 +233,27 @@
             <line number="198" hits="1"/>
             <line number="199" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="200"/>
             <line number="200" hits="0"/>
             <line number="201" hits="1"/>
             <line number="202" hits="1"/>
             <line number="203" hits="1"/>
             <line number="205" hits="1"/>
-            <line number="206" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="206" hits="1"/>
             <line number="207" hits="1"/>
             <line number="208" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="209" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="210" hits="1"/>
             <line number="211" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="212" hits="1"/>
             <line number="213" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="216"/>
             <line number="214" hits="1"/>
             <line number="216" hits="0"/>
             <line number="217" hits="1"/>
             <line number="219" hits="1"/>
-            <line number="220" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="220" hits="1"/>
             <line number="221" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,exit"/>
             <line number="227" hits="1"/>
             <line number="233" hits="1"/>
             <line number="235" hits="1"/>
             <line number="236" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="237"/>
             <line number="237" hits="0"/>
             <line number="238" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="239"/>
@@ -343,15 +343,15 @@
             <line number="142" hits="0"/>
             <line number="145" hits="0"/>
             <line number="149" hits="0"/>
             <line number="166" hits="0"/>
             <line number="167" hits="0"/>
           </lines>
         </class>
-        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9502" branch-rate="0.8696">
+        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9502" branch-rate="0.8571">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -363,28 +363,28 @@
             <line number="19" hits="1"/>
             <line number="22" hits="1"/>
             <line number="23" hits="1"/>
             <line number="26" hits="1"/>
             <line number="27" hits="1"/>
             <line number="30" hits="1"/>
             <line number="31" hits="1"/>
-            <line number="32" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="32" hits="1"/>
             <line number="33" hits="1"/>
             <line number="34" hits="1"/>
             <line number="35" hits="1"/>
             <line number="36" hits="1"/>
             <line number="38" hits="1"/>
             <line number="41" hits="1"/>
             <line number="42" hits="1"/>
             <line number="43" hits="1"/>
             <line number="45" hits="1"/>
-            <line number="46" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="46" hits="1"/>
             <line number="47" hits="1"/>
             <line number="49" hits="1"/>
-            <line number="50" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="50" hits="1"/>
             <line number="51" hits="1"/>
             <line number="53" hits="1"/>
             <line number="54" hits="1"/>
             <line number="55" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="56" hits="1"/>
             <line number="57" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="58" hits="1"/>
@@ -474,15 +474,15 @@
             <line number="211" hits="1"/>
             <line number="212" hits="1"/>
             <line number="213" hits="1"/>
             <line number="214" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="215" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="216" hits="1"/>
             <line number="217" hits="1"/>
-            <line number="219" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="219" hits="1"/>
             <line number="220" hits="1"/>
             <line number="221" hits="1"/>
             <line number="224" hits="1"/>
             <line number="239" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="240" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="241" hits="1"/>
             <line number="242" hits="1"/>
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/coverage_html.js` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,13 +89,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 2 statements   2 run 0 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1__version__ = "0.0.7" 
 2__hash__ = "" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -223,13 +223,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 72 statements   0 run 72 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1from __future__ import annotations 
 2 
 3import argparse 
 4import functools 
 5import logging 
@@ -151,8 +151,8 @@
 132 raise 
 133 
 134 return _fn1 
 135 
 136 return _fn 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   0 run 1 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1PLUGIN_NAME = "ci" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,13 +95,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,21 +7,21 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 5 statements   0 run 5 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1from hatchling.plugin import hookimpl 
 2 
 3from hatch_ci.version_hook import CIVersionSource 
 4 
 5 
 6@hookimpl 
 7def hatch_register_version_source(): 
 8 return CIVersionSource 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/scm.py: 83%</title>
+    <title>Coverage for src/hatch_ci/scm.py: 82%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/scm.py</b>:
-            <span class="pc_cov">83%</span>
+            <span class="pc_cov">82%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -353,13 +353,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/scm.py: 83% ******
+****** Coverage for src/hatch_ci/scm.py: 82% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 162 statements   135 run 27 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.scm 
 3from __future__ import annotations 
 4 
 5import dataclasses as dc 
@@ -287,8 +287,8 @@
 263 if str(cur) == cur.root: 263&#x202F;&#x219B;&#x202F;264line 263 didn't jump
 to line 264, because the condition on line 263 was never true
 264 break 
 265 cur = cur.parent 
 266 return None 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -258,13 +258,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 67 statements   0 run 67 missing 2 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1"""create a beta branch or release a beta branch 
 2 
 3This script will either create a new beta branch: 
 4 
 5 hatch-ci make-beta ./src/package_name/__init__.py 
@@ -188,8 +188,8 @@
 167 raise RuntimeError(f"unsupported mode {options.mode=}") 
 168 
 169 
 170if __name__ == "__main__": 
 171 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -478,13 +478,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 201 statements   191 run 10 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.tools 
 3from __future__ import annotations 
 4 
 5import ast 
@@ -418,8 +418,8 @@
 387 for path in list_of_paths(paths): 
 388 txt = apply_fixers(path.read_text(), fixers) 
 389 tmpl = env.from_string(txt) 
 390 path.write_text(tmpl.render(ctx=Context(**data))) 
 391 return data 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -150,13 +150,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 40 statements   0 run 40 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
 
 
 1from __future__ import annotations 
 2 
 3from typing import Any 
 4 
 5from hatchling.version.source.plugin.interface import VersionSourceInterface 
@@ -75,8 +75,8 @@
 59 ) 
 60 gdata = tools.process( 
 61 version_file, getenv("GITHUB_DUMP"), paths=paths, fixers=fixers 
 62 ) 
 63 return {"version": gdata["version"]} 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 05:56 +0000
+at 2023-08-07 06:27 +0000
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/favicon_32.png` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/index.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -75,17 +75,17 @@
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_cli_py.html">src/hatch_ci/cli.py</a></td>
                 <td>72</td>
                 <td>72</td>
                 <td>0</td>
-                <td>24</td>
+                <td>18</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 96">0%</td>
+                <td class="right" data-ratio="0 90">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_common_py.html">src/hatch_ci/common.py</a></td>
                 <td>1</td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
@@ -93,26 +93,26 @@
                 <td class="right" data-ratio="0 1">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_hooks_py.html">src/hatch_ci/hooks.py</a></td>
                 <td>5</td>
                 <td>5</td>
                 <td>0</td>
-                <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 7">0%</td>
+                <td>0</td>
+                <td class="right" data-ratio="0 5">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_scm_py.html">src/hatch_ci/scm.py</a></td>
                 <td>162</td>
                 <td>27</td>
                 <td>0</td>
-                <td>62</td>
+                <td>52</td>
                 <td>8</td>
-                <td class="right" data-ratio="185 224">83%</td>
+                <td class="right" data-ratio="175 214">82%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_script_py.html">src/hatch_ci/script.py</a></td>
                 <td>67</td>
                 <td>67</td>
                 <td>2</td>
                 <td>20</td>
@@ -120,17 +120,17 @@
                 <td class="right" data-ratio="0 87">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_tools_py.html">src/hatch_ci/tools.py</a></td>
                 <td>201</td>
                 <td>10</td>
                 <td>0</td>
-                <td>92</td>
+                <td>84</td>
                 <td>8</td>
-                <td class="right" data-ratio="271 293">92%</td>
+                <td class="right" data-ratio="263 285">92%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_version_hook_py.html">src/hatch_ci/version_hook.py</a></td>
                 <td>40</td>
                 <td>40</td>
                 <td>0</td>
                 <td>14</td>
@@ -140,29 +140,29 @@
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td>550</td>
                 <td>222</td>
                 <td>2</td>
-                <td>214</td>
+                <td>188</td>
                 <td>16</td>
-                <td class="right" data-ratio="458 764">60%</td>
+                <td class="right" data-ratio="440 738">60%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 05:56 +0000
+            created at 2023-08-07 06:27 +0000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html"/>
         <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,24 +2,24 @@
 ****** Coverage report: 60% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-08-07 05:56 +0000
+coverage.py_v7.2.7, created at 2023-08-07 06:27 +0000
 
 Module                   statements missing excluded branches partial coverage
 src/hatch_ci/__init__.py 2          0       0        0        0       100%
-src/hatch_ci/cli.py      72         72      0        24       0       0%
+src/hatch_ci/cli.py      72         72      0        18       0       0%
 src/hatch_ci/common.py   1          1       0        0        0       0%
-src/hatch_ci/hooks.py    5          5       0        2        0       0%
-src/hatch_ci/scm.py      162        27      0        62       8       83%
+src/hatch_ci/hooks.py    5          5       0        0        0       0%
+src/hatch_ci/scm.py      162        27      0        52       8       82%
 src/hatch_ci/script.py   67         67      2        20       0       0%
-src/hatch_ci/tools.py    201        10      0        92       8       92%
+src/hatch_ci/tools.py    201        10      0        84       8       92%
 src/hatch_ci/            40         40      0        14       0       0%
 version_hook.py
-Total                    550        222     2        214      16      60%
+Total                    550        222     2        188      16      60%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-08-07 05:56 +0000
+coverage.py_v7.2.7, created at 2023-08-07 06:27 +0000
  ____
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/keybd_closed.png` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/keybd_open.png` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/status.json` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/status.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8706886574074074%*

 * *Differences: {"'files'": "{'d_7005a4ce5d73f943_cli_py': {'index': {'nums': {insert: [(5, 18), (7, 18)], delete: "*

 * *            "[7, 5]}}}, 'd_7005a4ce5d73f943_hooks_py': {'index': {'nums': {insert: [(6, 0), (7, "*

 * *            "0)], delete: [7, 5]}}}, 'd_7005a4ce5d73f943_scm_py': {'hash': "*

 * *            "'09485baef443027d4b5d7014a9e7d1aa', 'index': {'nums': {insert: [(5, 52)], delete: "*

 * *            "[5]}}}, 'd_7005a4ce5d73f943_tools_py': {'hash': '920e588d8d5656224648cba4f71d8359', "*

 * *            "'index': {'nums': {insert:  […]*

```diff
@@ -23,17 +23,17 @@
                 "html_filename": "d_7005a4ce5d73f943_cli_py.html",
                 "nums": [
                     0,
                     1,
                     72,
                     0,
                     72,
-                    24,
+                    18,
                     0,
-                    24
+                    18
                 ],
                 "relative_filename": "src/hatch_ci/cli.py"
             }
         },
         "d_7005a4ce5d73f943_common_py": {
             "hash": "3f1c2e747e86fae3744447395f472601",
             "index": {
@@ -57,32 +57,32 @@
                 "html_filename": "d_7005a4ce5d73f943_hooks_py.html",
                 "nums": [
                     0,
                     1,
                     5,
                     0,
                     5,
-                    2,
                     0,
-                    2
+                    0,
+                    0
                 ],
                 "relative_filename": "src/hatch_ci/hooks.py"
             }
         },
         "d_7005a4ce5d73f943_scm_py": {
-            "hash": "c09626ba9d1198f601739980971644d0",
+            "hash": "09485baef443027d4b5d7014a9e7d1aa",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_scm_py.html",
                 "nums": [
                     0,
                     1,
                     162,
                     0,
                     27,
-                    62,
+                    52,
                     8,
                     12
                 ],
                 "relative_filename": "src/hatch_ci/scm.py"
             }
         },
         "d_7005a4ce5d73f943_script_py": {
@@ -99,24 +99,24 @@
                     0,
                     20
                 ],
                 "relative_filename": "src/hatch_ci/script.py"
             }
         },
         "d_7005a4ce5d73f943_tools_py": {
-            "hash": "d6cca3c8606571db885acc40cc13e30a",
+            "hash": "920e588d8d5656224648cba4f71d8359",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_tools_py.html",
                 "nums": [
                     0,
                     1,
                     201,
                     0,
                     10,
-                    92,
+                    84,
                     8,
                     12
                 ],
                 "relative_filename": "src/hatch_ci/tools.py"
             }
         },
         "d_7005a4ce5d73f943_version_hook_py": {
@@ -134,10 +134,10 @@
                     14
                 ],
                 "relative_filename": "src/hatch_ci/version_hook.py"
             }
         }
     },
     "format": 2,
-    "globals": "7fbb780b60230e9a8d5c370001e64978",
+    "globals": "43d15eb89a65c685bf50391a42e89e87",
     "version": "7.2.7"
 }
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/coverage/style.css` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/coverage/style.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/junit/junit.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/junit/junit.html`

 * *Files 0% similar despite different names*

```diff
@@ -435,17 +435,17 @@
     const rows = findAll('.results-table-row').filter(isAllRowsHidden);
     const allRowsHidden = rows.length == 0 ? true : false;
     const notFoundMessage = document.getElementById('not-found-message');
     notFoundMessage.hidden = !allRowsHidden;
 }
 </script>
     <h1>junit.html</h1>
-    <p>Report generated on 07-Aug-2023 at 05:56:38 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
+    <p>Report generated on 07-Aug-2023 at 06:27:52 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
     <h2>Summary</h2>
-    <p>16 tests ran in 0.98 seconds. </p>
+    <p>16 tests ran in 1.11 seconds. </p>
     <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">16 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
     <h2>Results</h2>
     <table id="results-table">
       <thead id="results-table-head">
         <tr>
           <th class="sortable result initial-sort" col="result">Result</th>
           <th class="sortable" col="name">Test</th>
@@ -453,34 +453,34 @@
           <th class="sortable links" col="links">Links</th></tr>
         <tr hidden="true" id="not-found-message">
           <th colspan="4">No results found. Try to check the filters</th></tr></thead>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_lookup</td>
-          <td class="col-duration">0.02</td>
+          <td class="col-duration">0.03</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_handle_remote_and_local_repos</td>
-          <td class="col-duration">0.18</td>
+          <td class="col-duration">0.25</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Switched to a new branch &#x27;beta/0.0.4&#x27;
 Switched to branch &#x27;master&#x27;
 Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.2&#x27;
-Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/RUFLAJ&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/WMANVZ&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.1&#x27;
 fatal: a branch named &#x27;master&#x27; already exists
 From /tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
  * [new branch]      beta/0.0.2 -&gt; repo1/beta/0.0.2
  * [new branch]      master     -&gt; repo1/master
 <br/></div></td></tr></tbody>
@@ -574,47 +574,47 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_master</td>
-          <td class="col-duration">0.03</td>
+          <td class="col-duration">0.05</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_beta</td>
-          <td class="col-duration">0.07</td>
+          <td class="col-duration">0.11</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.4&#x27;
 Updated 1 path from the index
 Updated 1 path from the index
 Switched to a new branch &#x27;beta/0.0.2&#x27;
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_release</td>
-          <td class="col-duration">0.04</td>
+          <td class="col-duration">0.06</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Updated 1 path from the index
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_process</td>
-          <td class="col-duration">0.09</td>
+          <td class="col-duration">0.12</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Updated 1 path from the index
 Switched to a new branch &#x27;beta/1.2.3&#x27;
 <br/></div></td></tr></tbody></table></body></html>
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 ****** junit.html ******
-Report generated on 07-Aug-2023 at 05:56:38 by pytest-html v3.2.0
+Report generated on 07-Aug-2023 at 06:27:52 by pytest-html v3.2.0
 ***** Summary *****
-16 tests ran in 0.98 seconds.
+16 tests ran in 1.11 seconds.
 (Un)check the boxes to filter the results.
 *16 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
 unexpected passes
 ***** Results *****
 Result Test                                                  Duration Links
 No results found. Try to check the filters
-Passed tests/test_scm.py::test_lookup                        0.02
+Passed tests/test_scm.py::test_lookup                        0.03
 No log output captured.
-Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.18
+Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.25
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Switched to a new branch
 &#x27;beta/0.0.4&#x27; Switched to branch &#x27;master&#x27; Cloning into
 &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/
 test_check_version-repo1&#x27;... done. Switched to a new branch &#x27;beta/
 0.0.2&#x27; Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/
-test_handle_remote_and_local_r0/RUFLAJ&#x27;... done. Switched to a new
+test_handle_remote_and_local_r0/WMANVZ&#x27;... done. Switched to a new
 branch &#x27;beta/0.0.1&#x27; fatal: a branch named &#x27;master&#x27;
 already exists From /tmp/pytest-of-runner/pytest-0/
 test_handle_remote_and_local_r0/test_check_version-repo1 * [new branch]
 beta/0.0.2 -> repo1/beta/0.0.2 * [new branch] master -> repo1/master
 Passed tests/test_tools.py::test_abort_exception             0.00
 No log output captured.
 Passed tests/test_tools.py::test_urmtree                     0.00
@@ -39,25 +39,25 @@
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var              0.00
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var_empty_file   0.00
 No log output captured.
 Passed tests/test_tools.py::test_bump_version                0.00
 No log output captured.
-Passed tests/test_tools.py::test_update_version_master       0.03
+Passed tests/test_tools.py::test_update_version_master       0.05
 No log output captured.
-Passed tests/test_tools.py::test_update_version_beta         0.07
+Passed tests/test_tools.py::test_update_version_beta         0.11
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.4&#x27; Updated 1 path from the
 index Updated 1 path from the index Switched to a new branch &#x27;beta/
 0.0.2&#x27;
-Passed tests/test_tools.py::test_update_version_release      0.04
+Passed tests/test_tools.py::test_update_version_release      0.06
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Updated 1 path from the
 index
-Passed tests/test_tools.py::test_process                     0.09
+Passed tests/test_tools.py::test_process                     0.12
 ------------------------------Captured stderr call--------------------------
 ----
 Updated 1 path from the index Switched to a new branch &#x27;beta/
 1.2.3&#x27;
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/junit/junit.xml`

 * *Files 6% similar despite different names*

#### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/junit/junit.xml`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <testsuites>
-  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="16" time="0.918" timestamp="2023-08-07T05:56:37.664338" hostname="fv-az593-762">
-    <testcase classname="tests.test_scm" name="test_lookup" time="0.026"/>
-    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.188"/>
+  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="16" time="1.094" timestamp="2023-08-07T06:27:51.345798" hostname="fv-az448-324">
+    <testcase classname="tests.test_scm" name="test_lookup" time="0.032"/>
+    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.254"/>
     <testcase classname="tests.test_tools" name="test_abort_exception" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_urmtree" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_indent" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_list_of_paths" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_lstrip" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_apply_fixers" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_get_module_var" time="0.003"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.004"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_bump_version" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.038"/>
-    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.078"/>
-    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.049"/>
-    <testcase classname="tests.test_tools" name="test_process" time="0.097"/>
+    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.050"/>
+    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.111"/>
+    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.064"/>
+    <testcase classname="tests.test_tools" name="test_process" time="0.120"/>
   </testsuite>
 </testsuites>
```

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/index.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/index.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/mypy-html.css` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html` & `hatch_ci-0.0.7b29/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/src/hatch_ci/cli.py` & `hatch_ci-0.0.7b29/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/src/hatch_ci/scm.py` & `hatch_ci-0.0.7b29/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/src/hatch_ci/script.py` & `hatch_ci-0.0.7b29/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/src/hatch_ci/tools.py` & `hatch_ci-0.0.7b29/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.7b29/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/tests/conftest.py` & `hatch_ci-0.0.7b29/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/tests/test_scm.py` & `hatch_ci-0.0.7b29/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/tests/test_tools.py` & `hatch_ci-0.0.7b29/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/LICENSE.txt` & `hatch_ci-0.0.7b29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.7b28/README.md` & `hatch_ci-0.0.7b29/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](\1beta\3)](\1/runs/5781543881)
-[![Coverage](\1/beta%2F0.0.7)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5781782459)
+[![Codecov](https://codecov.io/gh/cav71/hatch-ci/tree/beta%2F0.0.7/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.codecov.io/gh/cav71/hatch-ci/tree/beta%2F0.0.7)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 This provides a plugin to [Hatch](https://github.com/pypa/hatch) leveraging a CI/CD system (github at the moment)
```

### Comparing `hatch_ci-0.0.7b28/pyproject.toml` & `hatch_ci-0.0.7b29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,21 @@
 
 [tool.hatch.version]
 source = "ci"
 version-file = "src/hatch_ci/__init__.py"
 paths = [ "README.md" ]
 fixers = [
     [ 're:(https://github.com/.+/actions/workflows/)(master)(.yml/badge.svg)',
-        '\\1{{ ctx.workflow }}\\3' ],
+        '\1{{ ctx.workflow }}\3' ],
     [ 're:(https://github.com/.+/actions)/(workflows/)(master.yml)(?!/)',
-        '\\1/runs/{{ ctx.runid }}' ],
+        '\1/runs/{{ ctx.runid }}' ],
     [ 're:(https://codecov.io/gh/.+/tree)/master(/graph/badge.svg[?]token=.+)',
-        '\\1/{{ ctx.branch|urlquote }}\\2' ],
+        '\1/{{ ctx.branch|urlquote }}\2' ],
     [ 're:(https://codecov.io/gh/.+/tree)/master(?!/)',
-        '\\1/{{ ctx.branch|urlquote }}' ]
+        '\1/{{ ctx.branch|urlquote }}' ]
 ]
 
 [tool.ruff]
 target-version = "py38"
 line-length = 88
 select = [
   "A",
```

### Comparing `hatch_ci-0.0.7b28/PKG-INFO` & `hatch_ci-0.0.7b29/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.7b28
+Version: 0.0.7b29
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,plugin,scm,version
@@ -24,16 +24,16 @@
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](\1beta\3)](\1/runs/5781543881)
-[![Coverage](\1/beta%2F0.0.7)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5781782459)
+[![Codecov](https://codecov.io/gh/cav71/hatch-ci/tree/beta%2F0.0.7/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.codecov.io/gh/cav71/hatch-ci/tree/beta%2F0.0.7)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 This provides a plugin to [Hatch](https://github.com/pypa/hatch) leveraging a CI/CD system (github at the moment)
```

