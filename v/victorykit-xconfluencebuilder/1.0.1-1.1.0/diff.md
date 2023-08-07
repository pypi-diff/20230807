# Comparing `tmp/victorykit-xconfluencebuilder-1.0.1.tar.gz` & `tmp/victorykit-xconfluencebuilder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "victorykit-xconfluencebuilder-1.0.1.tar", last modified: Mon Aug  7 00:47:05 2023, max compression
+gzip compressed data, was "victorykit-xconfluencebuilder-1.1.0.tar", last modified: Mon Aug  7 17:04:34 2023, max compression
```

## Comparing `victorykit-xconfluencebuilder-1.0.1.tar` & `victorykit-xconfluencebuilder-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      100 2023-08-07 00:23:10.000000 victorykit-xconfluencebuilder-1.0.1/.gitignore
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4722 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/PKG-INFO
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      241 2023-08-06 22:13:42.000000 victorykit-xconfluencebuilder-1.0.1/Pipfile
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    22574 2023-08-06 22:14:10.000000 victorykit-xconfluencebuilder-1.0.1/Pipfile.lock
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4446 2023-08-07 00:45:34.000000 victorykit-xconfluencebuilder-1.0.1/README.md
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      238 2023-08-07 00:22:00.000000 victorykit-xconfluencebuilder-1.0.1/pyproject.toml
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/samples/
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        7 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/.gitignore
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      263 2023-08-06 23:53:40.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/Pipfile
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    19149 2023-07-25 00:32:00.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/Pipfile.lock
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      782 2023-08-06 22:09:56.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/README.md
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/_media/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  2919350 2023-08-06 23:15:34.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  1385576 2023-08-06 23:19:10.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      269 2023-08-06 23:23:20.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/cats.rst
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      826 2023-08-06 23:57:12.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/conf.py
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     3735 2023-08-06 22:02:34.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/confluence_conf.py
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      856 2023-08-06 23:23:50.000000 victorykit-xconfluencebuilder-1.0.1/samples/default/docs/index.rst
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      731 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/setup.cfg
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       61 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.0.1/setup.py
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/src/
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:06.000000 victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4722 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      816 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/dependency_links.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       42 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/requires.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       19 2023-08-07 00:47:04.000000 victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/top_level.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 00:22:44.000000 victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/zip-safe
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 00:47:06.000000 victorykit-xconfluencebuilder-1.0.1/src/xconfluencebuilder/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    10936 2023-08-07 00:16:52.000000 victorykit-xconfluencebuilder-1.0.1/src/xconfluencebuilder/__init__.py
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      923 2023-08-07 00:22:12.000000 victorykit-xconfluencebuilder-1.0.1/tox.ini
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      100 2023-08-07 00:23:10.000000 victorykit-xconfluencebuilder-1.1.0/.gitignore
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      928 2023-08-07 16:57:56.000000 victorykit-xconfluencebuilder-1.1.0/CHANGELOG.md
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     2476 2023-08-07 16:48:02.000000 victorykit-xconfluencebuilder-1.1.0/LICENSE
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4744 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/PKG-INFO
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      241 2023-08-06 22:13:42.000000 victorykit-xconfluencebuilder-1.1.0/Pipfile
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    22574 2023-08-06 22:14:10.000000 victorykit-xconfluencebuilder-1.1.0/Pipfile.lock
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4446 2023-08-07 00:45:34.000000 victorykit-xconfluencebuilder-1.1.0/README.md
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      238 2023-08-07 00:22:00.000000 victorykit-xconfluencebuilder-1.1.0/pyproject.toml
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/samples/
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        7 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/.gitignore
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      263 2023-08-06 23:53:40.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/Pipfile
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    19149 2023-07-25 00:32:00.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/Pipfile.lock
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      782 2023-08-06 22:09:56.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/README.md
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/_media/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  2919350 2023-08-06 23:15:34.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  1385576 2023-08-06 23:19:10.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      269 2023-08-06 23:23:20.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/cats.rst
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      826 2023-08-06 23:57:12.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/conf.py
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     3735 2023-08-06 22:02:34.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/confluence_conf.py
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      856 2023-08-06 23:23:50.000000 victorykit-xconfluencebuilder-1.1.0/samples/default/docs/index.rst
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      731 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/setup.cfg
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       61 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.1.0/setup.py
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4744 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      837 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       42 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/requires.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       19 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/top_level.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 00:22:44.000000 victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/zip-safe
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:04:34.000000 victorykit-xconfluencebuilder-1.1.0/src/xconfluencebuilder/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    10724 2023-08-07 16:58:02.000000 victorykit-xconfluencebuilder-1.1.0/src/xconfluencebuilder/__init__.py
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      923 2023-08-07 17:03:52.000000 victorykit-xconfluencebuilder-1.1.0/tox.ini
```

### Comparing `victorykit-xconfluencebuilder-1.0.1/PKG-INFO` & `victorykit-xconfluencebuilder-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: victorykit-xconfluencebuilder
-Version: 1.0.1
+Version: 1.1.0
 Summary: sphinxcontrib.confluencebuilder wrapper for delayed publishing
 Author: Theodor Rodweil
 Author-email: theodor.rodweil@victory-k.it
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # xconfluencebuilder
 
 This program is a drop-in replacement for the [Atlassian Confluence Builder for
 Sphinx](https://github.com/sphinx-contrib/confluencebuilder). It
 exports/dumps/archives the build output of the confluencebuilder Sphinx builder
 into a generic interchangeable format, which can be used in conjunction with
```

### Comparing `victorykit-xconfluencebuilder-1.0.1/Pipfile.lock` & `victorykit-xconfluencebuilder-1.1.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/README.md` & `victorykit-xconfluencebuilder-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/samples/default/Pipfile.lock` & `victorykit-xconfluencebuilder-1.1.0/samples/default/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/samples/default/README.md` & `victorykit-xconfluencebuilder-1.1.0/samples/default/README.md`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg` & `victorykit-xconfluencebuilder-1.1.0/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg` & `victorykit-xconfluencebuilder-1.1.0/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/samples/default/docs/conf.py` & `victorykit-xconfluencebuilder-1.1.0/samples/default/docs/conf.py`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/samples/default/docs/confluence_conf.py` & `victorykit-xconfluencebuilder-1.1.0/samples/default/docs/confluence_conf.py`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/samples/default/docs/index.rst` & `victorykit-xconfluencebuilder-1.1.0/samples/default/docs/index.rst`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/setup.cfg` & `victorykit-xconfluencebuilder-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO` & `victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: victorykit-xconfluencebuilder
-Version: 1.0.1
+Version: 1.1.0
 Summary: sphinxcontrib.confluencebuilder wrapper for delayed publishing
 Author: Theodor Rodweil
 Author-email: theodor.rodweil@victory-k.it
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # xconfluencebuilder
 
 This program is a drop-in replacement for the [Atlassian Confluence Builder for
 Sphinx](https://github.com/sphinx-contrib/confluencebuilder). It
 exports/dumps/archives the build output of the confluencebuilder Sphinx builder
 into a generic interchangeable format, which can be used in conjunction with
```

### Comparing `victorykit-xconfluencebuilder-1.0.1/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt` & `victorykit-xconfluencebuilder-1.1.0/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 .gitignore
+CHANGELOG.md
+LICENSE
 Pipfile
 Pipfile.lock
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
```

### Comparing `victorykit-xconfluencebuilder-1.0.1/src/xconfluencebuilder/__init__.py` & `victorykit-xconfluencebuilder-1.1.0/src/xconfluencebuilder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,24 +224,19 @@
     ) -> str:
         """request to store an attachment on a provided page
 
         :returns: the attachment identifier
         """
         logger.info('pass-through intercept: store_attachment')
 
-        # 😭 i wanted to use this method so bad, but since we're ditching
-        # hashing altogether, this isn't necessary. We'll keep it as an
-        # orbituary 🪦
-        # mime_extension = guess_extension(mimetype, False)
-
         file_name = quote_plus(name)
 
         output_basepath = Path(getattr(self.config, 'xconfluence_outdir'))
 
-        file_ = output_basepath / 'attachments' / file_name
+        file_ = output_basepath / 'attachments' / quote_plus(page_id) / file_name
 
         file_.parent.mkdir(parents = True, exist_ok = True)
 
         file_.write_bytes(data)
 
         self.dump.attachments.append(AttachmentMeta(
             name = name,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `victorykit-xconfluencebuilder-1.0.1/tox.ini` & `victorykit-xconfluencebuilder-1.1.0/tox.ini`

 * *Files identical despite different names*

