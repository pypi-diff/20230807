# Comparing `tmp/eliasliu-0.1.3.tar.gz` & `tmp/eliasliu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.3.tar", last modified: Mon Aug  7 02:04:51 2023, max compression
+gzip compressed data, was "eliasliu-0.1.4.tar", last modified: Mon Aug  7 02:24:02 2023, max compression
```

## Comparing `eliasliu-0.1.3.tar` & `eliasliu-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 02:04:51.381280 eliasliu-0.1.3/
--rw-rw-rw-   0        0        0      790 2023-08-07 02:04:51.380279 eliasliu-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 02:04:51.377777 eliasliu-0.1.3/eliasliu.egg-info/
--rw-rw-rw-   0        0        0      790 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:04:51.000000 eliasliu-0.1.3/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 02:04:51.381780 eliasliu-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1768 2023-08-07 02:04:41.000000 eliasliu-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:24:02.941252 eliasliu-0.1.4/
+-rw-rw-rw-   0        0        0      790 2023-08-07 02:24:02.940751 eliasliu-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 02:24:02.938249 eliasliu-0.1.4/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0      790 2023-08-07 02:24:02.000000 eliasliu-0.1.4/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2023-08-07 02:24:02.000000 eliasliu-0.1.4/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:24:02.000000 eliasliu-0.1.4/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:24:02.000000 eliasliu-0.1.4/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 02:24:02.941752 eliasliu-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1798 2023-08-07 02:23:43.000000 eliasliu-0.1.4/setup.py
```

### Comparing `eliasliu-0.1.3/PKG-INFO` & `eliasliu-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.3
+Version: 0.1.4
 Summary: A very easy tool to deal your data
 Home-page: https://gitee.com/eliasliu/elias.git
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.3/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.4/eliasliu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.3
+Version: 0.1.4
 Summary: A very easy tool to deal your data
 Home-page: https://gitee.com/eliasliu/elias.git
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.3/setup.py` & `eliasliu-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 """
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.3',  # 版本号
+    version='0.1.4',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://gitee.com/eliasliu/elias.git',  # 项目的URL
     packages=find_packages('elias'),  # 包含的包列表，使用find_packages()可以自动查找包含的包
     install_requires=[  # 依赖的其他包（如果有）
-        'pymysql',
+        # 'pymysql',
         # 'pymssql',
-        'pandas',
-        'sqlalchemy',
-        'mysql-connector',
-        'requests',
-        'mysql-connector-python',
-        'impyla',
-        'clickhouse_sqlalchemy',
-        'clickhouse_driver',
-        'odps',
-        'bs4',
-        'selenium',
-        'loguru',
-        'logging',
-        'zipfile'
+        # 'pandas',
+        # 'sqlalchemy',
+        # 'mysql-connector',
+        # 'requests',
+        # 'mysql-connector-python',
+        # 'impyla',
+        # 'clickhouse_sqlalchemy',
+        # 'clickhouse_driver',
+        # 'odps',
+        # 'bs4',
+        # 'selenium',
+        # 'loguru',
+        # 'logging',
+        # 'zipfile'
     ],
     classifiers=[  # 包的分类标签
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

