# Comparing `tmp/eliasliu-0.1.1.tar.gz` & `tmp/eliasliu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.1.tar", last modified: Mon Aug  7 01:05:53 2023, max compression
+gzip compressed data, was "eliasliu-0.1.2.tar", last modified: Mon Aug  7 02:02:34 2023, max compression
```

## Comparing `eliasliu-0.1.1.tar` & `eliasliu-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 01:05:53.120425 eliasliu-0.1.1/
--rw-rw-rw-   0        0        0      665 2023-08-07 01:05:53.119424 eliasliu-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 01:05:53.116923 eliasliu-0.1.1/eliasliu.egg-info/
--rw-rw-rw-   0        0        0      665 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 01:05:53.120925 eliasliu-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-08-07 01:05:44.000000 eliasliu-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:02:34.583665 eliasliu-0.1.2/
+-rw-rw-rw-   0        0        0      790 2023-08-07 02:02:34.582664 eliasliu-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 02:02:34.580162 eliasliu-0.1.2/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0      790 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      170 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 02:02:34.584165 eliasliu-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1766 2023-08-07 02:02:04.000000 eliasliu-0.1.2/setup.py
```

### Comparing `eliasliu-0.1.1/PKG-INFO` & `eliasliu-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.1
-Summary: A brief description of your package
+Version: 0.1.2
+Summary: A very easy tool to deal your data
+Home-page: https://gitee.com/eliasliu/elias.git
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+Data Engineer & Analyst will use
```

### Comparing `eliasliu-0.1.1/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.2/eliasliu.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.1
-Summary: A brief description of your package
+Version: 0.1.2
+Summary: A very easy tool to deal your data
+Home-page: https://gitee.com/eliasliu/elias.git
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+Data Engineer & Analyst will use
```

