# Comparing `tmp/mkdocs_pdf2image_plugin-0.1.0.tar.gz` & `tmp/mkdocs_pdf2image_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_pdf2image_plugin-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_pdf2image_plugin-0.1.1.tar", max compression
```

## Comparing `mkdocs_pdf2image_plugin-0.1.0.tar` & `mkdocs_pdf2image_plugin-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1948 2023-08-07 20:35:38.795534 mkdocs_pdf2image_plugin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 09:13:11.740585 mkdocs_pdf2image_plugin-0.1.0/mkdocs_pdf2image/__init__.py
--rw-r--r--   0        0        0     2593 2023-08-07 20:37:42.462838 mkdocs_pdf2image_plugin-0.1.0/mkdocs_pdf2image/plugin.py
--rw-r--r--   0        0        0     1070 2023-08-07 14:35:02.810273 mkdocs_pdf2image_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 mkdocs_pdf2image_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1964 2023-08-07 20:55:36.651917 mkdocs_pdf2image_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-07 20:55:36.651917 mkdocs_pdf2image_plugin-0.1.1/mkdocs_pdf2image/__init__.py
+-rw-r--r--   0        0        0     2593 2023-08-07 20:55:36.651917 mkdocs_pdf2image_plugin-0.1.1/mkdocs_pdf2image/plugin.py
+-rw-r--r--   0        0        0     1091 2023-08-07 20:55:36.651917 mkdocs_pdf2image_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 mkdocs_pdf2image_plugin-0.1.1/PKG-INFO
```

### Comparing `mkdocs_pdf2image_plugin-0.1.0/README.md` & `mkdocs_pdf2image_plugin-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # mkdocs-pdf2image-plugin
 
-This plugin generates an image from PDF files. It is particularly useful when you want
+This plugin generates images from the first page of PDF files. It is particularly useful when you want
 to include PDF presentations in your documentation.
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
```

### Comparing `mkdocs_pdf2image_plugin-0.1.0/mkdocs_pdf2image/plugin.py` & `mkdocs_pdf2image_plugin-0.1.1/mkdocs_pdf2image/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_pdf2image_plugin-0.1.0/pyproject.toml` & `mkdocs_pdf2image_plugin-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mkdocs-pdf2image-plugin"
-version = "0.1.0"
-description = "An MkDocs plugin to convert pdf to images'"
+version = "0.1.1"
+description = "An MkDocs plugin to convert the first page of a pdf to an image"
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-pdf2image-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "mkdocs_pdf2image" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
 classifiers = [
```

### Comparing `mkdocs_pdf2image_plugin-0.1.0/PKG-INFO` & `mkdocs_pdf2image_plugin-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mkdocs-pdf2image-plugin
-Version: 0.1.0
-Summary: An MkDocs plugin to convert pdf to images'
+Version: 0.1.1
+Summary: An MkDocs plugin to convert the first page of a pdf to an image
 Home-page: https://github.com/supcik/mkdocs-pdf2image-plugin
 License: Apache-2
 Keywords: mkdocs,python,markdown,wiki
 Author: Jacques Supcik
 Author-email: jacques.supcik@hefr.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Requires-Dist: mkdocs-material (>=9.1.15,<10.0.0) ; extra == "test"
 Requires-Dist: pdf2image (>=1.16.3,<2.0.0)
 Project-URL: Repository, https://github.com/supcik/mkdocs-pdf2image-plugin
 Description-Content-Type: text/markdown
 
 # mkdocs-pdf2image-plugin
 
-This plugin generates an image from PDF files. It is particularly useful when you want
+This plugin generates images from the first page of PDF files. It is particularly useful when you want
 to include PDF presentations in your documentation.
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
```

