# Comparing `tmp/eliasliu-0.1.6.tar.gz` & `tmp/eliasliu-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.6.tar", last modified: Mon Aug  7 03:00:29 2023, max compression
+gzip compressed data, was "eliasliu-0.1.7.tar", last modified: Mon Aug  7 04:47:05 2023, max compression
```

## Comparing `eliasliu-0.1.6.tar` & `eliasliu-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 03:00:29.097206 eliasliu-0.1.6/
--rw-rw-rw-   0        0        0      750 2023-08-07 03:00:29.096206 eliasliu-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-08-07 02:40:35.000000 eliasliu-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 03:00:29.093704 eliasliu-0.1.6/eliasliu.egg-info/
--rw-rw-rw-   0        0        0      750 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 03:00:28.000000 eliasliu-0.1.6/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 03:00:29.097707 eliasliu-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1884 2023-08-07 03:00:05.000000 eliasliu-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:47:05.584606 eliasliu-0.1.7/
+-rw-rw-rw-   0        0        0      748 2023-08-07 04:47:05.583606 eliasliu-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2023-08-07 02:40:35.000000 eliasliu-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 04:47:05.526066 eliasliu-0.1.7/elias/
+drwxrwxrwx   0        0        0        0 2023-08-07 04:47:05.557617 eliasliu-0.1.7/elias/Scripts/
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.7/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0    22053 2023-07-30 07:29:27.000000 eliasliu-0.1.7/elias/Scripts/auto_create_table_v1.py
+-rw-rw-rw-   0        0        0    25027 2023-08-04 03:07:59.000000 eliasliu-0.1.7/elias/Scripts/auto_create_table_v2.py
+-rw-rw-rw-   0        0        0    13563 2023-07-28 09:49:19.000000 eliasliu-0.1.7/elias/Scripts/clickhouse_base_line.py
+-rw-rw-rw-   0        0        0    62685 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/Scripts/daily_order.py
+-rw-rw-rw-   0        0        0      265 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/Scripts/extract_sql.py
+-rw-rw-rw-   0        0        0     5118 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     1917 2023-07-31 03:06:38.000000 eliasliu-0.1.7/elias/Scripts/log_base_line.py
+-rw-rw-rw-   0        0        0     3798 2023-07-27 03:13:08.000000 eliasliu-0.1.7/elias/Scripts/mysql_alter_comment.py
+-rw-rw-rw-   0        0        0     2438 2023-07-31 09:24:20.000000 eliasliu-0.1.7/elias/Scripts/mysql_comment_get.py
+-rw-rw-rw-   0        0        0      844 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15582 2023-08-03 01:59:48.000000 eliasliu-0.1.7/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0     1442 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/Scripts/py_maxcompute.py
+-rw-rw-rw-   0        0        0     4331 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/Scripts/quality_report.py
+-rw-rw-rw-   0        0        0     2844 2023-07-20 03:39:42.000000 eliasliu-0.1.7/elias/Scripts/send_file.py
+-rw-rw-rw-   0        0        0    13149 2023-08-03 09:58:47.000000 eliasliu-0.1.7/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     1783 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.7/elias/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-08-04 07:51:20.000000 eliasliu-0.1.7/elias/config.py
+-rw-rw-rw-   0        0        0     9670 2023-07-19 09:14:57.000000 eliasliu-0.1.7/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:47:05.570120 eliasliu-0.1.7/elias/datax/
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.7/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15505 2023-08-04 10:52:01.000000 eliasliu-0.1.7/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3304 2023-08-04 07:50:34.000000 eliasliu-0.1.7/elias/datax/job.py
+-rw-rw-rw-   0        0        0     2420 2023-08-04 11:07:52.000000 eliasliu-0.1.7/elias/datax/main.py
+-rw-rw-rw-   0        0        0     3223 2023-08-04 10:39:18.000000 eliasliu-0.1.7/elias/datax/reader.py
+-rw-rw-rw-   0        0        0      578 2023-08-04 11:43:56.000000 eliasliu-0.1.7/elias/datax/run.py
+-rw-rw-rw-   0        0        0     2352 2023-08-04 05:07:21.000000 eliasliu-0.1.7/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    76569 2023-07-27 00:56:04.000000 eliasliu-0.1.7/elias/etl.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:47:05.574128 eliasliu-0.1.7/elias/missions/
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.7/elias/missions/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/missions/pytest.py
+-rw-rw-rw-   0        0        0    70367 2023-08-07 02:23:08.000000 eliasliu-0.1.7/elias/usual.py
+-rw-rw-rw-   0        0        0    13898 2023-07-19 09:48:43.000000 eliasliu-0.1.7/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:47:05.581105 eliasliu-0.1.7/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-08-07 04:47:05.000000 eliasliu-0.1.7/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2023-08-07 04:47:05.000000 eliasliu-0.1.7/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 04:47:05.000000 eliasliu-0.1.7/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 04:47:05.000000 eliasliu-0.1.7/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 04:47:05.584606 eliasliu-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1875 2023-08-07 04:42:35.000000 eliasliu-0.1.7/setup.py
```

### Comparing `eliasliu-0.1.6/PKG-INFO` & `eliasliu-0.1.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.6
+Version: 0.1.7
 Summary: A very easy tool to deal your data
-Home-page: https://gitee.com/eliasliu/elias
+Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `eliasliu-0.1.6/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.7/eliasliu.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.6
+Version: 0.1.7
 Summary: A very easy tool to deal your data
-Home-page: https://gitee.com/eliasliu/elias
+Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `eliasliu-0.1.6/setup.py` & `eliasliu-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.6',  # 版本号
+    version='0.1.7',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
-    url='https://gitee.com/eliasliu/elias',  # 项目的URL
-    packages=find_packages('elias'),  # 包含的包列表，使用find_packages()可以自动查找包含的包
+    url='https://github.com/tenbj/elias',  # 项目的URL
+    packages=find_packages(),  # 包含的包列表，使用find_packages()可以自动查找包含的包
     install_requires=[  # 依赖的其他包（如果有）
         # 'pymysql',
         # 'pymssql',
         # 'pandas',
         # 'sqlalchemy',
         # 'mysql-connector',
         # 'requests',
```

