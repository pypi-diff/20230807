# Comparing `tmp/eliasliu-0.1.0.tar.gz` & `tmp/eliasliu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.0.tar", last modified: Mon Aug  7 00:53:23 2023, max compression
+gzip compressed data, was "eliasliu-0.1.1.tar", last modified: Mon Aug  7 01:05:53 2023, max compression
```

## Comparing `eliasliu-0.1.0.tar` & `eliasliu-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 00:53:23.903160 eliasliu-0.1.0/
--rw-rw-rw-   0        0        0      665 2023-08-07 00:53:23.902636 eliasliu-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 00:53:23.900152 eliasliu-0.1.0/eliasliu.egg-info/
--rw-rw-rw-   0        0        0      665 2023-08-07 00:53:23.000000 eliasliu-0.1.0/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-08-07 00:53:23.000000 eliasliu-0.1.0/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 00:53:23.000000 eliasliu-0.1.0/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 00:53:23.000000 eliasliu-0.1.0/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 00:53:23.903636 eliasliu-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1062 2023-08-07 00:49:12.000000 eliasliu-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 01:05:53.120425 eliasliu-0.1.1/
+-rw-rw-rw-   0        0        0      665 2023-08-07 01:05:53.119424 eliasliu-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 01:05:53.116923 eliasliu-0.1.1/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0      665 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 01:05:52.000000 eliasliu-0.1.1/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 01:05:53.120925 eliasliu-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-08-07 01:05:44.000000 eliasliu-0.1.1/setup.py
```

### Comparing `eliasliu-0.1.0/PKG-INFO` & `eliasliu-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.0
+Version: 0.1.1
 Summary: A brief description of your package
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eliasliu-0.1.0/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.1/eliasliu.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.0
+Version: 0.1.1
 Summary: A brief description of your package
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eliasliu-0.1.0/setup.py` & `eliasliu-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 @author: Elias.Liu
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.0',  # 版本号
+    version='0.1.1',  # 版本号
     description='A brief description of your package',  # 包的简要描述
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
-    packages=find_packages(),  # 包含的包列表
-    install_requires=[],  # 依赖的其他包（如果有）
+    packages=find_packages(r'C:\Users\Administrator\Desktop\other\elias'),  # 包含的包列表
+    install_requires=['pymysql','pymssql'],  # 依赖的其他包（如果有）
     classifiers=[  # 包的分类标签
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

