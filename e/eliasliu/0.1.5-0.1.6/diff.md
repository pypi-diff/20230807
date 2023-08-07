# Comparing `tmp/eliasliu-0.1.5.tar.gz` & `tmp/eliasliu-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.5.tar", last modified: Mon Aug  7 02:32:03 2023, max compression
+gzip compressed data, was "eliasliu-0.1.6.tar", last modified: Mon Aug  7 03:00:29 2023, max compression
```

## Comparing `eliasliu-0.1.5.tar` & `eliasliu-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 02:32:03.797597 eliasliu-0.1.5/
--rw-rw-rw-   0        0        0      790 2023-08-07 02:32:03.796596 eliasliu-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 02:32:03.794094 eliasliu-0.1.5/eliasliu.egg-info/
--rw-rw-rw-   0        0        0      790 2023-08-07 02:32:03.000000 eliasliu-0.1.5/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-08-07 02:32:03.000000 eliasliu-0.1.5/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:32:03.000000 eliasliu-0.1.5/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:32:03.000000 eliasliu-0.1.5/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 02:32:03.798097 eliasliu-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1798 2023-08-07 02:31:42.000000 eliasliu-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:00:29.097206 eliasliu-0.1.6/
+-rw-rw-rw-   0        0        0      750 2023-08-07 03:00:29.096206 eliasliu-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2023-08-07 02:40:35.000000 eliasliu-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 03:00:29.093704 eliasliu-0.1.6/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 03:00:29.097707 eliasliu-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1884 2023-08-07 03:00:05.000000 eliasliu-0.1.6/setup.py
```

### Comparing `eliasliu-0.1.5/PKG-INFO` & `eliasliu-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.5
+Version: 0.1.6
 Summary: A very easy tool to deal your data
-Home-page: https://gitee.com/eliasliu/elias.git
+Home-page: https://gitee.com/eliasliu/elias
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
 Description-Content-Type: text/markdown
-
-Data Engineer & Analyst will use
```

### Comparing `eliasliu-0.1.5/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.6/eliasliu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.5
+Version: 0.1.6
 Summary: A very easy tool to deal your data
-Home-page: https://gitee.com/eliasliu/elias.git
+Home-page: https://gitee.com/eliasliu/elias
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
 Description-Content-Type: text/markdown
-
-Data Engineer & Analyst will use
```

### Comparing `eliasliu-0.1.5/setup.py` & `eliasliu-0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 
 @author: Elias.Liu
 """
 
 
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='eliasliu',  # 包名
-    version='0.1.5',  # 版本号
+    version='0.1.6',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
-    long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
+    # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
-    url='https://gitee.com/eliasliu/elias.git',  # 项目的URL
+    url='https://gitee.com/eliasliu/elias',  # 项目的URL
     packages=find_packages('elias'),  # 包含的包列表，使用find_packages()可以自动查找包含的包
     install_requires=[  # 依赖的其他包（如果有）
         # 'pymysql',
         # 'pymssql',
         # 'pandas',
         # 'sqlalchemy',
         # 'mysql-connector',
```

