# Comparing `tmp/odin-slides-0.2.tar.gz` & `tmp/odin-slides-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin-slides-0.2.tar", last modified: Sun Aug  6 12:58:47 2023, max compression
+gzip compressed data, was "odin-slides-0.3.tar", last modified: Mon Aug  7 13:25:20 2023, max compression
```

## Comparing `odin-slides-0.2.tar` & `odin-slides-0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 12:58:47.860051 odin-slides-0.2/
--rw-rw-rw-   0        0        0     1068 2023-08-05 15:27:48.000000 odin-slides-0.2/LICENSE
--rw-rw-rw-   0        0        0      472 2023-08-06 12:58:47.857838 odin-slides-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6247 2023-08-06 11:56:53.000000 odin-slides-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 12:58:47.784110 odin-slides-0.2/odin_slides/
--rw-rw-rw-   0        0        0       15 2023-08-05 15:27:48.000000 odin-slides-0.2/odin_slides/__init__.py
--rw-rw-rw-   0        0        0     8226 2023-08-05 15:27:48.000000 odin-slides-0.2/odin_slides/llm_ops.py
--rw-rw-rw-   0        0        0     4846 2023-08-05 15:27:48.000000 odin-slides-0.2/odin_slides/main.py
--rw-rw-rw-   0        0        0    12067 2023-08-05 15:27:48.000000 odin-slides-0.2/odin_slides/presentation.py
--rw-rw-rw-   0        0        0     6138 2023-08-05 15:27:48.000000 odin-slides-0.2/odin_slides/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-06 12:58:47.834378 odin-slides-0.2/odin_slides.egg-info/
--rw-rw-rw-   0        0        0      472 2023-08-06 12:58:44.000000 odin-slides-0.2/odin_slides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-08-06 12:58:46.000000 odin-slides-0.2/odin_slides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 12:58:44.000000 odin-slides-0.2/odin_slides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-08-06 12:58:44.000000 odin-slides-0.2/odin_slides.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-08-06 12:58:44.000000 odin-slides-0.2/odin_slides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-06 12:58:44.000000 odin-slides-0.2/odin_slides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 12:58:47.860587 odin-slides-0.2/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-08-06 12:57:20.000000 odin-slides-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 12:58:47.852688 odin-slides-0.2/tests/
--rw-rw-rw-   0        0        0       15 2023-08-05 15:27:48.000000 odin-slides-0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2805 2023-08-05 15:27:48.000000 odin-slides-0.2/tests/test_presentation.py
--rw-rw-rw-   0        0        0     1537 2023-08-05 15:27:48.000000 odin-slides-0.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:25:20.667334 odin-slides-0.3/
+-rw-rw-rw-   0        0        0     1068 2023-08-05 15:27:48.000000 odin-slides-0.3/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-08-07 13:25:20.663337 odin-slides-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6247 2023-08-06 11:56:53.000000 odin-slides-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 13:25:20.590622 odin-slides-0.3/odin_slides/
+-rw-rw-rw-   0        0        0       15 2023-08-05 15:27:48.000000 odin-slides-0.3/odin_slides/__init__.py
+-rw-rw-rw-   0        0        0     8226 2023-08-05 15:27:48.000000 odin-slides-0.3/odin_slides/llm_ops.py
+-rw-rw-rw-   0        0        0     4846 2023-08-05 15:27:48.000000 odin-slides-0.3/odin_slides/main.py
+-rw-rw-rw-   0        0        0    12285 2023-08-07 12:24:22.000000 odin-slides-0.3/odin_slides/presentation.py
+-rw-rw-rw-   0        0        0     6138 2023-08-05 15:27:48.000000 odin-slides-0.3/odin_slides/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:25:20.637467 odin-slides-0.3/odin_slides.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-08-07 13:25:17.000000 odin-slides-0.3/odin_slides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-08-07 13:25:19.000000 odin-slides-0.3/odin_slides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 13:25:17.000000 odin-slides-0.3/odin_slides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-08-07 13:25:17.000000 odin-slides-0.3/odin_slides.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-08-07 13:25:17.000000 odin-slides-0.3/odin_slides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-07 13:25:17.000000 odin-slides-0.3/odin_slides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 13:25:20.668042 odin-slides-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-08-07 13:23:34.000000 odin-slides-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:25:20.659747 odin-slides-0.3/tests/
+-rw-rw-rw-   0        0        0       15 2023-08-05 15:27:48.000000 odin-slides-0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2805 2023-08-05 15:27:48.000000 odin-slides-0.3/tests/test_presentation.py
+-rw-rw-rw-   0        0        0     1537 2023-08-05 15:27:48.000000 odin-slides-0.3/tests/test_utils.py
```

### Comparing `odin-slides-0.2/LICENSE` & `odin-slides-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odin-slides-0.2/README.md` & `odin-slides-0.3/README.md`

 * *Files identical despite different names*

### Comparing `odin-slides-0.2/odin_slides/llm_ops.py` & `odin-slides-0.3/odin_slides/llm_ops.py`

 * *Files identical despite different names*

### Comparing `odin-slides-0.2/odin_slides/main.py` & `odin-slides-0.3/odin_slides/main.py`

 * *Files identical despite different names*

### Comparing `odin-slides-0.2/odin_slides/presentation.py` & `odin-slides-0.3/odin_slides/presentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,19 @@
             input()  # Wait for the user to close the file
         except Exception as e:
             print(format_error("An unexpected error occurred while saving the presentation: ")+f"{e}")
             logger.error(f"An unexpected error occurred while saving the presentation: {e}")
             break
     print(format_info("Presentation created successfully and saved as: ")+ f"{output_file}")
     # Open the saved presentation file
-    os.startfile(output_file)
+    try:
+        os.startfile(output_file)
+    except Exception as e:
+            print(format_info("Open the saved file manually to see the changes."))
+            logger.debug(f"Can not preview the presentation using os default viewer: {e}")
 
 
 def build_slides_with_llm(template_file,word_content, output_file, session_file, logger):
     """Build slides using a language model (LLM) based on user input.
 
     Args:
         template_file (str): The path to the template PowerPoint file.
```

### Comparing `odin-slides-0.2/odin_slides/utils.py` & `odin-slides-0.3/odin_slides/utils.py`

 * *Files identical despite different names*

### Comparing `odin-slides-0.2/setup.py` & `odin-slides-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odin-slides",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     install_requires=[
         'python-pptx',
         'python-docx',
         'requests',
         'colorama',
         'tqdm'
```

### Comparing `odin-slides-0.2/tests/test_presentation.py` & `odin-slides-0.3/tests/test_presentation.py`

 * *Files identical despite different names*

### Comparing `odin-slides-0.2/tests/test_utils.py` & `odin-slides-0.3/tests/test_utils.py`

 * *Files identical despite different names*

