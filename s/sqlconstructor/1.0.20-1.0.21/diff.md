# Comparing `tmp/sqlconstructor-1.0.20.tar.gz` & `tmp/sqlconstructor-1.0.21.tar.gz`

## Comparing `sqlconstructor-1.0.20.tar` & `sqlconstructor-1.0.21.tar`

### file list

```diff
@@ -1,53 +1,58 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/pytest.ini
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/__init__.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/constants.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/helpers.py
--rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_container.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_cte.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_query.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/src/sqlconstructor/sql_section.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/simple_query_dict.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/expected_examples/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/expected_examples/select_section_of_simple_query.sql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/fixtures/expected_examples/simple_query.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/__init__.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_bool.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_container_filled_by_section_call.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_del_vars.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_init.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_json_variable.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_reset_vars.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_set_vars.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_unwrap.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_container/test_wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_call.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_clear.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_delitem.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_getitem.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_init.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_iter.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_pop.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_reg.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_cte/test_setitem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_add.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_bool.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_building_process.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_call.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_init.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_iter.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_len.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_query/test_sections_pop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_bool.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_call.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_init.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/tests/test_sql_section/test_upper_sql_keywords.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/LICENSE
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/pyproject.toml
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 sqlconstructor-1.0.20/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/pytest.ini
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/cols.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/constants.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/helpers.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/sql_container.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/sql_cte.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/sql_enum.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/sql_query.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/sql_section.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/src/sqlconstructor/vals.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/fixtures/simple_query_dict.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/fixtures/expected_examples/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/fixtures/expected_examples/select_section_of_simple_query.sql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/fixtures/expected_examples/simple_query.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/__init__.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_bool.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_container_filled_by_section_call.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_del_vars.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_init.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_json_variable.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_reset_vars.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_set_vars.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_unwrap.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_container/test_wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_call.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_clear.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_delitem.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_getitem.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_init.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_iter.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_pop.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_reg.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_cte/test_setitem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_add.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_bool.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_building_process.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_call.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_init.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_iter.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_len.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_sections_pop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_cases/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_query/test_cases/test_insert_into.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_section/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_section/test_bool.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_section/test_call.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_section/test_init.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/tests/test_sql_section/test_upper_sql_keywords.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/LICENSE
+-rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/pyproject.toml
+-rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 sqlconstructor-1.0.21/PKG-INFO
```

### Comparing `sqlconstructor-1.0.20/src/sqlconstructor/constants.py` & `sqlconstructor-1.0.21/src/sqlconstructor/constants.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/src/sqlconstructor/sql_cte.py` & `sqlconstructor-1.0.21/src/sqlconstructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/src/sqlconstructor/sql_query.py` & `sqlconstructor-1.0.21/src/sqlconstructor/sql_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     def __text(
         self,
         ind: int = 0,  # indentation
     ) -> str:
         """
         Used in __call__ method.
         Description:
-            - Build SQL text by SQL sections and return string (not SqlContainer!).
+          - Build SQL text by SQL sections and return string (not SqlContainer!).
         Params:
-            - ind: int - add additional indentation for each line of SQL query.
+          - ind: int - add additional indentation for each line of SQL query.
         """
         sections = [section.container for section in self.sections if section]
         query_text = '\n'.join(str(x) for x in sections) if sections else ''
         query_text = helpers.indent_lines(query_text, ind=ind)
         return query_text
```

### Comparing `sqlconstructor-1.0.20/src/sqlconstructor/sql_section.py` & `sqlconstructor-1.0.21/src/sqlconstructor/sql_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,62 +4,69 @@
 """
 
 from typing import Optional
 
 from . import helpers
 from .constants import SECTIONS_WITH_COMMA_SEPARATOR, SQL_KEYWORDS
 from .sql_container import SqlContainer
+from .sql_enum import SqlEnum
+from .cols import Cols
+from .vals import Vals
 
 
 class SqlSection:
-    """SqlSection is invented to build one SQL block of query and put the result of 
+    """SqlSection is invented to build one SQL block of query and put the result of
     this process to self.container which is SqlContainer instance.
     SQL block is build of:
         - section header provided of self.section_header
         - section body which consists of:
             *statements provided in self.__call__ method.
     """
 
     def __init__(self, section_header: str = ''):
         """Constract SqlSection instance.
         Params:
             - section_header: str - could be any string (empty is also possible).
-            If it be an empty string then there will be no section header in SQL block, 
-            and section body will be added without indentation. Otherwise section header 
+            If it be an empty string then there will be no section header in SQL block,
+            and section body will be added without indentation. Otherwise section header
             will be added, and section body starts with new line with 2 space indentation.
         """
         self.section_header: str = section_header
         self.container: Optional[SqlContainer] = None
 
     def __bool__(self) -> bool:
         """True if self.container is True"""
         return bool(self.container)
 
     def __call__(
         self,
-        *statements: str | SqlContainer,  # or any objects with __str__ method
+        *statements: str
+        | SqlContainer
+        | SqlEnum
+        | Cols
+        | Vals,  # or any objects with __str__ method
         sep: Optional[str] = None,
         line_end: str = '\n',
         section_end: str = '',
         ind: int = 2,  # indentation
         upper_keywords: bool = True,
     ) -> SqlContainer:
         """Process building SQL block and put result to self.container and return latter.
         Params:
             - *statements: Iterable[str | SqlContainer] - statements which go to section body.
-            - sep: Optional[str] - separator for statements. By default is empty string 
+            - sep: Optional[str] - separator for statements. By default is empty string
             for majority of cases and is comma for special type of statements described in
             SECTIONS_WITH_COMMA_SEPARATOR constant.
             - line_end: str: end of each line. It is '\n' by default.
             - section_end: str - end of SQL block created. It is empty string by default.
             - ind: int - indentation of each line of section body. If section header is not empty
-            string then each line of section body will be indented for 2 spaces. 
+            string then each line of section body will be indented for 2 spaces.
             No indentation overwise.
-            - upper_keywords: bool - do upper SQL keywords in section header and section body 
-            or do not. All SQL keywords are registered in SQL_KEYWORDS constant. 
+            - upper_keywords: bool - do upper SQL keywords in section header and section body
+            or do not. All SQL keywords are registered in SQL_KEYWORDS constant.
         """
         sep = (
             sep
             if sep is not None
             else ','
             if self.section_header.upper() in SECTIONS_WITH_COMMA_SEPARATOR
             else ''
```

### Comparing `sqlconstructor-1.0.20/tests/fixtures/simple_query_dict.py` & `sqlconstructor-1.0.21/tests/fixtures/simple_query_dict.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/fixtures/expected_examples/__init__.py` & `sqlconstructor-1.0.21/tests/fixtures/expected_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_container/test_bool.py` & `sqlconstructor-1.0.21/tests/test_sql_container/test_bool.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_container/test_del_vars.py` & `sqlconstructor-1.0.21/tests/test_sql_container/test_del_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_container/test_init.py` & `sqlconstructor-1.0.21/tests/test_sql_container/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_container/test_reset_vars.py` & `sqlconstructor-1.0.21/tests/test_sql_container/test_reset_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_container/test_set_vars.py` & `sqlconstructor-1.0.21/tests/test_sql_container/test_set_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_cte/test_call.py` & `sqlconstructor-1.0.21/tests/test_sql_cte/test_call.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_cte/test_iter.py` & `sqlconstructor-1.0.21/tests/test_sql_cte/test_iter.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_cte/test_pop.py` & `sqlconstructor-1.0.21/tests/test_sql_cte/test_pop.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_query/test_add.py` & `sqlconstructor-1.0.21/tests/test_sql_query/test_add.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_query/test_building_process.py` & `sqlconstructor-1.0.21/tests/test_sql_query/test_building_process.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_query/test_call.py` & `sqlconstructor-1.0.21/tests/test_sql_query/test_call.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_query/test_init.py` & `sqlconstructor-1.0.21/tests/test_sql_query/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_query/test_sections_pop.py` & `sqlconstructor-1.0.21/tests/test_sql_query/test_sections_pop.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/tests/test_sql_section/test_upper_sql_keywords.py` & `sqlconstructor-1.0.21/tests/test_sql_section/test_upper_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/LICENSE` & `sqlconstructor-1.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.20/README.md` & `sqlconstructor-1.0.21/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -357,14 +357,60 @@
     )
     ...
 
 
 def get_ctes() -> sc.SqlContainer:
     ...
 ```
+
+### Enumerate columns, values
+In release >= 1.0.21 you could enumerate columns and values a little bit easier:
+```python
+from sqlconstructor import SqlQuery, Cols, Vals
+
+
+q = SqlQuery()
+_uuid = uuid.uuid4()
+q['insert into'](
+    'product',
+    Cols(
+        'brand_id',
+        'name',
+        'quality',
+        'uuid',
+    ),
+)
+q['values'](
+    Vals(
+        1,
+        'phone',
+        _uuid,
+    )
+)
+sql_text = str(q())
+```
+
+sql_text output will be
+```sql
+INSERT INTO
+  product
+  (
+    "brand_id",
+    "name",
+    "quality",
+    "uuid"
+  )
+VALUES
+  (
+    1,
+    'phone',
+    '82611533-25c4-4cbd-8497-3f5024ca29a1'
+  )
+```
+
 ### Debugging
 
 #### How to find piece of code by produced sql
 If you would like to find your piece of code in editor by ready sql which is produced by sqlconstructor then you have to mark SqlQuery instances by 'sql_id' parameter in advance (before you have produced ready sql):
 ```python
 import sqlconstructor as sc
```

### Comparing `sqlconstructor-1.0.20/pyproject.toml` & `sqlconstructor-1.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlconstructor"
-version = "1.0.20"
+version = "1.0.21"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlconstructor-1.0.20/PKG-INFO` & `sqlconstructor-1.0.21/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlconstructor
-Version: 1.0.20
+Version: 1.0.21
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
 Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
 Project-URL: Telegram, https://t.me/sqlconstructor
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -372,14 +372,60 @@
     )
     ...
 
 
 def get_ctes() -> sc.SqlContainer:
     ...
 ```
+
+### Enumerate columns, values
+In release >= 1.0.21 you could enumerate columns and values a little bit easier:
+```python
+from sqlconstructor import SqlQuery, Cols, Vals
+
+
+q = SqlQuery()
+_uuid = uuid.uuid4()
+q['insert into'](
+    'product',
+    Cols(
+        'brand_id',
+        'name',
+        'quality',
+        'uuid',
+    ),
+)
+q['values'](
+    Vals(
+        1,
+        'phone',
+        _uuid,
+    )
+)
+sql_text = str(q())
+```
+
+sql_text output will be
+```sql
+INSERT INTO
+  product
+  (
+    "brand_id",
+    "name",
+    "quality",
+    "uuid"
+  )
+VALUES
+  (
+    1,
+    'phone',
+    '82611533-25c4-4cbd-8497-3f5024ca29a1'
+  )
+```
+
 ### Debugging
 
 #### How to find piece of code by produced sql
 If you would like to find your piece of code in editor by ready sql which is produced by sqlconstructor then you have to mark SqlQuery instances by 'sql_id' parameter in advance (before you have produced ready sql):
 ```python
 import sqlconstructor as sc
```

