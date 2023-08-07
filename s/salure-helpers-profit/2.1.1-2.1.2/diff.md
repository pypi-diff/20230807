# Comparing `tmp/salure_helpers_profit-2.1.1.tar.gz` & `tmp/salure_helpers_profit-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-2.1.1.tar", last modified: Thu Jul 27 13:32:33 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-2.1.2.tar", last modified: Mon Aug  7 15:00:13 2023, max compression
```

## Comparing `salure_helpers_profit-2.1.1.tar` & `salure_helpers_profit-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   142536 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:00:13.000000 salure_helpers_profit-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-08-07 15:00:13.000000 salure_helpers_profit-2.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:00:13.000000 salure_helpers_profit-2.1.2/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:00:13.000000 salure_helpers_profit-2.1.2/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-08-07 14:59:59.000000 salure_helpers_profit-2.1.2/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-08-07 14:59:59.000000 salure_helpers_profit-2.1.2/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-08-07 14:59:59.000000 salure_helpers_profit-2.1.2/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-08-07 14:59:59.000000 salure_helpers_profit-2.1.2/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   142985 2023-08-07 14:59:59.000000 salure_helpers_profit-2.1.2/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:00:13.000000 salure_helpers_profit-2.1.2/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-08-07 15:00:12.000000 salure_helpers_profit-2.1.2/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-08-07 15:00:12.000000 salure_helpers_profit-2.1.2/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 15:00:12.000000 salure_helpers_profit-2.1.2/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 15:00:12.000000 salure_helpers_profit-2.1.2/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-08-07 15:00:12.000000 salure_helpers_profit-2.1.2/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-07 15:00:12.000000 salure_helpers_profit-2.1.2/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 15:00:13.000000 salure_helpers_profit-2.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-08-07 14:59:59.000000 salure_helpers_profit-2.1.2/setup.py
```

### Comparing `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-2.1.2/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-2.1.2/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-2.1.2/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-2.1.2/salure_helpers/profit/profit_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,15 @@
         if self.debug:
             print(json.dumps(base_body))
 
         update = requests.request("POST", url, data=json.dumps(base_body), headers=self.headers)
 
         return update
 
-    def update_contract(self, data: dict, overload_fields: dict = None, method='POST') -> requests.Response:
+    def update_contract(self, data: dict, overload_fields: dict = None, method: str = 'POST') -> requests.Response:
         """
         :param data: Dictionary of fields that you want to update in AFAS. Only fields listed in allowed arrays are accepted. Fields listed in required fields array, are mandatory
         :param overload_fields: Dictionary of dictionaries. Specify sub dictionaries for each section you want to update.
         Specify as key which element you want to update, available options are: schedule, salary, contract, function.
         Example: overload_fields = {"employee": {"field": value}}
         :param method: request type
         :return: status code for request and optional error message
@@ -574,16 +574,22 @@
         required_fields_timetable = ['weekly_hours', 'parttime_percentage']
         allowed_fields_timetable = ['changing_work_pattern', 'days_per_week', 'fte', 'on-call_contract', 'type_of_schedule']
 
         # Salary fields
         required_fields_salary = ['type_of_salary', 'period_table']
         allowed_fields_salary = ['step', 'function_scale', 'salary_scale', 'salary_year', 'net_salary', 'apply_timetable', 'salary_amount']
 
-        allowed_fields = allowed_fields_contract + allowed_fields_salary + allowed_fields_timetable + allowed_fields_function
-        required_fields = required_fields_contract + required_fields_function + required_fields_timetable + required_fields_salary
+        if method == 'POST':
+            allowed_fields = allowed_fields_contract + allowed_fields_salary + allowed_fields_timetable + allowed_fields_function
+            required_fields = required_fields_contract + required_fields_function + required_fields_timetable + required_fields_salary
+        elif method == 'PUT':
+            allowed_fields = allowed_fields_contract + required_fields_function + required_fields_timetable + required_fields_salary + allowed_fields_salary + allowed_fields_timetable + allowed_fields_function
+            required_fields = required_fields_contract
+        else:
+            raise ValueError(f'Method {method} not supported, only POST and PUT are supported')
 
         # Check if there are fields that are not allowed or fields missing that are required
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/AfasContract')
 
         base_body = {
```

### Comparing `salure_helpers_profit-2.1.1/setup.py` & `salure_helpers_profit-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='2.1.1',
+    version='2.1.2',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

