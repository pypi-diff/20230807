# Comparing `tmp/juno-ai-0.0.7.tar.gz` & `tmp/juno-ai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juno-ai-0.0.7.tar", last modified: Sun Jun  4 15:49:27 2023, max compression
+gzip compressed data, was "juno-ai-0.0.8.tar", last modified: Mon Aug  7 17:37:34 2023, max compression
```

## Comparing `juno-ai-0.0.7.tar` & `juno-ai-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.249196 juno-ai-0.0.7/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-06-04 15:49:27.248873 juno-ai-0.0.7/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1938 2023-05-26 07:12:21.000000 juno-ai-0.0.7/README.md
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.246071 juno-ai-0.0.7/juno/
--rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.7/juno/__init__.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1002 2023-05-24 08:38:40.000000 juno-ai-0.0.7/juno/agent_injection.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.7/juno/client_setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1916 2023-05-26 07:12:21.000000 juno-ai-0.0.7/juno/event_javascript.py
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.246666 juno-ai-0.0.7/juno/js/
--rw-r--r--   0 alexirobbins   (501) staff       (20)    15808 2023-06-04 15:46:16.000000 juno-ai-0.0.7/juno/js/juno.min.js
--rw-r--r--   0 alexirobbins   (501) staff       (20)     2723 2023-05-24 08:38:40.000000 juno-ai-0.0.7/juno/juno.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1984 2023-05-11 01:35:57.000000 juno-ai-0.0.7/juno/magic.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.7/juno/output_parser.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)    14065 2023-06-04 15:46:04.000000 juno-ai-0.0.7/juno/prompting_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     4685 2023-04-26 23:26:15.000000 juno-ai-0.0.7/juno/serialize_context.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-05-26 07:12:21.000000 juno-ai-0.0.7/juno/version.py
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.248507 juno-ai-0.0.7/juno_ai.egg-info/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)      399 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/SOURCES.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/dependency_links.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       53 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/requires.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/top_level.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-06-04 15:49:27.249282 juno-ai-0.0.7/setup.cfg
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1322 2023-06-04 15:46:04.000000 juno-ai-0.0.7/setup.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-08-07 17:37:34.695507 juno-ai-0.0.8/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-08-07 17:37:34.695232 juno-ai-0.0.8/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     2163 2023-08-07 17:20:35.000000 juno-ai-0.0.8/README.md
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-08-07 17:37:34.692474 juno-ai-0.0.8/juno/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.8/juno/__init__.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1002 2023-05-24 08:38:40.000000 juno-ai-0.0.8/juno/agent_injection.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.8/juno/client_setup.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1916 2023-05-26 07:12:21.000000 juno-ai-0.0.8/juno/event_javascript.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-08-07 17:37:34.693198 juno-ai-0.0.8/juno/js/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    15808 2023-08-07 17:23:19.000000 juno-ai-0.0.8/juno/js/juno.min.js
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     2723 2023-05-24 08:38:40.000000 juno-ai-0.0.8/juno/juno.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1984 2023-05-11 01:35:57.000000 juno-ai-0.0.8/juno/magic.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.8/juno/output_parser.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    14065 2023-06-04 15:46:04.000000 juno-ai-0.0.8/juno/prompting_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     5060 2023-08-07 17:20:35.000000 juno-ai-0.0.8/juno/serialize_context.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-05-26 07:12:21.000000 juno-ai-0.0.8/juno/version.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-08-07 17:37:34.694845 juno-ai-0.0.8/juno_ai.egg-info/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-08-07 17:37:34.000000 juno-ai-0.0.8/juno_ai.egg-info/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      399 2023-08-07 17:37:34.000000 juno-ai-0.0.8/juno_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-08-07 17:37:34.000000 juno-ai-0.0.8/juno_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       53 2023-08-07 17:37:34.000000 juno-ai-0.0.8/juno_ai.egg-info/requires.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-08-07 17:37:34.000000 juno-ai-0.0.8/juno_ai.egg-info/top_level.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-08-07 17:37:34.695586 juno-ai-0.0.8/setup.cfg
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1322 2023-08-07 17:23:19.000000 juno-ai-0.0.8/setup.py
```

### Comparing `juno-ai-0.0.7/PKG-INFO` & `juno-ai-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.7/README.md` & `juno-ai-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 ## Getting Started Guide
 
 To use Juno, you need to install the Juno package.
 ```bash
 pip install juno-ai
 ```
 
-Then, load the extension in your Jupyter notebook.
+Or you can also install directly from your Jupyter notebook.
+```bash
+%pip install juno-ai
+```
+
+### Load the extension
+
+Load the extension into your current Jupyter notebook. 
 ```python
 %load_ext juno
 ```
 
+> For those new to Jupyter extensions, note you must load the extension at the top of each notebook.
+
 ## Using Juno
 
 You can ask Juno to write code for you by running `%juno` followed by your prompt in a cell.
 
 It can write functions, create plots, or do data analysis in pandas.
 It knows about the variables you have defined in your notebook, so you ask it to work with your data without giving additional context.
 
@@ -47,8 +56,8 @@
 # sample a random number from 1-100
 random_number = random.randint(1, 100)
 random_number
 ```
 
 Finally, you can also use Juno to help debug errors in your code. Anytime you run into an exception in your Jupyter notebook, a `Debug` button will appear. When you click it, Juno will take a look at your error and try to fix it in a new cell.
 
-Thanks for trying Juno! If you have any questions or feedback, please reach out to us at hellojunoai@gmail.com
+Thanks for trying Juno! If you have any questions or feedback, please reach out to us at hellojunoai@gmail.com
```

### Comparing `juno-ai-0.0.7/juno/agent_injection.py` & `juno-ai-0.0.8/juno/agent_injection.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/client_setup.py` & `juno-ai-0.0.8/juno/client_setup.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/event_javascript.py` & `juno-ai-0.0.8/juno/event_javascript.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/js/juno.min.js` & `juno-ai-0.0.8/juno/js/juno.min.js`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/juno.py` & `juno-ai-0.0.8/juno/juno.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/magic.py` & `juno-ai-0.0.8/juno/magic.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/output_parser.py` & `juno-ai-0.0.8/juno/output_parser.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/prompting_javascript.py` & `juno-ai-0.0.8/juno/prompting_javascript.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.7/juno/serialize_context.py` & `juno-ai-0.0.8/juno/serialize_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,43 +8,56 @@
 
 phone_pattern = r"(\+\d{1,2}\s?)?1?\-?\.?\s?\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}"
 physical_address_pattern = r"\b(\d{1,6}\s([a-zA-z\.\s\-]+\s){0,3}([a-zA-z0-9\s]+[a-zA-Z\.])([\,\s]{0,2})?(road|street|avenue|boulevard|lane|drive|way|court|plaza|terrace|colony|close)[\,\s]{1,2}((Apt|Apartment|Floor|Suite|House)[\s\:]{1,2}\d{0,6}[\,\s]{1,2})?(([a-zA-Z]+[\s\-]?){1,4})?([\,\s]{0,2})?([A-Za-z]{2}|[a-zA-Z]+[\s\-])?([\,\s]{0,2}([0-9\-]{1,10})|[A-Z0-9]{3}\s[A-Z0-9]{3})?)\b"
 
 def set_values_enabled(enabled):
     global VALUES_ENABLED
     VALUES_ENABLED = enabled
-    
+
+def sample_values(df, column, n=3) -> list:
+    """Randomly sample n values from a dataframe column"""
+    return [truncate_value(v) for v in df[column].sample(n).tolist()]
+
 def filter_dataframe_pii(df, column) -> list:
-    first_three_values = [truncate_value(v) for v in df[column].head(3).tolist()]
-    for i, value in enumerate(first_three_values):
+    values = sample_values(df, column)
+    for i, value in enumerate(values):
         if isinstance(value, str):
             if validators.uuid(value) and ('id' in column or 'user' in column):
-                    first_three_values[i] = '(uuid)'
+                values[i] = '(uuid)'
             elif validators.email(value):
-                first_three_values[i] = '(email)'
+                values[i] = '(email)'
             elif validators.ip_address.ipv4(value) or validators.ip_address.ipv6(value):
-                first_three_values[i] = '(ip_address)'
+                values[i] = '(ip_address)'
             elif validators.card.card_number(value):
-                first_three_values[i] = '(card_number)'
+                values[i] = '(card_number)'
             elif re.match(phone_pattern, value):
-                first_three_values[i] = '(phone)'
+                values[i] = '(phone)'
             elif re.match(physical_address_pattern, value):
-                first_three_values[i] = '(address)'
-    return first_three_values
+                values[i] = '(address)'
+    return values
+
+def get_col_description(df, column, max_length=50) -> str:
+    is_index = column == df.index.name
+    dtype = df[column].dtype
+    if VALUES_ENABLED:
+        values = filter_dataframe_pii(df, column)
+        return f"{column}, index: {is_index}, dtype: {dtype}. Sample of values: {values}"
+    else:
+        return f"{column}, index: {is_index}, dtype: {dtype}."
     
 def describe_dataframe(df, max_cols=20) -> str:
     description = []
-    for column in df.columns[:max_cols]:
-        is_index = column == df.index.name
-        dtype = df[column].dtype
-        if VALUES_ENABLED:
-            first_three_values = filter_dataframe_pii(df, column)
-            description.append(f"{column}, index: {is_index}, dtype: {dtype}. First three values: {first_three_values}")
-        else:
-            description.append(f"{column}, index: {is_index}, dtype: {dtype}.")
+    if len(df.columns) > max_cols:
+        for column in df.columns[:max_cols-1]: 
+            description.append(get_col_description(df, column))
+        description.append(f"... {len(df.columns) - max_cols + 1} more columns...")
+        description.append(get_col_description(df,  df.columns[-1]))
+    else:
+        for column in df.columns: 
+            description.append(get_col_description(df, column))
     full_description = "\n".join(description)
     shape_description = f"Shape: {df.shape}"
     return shape_description + '\nColumns:\n' + full_description
 
 def describe_list(lst, max_length=50) -> str:
     if VALUES_ENABLED:
         truncated_list = list(lst)[:3]
```

### Comparing `juno-ai-0.0.7/juno_ai.egg-info/PKG-INFO` & `juno-ai-0.0.8/juno_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.7/setup.py` & `juno-ai-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # exec(open(read('juno/version.py')).read())
 print('packages:', [package for package in find_packages()
                 if package.startswith('juno')])
 setup(
     name='juno-ai', 
     # version=__version__, 
-    version='0.0.7',
+    version='0.0.8',
     packages=[package for package in find_packages()
                 if package.startswith('juno')], 
     package_data={'': ['js/juno.min.js']},
     include_package_data=True,
     long_description='Juno AI Assistant for Jupyter Notebook',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
```

