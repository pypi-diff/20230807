# Comparing `tmp/hatch_ci-0.0.8b31.tar.gz` & `tmp/hatch_ci-0.0.8b32.tar.gz`

## Comparing `hatch_ci-0.0.8b31.tar` & `hatch_ci-0.0.8b32.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/.gitattributes
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/.pre-commit-config.yaml
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/Makefile
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/.github/workflows/beta.yml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/.github/workflows/master.yml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/.github/workflows/tags.yml
--rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage.xml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
--rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
--rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
--rw-r--r--   0        0        0    49436 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
--rw-r--r--   0        0        0   115699 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
--rw-r--r--   0        0        0    22969 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/style.css
--rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/junit/junit.html
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/junit/junit.xml
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/index.html
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
--rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
--rw-r--r--   0        0        0    30321 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
--rw-r--r--   0        0        0    68104 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
--rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/cli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/script.py
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/tests/test_scm.py
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/LICENSE.txt
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/README.md
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/pyproject.toml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b31/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.gitattributes
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/Makefile
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.github/workflows/master.yml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    28053 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    49009 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
+-rw-r--r--   0        0        0   129332 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    30121 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
+-rw-r--r--   0        0        0    75063 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/script.py
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/test_scm.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/LICENSE.txt
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/README.md
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/pyproject.toml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/PKG-INFO
```

### Comparing `hatch_ci-0.0.8b31/Makefile` & `hatch_ci-0.0.8b32/Makefile`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/.github/workflows/beta.yml` & `hatch_ci-0.0.8b32/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/.github/workflows/master.yml` & `hatch_ci-0.0.8b32/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/.github/workflows/tags.yml` & `hatch_ci-0.0.8b32/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage.xml`

 * *Files 2% similar despite different names*

#### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1691400994139" lines-valid="550" lines-covered="328" line-rate="0.5964" branches-valid="188" branches-covered="112" branch-rate="0.5957" complexity="0">
+<coverage version="7.2.7" timestamp="1691439205054" lines-valid="572" lines-covered="340" line-rate="0.5944" branches-valid="202" branches-covered="117" branch-rate="0.5792" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/hatch-ci/hatch-ci</source>
   </sources>
   <packages>
-    <package name="src.hatch_ci" line-rate="0.5964" branch-rate="0.5957" complexity="0">
+    <package name="src.hatch_ci" line-rate="0.5944" branch-rate="0.5792" complexity="0">
       <classes>
         <class name="__init__.py" filename="src/hatch_ci/__init__.py" complexity="0" line-rate="1" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
           </lines>
@@ -312,46 +312,45 @@
             <line number="78" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="79,81"/>
             <line number="79" hits="0"/>
             <line number="81" hits="0"/>
             <line number="82" hits="0"/>
             <line number="83" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="84,87"/>
             <line number="84" hits="0"/>
             <line number="87" hits="0"/>
-            <line number="89" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="90,116"/>
+            <line number="89" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="90,115"/>
             <line number="90" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="91,95"/>
             <line number="91" hits="0"/>
             <line number="95" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="96,99"/>
             <line number="96" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="97,98"/>
             <line number="97" hits="0"/>
             <line number="98" hits="0"/>
             <line number="99" hits="0"/>
             <line number="100" hits="0"/>
             <line number="101" hits="0"/>
-            <line number="102" hits="0"/>
-            <line number="116" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="118,166"/>
-            <line number="118" hits="0"/>
-            <line number="119" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="120,126"/>
-            <line number="120" hits="0"/>
+            <line number="115" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="117,165"/>
+            <line number="117" hits="0"/>
+            <line number="118" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="119,125"/>
+            <line number="119" hits="0"/>
+            <line number="124" hits="0"/>
             <line number="125" hits="0"/>
-            <line number="126" hits="0"/>
-            <line number="127" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="128,131"/>
-            <line number="128" hits="0"/>
-            <line number="131" hits="0"/>
-            <line number="134" hits="0"/>
+            <line number="126" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="127,130"/>
+            <line number="127" hits="0"/>
+            <line number="130" hits="0"/>
+            <line number="133" hits="0"/>
+            <line number="136" hits="0"/>
             <line number="137" hits="0"/>
-            <line number="138" hits="0"/>
+            <line number="140" hits="0"/>
             <line number="141" hits="0"/>
-            <line number="142" hits="0"/>
-            <line number="145" hits="0"/>
-            <line number="149" hits="0"/>
+            <line number="144" hits="0"/>
+            <line number="148" hits="0"/>
+            <line number="165" hits="0"/>
             <line number="166" hits="0"/>
-            <line number="167" hits="0"/>
           </lines>
         </class>
-        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9502" branch-rate="0.8571">
+        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9062" branch-rate="0.7857">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -411,150 +410,173 @@
             <line number="92" hits="1"/>
             <line number="93" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="94" hits="1"/>
             <line number="95" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="98" hits="1"/>
             <line number="99" hits="1"/>
             <line number="102" hits="1"/>
-            <line number="103" hits="1"/>
-            <line number="104" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="105" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="106" hits="1"/>
-            <line number="108" hits="1"/>
-            <line number="109" hits="1"/>
-            <line number="112" hits="1"/>
-            <line number="132" hits="1"/>
-            <line number="133" hits="1"/>
-            <line number="134" hits="1"/>
-            <line number="135" hits="1"/>
-            <line number="137" hits="1"/>
-            <line number="139" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="140" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="141"/>
-            <line number="141" hits="0"/>
-            <line number="142" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="143" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="103" hits="0"/>
+            <line number="105" hits="0"/>
+            <line number="106" hits="0"/>
+            <line number="107" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="108,109"/>
+            <line number="108" hits="0"/>
+            <line number="109" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="110,111"/>
+            <line number="110" hits="0"/>
+            <line number="111" hits="0"/>
+            <line number="114" hits="1"/>
+            <line number="115" hits="1"/>
+            <line number="116" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="117" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="118" hits="1"/>
+            <line number="120" hits="1"/>
+            <line number="121" hits="1"/>
+            <line number="124" hits="1"/>
             <line number="144" hits="1"/>
-            <line number="145" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="145" hits="1"/>
             <line number="146" hits="1"/>
-            <line number="150" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="151" hits="1"/>
-            <line number="152" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="155"/>
-            <line number="153" hits="1"/>
-            <line number="155" hits="0"/>
-            <line number="156" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="157" hits="1"/>
-            <line number="160" hits="1"/>
-            <line number="161" hits="1"/>
+            <line number="147" hits="1"/>
+            <line number="149" hits="1"/>
+            <line number="151" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="152" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="153"/>
+            <line number="153" hits="0"/>
+            <line number="154" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="155" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="156" hits="1"/>
+            <line number="157" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="158" hits="1"/>
+            <line number="162" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="163" hits="1"/>
-            <line number="164" hits="1"/>
-            <line number="165" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="166" hits="1"/>
-            <line number="167" hits="1"/>
+            <line number="164" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="167"/>
+            <line number="165" hits="1"/>
+            <line number="167" hits="0"/>
             <line number="168" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="169" hits="1"/>
-            <line number="170" hits="1"/>
+            <line number="172" hits="1"/>
             <line number="173" hits="1"/>
-            <line number="189" hits="1"/>
-            <line number="192" hits="1"/>
-            <line number="193" hits="1"/>
-            <line number="194" hits="1"/>
-            <line number="196" hits="1"/>
-            <line number="197" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="198" hits="1"/>
-            <line number="199" hits="1"/>
+            <line number="175" hits="1"/>
+            <line number="176" hits="1"/>
+            <line number="177" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="178" hits="1"/>
+            <line number="179" hits="1"/>
+            <line number="180" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="181" hits="1"/>
+            <line number="182" hits="1"/>
+            <line number="185" hits="1"/>
             <line number="201" hits="1"/>
-            <line number="202" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="203" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="204" hits="1"/>
             <line number="205" hits="1"/>
             <line number="206" hits="1"/>
-            <line number="207" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="208" hits="1"/>
-            <line number="209" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="212"/>
+            <line number="209" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="210" hits="1"/>
             <line number="211" hits="1"/>
-            <line number="212" hits="1"/>
             <line number="213" hits="1"/>
             <line number="214" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="215" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="216" hits="1"/>
             <line number="217" hits="1"/>
-            <line number="219" hits="1"/>
+            <line number="218" hits="1"/>
+            <line number="219" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="220" hits="1"/>
-            <line number="221" hits="1"/>
+            <line number="221" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="224"/>
+            <line number="222" hits="1"/>
+            <line number="223" hits="1"/>
             <line number="224" hits="1"/>
-            <line number="239" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="240" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="241" hits="1"/>
-            <line number="242" hits="1"/>
-            <line number="243" hits="1"/>
-            <line number="244" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="245" hits="1"/>
-            <line number="246" hits="1"/>
-            <line number="247" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="248" hits="1"/>
-            <line number="249" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="252" hits="1"/>
+            <line number="225" hits="1"/>
+            <line number="226" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="227" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="228" hits="1"/>
+            <line number="229" hits="1"/>
+            <line number="231" hits="1"/>
+            <line number="232" hits="1"/>
+            <line number="233" hits="1"/>
+            <line number="236" hits="1"/>
+            <line number="251" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="252" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="253" hits="1"/>
+            <line number="254" hits="1"/>
+            <line number="255" hits="1"/>
+            <line number="256" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="257" hits="1"/>
+            <line number="258" hits="1"/>
+            <line number="259" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="260" hits="1"/>
+            <line number="261" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="264" hits="1"/>
-            <line number="274" hits="1"/>
-            <line number="275" hits="1"/>
-            <line number="277" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="278"/>
-            <line number="278" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="279,280"/>
-            <line number="279" hits="0"/>
-            <line number="280" hits="0"/>
-            <line number="282" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="283" hits="1"/>
-            <line number="289" hits="1"/>
+            <line number="280" hits="1"/>
+            <line number="290" hits="1"/>
             <line number="291" hits="1"/>
             <line number="292" hits="1"/>
-            <line number="294" hits="1"/>
-            <line number="295" hits="1"/>
-            <line number="297" hits="1"/>
-            <line number="298" hits="1"/>
-            <line number="299" hits="1"/>
-            <line number="300" hits="1"/>
-            <line number="301" hits="1"/>
-            <line number="303" hits="1"/>
-            <line number="304" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="307" hits="1"/>
-            <line number="308" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="309"/>
-            <line number="309" hits="0"/>
-            <line number="310" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="311" hits="1"/>
-            <line number="315" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="316" hits="1"/>
-            <line number="317" hits="1"/>
+            <line number="294" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="295"/>
+            <line number="295" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="296,300"/>
+            <line number="296" hits="0"/>
+            <line number="300" hits="0"/>
+            <line number="302" hits="1"/>
+            <line number="303" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="304" hits="1"/>
+            <line number="305" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="306"/>
+            <line number="306" hits="0"/>
+            <line number="307" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,319"/>
+            <line number="308" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="317"/>
+            <line number="309" hits="1"/>
+            <line number="315" hits="1"/>
+            <line number="317" hits="0"/>
             <line number="319" hits="1"/>
             <line number="320" hits="1"/>
+            <line number="322" hits="1"/>
             <line number="323" hits="1"/>
+            <line number="324" hits="1"/>
+            <line number="325" hits="1"/>
+            <line number="326" hits="1"/>
+            <line number="328" hits="1"/>
+            <line number="329" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="332" hits="1"/>
+            <line number="333" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="334"/>
+            <line number="334" hits="0"/>
+            <line number="335" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="336" hits="1"/>
-            <line number="337" hits="1"/>
-            <line number="338" hits="1"/>
-            <line number="339" hits="1"/>
+            <line number="340" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="341" hits="1"/>
             <line number="342" hits="1"/>
-            <line number="368" hits="1"/>
-            <line number="369" hits="1"/>
-            <line number="370" hits="1"/>
-            <line number="372" hits="1"/>
-            <line number="374" hits="1"/>
-            <line number="375" hits="1"/>
-            <line number="376" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="377" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="378"/>
-            <line number="378" hits="0"/>
-            <line number="379" hits="1"/>
-            <line number="381" hits="1"/>
-            <line number="382" hits="1"/>
-            <line number="383" hits="1"/>
-            <line number="385" hits="1"/>
-            <line number="386" hits="1"/>
-            <line number="387" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="388" hits="1"/>
-            <line number="389" hits="1"/>
-            <line number="390" hits="1"/>
-            <line number="391" hits="1"/>
+            <line number="344" hits="1"/>
+            <line number="345" hits="1"/>
+            <line number="348" hits="1"/>
+            <line number="361" hits="1"/>
+            <line number="362" hits="1"/>
+            <line number="363" hits="1"/>
+            <line number="364" hits="1"/>
+            <line number="367" hits="1"/>
+            <line number="396" hits="1"/>
+            <line number="397" hits="1"/>
+            <line number="398" hits="1"/>
+            <line number="400" hits="1"/>
+            <line number="402" hits="1"/>
+            <line number="403" hits="1"/>
+            <line number="404" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="405" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="406"/>
+            <line number="406" hits="0"/>
+            <line number="407" hits="1"/>
+            <line number="409" hits="1"/>
+            <line number="410" hits="1"/>
+            <line number="411" hits="1"/>
+            <line number="412" hits="1"/>
+            <line number="414" hits="1"/>
+            <line number="415" hits="1"/>
+            <line number="416" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="417" hits="1"/>
+            <line number="418" hits="1"/>
+            <line number="419" hits="1"/>
+            <line number="421" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="429"/>
+            <line number="422" hits="1"/>
+            <line number="423" hits="1"/>
+            <line number="424" hits="1"/>
+            <line number="425" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="426" hits="1"/>
+            <line number="427" hits="1"/>
+            <line number="429" hits="1"/>
           </lines>
         </class>
         <class name="version_hook.py" filename="src/hatch_ci/version_hook.py" complexity="0" line-rate="0" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
             <line number="3" hits="0"/>
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
 1__version__ = "0.0.8" 
 2__hash__ = "" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html`

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
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
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
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
 1PLUGIN_NAME = "ci" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
 1from hatchling.plugin import hookimpl 
 2 
 3from hatch_ci.version_hook import CIVersionSource 
 4 
 5 
 6@hookimpl 
 7def hatch_register_version_source(): 
 8 return CIVersionSource 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
 ***** 162 statements   135 run 27 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
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
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -51,27 +51,27 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">67 statements &nbsp;</span>
+            <span class="text">66 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">67<span class="text"> missing</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">66<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">0<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -178,93 +178,92 @@
     <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">for</span> <span class="nam">branch</span> <span class="key">in</span> <span class="op">[</span><span class="op">*</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branches</span><span class="op">.</span><span class="nam">local</span><span class="op">,</span> <span class="op">*</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branches</span><span class="op">.</span><span class="nam">remote</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">branch</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">f"beta/{version}"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"branch '{branch}' already present"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"creating branch '%s'"</span><span class="op">,</span> <span class="str">f"/beta/{version}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branch</span><span class="op">(</span><span class="str">f"beta/{version}"</span><span class="op">,</span> <span class="nam">master</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="nam">master</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">        The release branch beta/{version} has been created.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">            git push origin beta/{version}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">        To revert this beta branch:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t"><span class="str">            git branch -D beta/{version}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">            <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="key">elif</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span> <span class="key">in</span> <span class="op">{</span><span class="str">"micro"</span><span class="op">,</span> <span class="str">"minor"</span><span class="op">,</span> <span class="str">"major"</span><span class="op">}</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="com"># we need to be in the beta/N.M.O branch</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"refs/heads/beta/(?P&lt;beta>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="str">f"wrong branch '{options.repo.head.shorthand}'"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="str">f"expected to be in 'beta/{version}' branch"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                <span class="str">f"git checkout beta/{version}"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">local</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"beta"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="key">if</span> <span class="nam">local</span> <span class="op">!=</span> <span class="nam">version</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"wrong version file {version=} != {local}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="com"># create an empty commit to mark the release</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"commit"</span><span class="op">,</span> <span class="str">"--allow-empty"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="com"># tag</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">f"release/{version}"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="com"># switch to master (and incorporate the commit message)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="nam">master</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"merge"</span><span class="op">,</span> <span class="str">f"beta/{version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="com"># bump version</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">new_version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="nam">tools</span><span class="op">.</span><span class="nam">set_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">new_version</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="com"># commit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">f"version bump {version} -> {new_version}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">        The release is almost complete.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">            git push origin release/{version}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="str">            git push origin master</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">        To revert this release:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="str">            git reset --hard HEAD~1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">            git tag -d release/{version}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">        The release branch beta/{version} has been created.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">            git push origin beta/{version}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="str">        To revert this beta branch:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">            git branch -D beta/{version}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="key">elif</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span> <span class="key">in</span> <span class="op">{</span><span class="str">"micro"</span><span class="op">,</span> <span class="str">"minor"</span><span class="op">,</span> <span class="str">"major"</span><span class="op">}</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="com"># we need to be in the beta/N.M.O branch</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"refs/heads/beta/(?P&lt;beta>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                <span class="str">f"wrong branch '{options.repo.head.shorthand}'"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="str">f"expected to be in 'beta/{version}' branch"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="str">f"git checkout beta/{version}"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">local</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"beta"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="key">if</span> <span class="nam">local</span> <span class="op">!=</span> <span class="nam">version</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"wrong version file {version=} != {local}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="com"># create an empty commit to mark the release</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"commit"</span><span class="op">,</span> <span class="str">"--allow-empty"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="com"># tag</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">f"release/{version}"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="com"># switch to master (and incorporate the commit message)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="nam">master</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"merge"</span><span class="op">,</span> <span class="str">f"beta/{version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="com"># bump version</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">new_version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">tools</span><span class="op">.</span><span class="nam">set_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">new_version</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="com"># commit</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">f"version bump {version} -> {new_version}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="str">        The release is almost complete.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">            git push origin release/{version}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">            git push origin master</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="str">        To revert this release:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">            git reset --hard HEAD~1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="str">            git tag -d release/{version}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="nam">main</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">    <span class="nam">main</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 67 statements   0 run 67 missing 2 excluded 0 partial *****
+***** 66 statements   0 run 66 missing 2 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
 1"""create a beta branch or release a beta branch 
 2 
 3This script will either create a new beta branch: 
 4 
 5 hatch-ci make-beta ./src/package_name/__init__.py 
@@ -114,82 +114,81 @@
 95 for branch in [*options.repo.branches.local, *options.repo.branches.remote]:
  
 96 if not branch.endswith(f"beta/{version}"): 
 97 continue 
 98 options.error(f"branch '{branch}' already present") 
 99 log.info("creating branch '%s'", f"/beta/{version}") 
 100 options.repo.branch(f"beta/{version}", master) 
-101 options.repo(["checkout", master]) 
-102 print( # noqa: T201 
-103 tools.indent( 
-104 f""" 
-105 The release branch beta/{version} has been created. 
-106 
-107 To complete the release: 
-108 git push origin beta/{version} 
-109 
-110 To revert this beta branch: 
-111 git branch -D beta/{version} 
-112 """ 
-113 ), 
-114 file=sys.stderr, 
-115 ) 
-116 elif options.mode in {"micro", "minor", "major"}: 
-117 # we need to be in the beta/N.M.O branch 
-118 expr = re.compile(r"refs/heads/beta/(?P<beta>\d+([.]\d+)*)$") 
-119 if not (match := expr.search(options.repo.head.name)): 
-120 options.error( 
-121 f"wrong branch '{options.repo.head.shorthand}'", 
-122 f"expected to be in 'beta/{version}' branch", 
-123 f"git checkout beta/{version}", 
-124 ) 
-125 return 
-126 local = match.group("beta") 
-127 if local != version: 
-128 options.error(f"wrong version file {version=} != {local}") 
-129 
-130 # create an empty commit to mark the release 
-131 options.repo(["commit", "--allow-empty", "-m", f"released {version}"]) 
-132 
-133 # tag 
-134 options.repo(["tag", "-a", f"release/{version}", "-m", f"released
+101 print( # noqa: T201 
+102 tools.indent( 
+103 f""" 
+104 The release branch beta/{version} has been created. 
+105 
+106 To complete the release: 
+107 git push origin beta/{version} 
+108 
+109 To revert this beta branch: 
+110 git branch -D beta/{version} 
+111 """ 
+112 ), 
+113 file=sys.stderr, 
+114 ) 
+115 elif options.mode in {"micro", "minor", "major"}: 
+116 # we need to be in the beta/N.M.O branch 
+117 expr = re.compile(r"refs/heads/beta/(?P<beta>\d+([.]\d+)*)$") 
+118 if not (match := expr.search(options.repo.head.name)): 
+119 options.error( 
+120 f"wrong branch '{options.repo.head.shorthand}'", 
+121 f"expected to be in 'beta/{version}' branch", 
+122 f"git checkout beta/{version}", 
+123 ) 
+124 return 
+125 local = match.group("beta") 
+126 if local != version: 
+127 options.error(f"wrong version file {version=} != {local}") 
+128 
+129 # create an empty commit to mark the release 
+130 options.repo(["commit", "--allow-empty", "-m", f"released {version}"]) 
+131 
+132 # tag 
+133 options.repo(["tag", "-a", f"release/{version}", "-m", f"released
 {version}"]) 
-135 
-136 # switch to master (and incorporate the commit message) 
-137 options.repo(["checkout", master]) 
-138 options.repo(["merge", f"beta/{version}"]) 
-139 
-140 # bump version 
-141 new_version = tools.bump_version(version, options.mode) 
-142 tools.set_module_var(options.initfile, "__version__", new_version) 
-143 
-144 # commit 
-145 options.repo.commit( 
-146 options.initfile, f"version bump {version} -> {new_version}" 
-147 ) 
-148 
-149 print( # noqa: T201 
-150 tools.indent( 
-151 f""" 
-152 The release is almost complete. 
-153 
-154 To complete the release: 
-155 git push origin release/{version} 
-156 git push origin master 
-157 
-158 To revert this release: 
-159 git reset --hard HEAD~1 
-160 git tag -d release/{version} 
-161 """ 
-162 ), 
-163 file=sys.stderr, 
-164 ) 
-165 else: 
-166 options.error(f"unsupported mode {options.mode=}") 
-167 raise RuntimeError(f"unsupported mode {options.mode=}") 
+134 
+135 # switch to master (and incorporate the commit message) 
+136 options.repo(["checkout", master]) 
+137 options.repo(["merge", f"beta/{version}"]) 
+138 
+139 # bump version 
+140 new_version = tools.bump_version(version, options.mode) 
+141 tools.set_module_var(options.initfile, "__version__", new_version) 
+142 
+143 # commit 
+144 options.repo.commit( 
+145 options.initfile, f"version bump {version} -> {new_version}" 
+146 ) 
+147 
+148 print( # noqa: T201 
+149 tools.indent( 
+150 f""" 
+151 The release is almost complete. 
+152 
+153 To complete the release: 
+154 git push origin release/{version} 
+155 git push origin master 
+156 
+157 To revert this release: 
+158 git reset --hard HEAD~1 
+159 git tag -d release/{version} 
+160 """ 
+161 ), 
+162 file=sys.stderr, 
+163 ) 
+164 else: 
+165 options.error(f"unsupported mode {options.mode=}") 
+166 raise RuntimeError(f"unsupported mode {options.mode=}") 
+167 
 168 
-169 
-170if __name__ == "__main__": 
-171 main() 
+169if __name__ == "__main__": 
+170 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/tools.py: 92%</title>
+    <title>Coverage for src/hatch_ci/tools.py: 87%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/tools.py</b>:
-            <span class="pc_cov">92%</span>
+            <span class="pc_cov">87%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,27 +51,27 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">201 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">191<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">10<span class="text"> missing</span></button>
+            <span class="text">224 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">203<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">21<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
-            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">8<span class="text"> partial</span></button>
+            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">11<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -179,312 +179,350 @@
     <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="key">return</span> <span class="op">[</span><span class="nam">Path</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span> <span class="key">for</span> <span class="nam">s</span> <span class="key">in</span> <span class="op">(</span><span class="op">[</span><span class="nam">paths</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">paths</span><span class="op">,</span> <span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">)</span><span class="op">)</span> <span class="key">else</span> <span class="nam">paths</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="key">def</span> <span class="nam">lstrip</span><span class="op">(</span><span class="nam">txt</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">left</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="key">return</span> <span class="nam">txt</span><span class="op">[</span><span class="nam">len</span><span class="op">(</span><span class="nam">left</span><span class="op">)</span> <span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">left</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="key">def</span> <span class="nam">apply_fixers</span><span class="op">(</span><span class="nam">txt</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">fixers</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="key">for</span> <span class="nam">src</span><span class="op">,</span> <span class="nam">dst</span> <span class="key">in</span> <span class="op">(</span><span class="nam">fixers</span> <span class="key">or</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">if</span> <span class="nam">src</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"re:"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">            <span class="nam">result</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">sub</span><span class="op">(</span><span class="nam">src</span><span class="op">[</span><span class="num">3</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">dst</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">            <span class="nam">result</span> <span class="op">=</span> <span class="nam">result</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="nam">src</span><span class="op">,</span> <span class="nam">dst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="key">def</span> <span class="nam">get_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="str">"""extract from a python module in path the module level &lt;var> variable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse using ast (no code-execution)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">        abort (bool): raise MissingVariable if var is not present</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">        None or str: the variable value if found or None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="str">    Raises:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="str">        MissingVariable: if the var is not found and abort is True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="str">    Notes:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="str">        this uses ast to parse path, so it doesn't load the module</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="key">class</span> <span class="nam">V</span><span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">NodeVisitor</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">keys</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span> <span class="op">=</span> <span class="nam">keys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">result</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="key">def</span> <span class="nam">loadmod</span><span class="op">(</span><span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="key">from</span> <span class="nam">importlib</span><span class="op">.</span><span class="nam">util</span> <span class="key">import</span> <span class="nam">module_from_spec</span><span class="op">,</span> <span class="nam">spec_from_file_location</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="nam">module</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">    <span class="nam">spec</span> <span class="op">=</span> <span class="nam">spec_from_file_location</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="key">if</span> <span class="nam">spec</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">module</span> <span class="op">=</span> <span class="nam">module_from_spec</span><span class="op">(</span><span class="nam">spec</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="key">if</span> <span class="nam">module</span> <span class="key">and</span> <span class="nam">spec</span> <span class="key">and</span> <span class="nam">spec</span><span class="op">.</span><span class="nam">loader</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">spec</span><span class="op">.</span><span class="nam">loader</span><span class="op">.</span><span class="nam">exec_module</span><span class="op">(</span><span class="nam">module</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">return</span> <span class="nam">module</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t"><span class="key">def</span> <span class="nam">apply_fixers</span><span class="op">(</span><span class="nam">txt</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">fixers</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="key">for</span> <span class="nam">src</span><span class="op">,</span> <span class="nam">dst</span> <span class="key">in</span> <span class="op">(</span><span class="nam">fixers</span> <span class="key">or</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="key">if</span> <span class="nam">src</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"re:"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="nam">result</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">sub</span><span class="op">(</span><span class="nam">src</span><span class="op">[</span><span class="num">3</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">dst</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="nam">result</span> <span class="op">=</span> <span class="nam">result</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="nam">src</span><span class="op">,</span> <span class="nam">dst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t"><span class="key">def</span> <span class="nam">get_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">    <span class="str">"""extract from a python module in path the module level &lt;var> variable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse using ast (no code-execution)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">        abort (bool): raise MissingVariable if var is not present</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t"><span class="str">        None or str: the variable value if found or None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="key">def</span> <span class="nam">visit_Module</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: N802</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">            <span class="com"># we extract the module level variables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">            <span class="key">for</span> <span class="nam">subnode</span> <span class="key">in</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">iter_child_nodes</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">                <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Assign</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">140&#x202F;&#x219B;&#x202F;141</span><span class="annotate long">line 140 didn't jump to line 141, because the condition on line 140 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                <span class="key">for</span> <span class="nam">target</span> <span class="key">in</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">targets</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">                    <span class="key">if</span> <span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">                        <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">                    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Constant</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">                        <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                            <span class="str">f"cannot extract non Constant variable "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">                            <span class="str">f"{target.id} ({type(subnode.value)})"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">                        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">s</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">                    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">152&#x202F;&#x219B;&#x202F;155</span><span class="annotate long">line 152 didn't jump to line 155, because the condition on line 152 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">n</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">                    <span class="key">if</span> <span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">result</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">                        <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">                            <span class="str">f"found multiple repeated variables {target.id}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">                        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">result</span><span class="op">[</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">generic_visit</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="nam">v</span> <span class="op">=</span> <span class="nam">V</span><span class="op">(</span><span class="op">{</span><span class="nam">var</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">tree</span> <span class="op">=</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="nam">v</span><span class="op">.</span><span class="nam">visit</span><span class="op">(</span><span class="nam">tree</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">    <span class="key">if</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span> <span class="key">and</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">        <span class="key">raise</span> <span class="nam">MissingVariableError</span><span class="op">(</span><span class="str">f"cannot find {var} in {path}"</span><span class="op">,</span> <span class="nam">path</span><span class="op">,</span> <span class="nam">var</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">    <span class="key">return</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">var</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="key">def</span> <span class="nam">set_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">create</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="str">"""replace var in path with value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="str">        value (None or Any): if not None replace var in version_file</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t"><span class="str">        create (bool): create path if not present</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="str">    Raises:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">        MissingVariable: if the var is not found and abort is True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">    Notes:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="str">        this uses ast to parse path, so it doesn't load the module</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="key">class</span> <span class="nam">V</span><span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">NodeVisitor</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">keys</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span> <span class="op">=</span> <span class="nam">keys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">result</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="key">def</span> <span class="nam">visit_Module</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: N802</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="com"># we extract the module level variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">            <span class="key">for</span> <span class="nam">subnode</span> <span class="key">in</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">iter_child_nodes</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">                <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Assign</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">152&#x202F;&#x219B;&#x202F;153</span><span class="annotate long">line 152 didn't jump to line 153, because the condition on line 152 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">                <span class="key">for</span> <span class="nam">target</span> <span class="key">in</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">targets</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">                    <span class="key">if</span> <span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">                        <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">                    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Constant</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">                        <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">                            <span class="str">f"cannot extract non Constant variable "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">                            <span class="str">f"{target.id} ({type(subnode.value)})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">                        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">                    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">s</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">                    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">164&#x202F;&#x219B;&#x202F;167</span><span class="annotate long">line 164 didn't jump to line 167, because the condition on line 164 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">n</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">                    <span class="key">if</span> <span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">result</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">                        <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">                            <span class="str">f"found multiple repeated variables {target.id}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">                        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">result</span><span class="op">[</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">generic_visit</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="nam">v</span> <span class="op">=</span> <span class="nam">V</span><span class="op">(</span><span class="op">{</span><span class="nam">var</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">    <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">        <span class="nam">tree</span> <span class="op">=</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="nam">v</span><span class="op">.</span><span class="nam">visit</span><span class="op">(</span><span class="nam">tree</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">    <span class="key">if</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span> <span class="key">and</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="key">raise</span> <span class="nam">MissingVariableError</span><span class="op">(</span><span class="str">f"cannot find {var} in {path}"</span><span class="op">,</span> <span class="nam">path</span><span class="op">,</span> <span class="nam">var</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="key">return</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">var</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="str">        (str, str) the (&lt;previous-var-value|None>, &lt;the new text>)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="com"># validate the var</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">    <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">var</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="com"># module level var</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">f"^{var}\\s*=\\s*['\\\"](?P&lt;value>[^\\\"']*)['\\\"]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="nam">fixed</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="nam">lines</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="key">def</span> <span class="nam">set_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">create</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="str">"""replace var in path with value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">        value (None or Any): if not None replace var in version_file</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="str">        create (bool): create path if not present</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">    <span class="nam">src</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">src</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">mkdir</span><span class="op">(</span><span class="nam">parents</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">touch</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="nam">input_lines</span> <span class="op">=</span> <span class="nam">src</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">input_lines</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="key">if</span> <span class="nam">fixed</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">            <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">        <span class="nam">match</span> <span class="op">=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="nam">fixed</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"value"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">209&#x202F;&#x219B;&#x202F;212</span><span class="annotate long">line 209 didn't jump to line 212, because the condition on line 209 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">span</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="nam">line</span><span class="op">[</span><span class="op">:</span><span class="nam">x</span><span class="op">]</span> <span class="op">+</span> <span class="nam">value</span> <span class="op">+</span> <span class="nam">line</span><span class="op">[</span><span class="nam">y</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="nam">txt</span> <span class="op">=</span> <span class="str">"\n"</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">lines</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="key">if</span> <span class="op">(</span><span class="nam">fixed</span> <span class="key">is</span> <span class="key">None</span><span class="op">)</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="key">if</span> <span class="nam">txt</span> <span class="key">and</span> <span class="nam">txt</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"\n"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="nam">txt</span> <span class="op">+=</span> <span class="str">"\n"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="nam">txt</span> <span class="op">+=</span> <span class="str">f'{var} = "{value}"'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"w"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="nam">fp</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="key">return</span> <span class="nam">fixed</span><span class="op">,</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="key">def</span> <span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">mode</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="str">"""given a version str will bump it according to mode</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="str">        version: text in the N.M.O form</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="str">        mode: major, minor or micro</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t"><span class="str">        (str, str) the (&lt;previous-var-value|None>, &lt;the new text>)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="com"># validate the var</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">var</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">    <span class="com"># module level var</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">f"^{var}\\s*=\\s*['\\\"](?P&lt;value>[^\\\"']*)['\\\"]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">    <span class="nam">fixed</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="nam">lines</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">    <span class="nam">src</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">src</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">mkdir</span><span class="op">(</span><span class="nam">parents</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">touch</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="nam">input_lines</span> <span class="op">=</span> <span class="nam">src</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">input_lines</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="key">if</span> <span class="nam">fixed</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="nam">match</span> <span class="op">=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">            <span class="nam">fixed</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"value"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">221&#x202F;&#x219B;&#x202F;224</span><span class="annotate long">line 221 didn't jump to line 224, because the condition on line 221 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">                <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">span</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="nam">line</span><span class="op">[</span><span class="op">:</span><span class="nam">x</span><span class="op">]</span> <span class="op">+</span> <span class="nam">value</span> <span class="op">+</span> <span class="nam">line</span><span class="op">[</span><span class="nam">y</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="nam">txt</span> <span class="op">=</span> <span class="str">"\n"</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">lines</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="key">if</span> <span class="op">(</span><span class="nam">fixed</span> <span class="key">is</span> <span class="key">None</span><span class="op">)</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="key">if</span> <span class="nam">txt</span> <span class="key">and</span> <span class="nam">txt</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"\n"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">            <span class="nam">txt</span> <span class="op">+=</span> <span class="str">"\n"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="nam">txt</span> <span class="op">+=</span> <span class="str">f'{var} = "{value}"'</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">        increased text</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "micro")</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">    "1.0.4"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "minor")</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">    "1.1.0"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="nam">newver</span> <span class="op">=</span> <span class="op">[</span><span class="nam">int</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span> <span class="key">for</span> <span class="nam">n</span> <span class="key">in</span> <span class="nam">version</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="key">if</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"major"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">3</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"minor"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"micro"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">    <span class="key">return</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">for</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">newver</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="key">def</span> <span class="nam">get_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="nam">version_file</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">    <span class="str">"""extracts version information from github_dump and updates version_file in-place</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">        version_file (str, Path): path to a file  with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t"><span class="str">        dict[str,str|None]: a dict with the current config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">        <span class="str">"version"</span><span class="op">:</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">        <span class="str">"current"</span><span class="op">:</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">        <span class="str">"branch"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="str">"hash"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">        <span class="str">"build"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">        <span class="str">"runid"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">        <span class="str">"workflow"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">version_file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">    <span class="nam">repo</span> <span class="op">=</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">lookup</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"w"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="nam">fp</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="key">return</span> <span class="nam">fixed</span><span class="op">,</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="key">def</span> <span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">mode</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">    <span class="str">"""given a version str will bump it according to mode</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">        version: text in the N.M.O form</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">        mode: major, minor or micro</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t"><span class="str">        increased text</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "micro")</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t"><span class="str">    "1.0.4"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "minor")</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="str">    "1.1.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">    <span class="nam">newver</span> <span class="op">=</span> <span class="op">[</span><span class="nam">int</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span> <span class="key">for</span> <span class="nam">n</span> <span class="key">in</span> <span class="nam">version</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">    <span class="key">if</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"major"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">3</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"minor"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"micro"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">    <span class="key">return</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">for</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">newver</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="key">def</span> <span class="nam">get_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">    <span class="nam">version_file</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="nam">record_path</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">,</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="str">"""extracts version information from github_dump and updates version_file in-place</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="str">        version_file (str, Path): path to a file  with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t"><span class="str">        record: pull data from a _build.py file</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">repo</span> <span class="key">or</span> <span class="nam">github_dump</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">277&#x202F;&#x219B;&#x202F;278</span><span class="annotate long">line 277 didn't jump to line 278, because the condition on line 277 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">        <span class="key">if</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">            <span class="key">raise</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">InvalidGitRepoError</span><span class="op">(</span><span class="str">f"cannot find a valid git repo for {path}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">github_dump</span> <span class="key">and</span> <span class="nam">repo</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">            <span class="str">"ref"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">            <span class="str">"sha"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">target</span><span class="op">.</span><span class="nam">hex</span><span class="op">[</span><span class="op">:</span><span class="num">7</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">            <span class="str">"run_number"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">            <span class="str">"run_id"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="nam">dirty</span> <span class="op">=</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">dirty</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="nam">json</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">github_dump</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">        <span class="nam">dirty</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t"><span class="str">        dict[str,str|None]: a dict with the current config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="str">"version"</span><span class="op">:</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">        <span class="str">"current"</span><span class="op">:</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="str">"branch"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="str">"hash"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="str">"build"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">        <span class="str">"runid"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">        <span class="str">"workflow"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">version_file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">    <span class="nam">repo</span> <span class="op">=</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">lookup</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">    <span class="nam">record</span> <span class="op">=</span> <span class="nam">record_path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">record_path</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"/(?P&lt;what>beta|release)/(?P&lt;version>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">    <span class="nam">expr1</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"(?P&lt;version>\d+([.]\d+)*)(?P&lt;num>b\d+)?$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"branch"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">lstrip</span><span class="op">(</span><span class="nam">gdata</span><span class="op">[</span><span class="str">"ref"</span><span class="op">]</span><span class="op">,</span> <span class="str">"refs/heads/"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"sha"</span><span class="op">]</span> <span class="op">+</span> <span class="op">(</span><span class="str">"*"</span> <span class="key">if</span> <span class="nam">dirty</span> <span class="key">else</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"build"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"run_number"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"runid"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"run_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">result</span><span class="op">[</span><span class="str">"branch"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="nam">current</span> <span class="op">=</span> <span class="nam">result</span><span class="op">[</span><span class="str">"current"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">    <span class="key">if</span> <span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">gdata</span><span class="op">[</span><span class="str">"ref"</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">        <span class="com"># setuptools double calls the update_version,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">        <span class="com"># this fixes the issue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="nam">match1</span> <span class="op">=</span> <span class="nam">expr1</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">current</span> <span class="key">or</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">match1</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">308&#x202F;&#x219B;&#x202F;309</span><span class="annotate long">line 308 didn't jump to line 309, because the condition on line 308 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span><span class="str">f"cannot parse current version '{current}'"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">        <span class="key">if</span> <span class="nam">match1</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">                <span class="str">f"building package for {current} from '{gdata['ref']}' "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">                <span class="str">f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"what"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"beta"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"{match1.group('version')}b{gdata['run_number']}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"beta"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"tags"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">repo</span> <span class="key">or</span> <span class="nam">github_dump</span> <span class="key">or</span> <span class="nam">record</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">294&#x202F;&#x219B;&#x202F;295</span><span class="annotate long">line 294 didn't jump to line 295, because the condition on line 294 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">        <span class="key">if</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">            <span class="key">raise</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">InvalidGitRepoError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                <span class="str">f"cannot figure out settings (no repo in {path}, "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">                <span class="str">f"a GITHUB_DUMP or a _build.py file)"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">    <span class="nam">dirty</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="key">if</span> <span class="nam">github_dump</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="nam">json</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">github_dump</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">    <span class="key">elif</span> <span class="nam">record_path</span> <span class="key">and</span> <span class="nam">record_path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">305&#x202F;&#x219B;&#x202F;306</span><span class="annotate long">line 305 didn't jump to line 306, because the condition on line 305 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">        <span class="nam">mod</span> <span class="op">=</span> <span class="nam">loadmod</span><span class="op">(</span><span class="nam">record_path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">mod</span><span class="op">,</span> <span class="nam">k</span><span class="op">)</span> <span class="key">for</span> <span class="nam">k</span> <span class="key">in</span> <span class="nam">dir</span><span class="op">(</span><span class="nam">mod</span><span class="op">)</span> <span class="key">if</span> <span class="key">not</span> <span class="nam">k</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">    <span class="key">elif</span> <span class="nam">repo</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">308&#x202F;&#x219B;&#x202F;317</span><span class="annotate long">line 308 didn't jump to line 317, because the condition on line 308 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">            <span class="str">"ref"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">            <span class="str">"sha"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">target</span><span class="op">.</span><span class="nam">hex</span><span class="op">[</span><span class="op">:</span><span class="num">7</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">            <span class="str">"run_number"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">            <span class="str">"run_id"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="nam">dirty</span> <span class="op">=</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">dirty</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">        <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">"un-reacheable code"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"/(?P&lt;what>beta|release)/(?P&lt;version>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">    <span class="nam">expr1</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"(?P&lt;version>\d+([.]\d+)*)(?P&lt;num>b\d+)?$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="key">def</span> <span class="nam">update_version</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">    <span class="nam">version_file</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">    <span class="str">"""extracts version information from github_dump and updates version_file in-place</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"branch"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">lstrip</span><span class="op">(</span><span class="nam">gdata</span><span class="op">[</span><span class="str">"ref"</span><span class="op">]</span><span class="op">,</span> <span class="str">"refs/heads/"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"sha"</span><span class="op">]</span> <span class="op">+</span> <span class="op">(</span><span class="str">"*"</span> <span class="key">if</span> <span class="nam">dirty</span> <span class="key">else</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"build"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"run_number"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"runid"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"run_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">result</span><span class="op">[</span><span class="str">"branch"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">        version_file (str, Path): path to a file with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t"><span class="str">        str: the new version for the package</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">get_data</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">,</span> <span class="nam">abort</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__hash__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="key">def</span> <span class="nam">process</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">    <span class="nam">version_file</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">    <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="nam">paths</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">fixers</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">    <span class="str">"""get version from github_dump and updates version_file/paths</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="str">        paths (str, Path): path(s) to files jinja2 processeable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">        version_file (str, Path): path to a file with __version__ variable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">        str: the new version for the package</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">        {'branch': 'beta/0.3.1',</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="str">         'build': 0,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">         'current': '0.3.1',</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">         'hash': 'c9e484a*',</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t"><span class="str">         'version': '0.3.1b0',</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t"><span class="str">         'runid': 0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t"><span class="str">        }</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">from</span> <span class="nam">argparse</span> <span class="key">import</span> <span class="nam">Namespace</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">partial</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">    <span class="key">from</span> <span class="nam">urllib</span><span class="op">.</span><span class="nam">parse</span> <span class="key">import</span> <span class="nam">quote</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">    <span class="key">from</span> <span class="nam">jinja2</span> <span class="key">import</span> <span class="nam">Environment</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="key">class</span> <span class="nam">Context</span><span class="op">(</span><span class="nam">Namespace</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">        <span class="key">def</span> <span class="nam">items</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">            <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">                <span class="key">if</span> <span class="nam">name</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">377&#x202F;&#x219B;&#x202F;378</span><span class="annotate long">line 377 didn't jump to line 378, because the condition on line 377 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">                <span class="key">yield</span> <span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">get_data</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">,</span> <span class="nam">abort</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__hash__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">    <span class="nam">env</span> <span class="op">=</span> <span class="nam">Environment</span><span class="op">(</span><span class="nam">autoescape</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">env</span><span class="op">.</span><span class="nam">filters</span><span class="op">[</span><span class="str">"urlquote"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">partial</span><span class="op">(</span><span class="nam">quote</span><span class="op">,</span> <span class="nam">safe</span><span class="op">=</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="key">for</span> <span class="nam">path</span> <span class="key">in</span> <span class="nam">list_of_paths</span><span class="op">(</span><span class="nam">paths</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">apply_fixers</span><span class="op">(</span><span class="nam">path</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">fixers</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">        <span class="nam">tmpl</span> <span class="op">=</span> <span class="nam">env</span><span class="op">.</span><span class="nam">from_string</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">        <span class="nam">path</span><span class="op">.</span><span class="nam">write_text</span><span class="op">(</span><span class="nam">tmpl</span><span class="op">.</span><span class="nam">render</span><span class="op">(</span><span class="nam">ctx</span><span class="op">=</span><span class="nam">Context</span><span class="op">(</span><span class="op">**</span><span class="nam">data</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">    <span class="nam">current</span> <span class="op">=</span> <span class="nam">result</span><span class="op">[</span><span class="str">"current"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">    <span class="key">if</span> <span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">gdata</span><span class="op">[</span><span class="str">"ref"</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">        <span class="com"># setuptools double calls the update_version,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">        <span class="com"># this fixes the issue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="nam">match1</span> <span class="op">=</span> <span class="nam">expr1</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">current</span> <span class="key">or</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">match1</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">333&#x202F;&#x219B;&#x202F;334</span><span class="annotate long">line 333 didn't jump to line 334, because the condition on line 333 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span><span class="str">f"cannot parse current version '{current}'"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">        <span class="key">if</span> <span class="nam">match1</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">                <span class="str">f"building package for {current} from '{gdata['ref']}' "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">                <span class="str">f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"what"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"beta"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"{match1.group('version')}b{gdata['run_number']}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"beta"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"tags"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">,</span> <span class="nam">gdata</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t"><span class="key">def</span> <span class="nam">update_version</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">    <span class="nam">version_file</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="str">"""extracts version information from github_dump and updates version_file in-place</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">        version_file (str, Path): path to a file with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">        str: the new version for the package</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">get_data</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="nam">abort</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__hash__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t"><span class="key">def</span> <span class="nam">process</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="nam">version_file</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">    <span class="nam">paths</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">    <span class="nam">fixers</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">    <span class="nam">record</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">=</span> <span class="str">"_build.py"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="str">"""get version from github_dump and updates version_file/paths</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t"><span class="str">        version_file (str, Path): path to a file with __version__ variable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t"><span class="str">        paths (str, Path): path(s) to files jinja2 processeable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">        fixers (dict[str,str]): fixer dictionary</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="str">        record: set to True will generate a _build.py sibling of version_file</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="str">        str: the new version for the package</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t"><span class="str">        {'branch': 'beta/0.3.1',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t"><span class="str">         'build': 0,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t"><span class="str">         'current': '0.3.1',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t"><span class="str">         'hash': 'c9e484a*',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t"><span class="str">         'version': '0.3.1b0',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="str">         'runid': 0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t"><span class="str">        }</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="key">from</span> <span class="nam">argparse</span> <span class="key">import</span> <span class="nam">Namespace</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">partial</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="key">from</span> <span class="nam">urllib</span><span class="op">.</span><span class="nam">parse</span> <span class="key">import</span> <span class="nam">quote</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">    <span class="key">from</span> <span class="nam">jinja2</span> <span class="key">import</span> <span class="nam">Environment</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">    <span class="key">class</span> <span class="nam">Context</span><span class="op">(</span><span class="nam">Namespace</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">        <span class="key">def</span> <span class="nam">items</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">            <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">                <span class="key">if</span> <span class="nam">name</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">405&#x202F;&#x219B;&#x202F;406</span><span class="annotate long">line 405 didn't jump to line 406, because the condition on line 405 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">                <span class="key">yield</span> <span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="nam">record_path</span> <span class="op">=</span> <span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">version_file</span><span class="op">)</span><span class="op">.</span><span class="nam">parent</span> <span class="op">/</span> <span class="nam">record</span><span class="op">)</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">record</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="nam">data</span><span class="op">,</span> <span class="nam">gdata</span> <span class="op">=</span> <span class="nam">get_data</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">,</span> <span class="nam">record_path</span><span class="op">,</span> <span class="nam">abort</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">version_file</span><span class="op">,</span> <span class="str">"__hash__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">    <span class="nam">env</span> <span class="op">=</span> <span class="nam">Environment</span><span class="op">(</span><span class="nam">autoescape</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="nam">env</span><span class="op">.</span><span class="nam">filters</span><span class="op">[</span><span class="str">"urlquote"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">partial</span><span class="op">(</span><span class="nam">quote</span><span class="op">,</span> <span class="nam">safe</span><span class="op">=</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">    <span class="key">for</span> <span class="nam">path</span> <span class="key">in</span> <span class="nam">list_of_paths</span><span class="op">(</span><span class="nam">paths</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">apply_fixers</span><span class="op">(</span><span class="nam">path</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">fixers</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">        <span class="nam">tmpl</span> <span class="op">=</span> <span class="nam">env</span><span class="op">.</span><span class="nam">from_string</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">        <span class="nam">path</span><span class="op">.</span><span class="nam">write_text</span><span class="op">(</span><span class="nam">tmpl</span><span class="op">.</span><span class="nam">render</span><span class="op">(</span><span class="nam">ctx</span><span class="op">=</span><span class="nam">Context</span><span class="op">(</span><span class="op">**</span><span class="nam">data</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">    <span class="key">if</span> <span class="nam">record_path</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">421&#x202F;&#x219B;&#x202F;429</span><span class="annotate long">line 421 didn't jump to line 429, because the condition on line 421 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">        <span class="nam">record_path</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">mkdir</span><span class="op">(</span><span class="nam">parents</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">        <span class="key">with</span> <span class="nam">record_path</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"w"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="str">"# autogenerate build file"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">fp</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">            <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">sorted</span><span class="op">(</span><span class="op">(</span><span class="nam">gdata</span> <span class="key">or</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="str">f"'{value}'"</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="str">f"{key} = {value}"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">fp</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/tools.py: 92% ******
+****** Coverage for src/hatch_ci/tools.py: 87% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 201 statements   191 run 10 missing 0 excluded 8 partial *****
+***** 224 statements   203 run 21 missing 0 excluded 11 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.tools 
 3from __future__ import annotations 
 4 
 5import ast 
@@ -115,311 +115,353 @@
 paths)] 
 96 
 97 
 98def lstrip(txt: str, left: str) -> str: 
 99 return txt[len(left) :] if txt.startswith(left) else txt 
 100 
 101 
-102def apply_fixers(txt: str, fixers: dict[str, str] | None = None) -> str: 
-103 result = txt 
-104 for src, dst in (fixers or {}).items(): 
-105 if src.startswith("re:"): 
-106 result = re.sub(src[3:], dst, result) 
-107 else: 
-108 result = result.replace(src, dst) 
-109 return result 
-110 
-111 
-112def get_module_var( 
-113 path: Path | str, var: str = "__version__", abort=True 
-114) -> str | None: 
-115 """extract from a python module in path the module level <var> variable 
-116 
-117 Args: 
-118 path (str,Path): python module file to parse using ast (no code-execution) 
-119 var (str): module level variable name to extract 
-120 abort (bool): raise MissingVariable if var is not present 
-121 
-122 Returns: 
-123 None or str: the variable value if found or None 
-124 
-125 Raises: 
-126 MissingVariable: if the var is not found and abort is True 
-127 
-128 Notes: 
-129 this uses ast to parse path, so it doesn't load the module 
-130 """ 
-131 
-132 class V(ast.NodeVisitor): 
-133 def __init__(self, keys): 
-134 self.keys = keys 
-135 self.result = {} 
+102def loadmod(path: Path) -> Any: 
+103 from importlib.util import module_from_spec, spec_from_file_location 
+104 
+105 module = None 
+106 spec = spec_from_file_location(Path(path).name, Path(path)) 
+107 if spec: 
+108 module = module_from_spec(spec) 
+109 if module and spec and spec.loader: 
+110 spec.loader.exec_module(module) 
+111 return module 
+112 
+113 
+114def apply_fixers(txt: str, fixers: dict[str, str] | None = None) -> str: 
+115 result = txt 
+116 for src, dst in (fixers or {}).items(): 
+117 if src.startswith("re:"): 
+118 result = re.sub(src[3:], dst, result) 
+119 else: 
+120 result = result.replace(src, dst) 
+121 return result 
+122 
+123 
+124def get_module_var( 
+125 path: Path | str, var: str = "__version__", abort=True 
+126) -> str | None: 
+127 """extract from a python module in path the module level <var> variable 
+128 
+129 Args: 
+130 path (str,Path): python module file to parse using ast (no code-execution) 
+131 var (str): module level variable name to extract 
+132 abort (bool): raise MissingVariable if var is not present 
+133 
+134 Returns: 
+135 None or str: the variable value if found or None 
 136 
-137 def visit_Module(self, node): # noqa: N802 
-138 # we extract the module level variables 
-139 for subnode in ast.iter_child_nodes(node): 
-140 if not isinstance(subnode, ast.Assign): 140&#x202F;&#x219B;&#x202F;141line
-140 didn't jump to line 141, because the condition on line 140 was never true
-141 continue 
-142 for target in subnode.targets: 
-143 if target.id not in self.keys: 
-144 continue 
-145 if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)): 
-146 raise ValidationError( 
-147 f"cannot extract non Constant variable " 
-148 f"{target.id} ({type(subnode.value)})" 
-149 ) 
-150 if isinstance(subnode.value, ast.Str): 
-151 value = subnode.value.s 
-152 elif isinstance(subnode.value, ast.Num): 152&#x202F;&#x219B;&#x202F;155line
-152 didn't jump to line 155, because the condition on line 152 was never false
-153 value = subnode.value.n 
-154 else: 
-155 value = subnode.value.value 
-156 if target.id in self.result: 
-157 raise ValidationError( 
-158 f"found multiple repeated variables {target.id}" 
-159 ) 
-160 self.result[target.id] = value 
-161 return self.generic_visit(node) 
-162 
-163 v = V({var}) 
-164 path = Path(path) 
-165 if path.exists(): 
-166 tree = ast.parse(Path(path).read_text()) 
-167 v.visit(tree) 
-168 if var not in v.result and abort: 
-169 raise MissingVariableError(f"cannot find {var} in {path}", path, var) 
-170 return v.result.get(var, None) 
-171 
-172 
-173def set_module_var( 
-174 path: str | Path, var: str, value: Any, create: bool = True 
-175) -> tuple[Any, str]: 
-176 """replace var in path with value 
-177 
-178 Args: 
-179 path (str,Path): python module file to parse 
-180 var (str): module level variable name to extract 
-181 value (None or Any): if not None replace var in version_file 
-182 create (bool): create path if not present 
+137 Raises: 
+138 MissingVariable: if the var is not found and abort is True 
+139 
+140 Notes: 
+141 this uses ast to parse path, so it doesn't load the module 
+142 """ 
+143 
+144 class V(ast.NodeVisitor): 
+145 def __init__(self, keys): 
+146 self.keys = keys 
+147 self.result = {} 
+148 
+149 def visit_Module(self, node): # noqa: N802 
+150 # we extract the module level variables 
+151 for subnode in ast.iter_child_nodes(node): 
+152 if not isinstance(subnode, ast.Assign): 152&#x202F;&#x219B;&#x202F;153line
+152 didn't jump to line 153, because the condition on line 152 was never true
+153 continue 
+154 for target in subnode.targets: 
+155 if target.id not in self.keys: 
+156 continue 
+157 if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)): 
+158 raise ValidationError( 
+159 f"cannot extract non Constant variable " 
+160 f"{target.id} ({type(subnode.value)})" 
+161 ) 
+162 if isinstance(subnode.value, ast.Str): 
+163 value = subnode.value.s 
+164 elif isinstance(subnode.value, ast.Num): 164&#x202F;&#x219B;&#x202F;167line
+164 didn't jump to line 167, because the condition on line 164 was never false
+165 value = subnode.value.n 
+166 else: 
+167 value = subnode.value.value 
+168 if target.id in self.result: 
+169 raise ValidationError( 
+170 f"found multiple repeated variables {target.id}" 
+171 ) 
+172 self.result[target.id] = value 
+173 return self.generic_visit(node) 
+174 
+175 v = V({var}) 
+176 path = Path(path) 
+177 if path.exists(): 
+178 tree = ast.parse(Path(path).read_text()) 
+179 v.visit(tree) 
+180 if var not in v.result and abort: 
+181 raise MissingVariableError(f"cannot find {var} in {path}", path, var) 
+182 return v.result.get(var, None) 
 183 
-184 Returns: 
-185 (str, str) the (<previous-var-value|None>, <the new text>) 
-186 """ 
-187 
-188 # validate the var 
-189 get_module_var(path, var, abort=False) 
-190 
-191 # module level var 
-192 expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]") 
-193 fixed = None 
-194 lines = [] 
+184 
+185def set_module_var( 
+186 path: str | Path, var: str, value: Any, create: bool = True 
+187) -> tuple[Any, str]: 
+188 """replace var in path with value 
+189 
+190 Args: 
+191 path (str,Path): python module file to parse 
+192 var (str): module level variable name to extract 
+193 value (None or Any): if not None replace var in version_file 
+194 create (bool): create path if not present 
 195 
-196 src = Path(path) 
-197 if not src.exists() and create: 
-198 src.parent.mkdir(parents=True, exist_ok=True) 
-199 src.touch() 
-200 
-201 input_lines = src.read_text().split("\n") 
-202 for line in input_lines: 
-203 if fixed is not None: 
-204 lines.append(line) 
-205 continue 
-206 match = expr.search(line) 
-207 if match: 
-208 fixed = match.group("value") 
-209 if value is not None: 209&#x202F;&#x219B;&#x202F;212line 209 didn't jump to
-line 212, because the condition on line 209 was never false
-210 x, y = match.span(1) 
-211 line = line[:x] + value + line[y:] 
-212 lines.append(line) 
-213 txt = "\n".join(lines) 
-214 if (fixed is None) and create: 
-215 if txt and txt[-1] != "\n": 
-216 txt += "\n" 
-217 txt += f'{var} = "{value}"' 
-218 
-219 with Path(path).open("w") as fp: 
-220 fp.write(txt) 
-221 return fixed, txt 
-222 
-223 
-224def bump_version(version: str, mode: str) -> str: 
-225 """given a version str will bump it according to mode 
-226 
-227 Arguments: 
-228 version: text in the N.M.O form 
-229 mode: major, minor or micro 
+196 Returns: 
+197 (str, str) the (<previous-var-value|None>, <the new text>) 
+198 """ 
+199 
+200 # validate the var 
+201 get_module_var(path, var, abort=False) 
+202 
+203 # module level var 
+204 expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]") 
+205 fixed = None 
+206 lines = [] 
+207 
+208 src = Path(path) 
+209 if not src.exists() and create: 
+210 src.parent.mkdir(parents=True, exist_ok=True) 
+211 src.touch() 
+212 
+213 input_lines = src.read_text().split("\n") 
+214 for line in input_lines: 
+215 if fixed is not None: 
+216 lines.append(line) 
+217 continue 
+218 match = expr.search(line) 
+219 if match: 
+220 fixed = match.group("value") 
+221 if value is not None: 221&#x202F;&#x219B;&#x202F;224line 221 didn't jump to
+line 224, because the condition on line 221 was never false
+222 x, y = match.span(1) 
+223 line = line[:x] + value + line[y:] 
+224 lines.append(line) 
+225 txt = "\n".join(lines) 
+226 if (fixed is None) and create: 
+227 if txt and txt[-1] != "\n": 
+228 txt += "\n" 
+229 txt += f'{var} = "{value}"' 
 230 
-231 Returns: 
-232 increased text 
-233 
-234 >>> bump_version("1.0.3", "micro") 
-235 "1.0.4" 
-236 >>> bump_version("1.0.3", "minor") 
-237 "1.1.0" 
-238 """ 
-239 newver = [int(n) for n in version.split(".")] 
-240 if mode == "major": 
-241 newver[-3] += 1 
-242 newver[-2] = 0 
-243 newver[-1] = 0 
-244 elif mode == "minor": 
-245 newver[-2] += 1 
-246 newver[-1] = 0 
-247 elif mode == "micro": 
-248 newver[-1] += 1 
-249 return ".".join(str(v) for v in newver) 
-250 
-251 
-252def get_data( 
-253 version_file: str | Path, github_dump: str | None = None, abort: bool =
-True 
-254) -> dict[str, str | None]: 
-255 """extracts version information from github_dump and updates version_file
+231 with Path(path).open("w") as fp: 
+232 fp.write(txt) 
+233 return fixed, txt 
+234 
+235 
+236def bump_version(version: str, mode: str) -> str: 
+237 """given a version str will bump it according to mode 
+238 
+239 Arguments: 
+240 version: text in the N.M.O form 
+241 mode: major, minor or micro 
+242 
+243 Returns: 
+244 increased text 
+245 
+246 >>> bump_version("1.0.3", "micro") 
+247 "1.0.4" 
+248 >>> bump_version("1.0.3", "minor") 
+249 "1.1.0" 
+250 """ 
+251 newver = [int(n) for n in version.split(".")] 
+252 if mode == "major": 
+253 newver[-3] += 1 
+254 newver[-2] = 0 
+255 newver[-1] = 0 
+256 elif mode == "minor": 
+257 newver[-2] += 1 
+258 newver[-1] = 0 
+259 elif mode == "micro": 
+260 newver[-1] += 1 
+261 return ".".join(str(v) for v in newver) 
+262 
+263 
+264def get_data( 
+265 version_file: str | Path, 
+266 github_dump: str | None = None, 
+267 record_path: Path | None = None, 
+268 abort: bool = True, 
+269) -> tuple[dict[str, str | None], dict[str, Any]]: 
+270 """extracts version information from github_dump and updates version_file
 in-place 
-256 
-257 Args: 
-258 version_file (str, Path): path to a file with a __version__ variable 
-259 github_dump (str): the os.getenv("GITHUB_DUMP") value 
-260 
-261 Returns: 
-262 dict[str,str|None]: a dict with the current config 
-263 """ 
-264 result = { 
-265 "version": get_module_var(version_file, "__version__"), 
-266 "current": get_module_var(version_file, "__version__"), 
-267 "branch": None, 
-268 "hash": None, 
-269 "build": None, 
-270 "runid": None, 
-271 "workflow": None, 
-272 } 
-273 
-274 path = Path(version_file) 
-275 repo = scm.lookup(path) 
+271 
+272 Args: 
+273 version_file (str, Path): path to a file with a __version__ variable 
+274 github_dump (str): the os.getenv("GITHUB_DUMP") value 
+275 record: pull data from a _build.py file 
 276 
-277 if not (repo or github_dump): 277&#x202F;&#x219B;&#x202F;278line 277 didn't
-jump to line 278, because the condition on line 277 was never true
-278 if abort: 
-279 raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}") 
-280 return result 
-281 
-282 if not github_dump and repo: 
-283 gdata = { 
-284 "ref": repo.head.name, 
-285 "sha": repo.head.target.hex[:7], 
-286 "run_number": 0, 
-287 "run_id": 0, 
+277 Returns: 
+278 dict[str,str|None]: a dict with the current config 
+279 """ 
+280 result = { 
+281 "version": get_module_var(version_file, "__version__"), 
+282 "current": get_module_var(version_file, "__version__"), 
+283 "branch": None, 
+284 "hash": None, 
+285 "build": None, 
+286 "runid": None, 
+287 "workflow": None, 
 288 } 
-289 dirty = repo.dirty() 
-290 else: 
-291 gdata = json.loads(github_dump) if isinstance(github_dump, str) else
-github_dump 
-292 dirty = False 
+289 
+290 path = Path(version_file) 
+291 repo = scm.lookup(path) 
+292 record = record_path.exists() if record_path else None 
 293 
-294 expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$") 
-295 expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$") 
-296 
-297 result["branch"] = lstrip(gdata["ref"], "refs/heads/") 
-298 result["hash"] = gdata["sha"] + ("*" if dirty else "") 
-299 result["build"] = gdata["run_number"] 
-300 result["runid"] = gdata["run_id"] 
-301 result["workflow"] = result["branch"] 
-302 
-303 current = result["current"] 
-304 if match := expr.search(gdata["ref"]): 
-305 # setuptools double calls the update_version, 
-306 # this fixes the issue 
-307 match1 = expr1.search(current or "") 
-308 if not match1: 308&#x202F;&#x219B;&#x202F;309line 308 didn't jump to line
-309, because the condition on line 308 was never true
-309 raise InvalidVersionError(f"cannot parse current version '{current}'") 
-310 if match1.group("version") != match.group("version"): 
-311 raise InvalidVersionError( 
-312 f"building package for {current} from '{gdata['ref']}' " 
-313 f"branch ({match.groupdict()} mismatch {match1.groupdict()})" 
-314 ) 
-315 if match.group("what") == "beta": 
-316 result["version"] = f"{match1.group('version')}b{gdata['run_number']}" 
-317 result["workflow"] = "beta" 
-318 else: 
-319 result["workflow"] = "tags" 
-320 return result 
+294 if not (repo or github_dump or record): 294&#x202F;&#x219B;&#x202F;295line
+294 didn't jump to line 295, because the condition on line 294 was never true
+295 if abort: 
+296 raise scm.InvalidGitRepoError( 
+297 f"cannot figure out settings (no repo in {path}, " 
+298 f"a GITHUB_DUMP or a _build.py file)" 
+299 ) 
+300 return result, {} 
+301 
+302 dirty = False 
+303 if github_dump: 
+304 gdata = json.loads(github_dump) if isinstance(github_dump, str) else
+github_dump 
+305 elif record_path and record_path.exists():
+ 305&#x202F;&#x219B;&#x202F;306line 305 didn't jump to line 306, because the
+condition on line 305 was never true
+306 mod = loadmod(record_path) 
+307 gdata = {k: getattr(mod, k) for k in dir(mod) if not k.startswith("_")} 
+308 elif repo: 308&#x202F;&#x219B;&#x202F;317line 308 didn't jump to line 317,
+because the condition on line 308 was never false
+309 gdata = { 
+310 "ref": repo.head.name, 
+311 "sha": repo.head.target.hex[:7], 
+312 "run_number": 0, 
+313 "run_id": 0, 
+314 } 
+315 dirty = repo.dirty() 
+316 else: 
+317 raise RuntimeError("un-reacheable code") 
+318 
+319 expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$") 
+320 expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$") 
 321 
-322 
-323def update_version( 
-324 version_file: str | Path, github_dump: str | None = None, abort: bool =
+322 result["branch"] = lstrip(gdata["ref"], "refs/heads/") 
+323 result["hash"] = gdata["sha"] + ("*" if dirty else "") 
+324 result["build"] = gdata["run_number"] 
+325 result["runid"] = gdata["run_id"] 
+326 result["workflow"] = result["branch"] 
+327 
+328 current = result["current"] 
+329 if match := expr.search(gdata["ref"]): 
+330 # setuptools double calls the update_version, 
+331 # this fixes the issue 
+332 match1 = expr1.search(current or "") 
+333 if not match1: 333&#x202F;&#x219B;&#x202F;334line 333 didn't jump to line
+334, because the condition on line 333 was never true
+334 raise InvalidVersionError(f"cannot parse current version '{current}'") 
+335 if match1.group("version") != match.group("version"): 
+336 raise InvalidVersionError( 
+337 f"building package for {current} from '{gdata['ref']}' " 
+338 f"branch ({match.groupdict()} mismatch {match1.groupdict()})" 
+339 ) 
+340 if match.group("what") == "beta": 
+341 result["version"] = f"{match1.group('version')}b{gdata['run_number']}" 
+342 result["workflow"] = "beta" 
+343 else: 
+344 result["workflow"] = "tags" 
+345 return result, gdata 
+346 
+347 
+348def update_version( 
+349 version_file: str | Path, github_dump: str | None = None, abort: bool =
 True 
-325) -> str | None: 
-326 """extracts version information from github_dump and updates version_file
+350) -> str | None: 
+351 """extracts version information from github_dump and updates version_file
 in-place 
-327 
-328 Args: 
-329 version_file (str, Path): path to a file with a __version__ variable 
-330 github_dump (str): the os.getenv("GITHUB_DUMP") value 
-331 
-332 Returns: 
-333 str: the new version for the package 
-334 """ 
-335 
-336 data = get_data(version_file, github_dump, abort) 
-337 set_module_var(version_file, "__version__", data["version"]) 
-338 set_module_var(version_file, "__hash__", data["hash"]) 
-339 return data["version"] 
-340 
-341 
-342def process( 
-343 version_file: str | Path, 
-344 github_dump: str | None = None, 
-345 paths: str | Path | list[str | Path] | None = None, 
-346 fixers: dict[str, str] | None = None, 
-347 abort: bool = True, 
-348) -> dict[str, str | None]: 
-349 """get version from github_dump and updates version_file/paths 
-350 
-351 Args: 
-352 paths (str, Path): path(s) to files jinja2 processeable 
-353 version_file (str, Path): path to a file with __version__ variable 
-354 github_dump (str): the os.getenv("GITHUB_DUMP") value 
-355 
-356 Returns: 
-357 str: the new version for the package 
-358 
-359 Example: 
-360 {'branch': 'beta/0.3.1', 
-361 'build': 0, 
-362 'current': '0.3.1', 
-363 'hash': 'c9e484a*', 
-364 'version': '0.3.1b0', 
-365 'runid': 0 
-366 } 
-367 """ 
-368 from argparse import Namespace 
-369 from functools import partial 
-370 from urllib.parse import quote 
-371 
-372 from jinja2 import Environment 
-373 
-374 class Context(Namespace): 
-375 def items(self): 
-376 for name, value in self.__dict__.items(): 
-377 if name.startswith("_"): 377&#x202F;&#x219B;&#x202F;378line 377 didn't jump
-to line 378, because the condition on line 377 was never true
-378 continue 
-379 yield (name, value) 
-380 
-381 data = get_data(version_file, github_dump, abort) 
-382 set_module_var(version_file, "__version__", data["version"]) 
-383 set_module_var(version_file, "__hash__", data["hash"]) 
-384 
-385 env = Environment(autoescape=True) 
-386 env.filters["urlquote"] = partial(quote, safe="") 
-387 for path in list_of_paths(paths): 
-388 txt = apply_fixers(path.read_text(), fixers) 
-389 tmpl = env.from_string(txt) 
-390 path.write_text(tmpl.render(ctx=Context(**data))) 
-391 return data 
+352 
+353 Args: 
+354 version_file (str, Path): path to a file with a __version__ variable 
+355 github_dump (str): the os.getenv("GITHUB_DUMP") value 
+356 
+357 Returns: 
+358 str: the new version for the package 
+359 """ 
+360 
+361 data = get_data(version_file, github_dump, abort=abort)[0] 
+362 set_module_var(version_file, "__version__", data["version"]) 
+363 set_module_var(version_file, "__hash__", data["hash"]) 
+364 return data["version"] 
+365 
+366 
+367def process( 
+368 version_file: str | Path, 
+369 github_dump: str | None = None, 
+370 paths: str | Path | list[str | Path] | None = None, 
+371 fixers: dict[str, str] | None = None, 
+372 record: str | Path = "_build.py", 
+373 abort: bool = True, 
+374) -> dict[str, str | None]: 
+375 """get version from github_dump and updates version_file/paths 
+376 
+377 Args: 
+378 version_file (str, Path): path to a file with __version__ variable 
+379 github_dump (str): the os.getenv("GITHUB_DUMP") value 
+380 paths (str, Path): path(s) to files jinja2 processeable 
+381 fixers (dict[str,str]): fixer dictionary 
+382 record: set to True will generate a _build.py sibling of version_file 
+383 
+384 Returns: 
+385 str: the new version for the package 
+386 
+387 Example: 
+388 {'branch': 'beta/0.3.1', 
+389 'build': 0, 
+390 'current': '0.3.1', 
+391 'hash': 'c9e484a*', 
+392 'version': '0.3.1b0', 
+393 'runid': 0 
+394 } 
+395 """ 
+396 from argparse import Namespace 
+397 from functools import partial 
+398 from urllib.parse import quote 
+399 
+400 from jinja2 import Environment 
+401 
+402 class Context(Namespace): 
+403 def items(self): 
+404 for name, value in self.__dict__.items(): 
+405 if name.startswith("_"): 405&#x202F;&#x219B;&#x202F;406line 405 didn't jump
+to line 406, because the condition on line 405 was never true
+406 continue 
+407 yield (name, value) 
+408 
+409 record_path = (Path(version_file).parent / record).absolute() if record
+else None 
+410 data, gdata = get_data(version_file, github_dump, record_path, abort) 
+411 set_module_var(version_file, "__version__", data["version"]) 
+412 set_module_var(version_file, "__hash__", data["hash"]) 
+413 
+414 env = Environment(autoescape=True) 
+415 env.filters["urlquote"] = partial(quote, safe="") 
+416 for path in list_of_paths(paths): 
+417 txt = apply_fixers(path.read_text(), fixers) 
+418 tmpl = env.from_string(txt) 
+419 path.write_text(tmpl.render(ctx=Context(**data))) 
+420 
+421 if record_path: 421&#x202F;&#x219B;&#x202F;429line 421 didn't jump to line
+429, because the condition on line 421 was never false
+422 record_path.parent.mkdir(parents=True, exist_ok=True) 
+423 with record_path.open("w") as fp: 
+424 print("# autogenerate build file", file=fp) 
+425 for key, value in sorted((gdata or {}).items()): 
+426 value = f"'{value}'" if isinstance(value, str) else value 
+427 print(f"{key} = {value}", file=fp) 
+428 
+429 return data 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -139,24 +139,24 @@
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">version_file</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">                <span class="str">f"no 'version-file' key for plugin {self.PLUGIN_NAME}"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">process</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="nam">version_file</span><span class="op">,</span> <span class="nam">getenv</span><span class="op">(</span><span class="str">"GITHUB_DUMP"</span><span class="op">)</span><span class="op">,</span> <span class="nam">paths</span><span class="op">=</span><span class="nam">paths</span><span class="op">,</span> <span class="nam">fixers</span><span class="op">=</span><span class="nam">fixers</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="str">"version"</span><span class="op">:</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
 
 
 1from __future__ import annotations 
 2 
 3from typing import Any 
 4 
 5from hatchling.version.source.plugin.interface import VersionSourceInterface 
@@ -71,12 +71,12 @@
 55 
 56 if not version_file.exists(): 
 57 raise ValidationError( 
 58 f"no 'version-file' key for plugin {self.PLUGIN_NAME}" 
 59 ) 
 60 gdata = tools.process( 
 61 version_file, getenv("GITHUB_DUMP"), paths=paths, fixers=fixers 
-62 ) 
+62 )[0] 
 63 return {"version": gdata["version"]} 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 09:36 +0000
+at 2023-08-07 20:13 +0000
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/index.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">60%</span>
+            <span class="pc_cov">59%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -43,15 +43,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -108,61 +108,61 @@
                 <td>0</td>
                 <td>52</td>
                 <td>8</td>
                 <td class="right" data-ratio="175 214">82%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_script_py.html">src/hatch_ci/script.py</a></td>
-                <td>67</td>
-                <td>67</td>
+                <td>66</td>
+                <td>66</td>
                 <td>2</td>
                 <td>20</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 87">0%</td>
+                <td class="right" data-ratio="0 86">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_tools_py.html">src/hatch_ci/tools.py</a></td>
-                <td>201</td>
-                <td>10</td>
+                <td>224</td>
+                <td>21</td>
                 <td>0</td>
-                <td>84</td>
-                <td>8</td>
-                <td class="right" data-ratio="263 285">92%</td>
+                <td>98</td>
+                <td>11</td>
+                <td class="right" data-ratio="280 322">87%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_version_hook_py.html">src/hatch_ci/version_hook.py</a></td>
                 <td>40</td>
                 <td>40</td>
                 <td>0</td>
                 <td>14</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 54">0%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>550</td>
-                <td>222</td>
+                <td>572</td>
+                <td>232</td>
                 <td>2</td>
-                <td>188</td>
-                <td>16</td>
-                <td class="right" data-ratio="440 738">60%</td>
+                <td>202</td>
+                <td>19</td>
+                <td class="right" data-ratio="457 774">59%</td>
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
-            created at 2023-08-07 09:36 +0000
+            created at 2023-08-07 20:13 +0000
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
@@ -1,25 +1,25 @@
 
-****** Coverage report: 60% ******
+****** Coverage report: 59% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-08-07 09:36 +0000
+coverage.py_v7.2.7, created at 2023-08-07 20:13 +0000
 
 Module                   statements missing excluded branches partial coverage
 src/hatch_ci/__init__.py 2          0       0        0        0       100%
 src/hatch_ci/cli.py      72         72      0        18       0       0%
 src/hatch_ci/common.py   1          1       0        0        0       0%
 src/hatch_ci/hooks.py    5          5       0        0        0       0%
 src/hatch_ci/scm.py      162        27      0        52       8       82%
-src/hatch_ci/script.py   67         67      2        20       0       0%
-src/hatch_ci/tools.py    201        10      0        84       8       92%
+src/hatch_ci/script.py   66         66      2        20       0       0%
+src/hatch_ci/tools.py    224        21      0        98       11      87%
 src/hatch_ci/            40         40      0        14       0       0%
 version_hook.py
-Total                    550        222     2        188      16      60%
+Total                    572        232     2        202      19      59%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-08-07 09:36 +0000
+coverage.py_v7.2.7, created at 2023-08-07 20:13 +0000
  ____
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/status.json` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/status.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.866806891025641%*

 * *Differences: {"'files'": "{'d_7005a4ce5d73f943_scm_py': {'hash': 'b208d1663706f031c634592ef10b4313'}, "*

 * *            "'d_7005a4ce5d73f943_script_py': {'hash': '8ee62da09a4cade164014211a2cdbea5', 'index': "*

 * *            "{'nums': {insert: [(2, 66), (4, 66)], delete: [4, 2]}}}, "*

 * *            "'d_7005a4ce5d73f943_tools_py': {'hash': '85d900cb995532ebb0a96d363886ec40', 'index': "*

 * *            "{'nums': {insert: [(2, 224), (4, 21), (5, 98), (6, 11), (7, 21)], delete: [7, 6, 5, "*

 * *            "4, 2]}}}, 'd_7005a4ce5d73f943_versio […]*

```diff
@@ -65,15 +65,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/hatch_ci/hooks.py"
             }
         },
         "d_7005a4ce5d73f943_scm_py": {
-            "hash": "09485baef443027d4b5d7014a9e7d1aa",
+            "hash": "b208d1663706f031c634592ef10b4313",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_scm_py.html",
                 "nums": [
                     0,
                     1,
                     162,
                     0,
@@ -82,49 +82,49 @@
                     8,
                     12
                 ],
                 "relative_filename": "src/hatch_ci/scm.py"
             }
         },
         "d_7005a4ce5d73f943_script_py": {
-            "hash": "1f1f9597ce7c541f1fe029e8c67db0ee",
+            "hash": "8ee62da09a4cade164014211a2cdbea5",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_script_py.html",
                 "nums": [
                     0,
                     1,
-                    67,
+                    66,
                     2,
-                    67,
+                    66,
                     20,
                     0,
                     20
                 ],
                 "relative_filename": "src/hatch_ci/script.py"
             }
         },
         "d_7005a4ce5d73f943_tools_py": {
-            "hash": "920e588d8d5656224648cba4f71d8359",
+            "hash": "85d900cb995532ebb0a96d363886ec40",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_tools_py.html",
                 "nums": [
                     0,
                     1,
-                    201,
+                    224,
                     0,
-                    10,
-                    84,
-                    8,
-                    12
+                    21,
+                    98,
+                    11,
+                    21
                 ],
                 "relative_filename": "src/hatch_ci/tools.py"
             }
         },
         "d_7005a4ce5d73f943_version_hook_py": {
-            "hash": "d8574928e09ee770fc8c01204295b58e",
+            "hash": "197d56b78147cb520d768df9d8c6d098",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_version_hook_py.html",
                 "nums": [
                     0,
                     1,
                     40,
                     0,
@@ -134,10 +134,10 @@
                     14
                 ],
                 "relative_filename": "src/hatch_ci/version_hook.py"
             }
         }
     },
     "format": 2,
-    "globals": "fdfd0fb9cac86f6bd55b132a994cbf47",
+    "globals": "67047f35a6135996fb3c824e7903a7a4",
     "version": "7.2.7"
 }
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/coverage/style.css` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/style.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/junit/junit.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.html`

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
-    <p>Report generated on 07-Aug-2023 at 09:36:34 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
+    <p>Report generated on 07-Aug-2023 at 20:13:25 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
     <h2>Summary</h2>
-    <p>16 tests ran in 1.54 seconds. </p>
+    <p>16 tests ran in 1.49 seconds. </p>
     <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">16 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
     <h2>Results</h2>
     <table id="results-table">
       <thead id="results-table-head">
         <tr>
           <th class="sortable result initial-sort" col="result">Result</th>
           <th class="sortable" col="name">Test</th>
@@ -462,25 +462,25 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_handle_remote_and_local_repos</td>
-          <td class="col-duration">0.34</td>
+          <td class="col-duration">0.32</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Switched to a new branch &#x27;beta/0.0.4&#x27;
 Switched to branch &#x27;master&#x27;
 Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.2&#x27;
-Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/LEX51V&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/0C95EU&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.1&#x27;
 fatal: a branch named &#x27;master&#x27; already exists
 From /tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
  * [new branch]      beta/0.0.2 -&gt; repo1/beta/0.0.2
  * [new branch]      master     -&gt; repo1/master
 <br/></div></td></tr></tbody>
@@ -596,25 +596,25 @@
 Updated 1 path from the index
 Switched to a new branch &#x27;beta/0.0.2&#x27;
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_release</td>
-          <td class="col-duration">0.09</td>
+          <td class="col-duration">0.08</td>
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
-          <td class="col-duration">0.16</td>
+          <td class="col-duration">0.17</td>
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
-Report generated on 07-Aug-2023 at 09:36:34 by pytest-html v3.2.0
+Report generated on 07-Aug-2023 at 20:13:25 by pytest-html v3.2.0
 ***** Summary *****
-16 tests ran in 1.54 seconds.
+16 tests ran in 1.49 seconds.
 (Un)check the boxes to filter the results.
 *16 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
 unexpected passes
 ***** Results *****
 Result Test                                                  Duration Links
 No results found. Try to check the filters
 Passed tests/test_scm.py::test_lookup                        0.04
 No log output captured.
-Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.34
+Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.32
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Switched to a new branch
 &#x27;beta/0.0.4&#x27; Switched to branch &#x27;master&#x27; Cloning into
 &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/
 test_check_version-repo1&#x27;... done. Switched to a new branch &#x27;beta/
 0.0.2&#x27; Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/
-test_handle_remote_and_local_r0/LEX51V&#x27;... done. Switched to a new
+test_handle_remote_and_local_r0/0C95EU&#x27;... done. Switched to a new
 branch &#x27;beta/0.0.1&#x27; fatal: a branch named &#x27;master&#x27;
 already exists From /tmp/pytest-of-runner/pytest-0/
 test_handle_remote_and_local_r0/test_check_version-repo1 * [new branch]
 beta/0.0.2 -> repo1/beta/0.0.2 * [new branch] master -> repo1/master
 Passed tests/test_tools.py::test_abort_exception             0.00
 No log output captured.
 Passed tests/test_tools.py::test_urmtree                     0.00
@@ -47,17 +47,17 @@
 No log output captured.
 Passed tests/test_tools.py::test_update_version_beta         0.14
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.4&#x27; Updated 1 path from the
 index Updated 1 path from the index Switched to a new branch &#x27;beta/
 0.0.2&#x27;
-Passed tests/test_tools.py::test_update_version_release      0.09
+Passed tests/test_tools.py::test_update_version_release      0.08
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Updated 1 path from the
 index
-Passed tests/test_tools.py::test_process                     0.16
+Passed tests/test_tools.py::test_process                     0.17
 ------------------------------Captured stderr call--------------------------
 ----
 Updated 1 path from the index Switched to a new branch &#x27;beta/
 1.2.3&#x27;
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.xml`

 * *Files 3% similar despite different names*

#### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.xml`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <testsuites>
-  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="16" time="1.475" timestamp="2023-08-07T09:36:32.773066" hostname="fv-az351-917">
-    <testcase classname="tests.test_scm" name="test_lookup" time="0.042"/>
-    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.348"/>
+  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="16" time="1.468" timestamp="2023-08-07T20:13:23.703498" hostname="fv-az563-119">
+    <testcase classname="tests.test_scm" name="test_lookup" time="0.046"/>
+    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.329"/>
     <testcase classname="tests.test_tools" name="test_abort_exception" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_urmtree" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_indent" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_list_of_paths" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_lstrip" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_apply_fixers" time="0.004"/>
-    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.004"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.005"/>
+    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.003"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.007"/>
     <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_bump_version" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.067"/>
-    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.146"/>
-    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.091"/>
-    <testcase classname="tests.test_tools" name="test_process" time="0.163"/>
+    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.065"/>
+    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.142"/>
+    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.083"/>
+    <testcase classname="tests.test_tools" name="test_process" time="0.173"/>
   </testsuite>
 </testsuites>
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/index.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 <thead><tr class="summary">
 <th class="summary">File</th>
 <th class="summary">Imprecision</th>
 <th class="summary">Lines</th>
 </tr></thead>
 <tfoot><tr class="summary summary-quality-1">
 <th class="summary summary-filename">Total</th>
-<th class="summary summary-precision">18.69% imprecise</th>
-<th class="summary summary-lines">1038 LOC</th>
+<th class="summary summary-precision">18.88% imprecise</th>
+<th class="summary summary-lines">1075 LOC</th>
 </tr></tfoot>
 <tbody>
 <tr class="summary summary-quality-0">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/__init__.py.html">hatch_ci</a></td>
 <td class="summary summary-precision">0.00% imprecise</td>
 <td class="summary summary-lines">2 LOC</td>
 </tr>
@@ -41,24 +41,24 @@
 <tr class="summary summary-quality-1">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/scm.py.html">hatch_ci.scm</a></td>
 <td class="summary summary-precision">9.02% imprecise</td>
 <td class="summary summary-lines">266 LOC</td>
 </tr>
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/script.py.html">hatch_ci.script</a></td>
-<td class="summary summary-precision">26.90% imprecise</td>
-<td class="summary summary-lines">171 LOC</td>
+<td class="summary summary-precision">26.47% imprecise</td>
+<td class="summary summary-lines">170 LOC</td>
 </tr>
-<tr class="summary summary-quality-1">
+<tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/tools.py.html">hatch_ci.tools</a></td>
-<td class="summary summary-precision">19.95% imprecise</td>
-<td class="summary summary-lines">391 LOC</td>
+<td class="summary summary-precision">20.28% imprecise</td>
+<td class="summary summary-lines">429 LOC</td>
 </tr>
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/version_hook.py.html">hatch_ci.version_hook</a></td>
-<td class="summary summary-precision">25.40% imprecise</td>
+<td class="summary summary-precision">26.98% imprecise</td>
 <td class="summary summary-lines">63 LOC</td>
 </tr>
 </tbody>
 </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 
 ****** Mypy Type Check Coverage Summary ******
               Summary from index
 File                  Imprecision      Lines
-Total                 18.69% imprecise 1038 LOC
+Total                 18.88% imprecise 1075 LOC
 hatch_ci              0.00% imprecise  2 LOC
 hatch_ci.cli          19.85% imprecise 136 LOC
 hatch_ci.common       0.00% imprecise  1 LOC
 hatch_ci.hooks        37.50% imprecise 8 LOC
 hatch_ci.scm          9.02% imprecise  266 LOC
-hatch_ci.script       26.90% imprecise 171 LOC
-hatch_ci.tools        19.95% imprecise 391 LOC
-hatch_ci.version_hook 25.40% imprecise 63 LOC
+hatch_ci.script       26.47% imprecise 170 LOC
+hatch_ci.tools        20.28% imprecise 429 LOC
+hatch_ci.version_hook 26.98% imprecise 63 LOC
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,14 @@
 <span id="L164" class="lineno"><a class="lineno" href="#L164">164</a></span>
 <span id="L165" class="lineno"><a class="lineno" href="#L165">165</a></span>
 <span id="L166" class="lineno"><a class="lineno" href="#L166">166</a></span>
 <span id="L167" class="lineno"><a class="lineno" href="#L167">167</a></span>
 <span id="L168" class="lineno"><a class="lineno" href="#L168">168</a></span>
 <span id="L169" class="lineno"><a class="lineno" href="#L169">169</a></span>
 <span id="L170" class="lineno"><a class="lineno" href="#L170">170</a></span>
-<span id="L171" class="lineno"><a class="lineno" href="#L171">171</a></span>
 </pre></td>
 <td class="table-code"><pre><span class="line-empty" title="No Anys on this line!">"""create a beta branch or release a beta branch</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">This script will either create a new beta branch:</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">     hatch-ci make-beta ./src/package_name/__init__.py</span>
 <span class="line-empty" title="No Anys on this line!"></span>
@@ -310,16 +309,14 @@
 <span class="line-precise" title="No Anys on this line!">                continue</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x3)
 Error (x1)">            options.error(f"branch '{branch}' already present")</span>
 <span class="line-precise" title="No Anys on this line!">        log.info("creating branch '%s'", f"/beta/{version}")</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x5)">        options.repo.branch(f"beta/{version}", master)</span>
-<span class="line-any" title="Any Types on this line: 
-Unannotated (x4)">        options.repo(["checkout", master])</span>
 <span class="line-precise" title="No Anys on this line!">        print(  # noqa: T201</span>
 <span class="line-precise" title="No Anys on this line!">            tools.indent(</span>
 <span class="line-precise" title="No Anys on this line!">                f"""</span>
 <span class="line-empty" title="No Anys on this line!">        The release branch beta/{version} has been created.</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">        To complete the release:</span>
 <span class="line-empty" title="No Anys on this line!">            git push origin beta/{version}</span>
```

#### html2text {}

```diff
@@ -102,80 +102,79 @@
 96          for branch in [*options.repo.branches.local,
 97  *options.repo.branches.remote]:
 98              if not branch.endswith(f"beta/{version}"):
 99                  continue
 100             options.error(f"branch '{branch}' already present")
 101         log.info("creating branch '%s'", f"/beta/{version}")
 102         options.repo.branch(f"beta/{version}", master)
-103         options.repo(["checkout", master])
-104         print(  # noqa: T201
-105             tools.indent(
-106                 f"""
-107         The release branch beta/{version} has been created.
-108
-109         To complete the release:
-110             git push origin beta/{version}
-111
-112         To revert this beta branch:
-113             git branch -D beta/{version}
-114         """
-115             ),
-116             file=sys.stderr,
-117         )
-118     elif options.mode in {"micro", "minor", "major"}:
-119         # we need to be in the beta/N.M.O branch
-120         expr = re.compile(r"refs/heads/beta/(?P<beta>\d+([.]\d+)*)$")
-121         if not (match := expr.search(options.repo.head.name)):
-122             options.error(
-123                 f"wrong branch '{options.repo.head.shorthand}'",
-124                 f"expected to be in 'beta/{version}' branch",
-125                 f"git checkout beta/{version}",
-126             )
-127             return
-128         local = match.group("beta")
-129         if local != version:
-130             options.error(f"wrong version file {version=} != {local}")
-131
-132         # create an empty commit to mark the release
-133         options.repo(["commit", "--allow-empty", "-m", f"released
-134 {version}"])
-135
-136         # tag
-137         options.repo(["tag", "-a", f"release/{version}", "-m", f"released
-138 {version}"])
-139
-140         # switch to master (and incorporate the commit message)
-141         options.repo(["checkout", master])
-142         options.repo(["merge", f"beta/{version}"])
-143
-144         # bump version
-145         new_version = tools.bump_version(version, options.mode)
-146         tools.set_module_var(options.initfile, "__version__", new_version)
-147
-148         # commit
-149         options.repo.commit(
-150             options.initfile, f"version bump {version} -> {new_version}"
-151         )
-152
-153         print(  # noqa: T201
-154             tools.indent(
-155                 f"""
-156         The release is almost complete.
-157
-158         To complete the release:
-159             git push origin release/{version}
-160             git push origin master
-161
-162         To revert this release:
-163             git reset --hard HEAD~1
-164             git tag -d release/{version}
-165         """
-166             ),
-167             file=sys.stderr,
-168         )
-169     else:
-170         options.error(f"unsupported mode {options.mode=}")
-171         raise RuntimeError(f"unsupported mode {options.mode=}")
+103         print(  # noqa: T201
+104             tools.indent(
+105                 f"""
+106         The release branch beta/{version} has been created.
+107
+108         To complete the release:
+109             git push origin beta/{version}
+110
+111         To revert this beta branch:
+112             git branch -D beta/{version}
+113         """
+114             ),
+115             file=sys.stderr,
+116         )
+117     elif options.mode in {"micro", "minor", "major"}:
+118         # we need to be in the beta/N.M.O branch
+119         expr = re.compile(r"refs/heads/beta/(?P<beta>\d+([.]\d+)*)$")
+120         if not (match := expr.search(options.repo.head.name)):
+121             options.error(
+122                 f"wrong branch '{options.repo.head.shorthand}'",
+123                 f"expected to be in 'beta/{version}' branch",
+124                 f"git checkout beta/{version}",
+125             )
+126             return
+127         local = match.group("beta")
+128         if local != version:
+129             options.error(f"wrong version file {version=} != {local}")
+130
+131         # create an empty commit to mark the release
+132         options.repo(["commit", "--allow-empty", "-m", f"released
+133 {version}"])
+134
+135         # tag
+136         options.repo(["tag", "-a", f"release/{version}", "-m", f"released
+137 {version}"])
+138
+139         # switch to master (and incorporate the commit message)
+140         options.repo(["checkout", master])
+141         options.repo(["merge", f"beta/{version}"])
+142
+143         # bump version
+144         new_version = tools.bump_version(version, options.mode)
+145         tools.set_module_var(options.initfile, "__version__", new_version)
+146
+147         # commit
+148         options.repo.commit(
+149             options.initfile, f"version bump {version} -> {new_version}"
+150         )
+151
+152         print(  # noqa: T201
+153             tools.indent(
+154                 f"""
+155         The release is almost complete.
+156
+157         To complete the release:
+158             git push origin release/{version}
+159             git push origin master
+160
+161         To revert this release:
+162             git reset --hard HEAD~1
+163             git tag -d release/{version}
+164         """
+165             ),
+166             file=sys.stderr,
+167         )
+168     else:
+169         options.error(f"unsupported mode {options.mode=}")
+170         raise RuntimeError(f"unsupported mode {options.mode=}")
 
 
     if __name__ == "__main__":
         main()
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html`

 * *Files 4% similar despite different names*

```diff
@@ -395,14 +395,52 @@
 <span id="L385" class="lineno"><a class="lineno" href="#L385">385</a></span>
 <span id="L386" class="lineno"><a class="lineno" href="#L386">386</a></span>
 <span id="L387" class="lineno"><a class="lineno" href="#L387">387</a></span>
 <span id="L388" class="lineno"><a class="lineno" href="#L388">388</a></span>
 <span id="L389" class="lineno"><a class="lineno" href="#L389">389</a></span>
 <span id="L390" class="lineno"><a class="lineno" href="#L390">390</a></span>
 <span id="L391" class="lineno"><a class="lineno" href="#L391">391</a></span>
+<span id="L392" class="lineno"><a class="lineno" href="#L392">392</a></span>
+<span id="L393" class="lineno"><a class="lineno" href="#L393">393</a></span>
+<span id="L394" class="lineno"><a class="lineno" href="#L394">394</a></span>
+<span id="L395" class="lineno"><a class="lineno" href="#L395">395</a></span>
+<span id="L396" class="lineno"><a class="lineno" href="#L396">396</a></span>
+<span id="L397" class="lineno"><a class="lineno" href="#L397">397</a></span>
+<span id="L398" class="lineno"><a class="lineno" href="#L398">398</a></span>
+<span id="L399" class="lineno"><a class="lineno" href="#L399">399</a></span>
+<span id="L400" class="lineno"><a class="lineno" href="#L400">400</a></span>
+<span id="L401" class="lineno"><a class="lineno" href="#L401">401</a></span>
+<span id="L402" class="lineno"><a class="lineno" href="#L402">402</a></span>
+<span id="L403" class="lineno"><a class="lineno" href="#L403">403</a></span>
+<span id="L404" class="lineno"><a class="lineno" href="#L404">404</a></span>
+<span id="L405" class="lineno"><a class="lineno" href="#L405">405</a></span>
+<span id="L406" class="lineno"><a class="lineno" href="#L406">406</a></span>
+<span id="L407" class="lineno"><a class="lineno" href="#L407">407</a></span>
+<span id="L408" class="lineno"><a class="lineno" href="#L408">408</a></span>
+<span id="L409" class="lineno"><a class="lineno" href="#L409">409</a></span>
+<span id="L410" class="lineno"><a class="lineno" href="#L410">410</a></span>
+<span id="L411" class="lineno"><a class="lineno" href="#L411">411</a></span>
+<span id="L412" class="lineno"><a class="lineno" href="#L412">412</a></span>
+<span id="L413" class="lineno"><a class="lineno" href="#L413">413</a></span>
+<span id="L414" class="lineno"><a class="lineno" href="#L414">414</a></span>
+<span id="L415" class="lineno"><a class="lineno" href="#L415">415</a></span>
+<span id="L416" class="lineno"><a class="lineno" href="#L416">416</a></span>
+<span id="L417" class="lineno"><a class="lineno" href="#L417">417</a></span>
+<span id="L418" class="lineno"><a class="lineno" href="#L418">418</a></span>
+<span id="L419" class="lineno"><a class="lineno" href="#L419">419</a></span>
+<span id="L420" class="lineno"><a class="lineno" href="#L420">420</a></span>
+<span id="L421" class="lineno"><a class="lineno" href="#L421">421</a></span>
+<span id="L422" class="lineno"><a class="lineno" href="#L422">422</a></span>
+<span id="L423" class="lineno"><a class="lineno" href="#L423">423</a></span>
+<span id="L424" class="lineno"><a class="lineno" href="#L424">424</a></span>
+<span id="L425" class="lineno"><a class="lineno" href="#L425">425</a></span>
+<span id="L426" class="lineno"><a class="lineno" href="#L426">426</a></span>
+<span id="L427" class="lineno"><a class="lineno" href="#L427">427</a></span>
+<span id="L428" class="lineno"><a class="lineno" href="#L428">428</a></span>
+<span id="L429" class="lineno"><a class="lineno" href="#L429">429</a></span>
 </pre></td>
 <td class="table-code"><pre><span class="line-empty" title="No Anys on this line!"># see https://pypi.org/project/setuptools-github</span>
 <span class="line-empty" title="No Anys on this line!"># copy of setuptools_github.tools</span>
 <span class="line-precise" title="No Anys on this line!">from __future__ import annotations</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">import ast</span>
 <span class="line-precise" title="No Anys on this line!">import json</span>
@@ -511,14 +549,28 @@
 Explicit (x2)">    return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">def lstrip(txt: str, left: str) -&gt; str:</span>
 <span class="line-precise" title="No Anys on this line!">    return txt[len(left) :] if txt.startswith(left) else txt</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x1)">def loadmod(path: Path) -&gt; Any:</span>
+<span class="line-precise" title="No Anys on this line!">    from importlib.util import module_from_spec, spec_from_file_location</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    module = None</span>
+<span class="line-precise" title="Any Types on this line: 
+Explicit (x2)">    spec = spec_from_file_location(Path(path).name, Path(path))</span>
+<span class="line-precise" title="No Anys on this line!">    if spec:</span>
+<span class="line-precise" title="No Anys on this line!">        module = module_from_spec(spec)</span>
+<span class="line-precise" title="No Anys on this line!">    if module and spec and spec.loader:</span>
+<span class="line-precise" title="No Anys on this line!">        spec.loader.exec_module(module)</span>
+<span class="line-precise" title="No Anys on this line!">    return module</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">def apply_fixers(txt: str, fixers: dict[str, str] | None = None) -&gt; str:</span>
 <span class="line-precise" title="No Anys on this line!">    result = txt</span>
 <span class="line-precise" title="No Anys on this line!">    for src, dst in (fixers or {}).items():</span>
 <span class="line-precise" title="No Anys on this line!">        if src.startswith("re:"):</span>
 <span class="line-precise" title="No Anys on this line!">            result = re.sub(src[3:], dst, result)</span>
 <span class="line-empty" title="No Anys on this line!">        else:</span>
 <span class="line-precise" title="No Anys on this line!">            result = result.replace(src, dst)</span>
@@ -568,18 +620,17 @@
 <span class="line-any" title="No Anys on this line!">                        continue</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)
 Explicit (x6)">                    if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)):</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x1)">                        raise ValidationError(</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x8)">                            f"cannot extract non Constant variable "</span>
-<span class="line-any" title="Any Types on this line: 
-Unannotated (x2)
-Explicit (x2)">                            f"{target.id} ({type(subnode.value)})"</span>
+Unannotated (x10)
+Explicit (x2)">                            f"cannot extract non Constant variable "</span>
+<span class="line-empty" title="No Anys on this line!">                            f"{target.id} ({type(subnode.value)})"</span>
 <span class="line-empty" title="No Anys on this line!">                        )</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)
 Explicit (x2)">                    if isinstance(subnode.value, ast.Str):</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">                        value = subnode.value.s</span>
 <span class="line-any" title="Any Types on this line: 
@@ -704,22 +755,27 @@
 <span class="line-precise" title="No Anys on this line!">        newver[-2] += 1</span>
 <span class="line-precise" title="No Anys on this line!">        newver[-1] = 0</span>
 <span class="line-precise" title="No Anys on this line!">    elif mode == "micro":</span>
 <span class="line-precise" title="No Anys on this line!">        newver[-1] += 1</span>
 <span class="line-precise" title="No Anys on this line!">    return ".".join(str(v) for v in newver)</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="No Anys on this line!">def get_data(</span>
-<span class="line-precise" title="No Anys on this line!">    version_file: str | Path, github_dump: str | None = None, abort: bool = True</span>
-<span class="line-empty" title="No Anys on this line!">) -&gt; dict[str, str | None]:</span>
+<span class="line-imprecise" title="Any Types on this line: 
+Explicit (x1)">def get_data(</span>
+<span class="line-empty" title="No Anys on this line!">    version_file: str | Path,</span>
+<span class="line-precise" title="No Anys on this line!">    github_dump: str | None = None,</span>
+<span class="line-precise" title="No Anys on this line!">    record_path: Path | None = None,</span>
+<span class="line-precise" title="No Anys on this line!">    abort: bool = True,</span>
+<span class="line-empty" title="No Anys on this line!">) -&gt; tuple[dict[str, str | None], dict[str, Any]]:</span>
 <span class="line-empty" title="No Anys on this line!">    """extracts version information from github_dump and updates version_file in-place</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Args:</span>
 <span class="line-empty" title="No Anys on this line!">        version_file (str, Path): path to a file  with a __version__ variable</span>
 <span class="line-empty" title="No Anys on this line!">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>
+<span class="line-empty" title="No Anys on this line!">        record: pull data from a _build.py file</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Returns:</span>
 <span class="line-empty" title="No Anys on this line!">        dict[str,str|None]: a dict with the current config</span>
 <span class="line-empty" title="No Anys on this line!">    """</span>
 <span class="line-precise" title="No Anys on this line!">    result = {</span>
 <span class="line-precise" title="Any Types on this line: 
 Unannotated (x1)">        "version": get_module_var(version_file, "__version__"),</span>
@@ -731,79 +787,88 @@
 <span class="line-precise" title="No Anys on this line!">        "runid": None,</span>
 <span class="line-precise" title="No Anys on this line!">        "workflow": None,</span>
 <span class="line-empty" title="No Anys on this line!">    }</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="Any Types on this line: 
 Explicit (x1)">    path = Path(version_file)</span>
 <span class="line-precise" title="No Anys on this line!">    repo = scm.lookup(path)</span>
+<span class="line-precise" title="No Anys on this line!">    record = record_path.exists() if record_path else None</span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="No Anys on this line!">    if not (repo or github_dump):</span>
+<span class="line-precise" title="No Anys on this line!">    if not (repo or github_dump or record):</span>
 <span class="line-precise" title="No Anys on this line!">        if abort:</span>
-<span class="line-precise" title="No Anys on this line!">            raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}")</span>
-<span class="line-precise" title="No Anys on this line!">        return result</span>
+<span class="line-precise" title="No Anys on this line!">            raise scm.InvalidGitRepoError(</span>
+<span class="line-precise" title="No Anys on this line!">                f"cannot figure out settings (no repo in {path}, "</span>
+<span class="line-empty" title="No Anys on this line!">                f"a GITHUB_DUMP or a _build.py file)"</span>
+<span class="line-empty" title="No Anys on this line!">            )</span>
+<span class="line-precise" title="No Anys on this line!">        return result, {}</span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="No Anys on this line!">    if not github_dump and repo:</span>
-<span class="line-imprecise" title="Any Types on this line: 
-Unannotated (x1)">        gdata = {</span>
+<span class="line-precise" title="No Anys on this line!">    dirty = False</span>
+<span class="line-precise" title="No Anys on this line!">    if github_dump:</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x13)">        gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump</span>
+<span class="line-precise" title="No Anys on this line!">    elif record_path and record_path.exists():</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x3)">        mod = loadmod(record_path)</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x16)
+Omitted Generics (x2)">        gdata = {k: getattr(mod, k) for k in dir(mod) if not k.startswith("_")}</span>
+<span class="line-precise" title="No Anys on this line!">    elif repo:</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x1)">        gdata = {</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">            "ref": repo.head.name,</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x4)">            "sha": repo.head.target.hex[:7],</span>
 <span class="line-precise" title="No Anys on this line!">            "run_number": 0,</span>
 <span class="line-precise" title="No Anys on this line!">            "run_id": 0,</span>
 <span class="line-empty" title="No Anys on this line!">        }</span>
 <span class="line-precise" title="No Anys on this line!">        dirty = repo.dirty()</span>
 <span class="line-empty" title="No Anys on this line!">    else:</span>
-<span class="line-any" title="Any Types on this line: 
-Explicit (x12)
-Unannotated (x1)">        gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump</span>
-<span class="line-precise" title="No Anys on this line!">        dirty = False</span>
+<span class="line-precise" title="No Anys on this line!">        raise RuntimeError("un-reacheable code")</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="Any Types on this line: 
 Omitted Generics (x4)">    expr = re.compile(r"/(?P&lt;what&gt;beta|release)/(?P&lt;version&gt;\d+([.]\d+)*)$")</span>
 <span class="line-precise" title="Any Types on this line: 
 Omitted Generics (x4)">    expr1 = re.compile(r"(?P&lt;version&gt;\d+([.]\d+)*)(?P&lt;num&gt;b\d+)?$")</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x2)">    result["branch"] = lstrip(gdata["ref"], "refs/heads/")</span>
+Explicit (x2)">    result["branch"] = lstrip(gdata["ref"], "refs/heads/")</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x3)">    result["hash"] = gdata["sha"] + ("*" if dirty else "")</span>
+Explicit (x3)">    result["hash"] = gdata["sha"] + ("*" if dirty else "")</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x2)">    result["build"] = gdata["run_number"]</span>
+Explicit (x2)">    result["build"] = gdata["run_number"]</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x2)">    result["runid"] = gdata["run_id"]</span>
+Explicit (x2)">    result["runid"] = gdata["run_id"]</span>
 <span class="line-precise" title="No Anys on this line!">    result["workflow"] = result["branch"]</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">    current = result["current"]</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x2)">    if match := expr.search(gdata["ref"]):</span>
+Explicit (x2)">    if match := expr.search(gdata["ref"]):</span>
 <span class="line-empty" title="No Anys on this line!">        # setuptools double calls the update_version,</span>
 <span class="line-empty" title="No Anys on this line!">        # this fixes the issue</span>
 <span class="line-precise" title="No Anys on this line!">        match1 = expr1.search(current or "")</span>
 <span class="line-precise" title="No Anys on this line!">        if not match1:</span>
 <span class="line-precise" title="No Anys on this line!">            raise InvalidVersionError(f"cannot parse current version '{current}'")</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x7)">        if match1.group("version") != match.group("version"):</span>
 <span class="line-precise" title="No Anys on this line!">            raise InvalidVersionError(</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x2)
-Explicit (x2)">                f"building package for {current} from '{gdata['ref']}' "</span>
-<span class="line-precise" title="Any Types on this line: 
-Explicit (x2)
-Omitted Generics (x4)">                f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>
+Explicit (x6)
+Omitted Generics (x4)">                f"building package for {current} from '{gdata['ref']}' "</span>
+<span class="line-empty" title="No Anys on this line!">                f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>
 <span class="line-empty" title="No Anys on this line!">            )</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x4)">        if match.group("what") == "beta":</span>
 <span class="line-any" title="Any Types on this line: 
-Explicit (x3)
-Unannotated (x2)">            result["version"] = f"{match1.group('version')}b{gdata['run_number']}"</span>
+Explicit (x5)">            result["version"] = f"{match1.group('version')}b{gdata['run_number']}"</span>
 <span class="line-precise" title="No Anys on this line!">            result["workflow"] = "beta"</span>
 <span class="line-empty" title="No Anys on this line!">        else:</span>
 <span class="line-precise" title="No Anys on this line!">            result["workflow"] = "tags"</span>
-<span class="line-precise" title="No Anys on this line!">    return result</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x1)">    return result, gdata</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">def update_version(</span>
 <span class="line-precise" title="No Anys on this line!">    version_file: str | Path, github_dump: str | None = None, abort: bool = True</span>
 <span class="line-empty" title="No Anys on this line!">) -&gt; str | None:</span>
 <span class="line-empty" title="No Anys on this line!">    """extracts version information from github_dump and updates version_file in-place</span>
 <span class="line-empty" title="No Anys on this line!"></span>
@@ -811,35 +876,39 @@
 <span class="line-empty" title="No Anys on this line!">        version_file (str, Path): path to a file with a __version__ variable</span>
 <span class="line-empty" title="No Anys on this line!">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Returns:</span>
 <span class="line-empty" title="No Anys on this line!">        str: the new version for the package</span>
 <span class="line-empty" title="No Anys on this line!">    """</span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="No Anys on this line!">    data = get_data(version_file, github_dump, abort)</span>
+<span class="line-imprecise" title="Any Types on this line: 
+Explicit (x2)">    data = get_data(version_file, github_dump, abort=abort)[0]</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)">    set_module_var(version_file, "__version__", data["version"])</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)">    set_module_var(version_file, "__hash__", data["hash"])</span>
 <span class="line-precise" title="No Anys on this line!">    return data["version"]</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">def process(</span>
 <span class="line-empty" title="No Anys on this line!">    version_file: str | Path,</span>
 <span class="line-precise" title="No Anys on this line!">    github_dump: str | None = None,</span>
 <span class="line-precise" title="No Anys on this line!">    paths: str | Path | list[str | Path] | None = None,</span>
 <span class="line-precise" title="No Anys on this line!">    fixers: dict[str, str] | None = None,</span>
+<span class="line-precise" title="No Anys on this line!">    record: str | Path = "_build.py",</span>
 <span class="line-precise" title="No Anys on this line!">    abort: bool = True,</span>
 <span class="line-empty" title="No Anys on this line!">) -&gt; dict[str, str | None]:</span>
 <span class="line-empty" title="No Anys on this line!">    """get version from github_dump and updates version_file/paths</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Args:</span>
-<span class="line-empty" title="No Anys on this line!">        paths (str, Path): path(s) to files jinja2 processeable</span>
 <span class="line-empty" title="No Anys on this line!">        version_file (str, Path): path to a file with __version__ variable</span>
 <span class="line-empty" title="No Anys on this line!">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>
+<span class="line-empty" title="No Anys on this line!">        paths (str, Path): path(s) to files jinja2 processeable</span>
+<span class="line-empty" title="No Anys on this line!">        fixers (dict[str,str]): fixer dictionary</span>
+<span class="line-empty" title="No Anys on this line!">        record: set to True will generate a _build.py sibling of version_file</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Returns:</span>
 <span class="line-empty" title="No Anys on this line!">        str: the new version for the package</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Example:</span>
 <span class="line-empty" title="No Anys on this line!">        {'branch': 'beta/0.3.1',</span>
 <span class="line-empty" title="No Anys on this line!">         'build': 0,</span>
@@ -861,15 +930,18 @@
 Unannotated (x5)">            for name, value in self.__dict__.items():</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x3)">                if name.startswith("_"):</span>
 <span class="line-any" title="No Anys on this line!">                    continue</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">                yield (name, value)</span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="No Anys on this line!">    data = get_data(version_file, github_dump, abort)</span>
+<span class="line-precise" title="Any Types on this line: 
+Explicit (x1)">    record_path = (Path(version_file).parent / record).absolute() if record else None</span>
+<span class="line-imprecise" title="Any Types on this line: 
+Explicit (x3)">    data, gdata = get_data(version_file, github_dump, record_path, abort)</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)">    set_module_var(version_file, "__version__", data["version"])</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)">    set_module_var(version_file, "__hash__", data["hash"])</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="Any Types on this line: 
 Explicit (x3)">    env = Environment(autoescape=True)</span>
@@ -878,13 +950,27 @@
 Explicit (x4)">    env.filters["urlquote"] = partial(quote, safe="")</span>
 <span class="line-precise" title="No Anys on this line!">    for path in list_of_paths(paths):</span>
 <span class="line-precise" title="No Anys on this line!">        txt = apply_fixers(path.read_text(), fixers)</span>
 <span class="line-precise" title="Any Types on this line: 
 Explicit (x1)">        tmpl = env.from_string(txt)</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)">        path.write_text(tmpl.render(ctx=Context(**data)))</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    if record_path:</span>
+<span class="line-precise" title="No Anys on this line!">        record_path.parent.mkdir(parents=True, exist_ok=True)</span>
+<span class="line-precise" title="Any Types on this line: 
+Explicit (x1)">        with record_path.open("w") as fp:</span>
+<span class="line-precise" title="No Anys on this line!">            print("# autogenerate build file", file=fp)</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x6)
+Omitted Generics (x5)">            for key, value in sorted((gdata or {}).items()):</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x3)">                value = f"'{value}'" if isinstance(value, str) else value</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x1)">                print(f"{key} = {value}", file=fp)</span>
+<span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">    return data</span>
 </pre></td>
 </tr></tbody>
 </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -102,313 +102,352 @@
 89  else paths)]
 90
 91
 92  def lstrip(txt: str, left: str) -> str:
 93      return txt[len(left) :] if txt.startswith(left) else txt
 94
 95
-96  def apply_fixers(txt: str, fixers: dict[str, str] | None = None) -> str:
-97      result = txt
-98      for src, dst in (fixers or {}).items():
-99          if src.startswith("re:"):
-100             result = re.sub(src[3:], dst, result)
-101         else:
-102             result = result.replace(src, dst)
-103     return result
-104
-105
-106 def get_module_var(
-107     path: Path | str, var: str = "__version__", abort=True
-108 ) -> str | None:
-109     """extract from a python module in path the module level <var> variable
-110
-111     Args:
-112         path (str,Path): python module file to parse using ast (no code-
-113 execution)
-114         var (str): module level variable name to extract
-115         abort (bool): raise MissingVariable if var is not present
+96  def loadmod(path: Path) -> Any:
+97      from importlib.util import module_from_spec, spec_from_file_location
+98
+99      module = None
+100     spec = spec_from_file_location(Path(path).name, Path(path))
+101     if spec:
+102         module = module_from_spec(spec)
+103     if module and spec and spec.loader:
+104         spec.loader.exec_module(module)
+105     return module
+106
+107
+108 def apply_fixers(txt: str, fixers: dict[str, str] | None = None) -> str:
+109     result = txt
+110     for src, dst in (fixers or {}).items():
+111         if src.startswith("re:"):
+112             result = re.sub(src[3:], dst, result)
+113         else:
+114             result = result.replace(src, dst)
+115     return result
 116
-117     Returns:
-118         None or str: the variable value if found or None
-119
-120     Raises:
-121         MissingVariable: if the var is not found and abort is True
+117
+118 def get_module_var(
+119     path: Path | str, var: str = "__version__", abort=True
+120 ) -> str | None:
+121     """extract from a python module in path the module level <var> variable
 122
-123     Notes:
-124         this uses ast to parse path, so it doesn't load the module
-125     """
-126
-127     class V(ast.NodeVisitor):
-128         def __init__(self, keys):
-129             self.keys = keys
-130             self.result = {}
+123     Args:
+124         path (str,Path): python module file to parse using ast (no code-
+125 execution)
+126         var (str): module level variable name to extract
+127         abort (bool): raise MissingVariable if var is not present
+128
+129     Returns:
+130         None or str: the variable value if found or None
 131
-132         def visit_Module(self, node):  # noqa: N802
-133             # we extract the module level variables
-134             for subnode in ast.iter_child_nodes(node):
-135                 if not isinstance(subnode, ast.Assign):
-136                     continue
-137                 for target in subnode.targets:
-138                     if target.id not in self.keys:
-139                         continue
-140                     if not isinstance(subnode.value, (ast.Num, ast.Str,
-141 ast.Constant)):
-142                         raise ValidationError(
-143                             f"cannot extract non Constant variable "
-144                             f"{target.id} ({type(subnode.value)})"
-145                         )
-146                     if isinstance(subnode.value, ast.Str):
-147                         value = subnode.value.s
-148                     elif isinstance(subnode.value, ast.Num):
-149                         value = subnode.value.n
-150                     else:
-151                         value = subnode.value.value
-152                     if target.id in self.result:
-153                         raise ValidationError(
-154                             f"found multiple repeated variables
-155 {target.id}"
-156                         )
-157                     self.result[target.id] = value
-158             return self.generic_visit(node)
-159
-160     v = V({var})
-161     path = Path(path)
-162     if path.exists():
-163         tree = ast.parse(Path(path).read_text())
-164         v.visit(tree)
-165     if var not in v.result and abort:
-166         raise MissingVariableError(f"cannot find {var} in {path}", path,
-167 var)
-168     return v.result.get(var, None)
-169
-170
-171 def set_module_var(
-172     path: str | Path, var: str, value: Any, create: bool = True
-173 ) -> tuple[Any, str]:
-174     """replace var in path with value
-175
-176     Args:
-177         path (str,Path): python module file to parse
-178         var (str): module level variable name to extract
-179         value (None or Any): if not None replace var in version_file
-180         create (bool): create path if not present
+132     Raises:
+133         MissingVariable: if the var is not found and abort is True
+134
+135     Notes:
+136         this uses ast to parse path, so it doesn't load the module
+137     """
+138
+139     class V(ast.NodeVisitor):
+140         def __init__(self, keys):
+141             self.keys = keys
+142             self.result = {}
+143
+144         def visit_Module(self, node):  # noqa: N802
+145             # we extract the module level variables
+146             for subnode in ast.iter_child_nodes(node):
+147                 if not isinstance(subnode, ast.Assign):
+148                     continue
+149                 for target in subnode.targets:
+150                     if target.id not in self.keys:
+151                         continue
+152                     if not isinstance(subnode.value, (ast.Num, ast.Str,
+153 ast.Constant)):
+154                         raise ValidationError(
+155                             f"cannot extract non Constant variable "
+156                             f"{target.id} ({type(subnode.value)})"
+157                         )
+158                     if isinstance(subnode.value, ast.Str):
+159                         value = subnode.value.s
+160                     elif isinstance(subnode.value, ast.Num):
+161                         value = subnode.value.n
+162                     else:
+163                         value = subnode.value.value
+164                     if target.id in self.result:
+165                         raise ValidationError(
+166                             f"found multiple repeated variables
+167 {target.id}"
+168                         )
+169                     self.result[target.id] = value
+170             return self.generic_visit(node)
+171
+172     v = V({var})
+173     path = Path(path)
+174     if path.exists():
+175         tree = ast.parse(Path(path).read_text())
+176         v.visit(tree)
+177     if var not in v.result and abort:
+178         raise MissingVariableError(f"cannot find {var} in {path}", path,
+179 var)
+180     return v.result.get(var, None)
 181
-182     Returns:
-183         (str, str) the (<previous-var-value|None>, <the new text>)
-184     """
-185
-186     # validate the var
-187     get_module_var(path, var, abort=False)
-188
-189     # module level var
-190     expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]")
-191     fixed = None
-192     lines = []
+182
+183 def set_module_var(
+184     path: str | Path, var: str, value: Any, create: bool = True
+185 ) -> tuple[Any, str]:
+186     """replace var in path with value
+187
+188     Args:
+189         path (str,Path): python module file to parse
+190         var (str): module level variable name to extract
+191         value (None or Any): if not None replace var in version_file
+192         create (bool): create path if not present
 193
-194     src = Path(path)
-195     if not src.exists() and create:
-196         src.parent.mkdir(parents=True, exist_ok=True)
-197         src.touch()
-198
-199     input_lines = src.read_text().split("\n")
-200     for line in input_lines:
-201         if fixed is not None:
-202             lines.append(line)
-203             continue
-204         match = expr.search(line)
-205         if match:
-206             fixed = match.group("value")
-207             if value is not None:
-208                 x, y = match.span(1)
-209                 line = line[:x] + value + line[y:]
-210         lines.append(line)
-211     txt = "\n".join(lines)
-212     if (fixed is None) and create:
-213         if txt and txt[-1] != "\n":
-214             txt += "\n"
-215         txt += f'{var} = "{value}"'
-216
-217     with Path(path).open("w") as fp:
-218         fp.write(txt)
-219     return fixed, txt
-220
-221
-222 def bump_version(version: str, mode: str) -> str:
-223     """given a version str will bump it according to mode
-224
-225     Arguments:
-226         version: text in the N.M.O form
-227         mode: major, minor or micro
+194     Returns:
+195         (str, str) the (<previous-var-value|None>, <the new text>)
+196     """
+197
+198     # validate the var
+199     get_module_var(path, var, abort=False)
+200
+201     # module level var
+202     expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]")
+203     fixed = None
+204     lines = []
+205
+206     src = Path(path)
+207     if not src.exists() and create:
+208         src.parent.mkdir(parents=True, exist_ok=True)
+209         src.touch()
+210
+211     input_lines = src.read_text().split("\n")
+212     for line in input_lines:
+213         if fixed is not None:
+214             lines.append(line)
+215             continue
+216         match = expr.search(line)
+217         if match:
+218             fixed = match.group("value")
+219             if value is not None:
+220                 x, y = match.span(1)
+221                 line = line[:x] + value + line[y:]
+222         lines.append(line)
+223     txt = "\n".join(lines)
+224     if (fixed is None) and create:
+225         if txt and txt[-1] != "\n":
+226             txt += "\n"
+227         txt += f'{var} = "{value}"'
 228
-229     Returns:
-230         increased text
-231
-232     >>> bump_version("1.0.3", "micro")
-233     "1.0.4"
-234     >>> bump_version("1.0.3", "minor")
-235     "1.1.0"
-236     """
-237     newver = [int(n) for n in version.split(".")]
-238     if mode == "major":
-239         newver[-3] += 1
-240         newver[-2] = 0
-241         newver[-1] = 0
-242     elif mode == "minor":
-243         newver[-2] += 1
-244         newver[-1] = 0
-245     elif mode == "micro":
-246         newver[-1] += 1
-247     return ".".join(str(v) for v in newver)
-248
-249
-250 def get_data(
-251     version_file: str | Path, github_dump: str | None = None, abort: bool =
-252 True
-253 ) -> dict[str, str | None]:
-254     """extracts version information from github_dump and updates
-255 version_file in-place
-256
-257     Args:
-258         version_file (str, Path): path to a file  with a __version__
-259 variable
-260         github_dump (str): the os.getenv("GITHUB_DUMP") value
+229     with Path(path).open("w") as fp:
+230         fp.write(txt)
+231     return fixed, txt
+232
+233
+234 def bump_version(version: str, mode: str) -> str:
+235     """given a version str will bump it according to mode
+236
+237     Arguments:
+238         version: text in the N.M.O form
+239         mode: major, minor or micro
+240
+241     Returns:
+242         increased text
+243
+244     >>> bump_version("1.0.3", "micro")
+245     "1.0.4"
+246     >>> bump_version("1.0.3", "minor")
+247     "1.1.0"
+248     """
+249     newver = [int(n) for n in version.split(".")]
+250     if mode == "major":
+251         newver[-3] += 1
+252         newver[-2] = 0
+253         newver[-1] = 0
+254     elif mode == "minor":
+255         newver[-2] += 1
+256         newver[-1] = 0
+257     elif mode == "micro":
+258         newver[-1] += 1
+259     return ".".join(str(v) for v in newver)
+260
 261
-262     Returns:
-263         dict[str,str|None]: a dict with the current config
-264     """
-265     result = {
-266         "version": get_module_var(version_file, "__version__"),
-267         "current": get_module_var(version_file, "__version__"),
-268         "branch": None,
-269         "hash": None,
-270         "build": None,
-271         "runid": None,
-272         "workflow": None,
-273     }
-274
-275     path = Path(version_file)
-276     repo = scm.lookup(path)
-277
-278     if not (repo or github_dump):
-279         if abort:
-280             raise scm.InvalidGitRepoError(f"cannot find a valid git repo
-281 for {path}")
-282         return result
-283
-284     if not github_dump and repo:
-285         gdata = {
-286             "ref": repo.head.name,
-287             "sha": repo.head.target.hex[:7],
-288             "run_number": 0,
-289             "run_id": 0,
-290         }
-291         dirty = repo.dirty()
-292     else:
-293         gdata = json.loads(github_dump) if isinstance(github_dump, str)
-294 else github_dump
-295         dirty = False
-296
-297     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+(
-298 [.]\d+)*)$")
-299     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
-300
-301     result["branch"] = lstrip(gdata["ref"], "refs/heads/")
-302     result["hash"] = gdata["sha"] + ("*" if dirty else "")
-303     result["build"] = gdata["run_number"]
-304     result["runid"] = gdata["run_id"]
-305     result["workflow"] = result["branch"]
-306
-307     current = result["current"]
-308     if match := expr.search(gdata["ref"]):
-309         # setuptools double calls the update_version,
-310         # this fixes the issue
-311         match1 = expr1.search(current or "")
-312         if not match1:
-313             raise InvalidVersionError(f"cannot parse current version '
-314 {current}'")
-315         if match1.group("version") != match.group("version"):
-316             raise InvalidVersionError(
-317                 f"building package for {current} from '{gdata['ref']}' "
-318                 f"branch ({match.groupdict()} mismatch {match1.groupdict
-319 ()})"
-320             )
-321         if match.group("what") == "beta":
-322             result["version"] = f"{match1.group('version')}b{gdata
-323 ['run_number']}"
-324             result["workflow"] = "beta"
-325         else:
-326             result["workflow"] = "tags"
-327     return result
-328
-329
-330 def update_version(
-331     version_file: str | Path, github_dump: str | None = None, abort: bool =
-332 True
-333 ) -> str | None:
-334     """extracts version information from github_dump and updates
-335 version_file in-place
-336
-337     Args:
-338         version_file (str, Path): path to a file with a __version__
-339 variable
-340         github_dump (str): the os.getenv("GITHUB_DUMP") value
-341
-342     Returns:
-343         str: the new version for the package
-344     """
-345
-346     data = get_data(version_file, github_dump, abort)
-347     set_module_var(version_file, "__version__", data["version"])
-348     set_module_var(version_file, "__hash__", data["hash"])
-349     return data["version"]
-350
-351
-352 def process(
-353     version_file: str | Path,
-354     github_dump: str | None = None,
-355     paths: str | Path | list[str | Path] | None = None,
-356     fixers: dict[str, str] | None = None,
-357     abort: bool = True,
-358 ) -> dict[str, str | None]:
-359     """get version from github_dump and updates version_file/paths
+262 def get_data(
+263     version_file: str | Path,
+264     github_dump: str | None = None,
+265     record_path: Path | None = None,
+266     abort: bool = True,
+267 ) -> tuple[dict[str, str | None], dict[str, Any]]:
+268     """extracts version information from github_dump and updates
+269 version_file in-place
+270
+271     Args:
+272         version_file (str, Path): path to a file  with a __version__
+273 variable
+274         github_dump (str): the os.getenv("GITHUB_DUMP") value
+275         record: pull data from a _build.py file
+276
+277     Returns:
+278         dict[str,str|None]: a dict with the current config
+279     """
+280     result = {
+281         "version": get_module_var(version_file, "__version__"),
+282         "current": get_module_var(version_file, "__version__"),
+283         "branch": None,
+284         "hash": None,
+285         "build": None,
+286         "runid": None,
+287         "workflow": None,
+288     }
+289
+290     path = Path(version_file)
+291     repo = scm.lookup(path)
+292     record = record_path.exists() if record_path else None
+293
+294     if not (repo or github_dump or record):
+295         if abort:
+296             raise scm.InvalidGitRepoError(
+297                 f"cannot figure out settings (no repo in {path}, "
+298                 f"a GITHUB_DUMP or a _build.py file)"
+299             )
+300         return result, {}
+301
+302     dirty = False
+303     if github_dump:
+304         gdata = json.loads(github_dump) if isinstance(github_dump, str)
+305 else github_dump
+306     elif record_path and record_path.exists():
+307         mod = loadmod(record_path)
+308         gdata = {k: getattr(mod, k) for k in dir(mod) if not k.startswith
+309 ("_")}
+310     elif repo:
+311         gdata = {
+312             "ref": repo.head.name,
+313             "sha": repo.head.target.hex[:7],
+314             "run_number": 0,
+315             "run_id": 0,
+316         }
+317         dirty = repo.dirty()
+318     else:
+319         raise RuntimeError("un-reacheable code")
+320
+321     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+(
+322 [.]\d+)*)$")
+323     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
+324
+325     result["branch"] = lstrip(gdata["ref"], "refs/heads/")
+326     result["hash"] = gdata["sha"] + ("*" if dirty else "")
+327     result["build"] = gdata["run_number"]
+328     result["runid"] = gdata["run_id"]
+329     result["workflow"] = result["branch"]
+330
+331     current = result["current"]
+332     if match := expr.search(gdata["ref"]):
+333         # setuptools double calls the update_version,
+334         # this fixes the issue
+335         match1 = expr1.search(current or "")
+336         if not match1:
+337             raise InvalidVersionError(f"cannot parse current version '
+338 {current}'")
+339         if match1.group("version") != match.group("version"):
+340             raise InvalidVersionError(
+341                 f"building package for {current} from '{gdata['ref']}' "
+342                 f"branch ({match.groupdict()} mismatch {match1.groupdict
+343 ()})"
+344             )
+345         if match.group("what") == "beta":
+346             result["version"] = f"{match1.group('version')}b{gdata
+347 ['run_number']}"
+348             result["workflow"] = "beta"
+349         else:
+350             result["workflow"] = "tags"
+351     return result, gdata
+352
+353
+354 def update_version(
+355     version_file: str | Path, github_dump: str | None = None, abort: bool =
+356 True
+357 ) -> str | None:
+358     """extracts version information from github_dump and updates
+359 version_file in-place
 360
 361     Args:
-362         paths (str, Path): path(s) to files jinja2 processeable
-363         version_file (str, Path): path to a file with __version__ variable
+362         version_file (str, Path): path to a file with a __version__
+363 variable
 364         github_dump (str): the os.getenv("GITHUB_DUMP") value
 365
 366     Returns:
 367         str: the new version for the package
-368
-369     Example:
-370         {'branch': 'beta/0.3.1',
-371          'build': 0,
-372          'current': '0.3.1',
-373          'hash': 'c9e484a*',
-374          'version': '0.3.1b0',
-375          'runid': 0
-376         }
-377     """
-378     from argparse import Namespace
-379     from functools import partial
-380     from urllib.parse import quote
-381
-382     from jinja2 import Environment
-383
-384     class Context(Namespace):
-385         def items(self):
-386             for name, value in self.__dict__.items():
-387                 if name.startswith("_"):
-388                     continue
-389                 yield (name, value)
-390
-391     data = get_data(version_file, github_dump, abort)
-        set_module_var(version_file, "__version__", data["version"])
-        set_module_var(version_file, "__hash__", data["hash"])
-
-        env = Environment(autoescape=True)
-        env.filters["urlquote"] = partial(quote, safe="")
-        for path in list_of_paths(paths):
-            txt = apply_fixers(path.read_text(), fixers)
-            tmpl = env.from_string(txt)
+368     """
+369
+370     data = get_data(version_file, github_dump, abort=abort)[0]
+371     set_module_var(version_file, "__version__", data["version"])
+372     set_module_var(version_file, "__hash__", data["hash"])
+373     return data["version"]
+374
+375
+376 def process(
+377     version_file: str | Path,
+378     github_dump: str | None = None,
+379     paths: str | Path | list[str | Path] | None = None,
+380     fixers: dict[str, str] | None = None,
+381     record: str | Path = "_build.py",
+382     abort: bool = True,
+383 ) -> dict[str, str | None]:
+384     """get version from github_dump and updates version_file/paths
+385
+386     Args:
+387         version_file (str, Path): path to a file with __version__ variable
+388         github_dump (str): the os.getenv("GITHUB_DUMP") value
+389         paths (str, Path): path(s) to files jinja2 processeable
+390         fixers (dict[str,str]): fixer dictionary
+391         record: set to True will generate a _build.py sibling of
+392 version_file
+393
+394     Returns:
+395         str: the new version for the package
+396
+397     Example:
+398         {'branch': 'beta/0.3.1',
+399          'build': 0,
+400          'current': '0.3.1',
+401          'hash': 'c9e484a*',
+402          'version': '0.3.1b0',
+403          'runid': 0
+404         }
+405     """
+406     from argparse import Namespace
+407     from functools import partial
+408     from urllib.parse import quote
+409
+410     from jinja2 import Environment
+411
+412     class Context(Namespace):
+413         def items(self):
+414             for name, value in self.__dict__.items():
+415                 if name.startswith("_"):
+416                     continue
+417                 yield (name, value)
+418
+419     record_path = (Path(version_file).parent / record).absolute() if record
+420 else None
+421     data, gdata = get_data(version_file, github_dump, record_path, abort)
+422     set_module_var(version_file, "__version__", data["version"])
+423     set_module_var(version_file, "__hash__", data["hash"])
+424
+425     env = Environment(autoescape=True)
+426     env.filters["urlquote"] = partial(quote, safe="")
+427     for path in list_of_paths(paths):
+428         txt = apply_fixers(path.read_text(), fixers)
+429         tmpl = env.from_string(txt)
             path.write_text(tmpl.render(ctx=Context(**data)))
+
+        if record_path:
+            record_path.parent.mkdir(parents=True, exist_ok=True)
+            with record_path.open("w") as fp:
+                print("# autogenerate build file", file=fp)
+                for key, value in sorted((gdata or {}).items()):
+                    value = f"'{value}'" if isinstance(value, str) else value
+                    print(f"{key} = {value}", file=fp)
+
         return data
```

### Comparing `hatch_ci-0.0.8b31/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html` & `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html`

 * *Files 1% similar despite different names*

```diff
@@ -144,19 +144,19 @@
 Unannotated (x3)">        if not version_file.exists():</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x1)">            raise ValidationError(</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x5)">                f"no 'version-file' key for plugin {self.PLUGIN_NAME}"</span>
 <span class="line-empty" title="No Anys on this line!">            )</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x2)">        gdata = tools.process(</span>
+Unannotated (x3)">        gdata = tools.process(</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x4)
 Omitted Generics (x2)">            version_file, getenv("GITHUB_DUMP"), paths=paths, fixers=fixers</span>
-<span class="line-empty" title="No Anys on this line!">        )</span>
+<span class="line-any" title="No Anys on this line!">        )[0]</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">        return {"version": gdata["version"]}</span>
 </pre></td>
 </tr></tbody>
 </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -63,9 +63,9 @@
 58
 59         if not version_file.exists():
 60             raise ValidationError(
 61                 f"no 'version-file' key for plugin {self.PLUGIN_NAME}"
 62             )
 63         gdata = tools.process(
                version_file, getenv("GITHUB_DUMP"), paths=paths, fixers=fixers
-           )
+           )[0]
            return {"version": gdata["version"]}
```

### Comparing `hatch_ci-0.0.8b31/src/hatch_ci/cli.py` & `hatch_ci-0.0.8b32/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/src/hatch_ci/scm.py` & `hatch_ci-0.0.8b32/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/src/hatch_ci/script.py` & `hatch_ci-0.0.8b32/src/hatch_ci/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
         for branch in [*options.repo.branches.local, *options.repo.branches.remote]:
             if not branch.endswith(f"beta/{version}"):
                 continue
             options.error(f"branch '{branch}' already present")
         log.info("creating branch '%s'", f"/beta/{version}")
         options.repo.branch(f"beta/{version}", master)
-        options.repo(["checkout", master])
         print(  # noqa: T201
             tools.indent(
                 f"""
         The release branch beta/{version} has been created.
 
         To complete the release:
             git push origin beta/{version}
```

### Comparing `hatch_ci-0.0.8b31/src/hatch_ci/tools.py` & `hatch_ci-0.0.8b32/src/hatch_ci/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,14 +95,26 @@
     return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
 
 def lstrip(txt: str, left: str) -> str:
     return txt[len(left) :] if txt.startswith(left) else txt
 
 
+def loadmod(path: Path) -> Any:
+    from importlib.util import module_from_spec, spec_from_file_location
+
+    module = None
+    spec = spec_from_file_location(Path(path).name, Path(path))
+    if spec:
+        module = module_from_spec(spec)
+    if module and spec and spec.loader:
+        spec.loader.exec_module(module)
+    return module
+
+
 def apply_fixers(txt: str, fixers: dict[str, str] | None = None) -> str:
     result = txt
     for src, dst in (fixers or {}).items():
         if src.startswith("re:"):
             result = re.sub(src[3:], dst, result)
         else:
             result = result.replace(src, dst)
@@ -246,21 +258,25 @@
         newver[-1] = 0
     elif mode == "micro":
         newver[-1] += 1
     return ".".join(str(v) for v in newver)
 
 
 def get_data(
-    version_file: str | Path, github_dump: str | None = None, abort: bool = True
-) -> dict[str, str | None]:
+    version_file: str | Path,
+    github_dump: str | None = None,
+    record_path: Path | None = None,
+    abort: bool = True,
+) -> tuple[dict[str, str | None], dict[str, Any]]:
     """extracts version information from github_dump and updates version_file in-place
 
     Args:
         version_file (str, Path): path to a file  with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
+        record: pull data from a _build.py file
 
     Returns:
         dict[str,str|None]: a dict with the current config
     """
     result = {
         "version": get_module_var(version_file, "__version__"),
         "current": get_module_var(version_file, "__version__"),
@@ -269,31 +285,40 @@
         "build": None,
         "runid": None,
         "workflow": None,
     }
 
     path = Path(version_file)
     repo = scm.lookup(path)
+    record = record_path.exists() if record_path else None
 
-    if not (repo or github_dump):
+    if not (repo or github_dump or record):
         if abort:
-            raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}")
-        return result
+            raise scm.InvalidGitRepoError(
+                f"cannot figure out settings (no repo in {path}, "
+                f"a GITHUB_DUMP or a _build.py file)"
+            )
+        return result, {}
 
-    if not github_dump and repo:
+    dirty = False
+    if github_dump:
+        gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump
+    elif record_path and record_path.exists():
+        mod = loadmod(record_path)
+        gdata = {k: getattr(mod, k) for k in dir(mod) if not k.startswith("_")}
+    elif repo:
         gdata = {
             "ref": repo.head.name,
             "sha": repo.head.target.hex[:7],
             "run_number": 0,
             "run_id": 0,
         }
         dirty = repo.dirty()
     else:
-        gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump
-        dirty = False
+        raise RuntimeError("un-reacheable code")
 
     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$")
     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
 
     result["branch"] = lstrip(gdata["ref"], "refs/heads/")
     result["hash"] = gdata["sha"] + ("*" if dirty else "")
     result["build"] = gdata["run_number"]
@@ -313,15 +338,15 @@
                 f"branch ({match.groupdict()} mismatch {match1.groupdict()})"
             )
         if match.group("what") == "beta":
             result["version"] = f"{match1.group('version')}b{gdata['run_number']}"
             result["workflow"] = "beta"
         else:
             result["workflow"] = "tags"
-    return result
+    return result, gdata
 
 
 def update_version(
     version_file: str | Path, github_dump: str | None = None, abort: bool = True
 ) -> str | None:
     """extracts version information from github_dump and updates version_file in-place
 
@@ -329,33 +354,36 @@
         version_file (str, Path): path to a file with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
         str: the new version for the package
     """
 
-    data = get_data(version_file, github_dump, abort)
+    data = get_data(version_file, github_dump, abort=abort)[0]
     set_module_var(version_file, "__version__", data["version"])
     set_module_var(version_file, "__hash__", data["hash"])
     return data["version"]
 
 
 def process(
     version_file: str | Path,
     github_dump: str | None = None,
     paths: str | Path | list[str | Path] | None = None,
     fixers: dict[str, str] | None = None,
+    record: str | Path = "_build.py",
     abort: bool = True,
 ) -> dict[str, str | None]:
     """get version from github_dump and updates version_file/paths
 
     Args:
-        paths (str, Path): path(s) to files jinja2 processeable
         version_file (str, Path): path to a file with __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
+        paths (str, Path): path(s) to files jinja2 processeable
+        fixers (dict[str,str]): fixer dictionary
+        record: set to True will generate a _build.py sibling of version_file
 
     Returns:
         str: the new version for the package
 
     Example:
         {'branch': 'beta/0.3.1',
          'build': 0,
@@ -374,18 +402,28 @@
     class Context(Namespace):
         def items(self):
             for name, value in self.__dict__.items():
                 if name.startswith("_"):
                     continue
                 yield (name, value)
 
-    data = get_data(version_file, github_dump, abort)
+    record_path = (Path(version_file).parent / record).absolute() if record else None
+    data, gdata = get_data(version_file, github_dump, record_path, abort)
     set_module_var(version_file, "__version__", data["version"])
     set_module_var(version_file, "__hash__", data["hash"])
 
     env = Environment(autoescape=True)
     env.filters["urlquote"] = partial(quote, safe="")
     for path in list_of_paths(paths):
         txt = apply_fixers(path.read_text(), fixers)
         tmpl = env.from_string(txt)
         path.write_text(tmpl.render(ctx=Context(**data)))
+
+    if record_path:
+        record_path.parent.mkdir(parents=True, exist_ok=True)
+        with record_path.open("w") as fp:
+            print("# autogenerate build file", file=fp)
+            for key, value in sorted((gdata or {}).items()):
+                value = f"'{value}'" if isinstance(value, str) else value
+                print(f"{key} = {value}", file=fp)
+
     return data
```

### Comparing `hatch_ci-0.0.8b31/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.8b32/src/hatch_ci/version_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,9 +55,9 @@
 
         if not version_file.exists():
             raise ValidationError(
                 f"no 'version-file' key for plugin {self.PLUGIN_NAME}"
             )
         gdata = tools.process(
             version_file, getenv("GITHUB_DUMP"), paths=paths, fixers=fixers
-        )
+        )[0]
         return {"version": gdata["version"]}
```

### Comparing `hatch_ci-0.0.8b31/tests/conftest.py` & `hatch_ci-0.0.8b32/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/tests/test_scm.py` & `hatch_ci-0.0.8b32/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/tests/test_tools.py` & `hatch_ci-0.0.8b32/tests/test_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,16 @@
 Key[version] = 1.2.3
 Key[workflow] = master
 """
     )
 
     # clean and switch to new branch
     repo.revert(repo.initfile)
+    (repo.initfile.parent / "_build.py").unlink()
+
     write_tfile(tfile)
     repo.branch("beta/1.2.3", "master")
 
     data = tools.process(repo.initfile, None, tfile)
     assert data["hash"][-1] != "*"
 
     assert (
```

### Comparing `hatch_ci-0.0.8b31/LICENSE.txt` & `hatch_ci-0.0.8b32/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/README.md` & `hatch_ci-0.0.8b32/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5783487331)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5789474090)
 [![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `hatch_ci-0.0.8b31/pyproject.toml` & `hatch_ci-0.0.8b32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b31/PKG-INFO` & `hatch_ci-0.0.8b32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.8b31
+Version: 0.0.8b32
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,plugin,scm,version
@@ -24,15 +24,15 @@
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5783487331)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5789474090)
 [![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

