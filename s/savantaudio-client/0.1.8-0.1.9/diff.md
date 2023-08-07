# Comparing `tmp/savantaudio-client-0.1.8.tar.gz` & `tmp/savantaudio-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "savantaudio-client-0.1.8.tar", last modified: Thu Sep 15 15:27:38 2022, max compression
+gzip compressed data, was "savantaudio-client-0.1.9.tar", last modified: Thu Sep 15 16:54:15 2022, max compression
```

## Comparing `savantaudio-client-0.1.8.tar` & `savantaudio-client-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-15 15:27:38.317871 savantaudio-client-0.1.8/
--rw-r--r--   0 adam       (501) staff       (20)      547 2022-09-09 15:22:34.000000 savantaudio-client-0.1.8/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)     1838 2022-09-15 15:27:38.317930 savantaudio-client-0.1.8/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1259 2022-09-09 16:59:56.000000 savantaudio-client-0.1.8/README.md
--rw-r--r--   0 adam       (501) staff       (20)       91 2022-09-09 15:40:13.000000 savantaudio-client-0.1.8/pyproject.toml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-15 15:27:38.317089 savantaudio-client-0.1.8/savantaudio/
--rw-r--r--   0 adam       (501) staff       (20)      120 2022-01-20 21:30:52.000000 savantaudio-client-0.1.8/savantaudio/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)      388 2022-09-15 15:27:11.000000 savantaudio-client-0.1.8/savantaudio/__version__.py
--rw-r--r--   0 adam       (501) staff       (20)    14828 2022-09-15 15:26:59.000000 savantaudio-client-0.1.8/savantaudio/client.py
--rw-r--r--   0 adam       (501) staff       (20)     2814 2022-09-13 16:15:28.000000 savantaudio-client-0.1.8/savantaudio/entry_points.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-15 15:27:38.317785 savantaudio-client-0.1.8/savantaudio_client.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     1838 2022-09-15 15:27:38.000000 savantaudio-client-0.1.8/savantaudio_client.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      465 2022-09-15 15:27:38.000000 savantaudio-client-0.1.8/savantaudio_client.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2022-09-15 15:27:38.000000 savantaudio-client-0.1.8/savantaudio_client.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)       69 2022-09-15 15:27:38.000000 savantaudio-client-0.1.8/savantaudio_client.egg-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       12 2022-09-15 15:27:38.000000 savantaudio-client-0.1.8/savantaudio_client.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      741 2022-09-15 15:27:38.318172 savantaudio-client-0.1.8/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-15 16:54:15.595349 savantaudio-client-0.1.9/
+-rw-r--r--   0 adam       (501) staff       (20)      547 2022-09-09 15:22:34.000000 savantaudio-client-0.1.9/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)     1838 2022-09-15 16:54:15.595410 savantaudio-client-0.1.9/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1259 2022-09-09 16:59:56.000000 savantaudio-client-0.1.9/README.md
+-rw-r--r--   0 adam       (501) staff       (20)       91 2022-09-09 15:40:13.000000 savantaudio-client-0.1.9/pyproject.toml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-15 16:54:15.594534 savantaudio-client-0.1.9/savantaudio/
+-rw-r--r--   0 adam       (501) staff       (20)      120 2022-01-20 21:30:52.000000 savantaudio-client-0.1.9/savantaudio/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)      388 2022-09-15 16:53:29.000000 savantaudio-client-0.1.9/savantaudio/__version__.py
+-rw-r--r--   0 adam       (501) staff       (20)    14829 2022-09-15 16:53:23.000000 savantaudio-client-0.1.9/savantaudio/client.py
+-rw-r--r--   0 adam       (501) staff       (20)     2814 2022-09-13 16:15:28.000000 savantaudio-client-0.1.9/savantaudio/entry_points.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-15 16:54:15.595257 savantaudio-client-0.1.9/savantaudio_client.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1838 2022-09-15 16:54:15.000000 savantaudio-client-0.1.9/savantaudio_client.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      465 2022-09-15 16:54:15.000000 savantaudio-client-0.1.9/savantaudio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2022-09-15 16:54:15.000000 savantaudio-client-0.1.9/savantaudio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)       69 2022-09-15 16:54:15.000000 savantaudio-client-0.1.9/savantaudio_client.egg-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       12 2022-09-15 16:54:15.000000 savantaudio-client-0.1.9/savantaudio_client.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      741 2022-09-15 16:54:15.595643 savantaudio-client-0.1.9/setup.cfg
```

### Comparing `savantaudio-client-0.1.8/LICENSE` & `savantaudio-client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `savantaudio-client-0.1.8/PKG-INFO` & `savantaudio-client-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savantaudio-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: A client library to interact with Savant Audio Switches (e.g. SSA-3220).
 Home-page: https://github.com/adam_kropp/savantaudio-client
 Author: Adam Kropp
 Author-email: adam_kropp@yahoo.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `savantaudio-client-0.1.8/README.md` & `savantaudio-client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `savantaudio-client-0.1.8/savantaudio/client.py` & `savantaudio-client-0.1.9/savantaudio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
             if m:
                 self._attributes['fpgarev'] = m.group(1)
         
         async for reply in self._connection.send('status'):
             m = re.search('statusAPI1.0; (.*)', reply)
             if m:
                 for part in m.group(1).split(';'):
-                    part = part.trim()
+                    part = part.strip()
                     if part.startswith('pn'):
                         self._attributes['pn'] = part
                     elif part.startswith('sn'):
                         self._attributes['sn'] = part
                     elif part.startswith('rev'):
                         self._attributes['rev'] = part
                     elif part == 'ready=yes':
```

### Comparing `savantaudio-client-0.1.8/savantaudio/entry_points.py` & `savantaudio-client-0.1.9/savantaudio/entry_points.py`

 * *Files identical despite different names*

### Comparing `savantaudio-client-0.1.8/savantaudio_client.egg-info/PKG-INFO` & `savantaudio-client-0.1.9/savantaudio_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savantaudio-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: A client library to interact with Savant Audio Switches (e.g. SSA-3220).
 Home-page: https://github.com/adam_kropp/savantaudio-client
 Author: Adam Kropp
 Author-email: adam_kropp@yahoo.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `savantaudio-client-0.1.8/setup.cfg` & `savantaudio-client-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = savantaudio-client
-version = 0.1.8
+version = 0.1.9
 author = Adam Kropp
 author_email = adam_kropp@yahoo.com
 description = A client library to interact with Savant Audio Switches (e.g. SSA-3220).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/adam_kropp/savantaudio-client
 classifiers =
```

