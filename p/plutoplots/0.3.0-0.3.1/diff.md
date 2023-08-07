# Comparing `tmp/plutoplots-0.3.0.tar.gz` & `tmp/plutoplots-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutoplots-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "plutoplots-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `plutoplots-0.3.0.tar` & `plutoplots-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.0/.gitignore
--rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.0/LICENSE
--rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.0/README.md
--rw-r--r--   0        0        0       43 2023-08-03 06:33:04.240483 plutoplots-0.3.0/plutoplots/__init__.py
--rw-r--r--   0        0        0     3706 2023-08-03 06:33:04.237374 plutoplots-0.3.0/plutoplots/plot.py
--rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.1/LICENSE
+-rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.1/README.md
+-rw-r--r--   0        0        0       43 2023-08-07 11:28:58.800737 plutoplots-0.3.1/plutoplots/__init__.py
+-rw-r--r--   0        0        0     3750 2023-08-07 11:21:25.094680 plutoplots-0.3.1/plutoplots/plot.py
+-rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.1/PKG-INFO
```

### Comparing `plutoplots-0.3.0/LICENSE` & `plutoplots-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.0/README.md` & `plutoplots-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.0/plutoplots/plot.py` & `plutoplots-0.3.1/plutoplots/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" plotting Module """
+
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 
 class Plot:
 
     def __init__(self):
@@ -103,17 +105,17 @@
     def create(self, data, x, hue, ax=None):
         self.axes = sns.kdeplot(data=data, x=x, hue=hue, multiple="stack", ax=ax, zorder=2)
         return self
 
 
 class Histplot(Plot):
 
-    def create(self, data, x, hue, ax=None):
+    def create(self, data, x, hue, ax=None, bandwdth=3):
         self.axes = sns.histplot(data=data, x=x, hue=hue,
-                                 binwidth=3, stat="count", palette="Set2", ax=ax, zorder=2)
+                                 binwidth=bandwdth, stat="count", palette="Set2", ax=ax, zorder=2)
         return self
 
 
 class Boxplot(Plot):
 
     def create(self, data, x, y):
         self.axes = sns.boxplot(x=x, y=y, data=data, zorder=2)
```

### Comparing `plutoplots-0.3.0/PKG-INFO` & `plutoplots-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutoplots
-Version: 0.3.0
+Version: 0.3.1
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
-Metadata-Version: 2.1 Name: plutoplots Version: 0.3.0 Summary: visualization
+Metadata-Version: 2.1 Name: plutoplots Version: 0.3.1 Summary: visualization
 Author-email: Oluwole Ilesanmi
 gmail.com> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: MIT License Project-URL: Home, https://github.com/oluwoleilesanmi/
 pluto
                               ****** Pluto ******
         Visualization library built on top of Seaborn and Matplotlib.
                                Easier plotting
```

