# Comparing `tmp/sqlconstructor-1.0.22.tar.gz` & `tmp/sqlconstructor-1.0.23.tar.gz`

## Comparing `sqlconstructor-1.0.22.tar` & `sqlconstructor-1.0.23.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/pytest.ini
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/cols.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/constants.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/helpers.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/sql_container.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/sql_cte.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/sql_enum.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/sql_query.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/sql_section.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/src/sqlconstructor/vals.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/fixtures/simple_query_dict.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/fixtures/expected_examples/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/fixtures/expected_examples/select_section_of_simple_query.sql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/fixtures/expected_examples/simple_query.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/__init__.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_bool.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_container_filled_by_section_call.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_del_vars.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_init.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_json_variable.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_reset_vars.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_set_vars.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_unwrap.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_container/test_wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_call.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_clear.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_delitem.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_getitem.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_init.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_iter.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_pop.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_reg.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_cte/test_setitem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_add.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_bool.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_building_process.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_call.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_init.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_iter.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_len.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_sections_pop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_cases/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_query/test_cases/test_insert_into.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_section/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_section/test_bool.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_section/test_call.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_section/test_init.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/tests/test_sql_section/test_upper_sql_keywords.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/LICENSE
--rw-r--r--   0        0        0     9805 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/pyproject.toml
--rw-r--r--   0        0        0    10606 2020-02-02 00:00:00.000000 sqlconstructor-1.0.22/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/pytest.ini
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/cols.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/constants.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/helpers.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/sql_container.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/sql_cte.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/sql_enum.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/sql_query.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/sql_section.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/src/sqlconstructor/vals.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/fixtures/simple_query_dict.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/fixtures/expected_examples/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/fixtures/expected_examples/select_section_of_simple_query.sql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/fixtures/expected_examples/simple_query.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/__init__.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_bool.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_container_filled_by_section_call.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_del_vars.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_init.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_json_variable.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_reset_vars.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_set_vars.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_unwrap.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_container/test_wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_call.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_clear.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_delitem.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_getitem.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_init.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_iter.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_pop.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_reg.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_cte/test_setitem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_add.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_bool.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_building_process.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_call.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_init.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_iter.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_len.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_sections_pop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_cases/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_query/test_cases/test_insert_into.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_section/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_section/test_bool.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_section/test_call.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_section/test_init.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/tests/test_sql_section/test_upper_sql_keywords.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/LICENSE
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/pyproject.toml
+-rw-r--r--   0        0        0    10618 2020-02-02 00:00:00.000000 sqlconstructor-1.0.23/PKG-INFO
```

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/cols.py` & `sqlconstructor-1.0.23/src/sqlconstructor/cols.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/constants.py` & `sqlconstructor-1.0.23/src/sqlconstructor/constants.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/helpers.py` & `sqlconstructor-1.0.23/src/sqlconstructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/sql_container.py` & `sqlconstructor-1.0.23/src/sqlconstructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/sql_cte.py` & `sqlconstructor-1.0.23/src/sqlconstructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/sql_enum.py` & `sqlconstructor-1.0.23/src/sqlconstructor/sql_enum.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/sql_query.py` & `sqlconstructor-1.0.23/src/sqlconstructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/sql_section.py` & `sqlconstructor-1.0.23/src/sqlconstructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/src/sqlconstructor/vals.py` & `sqlconstructor-1.0.23/src/sqlconstructor/vals.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/fixtures/simple_query_dict.py` & `sqlconstructor-1.0.23/tests/fixtures/simple_query_dict.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/fixtures/expected_examples/__init__.py` & `sqlconstructor-1.0.23/tests/fixtures/expected_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_container/test_bool.py` & `sqlconstructor-1.0.23/tests/test_sql_container/test_bool.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_container/test_del_vars.py` & `sqlconstructor-1.0.23/tests/test_sql_container/test_del_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_container/test_init.py` & `sqlconstructor-1.0.23/tests/test_sql_container/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_container/test_reset_vars.py` & `sqlconstructor-1.0.23/tests/test_sql_container/test_reset_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_container/test_set_vars.py` & `sqlconstructor-1.0.23/tests/test_sql_container/test_set_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_cte/test_call.py` & `sqlconstructor-1.0.23/tests/test_sql_cte/test_call.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_cte/test_iter.py` & `sqlconstructor-1.0.23/tests/test_sql_cte/test_iter.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_cte/test_pop.py` & `sqlconstructor-1.0.23/tests/test_sql_cte/test_pop.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_query/test_add.py` & `sqlconstructor-1.0.23/tests/test_sql_query/test_add.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_query/test_building_process.py` & `sqlconstructor-1.0.23/tests/test_sql_query/test_building_process.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_query/test_call.py` & `sqlconstructor-1.0.23/tests/test_sql_query/test_call.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_query/test_init.py` & `sqlconstructor-1.0.23/tests/test_sql_query/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_query/test_sections_pop.py` & `sqlconstructor-1.0.23/tests/test_sql_query/test_sections_pop.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_query/test_cases/test_insert_into.py` & `sqlconstructor-1.0.23/tests/test_sql_query/test_cases/test_insert_into.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_section/test_init.py` & `sqlconstructor-1.0.23/tests/test_sql_section/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/tests/test_sql_section/test_upper_sql_keywords.py` & `sqlconstructor-1.0.23/tests/test_sql_section/test_upper_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/LICENSE` & `sqlconstructor-1.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.22/README.md` & `sqlconstructor-1.0.23/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -361,14 +361,15 @@
 def get_ctes() -> sc.SqlContainer:
     ...
 ```
 
 ### Enumerate columns, values
 In release >= 1.0.21 you could enumerate columns and values a little bit easier:
 ```python
+import uuid
 from sqlconstructor import SqlQuery, Cols, Vals
 
 
 q = SqlQuery()
 _uuid = uuid.uuid4()
 q['insert into'](
     'product',
```

### Comparing `sqlconstructor-1.0.22/pyproject.toml` & `sqlconstructor-1.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlconstructor"
-version = "1.0.22"
+version = "1.0.23"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlconstructor-1.0.22/PKG-INFO` & `sqlconstructor-1.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlconstructor
-Version: 1.0.22
+Version: 1.0.23
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
 Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
 Project-URL: Telegram, https://t.me/sqlconstructor
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -376,14 +376,15 @@
 def get_ctes() -> sc.SqlContainer:
     ...
 ```
 
 ### Enumerate columns, values
 In release >= 1.0.21 you could enumerate columns and values a little bit easier:
 ```python
+import uuid
 from sqlconstructor import SqlQuery, Cols, Vals
 
 
 q = SqlQuery()
 _uuid = uuid.uuid4()
 q['insert into'](
     'product',
```

