# Comparing `tmp/NBRB-bki-xml-read-0.0.2.tar.gz` & `tmp/NBRB-bki-xml-read-0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NBRB-bki-xml-read-0.0.2.tar", last modified: Mon Aug  7 06:02:53 2023, max compression
+gzip compressed data, was "NBRB-bki-xml-read-0.0.post1.tar", last modified: Thu Jul 27 06:39:45 2023, max compression
```

## Comparing `NBRB-bki-xml-read-0.0.2.tar` & `NBRB-bki-xml-read-0.0.post1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 fedor     (1000) fedor     (1000)        0 2023-08-07 06:02:53.744199 NBRB-bki-xml-read-0.0.2/
-drwxrwxr-x   0 fedor     (1000) fedor     (1000)        0 2023-08-07 06:02:53.740198 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read/
--rw-rw-r--   0 fedor     (1000) fedor     (1000)        0 2023-07-26 15:31:01.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read/_init_.py
--rw-rw-r--   0 fedor     (1000) fedor     (1000)     2609 2023-08-03 09:16:10.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read/common_tools.py
--rw-rw-r--   0 fedor     (1000) fedor     (1000)     2107 2023-08-07 05:59:41.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read/individual_read.py
-drwxrwxr-x   0 fedor     (1000) fedor     (1000)        0 2023-08-07 06:02:53.744199 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read.egg-info/
--rw-rw-r--   0 fedor     (1000) fedor     (1000)      276 2023-08-07 06:02:53.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read.egg-info/PKG-INFO
--rw-rw-r--   0 fedor     (1000) fedor     (1000)      386 2023-08-07 06:02:53.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read.egg-info/SOURCES.txt
--rw-rw-r--   0 fedor     (1000) fedor     (1000)        1 2023-08-07 06:02:53.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read.egg-info/dependency_links.txt
--rw-rw-r--   0 fedor     (1000) fedor     (1000)        1 2023-07-27 06:22:42.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read.egg-info/not-zip-safe
--rw-rw-r--   0 fedor     (1000) fedor     (1000)       10 2023-08-07 06:02:53.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read.egg-info/requires.txt
--rw-rw-r--   0 fedor     (1000) fedor     (1000)       18 2023-08-07 06:02:53.000000 NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read.egg-info/top_level.txt
--rw-rw-r--   0 fedor     (1000) fedor     (1000)      276 2023-08-07 06:02:53.744199 NBRB-bki-xml-read-0.0.2/PKG-INFO
--rw-rw-r--   0 fedor     (1000) fedor     (1000)      192 2023-07-26 15:18:50.000000 NBRB-bki-xml-read-0.0.2/README.md
--rw-rw-r--   0 fedor     (1000) fedor     (1000)       90 2023-08-07 06:02:22.000000 NBRB-bki-xml-read-0.0.2/pyproject.toml
--rw-rw-r--   0 fedor     (1000) fedor     (1000)       78 2023-08-07 06:02:53.744199 NBRB-bki-xml-read-0.0.2/setup.cfg
--rw-rw-r--   0 fedor     (1000) fedor     (1000)      438 2023-08-07 06:00:26.000000 NBRB-bki-xml-read-0.0.2/setup.py
+drwxrwxr-x   0 fedor     (1000) fedor     (1000)        0 2023-07-27 06:39:45.517160 NBRB-bki-xml-read-0.0.post1/
+drwxrwxr-x   0 fedor     (1000) fedor     (1000)        0 2023-07-27 06:39:45.517160 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read/
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)        0 2023-07-26 15:31:01.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read/_init_.py
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)     1741 2023-07-27 05:50:41.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read/common_tools.py
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)      798 2023-07-27 05:50:06.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read/individual_read.py
+drwxrwxr-x   0 fedor     (1000) fedor     (1000)        0 2023-07-27 06:39:45.517160 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read.egg-info/
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)      280 2023-07-27 06:39:45.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read.egg-info/PKG-INFO
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)      386 2023-07-27 06:39:45.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read.egg-info/SOURCES.txt
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)        1 2023-07-27 06:39:45.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read.egg-info/dependency_links.txt
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)        1 2023-07-27 06:22:42.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read.egg-info/not-zip-safe
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)       10 2023-07-27 06:39:45.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read.egg-info/requires.txt
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)       18 2023-07-27 06:39:45.000000 NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read.egg-info/top_level.txt
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)      280 2023-07-27 06:39:45.517160 NBRB-bki-xml-read-0.0.post1/PKG-INFO
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)      192 2023-07-26 15:18:50.000000 NBRB-bki-xml-read-0.0.post1/README.md
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)       90 2023-07-27 06:39:14.000000 NBRB-bki-xml-read-0.0.post1/pyproject.toml
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)       78 2023-07-27 06:39:45.517160 NBRB-bki-xml-read-0.0.post1/setup.cfg
+-rw-rw-r--   0 fedor     (1000) fedor     (1000)      438 2023-07-27 06:39:01.000000 NBRB-bki-xml-read-0.0.post1/setup.py
```

### Comparing `NBRB-bki-xml-read-0.0.2/NBRB_bki_xml_read/common_tools.py` & `NBRB-bki-xml-read-0.0.post1/NBRB_bki_xml_read/common_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,67 @@
 import xmltodict
 
 def dict_from_xmlfile(filename):
     '''
         Get dictionary from filename.
-        Arguments
-        -------------
+        Args:
             filename : (str) path to the XML file to be read;
-        Returns
-        -------------
+        Return:
             (dict) with data;
     '''
     f = open(filename, "rb")
     data_dict = xmltodict.parse(f.read())
     f.close()
     return data_dict
 
 
-def recursive_dict_reader(my_dict, prev_pef_names = [], keys_separator = "/"):
+def recursive_dict_reader(my_dict, prev_pef_names = []):
     '''
         Recursive deployer of nested dictionaries 
         dictionaries into a single-level dictionary.
-
-        Arguments
-        ----------
-            my_dict : (dict) dictionary to be deployed;
-            prev_pef_names: (str) key paths of higher level dictionaries
-                            extremely important for recursion;
-            keys_separator: (str) describe symbols that will separate keys
-                            of input dictionaries in the result dictionary.
-        
-        Results
-        ---------
-            (dict) dictionary reduction of the input set of nested 
-                   dictionaries to a flat dictionary;
     '''
     res = {}
     
     for key, val in my_dict.items():
         curr_key_dict = prev_pef_names + [key]
         if type(val) == dict:
             res = {
                 **res,
                 **recursive_dict_reader(
-                    val, curr_key_dict,
-                    keys_separator = keys_separator
+                    val, curr_key_dict
                 )
             }
         else:
-            res[keys_separator.join(curr_key_dict)] = val
+            res["/".join(curr_key_dict)] = val
     return res
 
 
 def dict_reading_decorator(func):
     '''
         A decorator that checks if the searched key 
         is in the dictionary. Dictionary, if not, the 
         exception is triggered - an empty dictionary 
         is returned.
     '''
-    def wrapper(dict, **kwargs):
+    def wrapper(dict):
         try:
-            return func(dict, **kwargs)
+            return func(dict)
         except KeyError:
             return {}
     
     return wrapper
 
-def sub_dict_reader(my_dict, key_name, **kwargs):
+def dict_reader_wrapper(my_dict, key_name):
     '''
-        Arguments
-        -----------
-            my_dict : (dict) top-level dictionary;
-            key_name : (str) sub-dictionary key in the top-level dictionary;
-            kwargs : named arguments for recursive_dict_reader.
-            
-        Returns
-        ----------
-            (dict) Flat dictionary, created for the dictionary 
-                   under the key `key_name` in `my_dict`, 
-                   with all keys starting with `key_name`.
+        In order to quickly call
+        recursive_dict_reader for those cases
+        where the first level of the key is the same as
+        key of the expanded subdictionary.
+
+        Args:
+            my_dict - top-level dictionary;
+            key_name - sub-dictionary key in the top-level dictionary.
     '''
     return (
-        recursive_dict_reader(my_dict[key_name], [key_name], **kwargs)
+        recursive_dict_reader(my_dict[key_name], [key_name])
         if key_name in my_dict.keys() else {}
     )
```

