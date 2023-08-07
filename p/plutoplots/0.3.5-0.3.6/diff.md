# Comparing `tmp/plutoplots-0.3.5.tar.gz` & `tmp/plutoplots-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutoplots-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "plutoplots-0.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `plutoplots-0.3.5.tar` & `plutoplots-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.5/.gitignore
--rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.5/LICENSE
--rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.5/README.md
--rw-r--r--   0        0        0       43 2023-08-07 16:34:36.272548 plutoplots-0.3.5/plutoplots/__init__.py
--rw-r--r--   0        0        0     3930 2023-08-07 16:34:36.270689 plutoplots-0.3.5/plutoplots/plot.py
--rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.6/LICENSE
+-rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.6/README.md
+-rw-r--r--   0        0        0       43 2023-08-07 16:54:55.376779 plutoplots-0.3.6/plutoplots/__init__.py
+-rw-r--r--   0        0        0     4062 2023-08-07 16:54:01.729151 plutoplots-0.3.6/plutoplots/plot.py
+-rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.6/PKG-INFO
```

### Comparing `plutoplots-0.3.5/LICENSE` & `plutoplots-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.5/README.md` & `plutoplots-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.5/plutoplots/plot.py` & `plutoplots-0.3.6/plutoplots/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,7 +124,14 @@
 
 
 class QQplot(Plot):
 
     def create(self, col, ax=None):
         self.axes = sm.qqplot(col, line='s', ax=ax)
         return self
+
+
+class Carplot(Plot):
+
+    def create(self, col, ax=None):
+        self.axes = sm.qqplot(col, line='s', ax=ax)
+        return self
```

### Comparing `plutoplots-0.3.5/PKG-INFO` & `plutoplots-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutoplots
-Version: 0.3.5
+Version: 0.3.6
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
-Metadata-Version: 2.1 Name: plutoplots Version: 0.3.5 Summary: visualization
+Metadata-Version: 2.1 Name: plutoplots Version: 0.3.6 Summary: visualization
 Author-email: Oluwole Ilesanmi
 gmail.com> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: MIT License Project-URL: Home, https://github.com/oluwoleilesanmi/
 pluto
                               ****** Pluto ******
         Visualization library built on top of Seaborn and Matplotlib.
                                Easier plotting
```

