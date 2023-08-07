# Comparing `tmp/mkdocs_inline_svg_plugin-0.1.0.tar.gz` & `tmp/mkdocs_inline_svg_plugin-0.1.1.tar.gz`

## Comparing `mkdocs_inline_svg_plugin-0.1.0.tar` & `mkdocs_inline_svg_plugin-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,14 @@
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/content/a12a4823b09e1561
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/content/a87d460d54ac84ef
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/content/bb8ed6bcc92e2ccc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/content/e1fa5aea1112ee82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/content/ecd561685b32291e
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.ruff_cache/content/fbea8bb477e1cd11
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/docs/index.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/docs/css/extra.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/src/inline_svg/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/src/inline_svg/config.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/src/inline_svg/plugin.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/src/inline_svg/util.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/README.md
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/docs/index.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/docs/css/extra.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/src/inline_svg/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/src/inline_svg/config.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/src/inline_svg/plugin.py
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/src/inline_svg/util.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.1/PKG-INFO
```

### Comparing `mkdocs_inline_svg_plugin-0.1.0/mkdocs.yml` & `mkdocs_inline_svg_plugin-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/docs/index.md` & `mkdocs_inline_svg_plugin-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/docs/css/extra.css` & `mkdocs_inline_svg_plugin-0.1.1/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/src/inline_svg/plugin.py` & `mkdocs_inline_svg_plugin-0.1.1/src/inline_svg/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/src/inline_svg/util.py` & `mkdocs_inline_svg_plugin-0.1.1/src/inline_svg/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/.gitignore` & `mkdocs_inline_svg_plugin-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/LICENSE.txt` & `mkdocs_inline_svg_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/README.md` & `mkdocs_inline_svg_plugin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.0/pyproject.toml` & `mkdocs_inline_svg_plugin-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-	"mkdocs == 1.4.2",
-	"requests == 2.28.2",
-	"beautifulsoup4 == 4.12.0",
+	"mkdocs <= 1.4.2",
+	"requests <= 2.31.0",
+	"beautifulsoup4 <= 4.12.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/oniboni/mkdocs-inline-svg-plugin#readme"
 Issues = "https://github.com/oniboni/mkdocs-inline-svg-plugin/issues"
 Source = "https://github.com/oniboni/mkdocs-inline-svg-plugin"
```

### Comparing `mkdocs_inline_svg_plugin-0.1.0/PKG-INFO` & `mkdocs_inline_svg_plugin-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-inline-svg-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: MkDocs plugin for inlining svg-href img tags
 Project-URL: Documentation, https://github.com/oniboni/mkdocs-inline-svg-plugin#readme
 Project-URL: Issues, https://github.com/oniboni/mkdocs-inline-svg-plugin/issues
 Project-URL: Source, https://github.com/oniboni/mkdocs-inline-svg-plugin
 Author-email: Oni Boni <oniboni@mailbox.org>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
-Requires-Dist: beautifulsoup4==4.12.0
-Requires-Dist: mkdocs==1.4.2
-Requires-Dist: requests==2.28.2
+Requires-Dist: beautifulsoup4<=4.12.0
+Requires-Dist: mkdocs<=1.4.2
+Requires-Dist: requests<=2.31.0
 Description-Content-Type: text/markdown
 
 > **NOTE:** this project is still WIP!
 
 # mkdocs-inline-svg-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-inline-svg-plugin.svg)](https://pypi.org/project/mkdocs-inline-svg-plugin)
```

