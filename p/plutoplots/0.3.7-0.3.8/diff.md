# Comparing `tmp/plutoplots-0.3.7.tar.gz` & `tmp/plutoplots-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutoplots-0.3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "plutoplots-0.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `plutoplots-0.3.7.tar` & `plutoplots-0.3.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.7/.gitignore
--rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.7/LICENSE
--rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.7/README.md
--rw-r--r--   0        0        0       43 2023-08-07 17:36:36.072504 plutoplots-0.3.7/plutoplots/__init__.py
--rw-r--r--   0        0        0     4062 2023-08-07 16:54:01.729151 plutoplots-0.3.7/plutoplots/plot.py
--rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.8/LICENSE
+-rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.8/README.md
+-rw-r--r--   0        0        0       43 2023-08-07 20:56:26.854954 plutoplots-0.3.8/plutoplots/__init__.py
+-rw-r--r--   0        0        0     3938 2023-08-07 20:53:08.437135 plutoplots-0.3.8/plutoplots/plot.py
+-rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.8/PKG-INFO
```

### Comparing `plutoplots-0.3.7/LICENSE` & `plutoplots-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.7/README.md` & `plutoplots-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `plutoplots-0.3.7/plutoplots/plot.py` & `plutoplots-0.3.8/plutoplots/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,16 +122,9 @@
         self.axes = sns.boxplot(x=x, y=y, data=data, zorder=2)
         return self
 
 
 class QQplot(Plot):
 
     def create(self, col, ax=None):
-        self.axes = sm.qqplot(col, line='s', ax=ax)
-        return self
-
-
-class Carplot(Plot):
-
-    def create(self, col, ax=None):
-        self.axes = sm.qqplot(col, line='s', ax=ax)
+        self.axes = sm.qqplot(col, line='s', ax=ax).axes[0]
         return self
```

### Comparing `plutoplots-0.3.7/PKG-INFO` & `plutoplots-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutoplots
-Version: 0.3.7
+Version: 0.3.8
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
-Metadata-Version: 2.1 Name: plutoplots Version: 0.3.7 Summary: visualization
+Metadata-Version: 2.1 Name: plutoplots Version: 0.3.8 Summary: visualization
 Author-email: Oluwole Ilesanmi
 gmail.com> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: MIT License Project-URL: Home, https://github.com/oluwoleilesanmi/
 pluto
                               ****** Pluto ******
         Visualization library built on top of Seaborn and Matplotlib.
                                Easier plotting
```

