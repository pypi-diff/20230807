# Comparing `tmp/lessweb-commondao-1.0.4.tar.gz` & `tmp/lessweb-commondao-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-commondao-1.0.4.tar", last modified: Sat Jan 14 08:20:10 2023, max compression
+gzip compressed data, was "lessweb-commondao-1.0.6.tar", last modified: Mon Aug  7 13:28:48 2023, max compression
```

## Comparing `lessweb-commondao-1.0.4.tar` & `lessweb-commondao-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-01-14 08:20:10.415624 lessweb-commondao-1.0.4/
--rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-commondao-1.0.4/LICENSE.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-01-14 08:16:39.000000 lessweb-commondao-1.0.4/MANIFEST.in
--rw-r--r--   0 zhangji    (501) staff       (20)      386 2023-01-14 08:20:10.413936 lessweb-commondao-1.0.4/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)      327 2022-11-15 08:14:49.000000 lessweb-commondao-1.0.4/README.md
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-01-14 08:20:10.392904 lessweb-commondao-1.0.4/commondao/
--rw-r--r--   0 zhangji    (501) staff       (20)       22 2023-01-14 08:19:38.000000 lessweb-commondao-1.0.4/commondao/__init__.py
--rw-r--r--   0 zhangji    (501) staff       (20)       65 2022-11-15 08:18:30.000000 lessweb-commondao-1.0.4/commondao/__main__.py
--rw-r--r--   0 zhangji    (501) staff       (20)     2421 2022-11-15 08:21:15.000000 lessweb-commondao-1.0.4/commondao/codegen.py
--rw-r--r--   0 zhangji    (501) staff       (20)      233 2022-11-15 09:15:15.000000 lessweb-commondao-1.0.4/commondao/index.py
--rw-r--r--   0 zhangji    (501) staff       (20)     7998 2023-01-09 09:02:00.000000 lessweb-commondao-1.0.4/commondao/mapper.py
--rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-commondao-1.0.4/commondao/py.typed
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-01-14 08:20:10.403754 lessweb-commondao-1.0.4/commondao/utils/
--rw-r--r--   0 zhangji    (501) staff       (20)        0 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.4/commondao/utils/__init__.py
--rw-r--r--   0 zhangji    (501) staff       (20)     1790 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.4/commondao/utils/common.py
--rw-r--r--   0 zhangji    (501) staff       (20)     1597 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.4/commondao/utils/grammar.py
--rw-r--r--   0 zhangji    (501) staff       (20)     3027 2023-01-14 06:59:49.000000 lessweb-commondao-1.0.4/commondao/utils/templates.py
--rw-r--r--   0 zhangji    (501) staff       (20)     3375 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.4/commondao/utils/wordstyle.py
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-01-14 08:20:10.413026 lessweb-commondao-1.0.4/lessweb_commondao.egg-info/
--rw-r--r--   0 zhangji    (501) staff       (20)      386 2023-01-14 08:20:10.000000 lessweb-commondao-1.0.4/lessweb_commondao.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)      552 2023-01-14 08:20:10.000000 lessweb-commondao-1.0.4/lessweb_commondao.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-01-14 08:20:10.000000 lessweb-commondao-1.0.4/lessweb_commondao.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       52 2023-01-14 08:20:10.000000 lessweb-commondao-1.0.4/lessweb_commondao.egg-info/entry_points.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       49 2023-01-14 08:20:10.000000 lessweb-commondao-1.0.4/lessweb_commondao.egg-info/requires.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       10 2023-01-14 08:20:10.000000 lessweb-commondao-1.0.4/lessweb_commondao.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-01-14 08:20:10.416101 lessweb-commondao-1.0.4/setup.cfg
--rw-r--r--   0 zhangji    (501) staff       (20)     1232 2023-01-14 07:49:03.000000 lessweb-commondao-1.0.4/setup.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-08-07 13:28:48.085704 lessweb-commondao-1.0.6/
+-rw-r--r--   0 zhangji    (501) staff       (20)     1085 2020-02-08 04:12:40.000000 lessweb-commondao-1.0.6/.gitignore
+-rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-commondao-1.0.6/LICENSE.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)      563 2023-08-07 13:28:48.084527 lessweb-commondao-1.0.6/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)      278 2023-08-07 11:47:31.000000 lessweb-commondao-1.0.6/README.md
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-08-07 13:28:48.072829 lessweb-commondao-1.0.6/commondao/
+-rw-r--r--   0 zhangji    (501) staff       (20)       22 2023-08-07 13:27:25.000000 lessweb-commondao-1.0.6/commondao/__init__.py
+-rw-r--r--   0 zhangji    (501) staff       (20)       65 2022-11-15 08:18:30.000000 lessweb-commondao-1.0.6/commondao/__main__.py
+-rw-r--r--   0 zhangji    (501) staff       (20)     2617 2023-04-05 15:17:24.000000 lessweb-commondao-1.0.6/commondao/codegen.py
+-rw-r--r--   0 zhangji    (501) staff       (20)      233 2022-11-15 09:15:15.000000 lessweb-commondao-1.0.6/commondao/index.py
+-rw-r--r--   0 zhangji    (501) staff       (20)     8337 2023-08-07 12:09:28.000000 lessweb-commondao-1.0.6/commondao/mapper.py
+-rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-commondao-1.0.6/commondao/py.typed
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-08-07 13:28:48.076637 lessweb-commondao-1.0.6/commondao/utils/
+-rw-r--r--   0 zhangji    (501) staff       (20)        0 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.6/commondao/utils/__init__.py
+-rw-r--r--   0 zhangji    (501) staff       (20)     1790 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.6/commondao/utils/common.py
+-rw-r--r--   0 zhangji    (501) staff       (20)     1597 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.6/commondao/utils/grammar.py
+-rw-r--r--   0 zhangji    (501) staff       (20)     3027 2023-01-14 06:59:49.000000 lessweb-commondao-1.0.6/commondao/utils/templates.py
+-rw-r--r--   0 zhangji    (501) staff       (20)     3375 2022-07-31 15:36:11.000000 lessweb-commondao-1.0.6/commondao/utils/wordstyle.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-08-07 13:28:48.082641 lessweb-commondao-1.0.6/lessweb_commondao.egg-info/
+-rw-r--r--   0 zhangji    (501) staff       (20)      563 2023-08-07 13:28:47.000000 lessweb-commondao-1.0.6/lessweb_commondao.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)      557 2023-08-07 13:28:48.000000 lessweb-commondao-1.0.6/lessweb_commondao.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-08-07 13:28:47.000000 lessweb-commondao-1.0.6/lessweb_commondao.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       51 2023-08-07 13:28:47.000000 lessweb-commondao-1.0.6/lessweb_commondao.egg-info/entry_points.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       49 2023-08-07 13:28:47.000000 lessweb-commondao-1.0.6/lessweb_commondao.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       10 2023-08-07 13:28:47.000000 lessweb-commondao-1.0.6/lessweb_commondao.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)      544 2023-08-07 13:22:07.000000 lessweb-commondao-1.0.6/pyproject.toml
+-rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-08-07 13:28:48.086137 lessweb-commondao-1.0.6/setup.cfg
```

### Comparing `lessweb-commondao-1.0.4/LICENSE.txt` & `lessweb-commondao-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-commondao-1.0.4/commondao/codegen.py` & `lessweb-commondao-1.0.6/commondao/codegen.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import os
 from pathlib import Path
 import re
 from commondao.utils.templates import render_class_frame, render_class_methods
 from commondao.utils.grammar import is_column_sql, parse_column_sql, guess_py_type, is_unique_key_sql, parse_unique_key_sql
 
 
-def parse_create_table_sql(sql_content):
+def parse_create_table_sql(sql_content, entity_filename):
     """
     :return 形如table_name, col_items, unique_keys
        * col_items: dict[name, (py_type, comment)]
        * unique_keys: list[list[str]]
     """
     col_items = {}
     unique_keys = []
     seed = re.compile(r'CREATE TABLE *`?(\w+)`? *\((.*)\)',
                       flags=re.I | re.DOTALL)
     match_size = len(find_ret := seed.findall(sql_content))
-    assert match_size == 1, 'cannot parse the create table SQL'
+    assert match_size != 0, f'cannot parse the create table SQL (No "CREATE TABLE ..." in {entity_filename})'
+    assert match_size == 1, f'cannot parse the create table SQL (Too many "CREATE TABLE ..." in {entity_filename})'
     table_name, sql_body = find_ret[0]
     for sql_line in sql_body.splitlines():
         if sql_line and is_column_sql(sql_line):
             col_name, sql_type, comment = parse_column_sql(sql_line)
             py_type = guess_py_type(sql_type)
             col_items[col_name] = py_type, comment
         elif sql_line and is_unique_key_sql(sql_line):
@@ -45,15 +46,15 @@
     class_body_blocks = []
     entity_filenames = os.listdir(schemadir)
     schema_path = Path(schemadir)
     for entity_filename in entity_filenames:
         entity_name = entity_filename.split('.', 1)[0]
         sql_content = (schema_path / entity_filename).open().read()
         table_name, col_items, unique_keys = parse_create_table_sql(
-            sql_content)
+            sql_content, entity_filename)
         class_methods = render_class_methods(table_name, entity_name,
                                              col_items, unique_keys)
         class_body_blocks.append(class_methods)
     class_body = ''.join(class_body_blocks)
     class_frame = render_class_frame(class_body)
     with open(outfile, 'w') as fout:
         fout.write(class_frame)
```

### Comparing `lessweb-commondao-1.0.4/commondao/mapper.py` & `lessweb-commondao-1.0.6/commondao/mapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,27 @@
 T = TypeVar('T')
 
 SELECT_ONE = 1
 SELECT_ALL = 2
 EXECUTE = 3
 
 
+FILTER_MAP = {
+    'eq': '`<field>`=:<field>.value',  # eq是默认的filter，可以省略
+    'like': "`<field>` like :<field>.value",
+    'between': '`<field>` between :<field>.value and :<field>.end',
+    'ne': '`<field>` <> :<field>.value',
+    'lt': '`<field>` < :<field>.value',
+    'gt': '`<field>` > :<field>.value',
+    'lte': '`<field>` <= :<field>.value',
+    'gte': '`<field>` >= :<field>.value',
+    'in': '`<field>` in :<field>.value',
+}
+
+
 @service
 class Mysql:
     app: Application
     pool: Pool
 
     def __init__(self, app: Application):
         self.app = app
@@ -72,45 +85,46 @@
 
 
 def make_sub_clause(query) -> tuple:
     """
     query: Dict | MutableMapping
     return: (value_map, limit_map, where_clause, order_clause, limit_clause)
     """
-    eq_filter = '`<field>`=:<field>.value'
     filter_map = {}  # filter_map[query_key] = filter
-    limit_map = {'limit': 1000}
+    limit_map = {'limit': 0}
     orderby_rules = []
     value_map = {}
     for query_key, query_val in query.items():
         if query_key == 'limit':
             limit_map['limit'] = int(query_val)
         elif query_key == 'offset':
-            limit_map['offset'] = int(
-                query_val
-            )  # todo 如果传入的limit=0，则只查询总数；否则正常分页查询。如果不传limit则默认1000。
+            limit_map['offset'] = int(query_val)
+        elif query_key == 'order':
+            orderby_rules.extend(
+                (f'{k[1:]} desc' if k.startswith('-') else k) 
+                for k in query_val.split(',') if re.match(r'-?[\w]+', k)
+            )
         elif '.' not in query_key:
-            filter_map.setdefault(query_key, eq_filter.replace('<field>', query_key))
+            filter_map.setdefault(query_key, 'eq')
             value_map[f'{query_key}.value'] = query_val
         elif query_key.endswith('.value'):
-            filter_map.setdefault(query_key[:-6], eq_filter.replace('<field>', query_key[:-6]))
+            filter_map.setdefault(query_key[:-6], 'eq')
             value_map[query_key] = query_val
         elif query_key.endswith('.filter'):
-            filter_map[query_key[:-7]] = query_val.replace('<field>', query_key[:-7])
-        elif query_key.endswith('.order'):
-            assert query_val in 'asc' or query_val in 'desc'
-            orderby_rules.append(query_key[:-6] + ' ' + query_val)
+            assert query_val in FILTER_MAP
+            filter_map[query_key[:-7]] = query_val
         else:
             value_map[query_key] = query_val
     where_clause = ''
     order_clause = ', '.join(orderby_rules)
     limit_clause = 'limit %d' % int(limit_map['limit'])
-    for filter_val in filter_map.values():
+    for field_name, filter_val in filter_map.items():
+        filter_text = FILTER_MAP[filter_val].replace('<field>', field_name)
         where_clause += ('WHERE' if not where_clause else 'AND')\
-                        + f' ({filter_val}) '
+                        + f' ({filter_text}) '
     if 'offset' in limit_map:
         limit_clause += ' offset %d' % int(limit_map['offset'])
     return value_map, limit_map, where_clause, order_clause, limit_clause
 
 
 @service
 class Mapper:
@@ -127,15 +141,15 @@
         logging.debug(sql)
         pg_sql, pg_params = RegexCollect().build(sql, data)
         logging.debug('%s => %s', pg_sql, pg_params)
         await cursor.execute(pg_sql, pg_params)
         if mode == SELECT_ONE:
             return await cursor.fetchone() or {}
         elif mode == SELECT_ALL:
-            return await cursor.fetchall()
+            return await cursor.fetchall() or []
         else:
             return cursor.rowcount
 
     async def select_one(self, sql: str, data: dict):
         return await self.execute(SELECT_ONE, sql, data)
 
     async def select_all(self, sql: str, data: dict):
```

### Comparing `lessweb-commondao-1.0.4/commondao/utils/common.py` & `lessweb-commondao-1.0.6/commondao/utils/common.py`

 * *Files identical despite different names*

### Comparing `lessweb-commondao-1.0.4/commondao/utils/grammar.py` & `lessweb-commondao-1.0.6/commondao/utils/grammar.py`

 * *Files identical despite different names*

### Comparing `lessweb-commondao-1.0.4/commondao/utils/templates.py` & `lessweb-commondao-1.0.6/commondao/utils/templates.py`

 * *Files identical despite different names*

### Comparing `lessweb-commondao-1.0.4/commondao/utils/wordstyle.py` & `lessweb-commondao-1.0.6/commondao/utils/wordstyle.py`

 * *Files identical despite different names*

### Comparing `lessweb-commondao-1.0.4/lessweb_commondao.egg-info/SOURCES.txt` & `lessweb-commondao-1.0.6/lessweb_commondao.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+.gitignore
 LICENSE.txt
-MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 commondao/__init__.py
 commondao/__main__.py
 commondao/codegen.py
 commondao/index.py
 commondao/mapper.py
 commondao/py.typed
 commondao/utils/__init__.py
```

