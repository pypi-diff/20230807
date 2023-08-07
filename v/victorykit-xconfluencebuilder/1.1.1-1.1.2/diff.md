# Comparing `tmp/victorykit-xconfluencebuilder-1.1.1.tar.gz` & `tmp/victorykit-xconfluencebuilder-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "victorykit-xconfluencebuilder-1.1.1.tar", last modified: Mon Aug  7 17:25:22 2023, max compression
+gzip compressed data, was "victorykit-xconfluencebuilder-1.1.2.tar", last modified: Mon Aug  7 17:38:06 2023, max compression
```

## Comparing `victorykit-xconfluencebuilder-1.1.1.tar` & `victorykit-xconfluencebuilder-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      100 2023-08-07 00:23:10.000000 victorykit-xconfluencebuilder-1.1.1/.gitignore
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     1345 2023-08-07 17:22:12.000000 victorykit-xconfluencebuilder-1.1.1/CHANGELOG.md
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     2476 2023-08-07 16:48:02.000000 victorykit-xconfluencebuilder-1.1.1/LICENSE
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4844 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/PKG-INFO
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      241 2023-08-06 22:13:42.000000 victorykit-xconfluencebuilder-1.1.1/Pipfile
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    22574 2023-08-06 22:14:10.000000 victorykit-xconfluencebuilder-1.1.1/Pipfile.lock
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4446 2023-08-07 00:45:34.000000 victorykit-xconfluencebuilder-1.1.1/README.md
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      238 2023-08-07 00:22:00.000000 victorykit-xconfluencebuilder-1.1.1/pyproject.toml
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/samples/
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        7 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/.gitignore
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      263 2023-08-06 23:53:40.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/Pipfile
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    19149 2023-07-25 00:32:00.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/Pipfile.lock
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      782 2023-08-06 22:09:56.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/README.md
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/docs/
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/docs/_media/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  2919350 2023-08-06 23:15:34.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  1385576 2023-08-06 23:19:10.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      269 2023-08-06 23:23:20.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/docs/cats.rst
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      781 2023-08-07 17:19:54.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/docs/conf.py
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      856 2023-08-06 23:23:50.000000 victorykit-xconfluencebuilder-1.1.1/samples/default/docs/index.rst
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      860 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/setup.cfg
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       61 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.1.1/setup.py
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4844 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      797 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/dependency_links.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       42 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/requires.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       19 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/top_level.txt
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 00:22:44.000000 victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/zip-safe
-drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:25:22.000000 victorykit-xconfluencebuilder-1.1.1/src/xconfluencebuilder/
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    10724 2023-08-07 16:58:02.000000 victorykit-xconfluencebuilder-1.1.1/src/xconfluencebuilder/__init__.py
--rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     1147 2023-08-07 17:10:10.000000 victorykit-xconfluencebuilder-1.1.1/tox.ini
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      100 2023-08-07 00:23:10.000000 victorykit-xconfluencebuilder-1.1.2/.gitignore
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     1654 2023-08-07 17:35:54.000000 victorykit-xconfluencebuilder-1.1.2/CHANGELOG.md
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     2476 2023-08-07 16:48:02.000000 victorykit-xconfluencebuilder-1.1.2/LICENSE
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4970 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/PKG-INFO
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      241 2023-08-06 22:13:42.000000 victorykit-xconfluencebuilder-1.1.2/Pipfile
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    22574 2023-08-06 22:14:10.000000 victorykit-xconfluencebuilder-1.1.2/Pipfile.lock
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4472 2023-08-07 17:33:38.000000 victorykit-xconfluencebuilder-1.1.2/README.md
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      238 2023-08-07 00:22:00.000000 victorykit-xconfluencebuilder-1.1.2/pyproject.toml
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/samples/
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        7 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/.gitignore
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      263 2023-08-06 23:53:40.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/Pipfile
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    19149 2023-07-25 00:32:00.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/Pipfile.lock
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      782 2023-08-06 22:09:56.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/README.md
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/docs/
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/docs/_media/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  2919350 2023-08-06 23:15:34.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)  1385576 2023-08-06 23:19:10.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      269 2023-08-06 23:23:20.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/docs/cats.rst
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      781 2023-08-07 17:19:54.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/docs/conf.py
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      856 2023-08-06 23:23:50.000000 victorykit-xconfluencebuilder-1.1.2/samples/default/docs/index.rst
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      950 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/setup.cfg
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       61 2023-07-16 12:02:50.000000 victorykit-xconfluencebuilder-1.1.2/setup.py
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     4970 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)      797 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       42 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/requires.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)       19 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/top_level.txt
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)        1 2023-08-07 00:22:44.000000 victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/zip-safe
+drwxrwxrwx   0 tiara.rodney   (503) staff       (20)        0 2023-08-07 17:38:06.000000 victorykit-xconfluencebuilder-1.1.2/src/xconfluencebuilder/
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)    10724 2023-08-07 16:58:02.000000 victorykit-xconfluencebuilder-1.1.2/src/xconfluencebuilder/__init__.py
+-rwxrwxrwx   0 tiara.rodney   (503) staff       (20)     1147 2023-08-07 17:10:10.000000 victorykit-xconfluencebuilder-1.1.2/tox.ini
```

### Comparing `victorykit-xconfluencebuilder-1.1.1/CHANGELOG.md` & `victorykit-xconfluencebuilder-1.1.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,27 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
 
 nothing as of yet
 
+## [1.1.2] - 2023-08-07
+
+### Added
+
+- link to changelog in package metadata
+
+### Changed
+
+- manifest example in README as to reflect the latest default sample output
+
+### Fixed
+
+- deprecated `license_file` property in package metadata 
 
 ## [1.1.1] - 2023-08-07
 
 ### Added
 
 - basic test which makes sure the default sample executes without errors
 
@@ -54,11 +67,12 @@
 
 ### Added
 
 - initial release
 
 
 [unreleased]: https://bitbucket.org/victorykit/xconfluencebuilder/branch/master
+[1.1.2]: https://bitbucket.org/victorykit/xconfluencebuilder/src/v1.1.2/
 [1.1.1]: https://bitbucket.org/victorykit/xconfluencebuilder/src/v1.1.1/
 [1.1.0]: https://bitbucket.org/victorykit/xconfluencebuilder/src/v1.1.0/
 [1.0.1]: https://bitbucket.org/victorykit/xconfluencebuilder/src/v1.0.1/
 [1.0.0]: https://bitbucket.org/victorykit/xconfluencebuilder/src/v1.0.0/
```

### Comparing `victorykit-xconfluencebuilder-1.1.1/LICENSE` & `victorykit-xconfluencebuilder-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/PKG-INFO` & `victorykit-xconfluencebuilder-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: victorykit-xconfluencebuilder
-Version: 1.1.1
+Version: 1.1.2
 Summary: sphinxcontrib.confluencebuilder wrapper for delayed publishing
 Author: Theodor Rodweil
 Author-email: theodor.rodweil@victory-k.it
 License: DL-DE-BY-2.0
+Project-URL: Changelog, https://bitbucket.org/victorykit/xconfluencebuilder/src/master/CHANGELOG.md
 Project-URL: Repository, https://bitbucket.org/victorykit/xconfluencebuilder/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xconfluencebuilder
 
@@ -46,27 +47,27 @@
         }
     ],
     "Attachments": [
         {
             "Name": "pexels-just-a-couple-photos-3777622.jpg",
             "ContainerPageTitle": "Cats",
             "MimeType": "image/jpeg",
-            "Ref": "attachments/pexels-just-a-couple-photos-3777622.jpg"
+            "Ref": "attachments/Cats/pexels-just-a-couple-photos-3777622.jpg"
         },
         {
             "Name": "pexels-sami-aksu-14356302.jpg",
             "ContainerPageTitle": "Cats",
             "MimeType": "image/jpeg",
-            "Ref": "attachments/pexels-sami-aksu-14356302.jpg"
+            "Ref": "attachments/Cats/pexels-sami-aksu-14356302.jpg"
         },
         {
             "Name": "objects.inv",
             "ContainerPageTitle": "Default Sample~",
             "MimeType": "application/octet-stream",
-            "Ref": "attachments/objects.inv"
+            "Ref": "attachments/Default+Sample~/objects.inv"
         }
     ]
 }
 ```
 
 > **NOTE**: The manifest's schema is currently part of the
   [PSConfluencePublisher](https://bitbucket.org/victorykit/psconfluencepublisher)
```

### Comparing `victorykit-xconfluencebuilder-1.1.1/Pipfile.lock` & `victorykit-xconfluencebuilder-1.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/README.md` & `victorykit-xconfluencebuilder-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
         }
     ],
     "Attachments": [
         {
             "Name": "pexels-just-a-couple-photos-3777622.jpg",
             "ContainerPageTitle": "Cats",
             "MimeType": "image/jpeg",
-            "Ref": "attachments/pexels-just-a-couple-photos-3777622.jpg"
+            "Ref": "attachments/Cats/pexels-just-a-couple-photos-3777622.jpg"
         },
         {
             "Name": "pexels-sami-aksu-14356302.jpg",
             "ContainerPageTitle": "Cats",
             "MimeType": "image/jpeg",
-            "Ref": "attachments/pexels-sami-aksu-14356302.jpg"
+            "Ref": "attachments/Cats/pexels-sami-aksu-14356302.jpg"
         },
         {
             "Name": "objects.inv",
             "ContainerPageTitle": "Default Sample~",
             "MimeType": "application/octet-stream",
-            "Ref": "attachments/objects.inv"
+            "Ref": "attachments/Default+Sample~/objects.inv"
         }
     ]
 }
 ```
 
 > **NOTE**: The manifest's schema is currently part of the
   [PSConfluencePublisher](https://bitbucket.org/victorykit/psconfluencepublisher)
```

### Comparing `victorykit-xconfluencebuilder-1.1.1/samples/default/Pipfile.lock` & `victorykit-xconfluencebuilder-1.1.2/samples/default/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/samples/default/README.md` & `victorykit-xconfluencebuilder-1.1.2/samples/default/README.md`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg` & `victorykit-xconfluencebuilder-1.1.2/samples/default/docs/_media/pexels-just-a-couple-photos-3777622.jpg`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg` & `victorykit-xconfluencebuilder-1.1.2/samples/default/docs/_media/pexels-sami-aksu-14356302.jpg`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/samples/default/docs/conf.py` & `victorykit-xconfluencebuilder-1.1.2/samples/default/docs/conf.py`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/samples/default/docs/index.rst` & `victorykit-xconfluencebuilder-1.1.2/samples/default/docs/index.rst`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/setup.cfg` & `victorykit-xconfluencebuilder-1.1.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 version = 1.0.0
 author = Theodor Rodweil
 author_email = theodor.rodweil@victory-k.it
 description = sphinxcontrib.confluencebuilder wrapper for delayed publishing
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = DL-DE-BY-2.0
-license_file = LICENSE
+license_files = LICENSE
 project_urls = 
+	Changelog = https://bitbucket.org/victorykit/xconfluencebuilder/src/master/CHANGELOG.md
 	Repository = https://bitbucket.org/victorykit/xconfluencebuilder/
 classifiers = 
 ´   topic = : Software Development :: Libraries :: Python Modules
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 	License :: Other/Proprietary License
```

### Comparing `victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO` & `victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: victorykit-xconfluencebuilder
-Version: 1.1.1
+Version: 1.1.2
 Summary: sphinxcontrib.confluencebuilder wrapper for delayed publishing
 Author: Theodor Rodweil
 Author-email: theodor.rodweil@victory-k.it
 License: DL-DE-BY-2.0
+Project-URL: Changelog, https://bitbucket.org/victorykit/xconfluencebuilder/src/master/CHANGELOG.md
 Project-URL: Repository, https://bitbucket.org/victorykit/xconfluencebuilder/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xconfluencebuilder
 
@@ -46,27 +47,27 @@
         }
     ],
     "Attachments": [
         {
             "Name": "pexels-just-a-couple-photos-3777622.jpg",
             "ContainerPageTitle": "Cats",
             "MimeType": "image/jpeg",
-            "Ref": "attachments/pexels-just-a-couple-photos-3777622.jpg"
+            "Ref": "attachments/Cats/pexels-just-a-couple-photos-3777622.jpg"
         },
         {
             "Name": "pexels-sami-aksu-14356302.jpg",
             "ContainerPageTitle": "Cats",
             "MimeType": "image/jpeg",
-            "Ref": "attachments/pexels-sami-aksu-14356302.jpg"
+            "Ref": "attachments/Cats/pexels-sami-aksu-14356302.jpg"
         },
         {
             "Name": "objects.inv",
             "ContainerPageTitle": "Default Sample~",
             "MimeType": "application/octet-stream",
-            "Ref": "attachments/objects.inv"
+            "Ref": "attachments/Default+Sample~/objects.inv"
         }
     ]
 }
 ```
 
 > **NOTE**: The manifest's schema is currently part of the
   [PSConfluencePublisher](https://bitbucket.org/victorykit/psconfluencepublisher)
```

### Comparing `victorykit-xconfluencebuilder-1.1.1/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt` & `victorykit-xconfluencebuilder-1.1.2/src/victorykit_xconfluencebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/src/xconfluencebuilder/__init__.py` & `victorykit-xconfluencebuilder-1.1.2/src/xconfluencebuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `victorykit-xconfluencebuilder-1.1.1/tox.ini` & `victorykit-xconfluencebuilder-1.1.2/tox.ini`

 * *Files identical despite different names*

