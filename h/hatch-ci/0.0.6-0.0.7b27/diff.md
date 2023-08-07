# Comparing `tmp/hatch_ci-0.0.6.tar.gz` & `tmp/hatch_ci-0.0.7b27.tar.gz`

## Comparing `hatch_ci-0.0.6.tar` & `hatch_ci-0.0.7b27.tar`

### file list

```diff
@@ -1,31 +1,52 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.gitattributes
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/Makefile
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.github/workflows/beta.yml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.github/workflows/master.yml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.github/workflows/tags.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/hatch-github.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/cli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/script.py
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/tests/test_scm.py
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/README.md
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 hatch_ci-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/.gitattributes
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/Makefile
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/.github/workflows/master.yml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    49436 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
+-rw-r--r--   0        0        0   115699 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    22969 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    30321 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
+-rw-r--r--   0        0        0    68068 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/script.py
+-rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/tests/test_scm.py
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/LICENSE.txt
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/README.md
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/pyproject.toml
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 hatch_ci-0.0.7b27/PKG-INFO
```

### Comparing `hatch_ci-0.0.6/.github/workflows/beta.yml` & `hatch_ci-0.0.7b27/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/.github/workflows/master.yml` & `hatch_ci-0.0.7b27/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/.github/workflows/tags.yml` & `hatch_ci-0.0.7b27/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/src/hatch_ci/cli.py` & `hatch_ci-0.0.7b27/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/src/hatch_ci/scm.py` & `hatch_ci-0.0.7b27/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/src/hatch_ci/script.py` & `hatch_ci-0.0.7b27/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/src/hatch_ci/tools.py` & `hatch_ci-0.0.7b27/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.7b27/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/tests/conftest.py` & `hatch_ci-0.0.7b27/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/tests/test_scm.py` & `hatch_ci-0.0.7b27/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/tests/test_tools.py` & `hatch_ci-0.0.7b27/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/LICENSE.txt` & `hatch_ci-0.0.7b27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/README.md` & `hatch_ci-0.0.7b27/README.md`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/pyproject.toml` & `hatch_ci-0.0.7b27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.6/PKG-INFO` & `hatch_ci-0.0.7b27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.6
+Version: 0.0.7b27
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,plugin,scm,version
```

