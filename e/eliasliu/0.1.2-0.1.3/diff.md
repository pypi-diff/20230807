# Comparing `tmp/eliasliu-0.1.2.tar.gz` & `tmp/eliasliu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.2.tar", last modified: Mon Aug  7 02:02:34 2023, max compression
+gzip compressed data, was "eliasliu-0.1.3.tar", last modified: Mon Aug  7 02:04:51 2023, max compression
```

## Comparing `eliasliu-0.1.2.tar` & `eliasliu-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 02:02:34.583665 eliasliu-0.1.2/
--rw-rw-rw-   0        0        0      790 2023-08-07 02:02:34.582664 eliasliu-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 02:02:34.580162 eliasliu-0.1.2/eliasliu.egg-info/
--rw-rw-rw-   0        0        0      790 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      170 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:02:34.000000 eliasliu-0.1.2/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 02:02:34.584165 eliasliu-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1766 2023-08-07 02:02:04.000000 eliasliu-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:04:51.381280 eliasliu-0.1.3/
+-rw-rw-rw-   0        0        0      790 2023-08-07 02:04:51.380279 eliasliu-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 02:04:51.377777 eliasliu-0.1.3/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0      790 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 02:04:51.381780 eliasliu-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1768 2023-08-07 02:04:41.000000 eliasliu-0.1.3/setup.py
```

### Comparing `eliasliu-0.1.2/PKG-INFO` & `eliasliu-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.2
+Version: 0.1.3
 Summary: A very easy tool to deal your data
 Home-page: https://gitee.com/eliasliu/elias.git
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.2/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.3/eliasliu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.2
+Version: 0.1.3
 Summary: A very easy tool to deal your data
 Home-page: https://gitee.com/eliasliu/elias.git
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.2/setup.py` & `eliasliu-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 """
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.2',  # 版本号
+    version='0.1.3',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://gitee.com/eliasliu/elias.git',  # 项目的URL
     packages=find_packages('elias'),  # 包含的包列表，使用find_packages()可以自动查找包含的包
     install_requires=[  # 依赖的其他包（如果有）
         'pymysql',
-        'pymssql',
+        # 'pymssql',
         'pandas',
         'sqlalchemy',
         'mysql-connector',
         'requests',
         'mysql-connector-python',
         'impyla',
         'clickhouse_sqlalchemy',
```

