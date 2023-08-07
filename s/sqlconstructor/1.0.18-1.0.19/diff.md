# Comparing `tmp/sqlconstructor-1.0.18.tar.gz` & `tmp/sqlconstructor-1.0.19.tar.gz`

## Comparing `sqlconstructor-1.0.18.tar` & `sqlconstructor-1.0.19.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/pytest.ini
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/__init__.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/constants.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/helpers.py
--rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_container.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_cte.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_query.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_section.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/simple_query_dict.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/expected_examples/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/expected_examples/select_section_of_simple_query.sql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/expected_examples/simple_query.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_container_filled_by_section_call.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_del_vars.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_init.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_reset_vars.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_set_vars.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/test_add.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/test_building_process.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/test_call_section.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/test_init.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/test_upper_sql_keywords.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/LICENSE
--rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/pyproject.toml
--rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/pytest.ini
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/__init__.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/constants.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/helpers.py
+-rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_container.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_cte.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_query.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_section.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/simple_query_dict.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/expected_examples/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/expected_examples/select_section_of_simple_query.sql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/expected_examples/simple_query.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_container_filled_by_section_call.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_del_vars.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_init.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_reset_vars.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_set_vars.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/test_add.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/test_building_process.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/test_call_section.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/test_init.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/test_upper_sql_keywords.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/LICENSE
+-rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/pyproject.toml
+-rw-r--r--   0        0        0     9770 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/PKG-INFO
```

### Comparing `sqlconstructor-1.0.18/src/sqlconstructor/constants.py` & `sqlconstructor-1.0.19/src/sqlconstructor/constants.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/src/sqlconstructor/helpers.py` & `sqlconstructor-1.0.19/src/sqlconstructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/src/sqlconstructor/sql_container.py` & `sqlconstructor-1.0.19/src/sqlconstructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/src/sqlconstructor/sql_cte.py` & `sqlconstructor-1.0.19/src/sqlconstructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/src/sqlconstructor/sql_query.py` & `sqlconstructor-1.0.19/src/sqlconstructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/src/sqlconstructor/sql_section.py` & `sqlconstructor-1.0.19/src/sqlconstructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/fixtures/simple_query_dict.py` & `sqlconstructor-1.0.19/tests/fixtures/simple_query_dict.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/fixtures/expected_examples/__init__.py` & `sqlconstructor-1.0.19/tests/fixtures/expected_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_container/test_del_vars.py` & `sqlconstructor-1.0.19/tests/test_sql_container/test_del_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_container/test_init.py` & `sqlconstructor-1.0.19/tests/test_sql_container/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_container/test_reset_vars.py` & `sqlconstructor-1.0.19/tests/test_sql_container/test_reset_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_container/test_set_vars.py` & `sqlconstructor-1.0.19/tests/test_sql_container/test_set_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_query/test_add.py` & `sqlconstructor-1.0.19/tests/test_sql_query/test_add.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_query/test_building_process.py` & `sqlconstructor-1.0.19/tests/test_sql_query/test_building_process.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_query/test_init.py` & `sqlconstructor-1.0.19/tests/test_sql_query/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/tests/test_sql_section/test_upper_sql_keywords.py` & `sqlconstructor-1.0.19/tests/test_sql_section/test_upper_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/LICENSE` & `sqlconstructor-1.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.18/README.md` & `sqlconstructor-1.0.19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: sqlconstructor
+Version: 1.0.19
+Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
+Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
+Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
+Project-URL: Telegram, https://t.me/sqlconstructor
+Author-email: Andrey Smirnov <abc-sm@yandex.ru>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # sqlconstructor
 **sqlconstructor** is simple, yet very flexible, sql building tool.
 
 ## How to install
 You could install from PyPi:
 ```console
 $ python3 -m pip install sqlconstructor
@@ -38,16 +53,17 @@
 container: sc.SqlContainer = q()
 # get sql as string
 sql_text: str = str(container)
 ```
 ### Output
 SqlSection automatically transform all sql keywords in uppercase.
 It does not upper in following cases:
-1) if sql keyword is located in inline/multiline comment.
-2) if sql keyword is located inside single/double quotes.
+- if sql keyword is located in inline/multiline comment.
+- if sql keyword is located inside single/double quotes.
+
 Output of sql_text is
 ```sql
 SELECT
   id,
   name
 FROM
   product
@@ -79,15 +95,15 @@
     )
     q['from'](
         'product'
     )
     q['where'](
         'quality = $quality',
         'and brand_id = $brand_id'
-    )(qulaity=product_quality, brand_id=brand_identifier)
+    )(quality=product_quality, brand_id=brand_identifier)
     q['order by']('name DESC')
     container: sc.SqlContainer = q()
     return container
 ```
 
 #### or later in SqlContainer
 ```python
@@ -130,16 +146,19 @@
 ### You could cache SqlContainer and set/change variables later
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
+    # you could set default values of variables inside of cached result
+    # and reset it later. 
+    # Or do not set them in cached result at all and set them later. 
     container: sc.SqlContainer = get_product_query()
-    # set variables to existing container
+    # set/reset variables to existing container
     container(quality='Best', brand_id=1)
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
 ```
@@ -196,15 +215,15 @@
         'product as p',
     )
     q['left join lateral'](
         get_left_join_lateral(),
     )
     q['where'](
       'p.quality = $quality',
-      'and brand_id = $brand_id'
+      'and p.brand_id = $brand_id'
     )(quality='Best', brand_id=1)
 
 
 def get_left_join_lateral() -> sc.SqlContainer:
     j = sc.SqlQuery()
     j['select'](
         'e.id',
```

### Comparing `sqlconstructor-1.0.18/pyproject.toml` & `sqlconstructor-1.0.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlconstructor"
-version = "1.0.18"
+version = "1.0.19"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlconstructor-1.0.18/PKG-INFO` & `sqlconstructor-1.0.19/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sqlconstructor
-Version: 1.0.18
-Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
-Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
-Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
-Project-URL: Telegram, https://t.me/sqlconstructor
-Author-email: Andrey Smirnov <abc-sm@yandex.ru>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # sqlconstructor
 **sqlconstructor** is simple, yet very flexible, sql building tool.
 
 ## How to install
 You could install from PyPi:
 ```console
 $ python3 -m pip install sqlconstructor
@@ -53,16 +38,17 @@
 container: sc.SqlContainer = q()
 # get sql as string
 sql_text: str = str(container)
 ```
 ### Output
 SqlSection automatically transform all sql keywords in uppercase.
 It does not upper in following cases:
-1) if sql keyword is located in inline/multiline comment.
-2) if sql keyword is located inside single/double quotes.
+- if sql keyword is located in inline/multiline comment.
+- if sql keyword is located inside single/double quotes.
+
 Output of sql_text is
 ```sql
 SELECT
   id,
   name
 FROM
   product
@@ -94,15 +80,15 @@
     )
     q['from'](
         'product'
     )
     q['where'](
         'quality = $quality',
         'and brand_id = $brand_id'
-    )(qulaity=product_quality, brand_id=brand_identifier)
+    )(quality=product_quality, brand_id=brand_identifier)
     q['order by']('name DESC')
     container: sc.SqlContainer = q()
     return container
 ```
 
 #### or later in SqlContainer
 ```python
@@ -145,16 +131,19 @@
 ### You could cache SqlContainer and set/change variables later
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
+    # you could set default values of variables inside of cached result
+    # and reset it later. 
+    # Or do not set them in cached result at all and set them later. 
     container: sc.SqlContainer = get_product_query()
-    # set variables to existing container
+    # set/reset variables to existing container
     container(quality='Best', brand_id=1)
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
 ```
@@ -211,15 +200,15 @@
         'product as p',
     )
     q['left join lateral'](
         get_left_join_lateral(),
     )
     q['where'](
       'p.quality = $quality',
-      'and brand_id = $brand_id'
+      'and p.brand_id = $brand_id'
     )(quality='Best', brand_id=1)
 
 
 def get_left_join_lateral() -> sc.SqlContainer:
     j = sc.SqlQuery()
     j['select'](
         'e.id',
```

