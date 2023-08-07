# Comparing `tmp/plutoplots-0.3.4.tar.gz` & `tmp/plutoplots-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutoplots-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "plutoplots-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `plutoplots-0.3.4.tar` & `plutoplots-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.4/.gitignore
--rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.4/LICENSE
--rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.4/README.md
--rw-r--r--   0        0        0       43 2023-08-07 15:50:38.499075 plutoplots-0.3.4/plutoplots/__init__.py
--rw-r--r--   0        0        0     3928 2023-08-07 15:08:49.990949 plutoplots-0.3.4/plutoplots/plot.py
--rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.5/LICENSE
+-rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.5/README.md
+-rw-r--r--   0        0        0       43 2023-08-07 16:34:36.272548 plutoplots-0.3.5/plutoplots/__init__.py
+-rw-r--r--   0        0        0     3930 2023-08-07 16:34:36.270689 plutoplots-0.3.5/plutoplots/plot.py
+-rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.5/PKG-INFO
```

### Comparing `plutoplots-0.3.4/LICENSE` & `plutoplots-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.4/README.md` & `plutoplots-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.4/plutoplots/plot.py` & `plutoplots-0.3.5/plutoplots/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ plotting Module """
 
 import seaborn as sns
 import matplotlib.pyplot as plt
 import statsmodels.api as sm
 
+
 class Plot:
 
     def __init__(self):
         self.axes = None
 
     def shape(self, dim=(10, 5)):
         plt.figure(figsize=dim)
@@ -122,8 +123,8 @@
         return self
 
 
 class QQplot(Plot):
 
     def create(self, col, ax=None):
         self.axes = sm.qqplot(col, line='s', ax=ax)
-        return self
+        return self
```

### Comparing `plutoplots-0.3.4/PKG-INFO` & `plutoplots-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutoplots
-Version: 0.3.4
+Version: 0.3.5
 Summary: visualization 
 Author-email: Oluwole Ilesanmi <oluwoleilesanmi@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/oluwoleilesanmi/pluto
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plutoplots Version: 0.3.4 Summary: visualization
+Metadata-Version: 2.1 Name: plutoplots Version: 0.3.5 Summary: visualization
 Author-email: Oluwole Ilesanmi
 gmail.com> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: MIT License Project-URL: Home, https://github.com/oluwoleilesanmi/
 pluto
                               ****** Pluto ******
         Visualization library built on top of Seaborn and Matplotlib.
                                Easier plotting
```

