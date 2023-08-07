# Comparing `tmp/eliasliu-0.1.8.tar.gz` & `tmp/eliasliu-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.8.tar", last modified: Mon Aug  7 07:28:22 2023, max compression
+gzip compressed data, was "eliasliu-0.1.9.tar", last modified: Mon Aug  7 07:46:51 2023, max compression
```

## Comparing `eliasliu-0.1.8.tar` & `eliasliu-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.704311 eliasliu-0.1.8/
--rw-rw-rw-   0        0        0      748 2023-08-07 07:28:22.703313 eliasliu-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-08-07 02:40:35.000000 eliasliu-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.643266 eliasliu-0.1.8/elias/
-drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.675288 eliasliu-0.1.8/elias/Scripts/
--rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.8/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0    22053 2023-07-30 07:29:27.000000 eliasliu-0.1.8/elias/Scripts/auto_create_table_v1.py
--rw-rw-rw-   0        0        0    25027 2023-08-04 03:07:59.000000 eliasliu-0.1.8/elias/Scripts/auto_create_table_v2.py
--rw-rw-rw-   0        0        0    13563 2023-07-28 09:49:19.000000 eliasliu-0.1.8/elias/Scripts/clickhouse_base_line.py
--rw-rw-rw-   0        0        0    62685 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/Scripts/daily_order.py
--rw-rw-rw-   0        0        0      265 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/Scripts/extract_sql.py
--rw-rw-rw-   0        0        0     5118 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     1917 2023-07-31 03:06:38.000000 eliasliu-0.1.8/elias/Scripts/log_base_line.py
--rw-rw-rw-   0        0        0     3798 2023-07-27 03:13:08.000000 eliasliu-0.1.8/elias/Scripts/mysql_alter_comment.py
--rw-rw-rw-   0        0        0     2438 2023-07-31 09:24:20.000000 eliasliu-0.1.8/elias/Scripts/mysql_comment_get.py
--rw-rw-rw-   0        0        0      844 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15582 2023-08-03 01:59:48.000000 eliasliu-0.1.8/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0     1442 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/Scripts/py_maxcompute.py
--rw-rw-rw-   0        0        0     4331 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/Scripts/quality_report.py
--rw-rw-rw-   0        0        0     2844 2023-07-20 03:39:42.000000 eliasliu-0.1.8/elias/Scripts/send_file.py
--rw-rw-rw-   0        0        0    13149 2023-08-03 09:58:47.000000 eliasliu-0.1.8/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     1783 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.8/elias/__init__.py
--rw-rw-rw-   0        0        0      196 2023-08-04 07:51:20.000000 eliasliu-0.1.8/elias/config.py
--rw-rw-rw-   0        0        0     9670 2023-07-19 09:14:57.000000 eliasliu-0.1.8/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.688302 eliasliu-0.1.8/elias/datax/
--rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.8/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15505 2023-08-04 10:52:01.000000 eliasliu-0.1.8/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3304 2023-08-04 07:50:34.000000 eliasliu-0.1.8/elias/datax/job.py
--rw-rw-rw-   0        0        0     2420 2023-08-04 11:07:52.000000 eliasliu-0.1.8/elias/datax/main.py
--rw-rw-rw-   0        0        0     3223 2023-08-04 10:39:18.000000 eliasliu-0.1.8/elias/datax/reader.py
--rw-rw-rw-   0        0        0      578 2023-08-04 11:43:56.000000 eliasliu-0.1.8/elias/datax/run.py
--rw-rw-rw-   0        0        0     2352 2023-08-04 05:07:21.000000 eliasliu-0.1.8/elias/datax/writer.py
--rw-rw-rw-   0        0        0    76569 2023-07-27 00:56:04.000000 eliasliu-0.1.8/elias/etl.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.691303 eliasliu-0.1.8/elias/missions/
--rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.8/elias/missions/__init__.py
--rw-rw-rw-   0        0        0      212 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/missions/pytest.py
--rw-rw-rw-   0        0        0    70367 2023-08-07 02:23:08.000000 eliasliu-0.1.8/elias/usual.py
--rw-rw-rw-   0        0        0    13898 2023-07-19 09:48:43.000000 eliasliu-0.1.8/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.701320 eliasliu-0.1.8/eliasliu.egg-info/
--rw-rw-rw-   0        0        0      748 2023-08-07 07:28:22.000000 eliasliu-0.1.8/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-08-07 07:28:22.000000 eliasliu-0.1.8/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 07:28:22.000000 eliasliu-0.1.8/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      170 2023-08-07 07:28:22.000000 eliasliu-0.1.8/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-07 07:28:22.000000 eliasliu-0.1.8/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 07:28:22.704311 eliasliu-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-08-07 07:05:43.000000 eliasliu-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:46:51.964891 eliasliu-0.1.9/
+-rw-rw-rw-   0        0        0      748 2023-08-07 07:46:51.963890 eliasliu-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2023-08-07 02:40:35.000000 eliasliu-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:46:51.909852 eliasliu-0.1.9/elias/
+drwxrwxrwx   0        0        0        0 2023-08-07 07:46:51.938872 eliasliu-0.1.9/elias/Scripts/
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.9/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0    22053 2023-07-30 07:29:27.000000 eliasliu-0.1.9/elias/Scripts/auto_create_table_v1.py
+-rw-rw-rw-   0        0        0    25027 2023-08-04 03:07:59.000000 eliasliu-0.1.9/elias/Scripts/auto_create_table_v2.py
+-rw-rw-rw-   0        0        0    13563 2023-07-28 09:49:19.000000 eliasliu-0.1.9/elias/Scripts/clickhouse_base_line.py
+-rw-rw-rw-   0        0        0    62685 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/Scripts/daily_order.py
+-rw-rw-rw-   0        0        0      265 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/Scripts/extract_sql.py
+-rw-rw-rw-   0        0        0     5118 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     1917 2023-07-31 03:06:38.000000 eliasliu-0.1.9/elias/Scripts/log_base_line.py
+-rw-rw-rw-   0        0        0     3798 2023-07-27 03:13:08.000000 eliasliu-0.1.9/elias/Scripts/mysql_alter_comment.py
+-rw-rw-rw-   0        0        0     2438 2023-07-31 09:24:20.000000 eliasliu-0.1.9/elias/Scripts/mysql_comment_get.py
+-rw-rw-rw-   0        0        0      844 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15582 2023-08-03 01:59:48.000000 eliasliu-0.1.9/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0     1442 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/Scripts/py_maxcompute.py
+-rw-rw-rw-   0        0        0     4331 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/Scripts/quality_report.py
+-rw-rw-rw-   0        0        0     2844 2023-07-20 03:39:42.000000 eliasliu-0.1.9/elias/Scripts/send_file.py
+-rw-rw-rw-   0        0        0    13149 2023-08-03 09:58:47.000000 eliasliu-0.1.9/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     1783 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.9/elias/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-08-04 07:51:20.000000 eliasliu-0.1.9/elias/config.py
+-rw-rw-rw-   0        0        0     9670 2023-07-19 09:14:57.000000 eliasliu-0.1.9/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:46:51.950881 eliasliu-0.1.9/elias/datax/
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.9/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15505 2023-08-04 10:52:01.000000 eliasliu-0.1.9/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3304 2023-08-04 07:50:34.000000 eliasliu-0.1.9/elias/datax/job.py
+-rw-rw-rw-   0        0        0     2420 2023-08-04 11:07:52.000000 eliasliu-0.1.9/elias/datax/main.py
+-rw-rw-rw-   0        0        0     3223 2023-08-04 10:39:18.000000 eliasliu-0.1.9/elias/datax/reader.py
+-rw-rw-rw-   0        0        0      578 2023-08-04 11:43:56.000000 eliasliu-0.1.9/elias/datax/run.py
+-rw-rw-rw-   0        0        0     2352 2023-08-04 05:07:21.000000 eliasliu-0.1.9/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    76569 2023-07-27 00:56:04.000000 eliasliu-0.1.9/elias/etl.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:46:51.953883 eliasliu-0.1.9/elias/missions/
+-rw-rw-rw-   0        0        0      131 2023-08-07 04:43:51.000000 eliasliu-0.1.9/elias/missions/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/missions/pytest.py
+-rw-rw-rw-   0        0        0    70367 2023-08-07 02:23:08.000000 eliasliu-0.1.9/elias/usual.py
+-rw-rw-rw-   0        0        0    13898 2023-07-19 09:48:43.000000 eliasliu-0.1.9/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:46:51.961889 eliasliu-0.1.9/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-08-07 07:46:51.000000 eliasliu-0.1.9/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2023-08-07 07:46:51.000000 eliasliu-0.1.9/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:46:51.000000 eliasliu-0.1.9/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2023-08-07 07:46:51.000000 eliasliu-0.1.9/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 07:46:51.000000 eliasliu-0.1.9/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:46:51.964891 eliasliu-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-08-07 07:46:28.000000 eliasliu-0.1.9/setup.py
```

### Comparing `eliasliu-0.1.8/PKG-INFO` & `eliasliu-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.8
+Version: 0.1.9
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.8/elias/Scripts/auto_create_table_v1.py` & `eliasliu-0.1.9/elias/Scripts/auto_create_table_v1.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/auto_create_table_v2.py` & `eliasliu-0.1.9/elias/Scripts/auto_create_table_v2.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/clickhouse_base_line.py` & `eliasliu-0.1.9/elias/Scripts/clickhouse_base_line.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/daily_order.py` & `eliasliu-0.1.9/elias/Scripts/daily_order.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/jd.py` & `eliasliu-0.1.9/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/log_base_line.py` & `eliasliu-0.1.9/elias/Scripts/log_base_line.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/mysql_alter_comment.py` & `eliasliu-0.1.9/elias/Scripts/mysql_alter_comment.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/mysql_comment_get.py` & `eliasliu-0.1.9/elias/Scripts/mysql_comment_get.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/name_in_db.py` & `eliasliu-0.1.9/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.9/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/py_maxcompute.py` & `eliasliu-0.1.9/elias/Scripts/py_maxcompute.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/quality_report.py` & `eliasliu-0.1.9/elias/Scripts/quality_report.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/send_file.py` & `eliasliu-0.1.9/elias/Scripts/send_file.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.9/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/Scripts/youdao.py` & `eliasliu-0.1.9/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/datamove.py` & `eliasliu-0.1.9/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/datax/auto_create_table.py` & `eliasliu-0.1.9/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/datax/job.py` & `eliasliu-0.1.9/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/datax/main.py` & `eliasliu-0.1.9/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/datax/reader.py` & `eliasliu-0.1.9/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/datax/run.py` & `eliasliu-0.1.9/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/datax/writer.py` & `eliasliu-0.1.9/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/etl.py` & `eliasliu-0.1.9/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/usual.py` & `eliasliu-0.1.9/elias/usual.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/elias/wechat.py` & `eliasliu-0.1.9/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.9/eliasliu.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.8
+Version: 0.1.9
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.8/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.9/eliasliu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.8/setup.py` & `eliasliu-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.8',  # 版本号
+    version='0.1.9',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
     packages=find_packages(),  # 包含的包列表，使用find_packages()可以自动查找包含的包
     install_requires=[  # 依赖的其他包（如果有）
         'pymysql',
-        'pymssql',
+        'pymssql==2.2.5',
         'pandas',
         'sqlalchemy',
         'mysql-connector',
         'requests',
         'mysql-connector-python',
         'impyla',
         'clickhouse_sqlalchemy',
```

