# Comparing `tmp/llm_friendly-0.1.0.tar.gz` & `tmp/llm_friendly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_friendly-0.1.0.tar", max compression
+gzip compressed data, was "llm_friendly-0.1.1.tar", max compression
```

## Comparing `llm_friendly-0.1.0.tar` & `llm_friendly-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      799 2023-08-02 03:31:49.324766 llm_friendly-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-02 03:01:08.001129 llm_friendly-0.1.0/llm_friendly/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 03:01:23.779526 llm_friendly-0.1.0/llm_friendly/aws/__init__.py
--rw-r--r--   0        0        0     2436 2023-07-28 07:57:16.478551 llm_friendly-0.1.0/llm_friendly/aws/table_parser.py
--rw-r--r--   0        0        0     2046 2023-08-02 03:37:16.710811 llm_friendly-0.1.0/llm_friendly/aws/textract.py
--rw-r--r--   0        0        0      385 2023-08-02 03:33:59.206099 llm_friendly-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 llm_friendly-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-08-07 04:19:13.872581 llm_friendly-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 03:01:08.001129 llm_friendly-0.1.1/llm_friendly/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:01:23.779526 llm_friendly-0.1.1/llm_friendly/aws/__init__.py
+-rw-r--r--   0        0        0     2383 2023-08-07 04:19:13.873492 llm_friendly-0.1.1/llm_friendly/aws/table_parser.py
+-rw-r--r--   0        0        0     3579 2023-08-07 04:19:13.874286 llm_friendly-0.1.1/llm_friendly/aws/textract.py
+-rw-r--r--   0        0        0      444 2023-08-07 04:19:13.896357 llm_friendly-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 llm_friendly-0.1.1/PKG-INFO
```

### Comparing `llm_friendly-0.1.0/llm_friendly/aws/table_parser.py` & `llm_friendly-0.1.1/llm_friendly/aws/table_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,19 +52,17 @@
 
     return _generate_table_csv(table_block, blocks_map, index)
 
 
 def _generate_table_csv(table_result: Dict[str, Any], blocks_map: Dict[str, Any], table_index=1):
     rows, scores = _get_rows_columns_map(table_result, blocks_map)
 
-    table_id = f'Table_{table_index}'
-
     # get cells.
-    csv = f'Table: {table_id}\n\n'
+    csv = ''
 
     for row_index, cols in rows.items():
         for col_index, text in cols.items():
-            csv += '{}'.format(text) + ","
+            csv += '{}'.format(text.strip()) + ","
         csv += '\n'
 
     csv += '\n\n\n'
     return csv
```

