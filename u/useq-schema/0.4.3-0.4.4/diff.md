# Comparing `tmp/useq_schema-0.4.3.tar.gz` & `tmp/useq_schema-0.4.4.tar.gz`

## Comparing `useq_schema-0.4.3.tar` & `useq_schema-0.4.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 useq_schema-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 useq_schema-0.4.3/mkdocs.yml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.4.3/.github/dependabot.yml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 useq_schema-0.4.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 useq_schema-0.4.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/images/favicon.ico
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/schema/axes.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/schema/event.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/schema/hardware_autofocus.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.4.3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_actions.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_base_model.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_channel.py
--rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_grid.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_hardware_autofocus.py
--rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_iter_sequence.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_mda_event.py
--rw-r--r--   0        0        0    15837 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_position.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_time.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_utils.py
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/py.typed
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 useq_schema-0.4.3/src/useq/pycromanager.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/test_autofocus.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/test_grid.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/test_misc.py
--rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/test_position_sequence.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/test_pycromanager.py
--rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/test_sequence.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/test_serialization.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/fixtures/mda.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.4.3/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.4.3/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.4.3/LICENSE
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 useq_schema-0.4.3/README.md
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 useq_schema-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 useq_schema-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 useq_schema-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 useq_schema-0.4.4/mkdocs.yml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.4.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 useq_schema-0.4.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 useq_schema-0.4.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/schema/axes.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/schema/event.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/schema/hardware_autofocus.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.4.4/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_actions.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_base_model.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_channel.py
+-rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_grid.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_hardware_autofocus.py
+-rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_iter_sequence.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    15837 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_position.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_time.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_utils.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/py.typed
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 useq_schema-0.4.4/src/useq/pycromanager.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/test_autofocus.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/test_grid.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/test_misc.py
+-rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/test_position_sequence.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/test_pycromanager.py
+-rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/test_sequence.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/test_serialization.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.4.4/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.4.4/LICENSE
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 useq_schema-0.4.4/README.md
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 useq_schema-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 useq_schema-0.4.4/PKG-INFO
```

### Comparing `useq_schema-0.4.3/.pre-commit-config.yaml` & `useq_schema-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/mkdocs.yml` & `useq_schema-0.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/.github/workflows/docs.yml` & `useq_schema-0.4.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/.github/workflows/test_and_deploy.yml` & `useq_schema-0.4.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/docs/index.md` & `useq_schema-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/docs/images/favicon.ico` & `useq_schema-0.4.4/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/docs/schema/axes.md` & `useq_schema-0.4.4/docs/schema/axes.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/docs/stylesheets/extra.css` & `useq_schema-0.4.4/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/__init__.py` & `useq_schema-0.4.4/src/useq/__init__.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_actions.py` & `useq_schema-0.4.4/src/useq/_actions.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_base_model.py` & `useq_schema-0.4.4/src/useq/_base_model.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_channel.py` & `useq_schema-0.4.4/src/useq/_channel.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_grid.py` & `useq_schema-0.4.4/src/useq/_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_hardware_autofocus.py` & `useq_schema-0.4.4/src/useq/_hardware_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_iter_sequence.py` & `useq_schema-0.4.4/src/useq/_iter_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_mda_event.py` & `useq_schema-0.4.4/src/useq/_mda_event.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_mda_sequence.py` & `useq_schema-0.4.4/src/useq/_mda_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_position.py` & `useq_schema-0.4.4/src/useq/_position.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_time.py` & `useq_schema-0.4.4/src/useq/_time.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_utils.py` & `useq_schema-0.4.4/src/useq/_utils.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/src/useq/_z.py` & `useq_schema-0.4.4/src/useq/_z.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,23 @@
         yield from positions
 
     def _start_stop_step(self) -> tuple[float, float, float]:
         raise NotImplementedError
 
     def positions(self) -> Sequence[float]:
         start, stop, step = self._start_stop_step()
+        if step == 0:
+            return [start]
         stop += step / 2  # make sure we include the last point
         return list(np.arange(start, stop, step))
 
     def num_positions(self) -> int:
         start, stop, step = self._start_stop_step()
+        if step == 0:
+            return 1
         nsteps = (stop + step - start) / step
         return math.ceil(round(nsteps, 6))
 
     @property
     def is_relative(self) -> bool:
         return True
```

### Comparing `useq_schema-0.4.3/src/useq/pycromanager.py` & `useq_schema-0.4.4/src/useq/pycromanager.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/conftest.py` & `useq_schema-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/test_autofocus.py` & `useq_schema-0.4.4/tests/test_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/test_grid.py` & `useq_schema-0.4.4/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/test_misc.py` & `useq_schema-0.4.4/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/test_position_sequence.py` & `useq_schema-0.4.4/tests/test_position_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/test_sequence.py` & `useq_schema-0.4.4/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/test_serialization.py` & `useq_schema-0.4.4/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/fixtures/mda.json` & `useq_schema-0.4.4/tests/fixtures/mda.json`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/tests/fixtures/mda.yaml` & `useq_schema-0.4.4/tests/fixtures/mda.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/.gitignore` & `useq_schema-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/LICENSE` & `useq_schema-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/README.md` & `useq_schema-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/pyproject.toml` & `useq_schema-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.3/PKG-INFO` & `useq_schema-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.4.3
+Version: 0.4.4
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
```

