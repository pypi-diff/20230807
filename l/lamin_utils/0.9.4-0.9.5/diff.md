# Comparing `tmp/lamin_utils-0.9.4.tar.gz` & `tmp/lamin_utils-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_utils-0.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_utils-0.9.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_utils-0.9.4.tar` & `lamin_utils-0.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.4/.gitignore
--rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.4/LICENSE
--rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.4/README.md
--rw-r--r--   0        0        0     7124 2023-08-06 15:33:52.714340 lamin_utils-0.9.4/docs/changelog.md
--rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.4/docs/quickstart.ipynb
--rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.4/lamin-project.yaml
--rw-r--r--   0        0        0      161 2023-08-06 15:33:43.830821 lamin_utils-0.9.4/lamin_utils/__init__.py
--rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.4/lamin_utils/_core.py
--rw-r--r--   0        0        0     4971 2023-08-06 15:33:10.092855 lamin_utils-0.9.4/lamin_utils/_inspect.py
--rw-r--r--   0        0        0     7411 2023-08-06 15:33:10.093172 lamin_utils-0.9.4/lamin_utils/_logger.py
--rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.4/lamin_utils/_lookup.py
--rw-r--r--   0        0        0     6843 2023-08-06 15:33:10.093571 lamin_utils-0.9.4/lamin_utils/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.4/lamin_utils/_python_version.py
--rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.4/lamin_utils/_search.py
--rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.4/noxfile.py
--rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.4/tests/test_base.py
--rw-r--r--   0        0        0     4574 2023-08-06 15:33:10.093958 lamin_utils-0.9.4/tests/test_inspect.py
--rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.4/tests/test_lookup.py
--rw-r--r--   0        0        0     5560 2023-08-06 15:33:10.094251 lamin_utils-0.9.4/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.4/tests/test_notebooks.py
--rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.4/tests/test_search.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.5/LICENSE
+-rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.5/README.md
+-rw-r--r--   0        0        0     7289 2023-08-07 19:42:42.226217 lamin_utils-0.9.5/docs/changelog.md
+-rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.5/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.5/lamin-project.yaml
+-rw-r--r--   0        0        0      161 2023-08-07 19:42:33.366232 lamin_utils-0.9.5/lamin_utils/__init__.py
+-rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.5/lamin_utils/_core.py
+-rw-r--r--   0        0        0     4971 2023-08-07 09:30:30.829953 lamin_utils-0.9.5/lamin_utils/_inspect.py
+-rw-r--r--   0        0        0     7658 2023-08-07 19:41:59.385758 lamin_utils-0.9.5/lamin_utils/_logger.py
+-rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.5/lamin_utils/_lookup.py
+-rw-r--r--   0        0        0     6843 2023-08-06 16:55:32.281387 lamin_utils-0.9.5/lamin_utils/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.5/lamin_utils/_python_version.py
+-rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.5/lamin_utils/_search.py
+-rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.5/noxfile.py
+-rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.5/tests/test_base.py
+-rw-r--r--   0        0        0     4574 2023-08-06 15:33:10.093958 lamin_utils-0.9.5/tests/test_inspect.py
+-rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.5/tests/test_lookup.py
+-rw-r--r--   0        0        0     5560 2023-08-06 15:33:10.094251 lamin_utils-0.9.5/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.5/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.5/tests/test_search.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.5/PKG-INFO
```

### Comparing `lamin_utils-0.9.4/.github/workflows/build.yml` & `lamin_utils-0.9.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/.github/workflows/latest-changes.yml` & `lamin_utils-0.9.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/.gitignore` & `lamin_utils-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/.pre-commit-config.yaml` & `lamin_utils-0.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/LICENSE` & `lamin_utils-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/docs/changelog.md` & `lamin_utils-0.9.5/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🎨 Rename download to save logging level | [50](https://github.com/laminlabs/lamin-utils/pull/50) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-07 | 0.9.5
 🎨 Simplified params in inspect | [48](https://github.com/laminlabs/lamin-utils/pull/48) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-06 | 0.9.4
 🚸 Introduce success-level verbosity | [49](https://github.com/laminlabs/lamin-utils/pull/49) | [falexwolf](https://github.com/falexwolf) | 2023-08-06 |
 Round percentages for mapping | [47](https://github.com/laminlabs/lamin-utils/pull/47) | [Zethson](https://github.com/Zethson) | 2023-07-31 |
 🐛 Fix for categorical index | [45](https://github.com/laminlabs/lamin-utils/pull/45) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.3
 ✨ Added italic and underline | [44](https://github.com/laminlabs/lamin-utils/pull/44) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.2
 🐛 Fix _append_records_to_list in lookup | [43](https://github.com/laminlabs/lamin-utils/pull/43) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-23 |
 ✨ Allow indenting logging messages | [42](https://github.com/laminlabs/lamin-utils/pull/42) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 | 0.9.0
```

### Comparing `lamin_utils-0.9.4/docs/quickstart.ipynb` & `lamin_utils-0.9.5/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/lamin_utils/_core.py` & `lamin_utils-0.9.5/lamin_utils/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/lamin_utils/_inspect.py` & `lamin_utils-0.9.5/lamin_utils/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/lamin_utils/_logger.py` & `lamin_utils-0.9.5/lamin_utils/_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,36 +34,36 @@
 import platform
 import sys
 from datetime import datetime, timedelta, timezone
 from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING, getLevelName
 from typing import Optional
 
 HINT = 15
-DOWNLOAD = 21
+SAVE = 21
 SUCCESS = 25
 logging.addLevelName(HINT, "HINT")
-logging.addLevelName(DOWNLOAD, "DOWNLOAD")
+logging.addLevelName(SAVE, "SAVE")
 logging.addLevelName(SUCCESS, "SUCCESS")
 
 VERBOSITY_TO_LOGLEVEL = {
-    0: "ERROR",
-    1: "WARNING",
-    2: "SUCCESS",
-    3: "INFO",
-    4: "HINT",
-    5: "DEBUG",
+    0: "ERROR",  # 40
+    1: "WARNING",  # 30
+    2: "SUCCESS",  # 25
+    3: "INFO",  # 20
+    4: "HINT",  # 15
+    5: "DEBUG",  # 10
 }
 
 
 LEVEL_TO_ICONS = {
     40: "❌",  # error
     30: "🔶",  # warning
     25: "✅",  # success
-    21: "💾",  # download
-    20: "💬",  # info
+    21: "🌱",  # save
+    20: "💡",  # info
     15: "💡",  # hint
     10: "🐛",  # debug
 }
 
 
 class RootLogger(logging.RootLogger):
     def __init__(self, level="INFO"):
@@ -95,17 +95,19 @@
                 this gets displayed as well
             extra: Additional values you can specify in `msg` like `{time_passed}`.
         """
         now = datetime.now(timezone.utc)
         time_passed: timedelta = None if time is None else now - time  # type: ignore
         extra = {
             **(extra or {}),
-            "deep": deep
-            if getLevelName(VERBOSITY_TO_LOGLEVEL[self._verbosity]) < level
-            else None,
+            "deep": (
+                deep
+                if getLevelName(VERBOSITY_TO_LOGLEVEL[self._verbosity]) < level
+                else None
+            ),
             "time_passed": time_passed,
         }
         msg = f"{self.indent}{msg}"
         super().log(level, msg, extra=extra)
         return now
 
     def critical(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
@@ -119,23 +121,27 @@
 
     def success(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
         return self.log(SUCCESS, msg, time=time, deep=deep, extra=extra)
 
     def info(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
         return self.log(INFO, msg, time=time, deep=deep, extra=extra)
 
-    def download(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
-        return self.log(DOWNLOAD, msg, time=time, deep=deep, extra=extra)
+    def save(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
+        return self.log(SAVE, msg, time=time, deep=deep, extra=extra)
 
     def hint(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
         return self.log(HINT, msg, time=time, deep=deep, extra=extra)
 
     def debug(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
         return self.log(DEBUG, msg, time=time, deep=deep, extra=extra)
 
+    # backward compat
+    def download(self, msg, *, time=None, deep=None, extra=None) -> datetime:  # type: ignore  # noqa
+        return self.log(SAVE, msg, time=time, deep=deep, extra=extra)
+
 
 class _LogFormatter(logging.Formatter):
     def __init__(
         self, fmt="{levelname}: {message}", datefmt="%Y-%m-%d %H:%M", style="{"
     ):
         super().__init__(fmt, datefmt, style)
```

### Comparing `lamin_utils-0.9.4/lamin_utils/_lookup.py` & `lamin_utils-0.9.5/lamin_utils/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/lamin_utils/_map_synonyms.py` & `lamin_utils-0.9.5/lamin_utils/_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/lamin_utils/_python_version.py` & `lamin_utils-0.9.5/lamin_utils/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/lamin_utils/_search.py` & `lamin_utils-0.9.5/lamin_utils/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/pyproject.toml` & `lamin_utils-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/tests/test_inspect.py` & `lamin_utils-0.9.5/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/tests/test_lookup.py` & `lamin_utils-0.9.5/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/tests/test_map_synonyms.py` & `lamin_utils-0.9.5/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/tests/test_search.py` & `lamin_utils-0.9.5/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.4/PKG-INFO` & `lamin_utils-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_utils
-Version: 0.9.4
+Version: 0.9.5
 Summary: Lamin Utils.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

