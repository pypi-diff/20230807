# Comparing `tmp/sqlconstructor-1.0.19.tar.gz` & `tmp/sqlconstructor-1.0.20.tar.gz`

## Comparing `sqlconstructor-1.0.19.tar` & `sqlconstructor-1.0.20.tar`

### file list

```diff
@@ -1,34 +1,53 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/pytest.ini
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/__init__.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/constants.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/helpers.py
--rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_container.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_cte.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_query.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/src/sqlconstructor/sql_section.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/simple_query_dict.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/expected_examples/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/expected_examples/select_section_of_simple_query.sql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/fixtures/expected_examples/simple_query.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_container_filled_by_section_call.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_del_vars.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_init.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_reset_vars.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_set_vars.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_container/test_wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/test_add.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/test_building_process.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_query/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/test_call_section.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/test_init.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/tests/test_sql_section/test_upper_sql_keywords.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/LICENSE
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/pyproject.toml
--rw-r--r--   0        0        0     9770 2020-02-02 00:00:00.000000 sqlconstructor-1.0.19/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/pytest.ini
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/__init__.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/constants.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/helpers.py
+-rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_container.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_cte.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_query.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_section.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/simple_query_dict.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/expected_examples/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/expected_examples/select_section_of_simple_query.sql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/expected_examples/simple_query.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/__init__.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_bool.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_container_filled_by_section_call.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_del_vars.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_init.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_json_variable.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_reset_vars.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_set_vars.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_unwrap.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_call.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_clear.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_delitem.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_getitem.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_init.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_iter.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_pop.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_reg.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_setitem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_add.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_bool.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_building_process.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_call.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_init.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_iter.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_len.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_sections_pop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_bool.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_call.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_init.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_upper_sql_keywords.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/LICENSE
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/pyproject.toml
+-rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/PKG-INFO
```

### Comparing `sqlconstructor-1.0.19/src/sqlconstructor/constants.py` & `sqlconstructor-1.0.20/src/sqlconstructor/constants.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/src/sqlconstructor/helpers.py` & `sqlconstructor-1.0.20/src/sqlconstructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/src/sqlconstructor/sql_container.py` & `sqlconstructor-1.0.20/src/sqlconstructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/src/sqlconstructor/sql_cte.py` & `sqlconstructor-1.0.20/src/sqlconstructor/sql_cte.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,10 +49,10 @@
         *,
         sql_id: Optional[str| uuid.UUID] = '',  # works only if sql_query parameter is not provided
     ) -> SqlQuery:
         """Create new cte and return SqlQuery instance"""
         kwargs = {}
         if sql_id:
             kwargs['sql_id'] = sql_id
-        query = sql_query or SqlQuery(**kwargs)
+        query = sql_query if isinstance(sql_query, SqlQuery) else SqlQuery(**kwargs)
         self[cte_name] = query
         return query
```

### Comparing `sqlconstructor-1.0.19/src/sqlconstructor/sql_query.py` & `sqlconstructor-1.0.20/src/sqlconstructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/src/sqlconstructor/sql_section.py` & `sqlconstructor-1.0.20/src/sqlconstructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/fixtures/simple_query_dict.py` & `sqlconstructor-1.0.20/tests/fixtures/simple_query_dict.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/fixtures/expected_examples/__init__.py` & `sqlconstructor-1.0.20/tests/fixtures/expected_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/test_sql_container/test_del_vars.py` & `sqlconstructor-1.0.20/tests/test_sql_container/test_del_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/test_sql_container/test_init.py` & `sqlconstructor-1.0.20/tests/test_sql_container/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/test_sql_container/test_reset_vars.py` & `sqlconstructor-1.0.20/tests/test_sql_container/test_reset_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/test_sql_container/test_set_vars.py` & `sqlconstructor-1.0.20/tests/test_sql_container/test_set_vars.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,37 @@
     container = SqlContainer(sql_text)
     assert len(container.vars) == 0
     container(quality='Best', brand_id=1)
     make_common_assertions(container)
 
 
 @pytest.mark.SqlContainer
+def test_set_variables_with_type_casting_by_calling_container():
+    sql_text = 'quality = $quality::text AND brand_id = $brand_id::int'
+    container = SqlContainer(sql_text)
+    assert len(container.vars) == 0
+    container(quality='Best', brand_id=1)
+    make_common_assertions(container, type_casting=True)
+
+
+@pytest.mark.SqlContainer
 def test_set_variables_by_vars_attribute():
     sql_text = 'quality = $quality AND brand_id = $brand_id'
     container = SqlContainer(sql_text)
     assert len(container.vars) == 0
-    container.vars['quality'] ='Best'
+    container.vars['quality'] = 'Best'
     container.vars['brand_id'] = 1
     make_common_assertions(container)
 
 
-def make_common_assertions(container):
+def make_common_assertions(container, type_casting=False):
     assert len(container.vars) == 2
     # check that in str representation placeholders are not replaced by vars
-    assert 'Best' not in str(container)
-    assert '1' not in str(container)
+    assert (
+        str(container) == f"quality = $quality{'::text' if type_casting else ''}"
+        f" AND brand_id = $brand_id{'::int' if type_casting else ''}"
+    )
     # check that placeholders are replaced by vars only in 'dumps' method result
-    assert "quality = 'Best' AND brand_id = 1" == container.dumps()
+    assert (
+        container.dumps() == f"quality = 'Best'{'::text' if type_casting else ''}"
+        f" AND brand_id = 1{'::int' if type_casting else ''}"
+    )
```

### Comparing `sqlconstructor-1.0.19/tests/test_sql_query/test_add.py` & `sqlconstructor-1.0.20/tests/test_sql_query/test_add.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/test_sql_query/test_building_process.py` & `sqlconstructor-1.0.20/tests/test_sql_query/test_building_process.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/tests/test_sql_query/test_init.py` & `sqlconstructor-1.0.20/tests/test_sql_query/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def test_init_with_no_args():
     q = SqlQuery()
     assert isinstance(q, SqlQuery)
 
 
 @pytest.mark.SqlQuery
 def test_init_with_sql_id():
-    sql_id = 'some'
+    sql_id = 'abc'
     q = SqlQuery(sql_id=sql_id)
     assert q.sql_id == sql_id
 
 
 @pytest.mark.SqlQuery
 @pytest.mark.SqlSection
 @pytest.mark.SqlContainer
```

### Comparing `sqlconstructor-1.0.19/tests/test_sql_section/test_upper_sql_keywords.py` & `sqlconstructor-1.0.20/tests/test_sql_section/test_upper_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/LICENSE` & `sqlconstructor-1.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.19/README.md` & `sqlconstructor-1.0.20/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,29 @@
 
 # build query into SqlContainer
 container: sc.SqlContainer = q()
 # get sql as string
 sql_text: str = str(container)
 ```
 ### Output
-SqlSection automatically transform all sql keywords in uppercase.
+**SqlSection** automatically transforms all sql keywords in uppercase. 
 It does not upper in following cases:
 - if sql keyword is located in inline/multiline comment.
 - if sql keyword is located inside single/double quotes.
 
+**SqlSection** automatically adds comma between provided sql statements in \_\_call\_\_ method for next headers:
+- SELECT
+- FROM
+- SET
+- VALUES
+- ORDER BY
+- GROUP BY
+- JSON_OBJECT_AGG
+- COALESCE
+
 Output of sql_text is
 ```sql
 SELECT
   id,
   name
 FROM
   product
```

### Comparing `sqlconstructor-1.0.19/pyproject.toml` & `sqlconstructor-1.0.20/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlconstructor"
-version = "1.0.19"
+version = "1.0.20"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlconstructor-1.0.19/PKG-INFO` & `sqlconstructor-1.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlconstructor
-Version: 1.0.19
+Version: 1.0.20
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
 Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
 Project-URL: Telegram, https://t.me/sqlconstructor
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -51,19 +51,29 @@
 
 # build query into SqlContainer
 container: sc.SqlContainer = q()
 # get sql as string
 sql_text: str = str(container)
 ```
 ### Output
-SqlSection automatically transform all sql keywords in uppercase.
+**SqlSection** automatically transforms all sql keywords in uppercase. 
 It does not upper in following cases:
 - if sql keyword is located in inline/multiline comment.
 - if sql keyword is located inside single/double quotes.
 
+**SqlSection** automatically adds comma between provided sql statements in \_\_call\_\_ method for next headers:
+- SELECT
+- FROM
+- SET
+- VALUES
+- ORDER BY
+- GROUP BY
+- JSON_OBJECT_AGG
+- COALESCE
+
 Output of sql_text is
 ```sql
 SELECT
   id,
   name
 FROM
   product
```

