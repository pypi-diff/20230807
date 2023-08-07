# Comparing `tmp/woodcut-0.5.0.tar.gz` & `tmp/woodcut-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/woodcut-0.5.0.tar", last modified: Sun Jul 14 17:02:40 2013, max compression
+gzip compressed data, was "woodcut-0.6.0.tar", last modified: Mon Aug  7 16:02:48 2023, max compression
```

## Comparing `woodcut-0.5.0.tar` & `woodcut-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2013-07-14 17:02:40.000000 woodcut-0.5.0/
--rw-r--r--   0 luke       (501) staff       (20)      970 2013-07-14 17:02:40.000000 woodcut-0.5.0/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)       59 2013-07-14 17:02:40.000000 woodcut-0.5.0/setup.cfg
--rw-r--r--   0 luke       (501) staff       (20)     1210 2013-07-14 17:01:30.000000 woodcut-0.5.0/setup.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2013-07-14 17:02:40.000000 woodcut-0.5.0/woodcut/
--rw-r--r--   0 luke       (501) staff       (20)     1276 2013-07-14 03:22:03.000000 woodcut-0.5.0/woodcut/__init__.py
--rwxr-xr-x   0 luke       (501) staff       (20)     7030 2013-07-14 16:50:16.000000 woodcut-0.5.0/woodcut/project.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2013-07-14 17:02:40.000000 woodcut-0.5.0/woodcut.egg-info/
--rw-r--r--   0 luke       (501) staff       (20)        1 2013-07-14 17:02:39.000000 woodcut-0.5.0/woodcut.egg-info/dependency_links.txt
--rw-r--r--   0 luke       (501) staff       (20)       42 2013-07-14 17:02:39.000000 woodcut-0.5.0/woodcut.egg-info/entry_points.txt
--rw-r--r--   0 luke       (501) staff       (20)      970 2013-07-14 17:02:39.000000 woodcut-0.5.0/woodcut.egg-info/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)       11 2013-07-14 17:02:39.000000 woodcut-0.5.0/woodcut.egg-info/requires.txt
--rw-r--r--   0 luke       (501) staff       (20)      235 2013-07-14 17:02:39.000000 woodcut-0.5.0/woodcut.egg-info/SOURCES.txt
--rw-r--r--   0 luke       (501) staff       (20)        8 2013-07-14 17:02:39.000000 woodcut-0.5.0/woodcut.egg-info/top_level.txt
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-08-07 16:02:48.761351 woodcut-0.6.0/
+-rw-r--r--   0 luke       (501) staff       (20)     1076 2023-08-07 15:24:06.000000 woodcut-0.6.0/LICENSE
+-rw-r--r--   0 luke       (501) staff       (20)      913 2023-08-07 16:02:48.761232 woodcut-0.6.0/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)       38 2023-08-07 16:02:48.761386 woodcut-0.6.0/setup.cfg
+-rw-r--r--   0 luke       (501) staff       (20)     1162 2023-08-07 15:53:01.000000 woodcut-0.6.0/setup.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-08-07 16:02:48.759936 woodcut-0.6.0/tests/
+-rw-r--r--   0 luke       (501) staff       (20)      968 2023-08-07 15:24:06.000000 woodcut-0.6.0/tests/test_example.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-08-07 16:02:48.760355 woodcut-0.6.0/woodcut/
+-rw-r--r--   0 luke       (501) staff       (20)     1276 2023-08-07 15:24:06.000000 woodcut-0.6.0/woodcut/__init__.py
+-rwxr-xr-x   0 luke       (501) staff       (20)     7123 2023-08-07 15:32:12.000000 woodcut-0.6.0/woodcut/project.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-08-07 16:02:48.761093 woodcut-0.6.0/woodcut.egg-info/
+-rw-r--r--   0 luke       (501) staff       (20)      913 2023-08-07 16:02:48.000000 woodcut-0.6.0/woodcut.egg-info/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)      265 2023-08-07 16:02:48.000000 woodcut-0.6.0/woodcut.egg-info/SOURCES.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2023-08-07 16:02:48.000000 woodcut-0.6.0/woodcut.egg-info/dependency_links.txt
+-rw-r--r--   0 luke       (501) staff       (20)       41 2023-08-07 16:02:48.000000 woodcut-0.6.0/woodcut.egg-info/entry_points.txt
+-rw-r--r--   0 luke       (501) staff       (20)       12 2023-08-07 16:02:48.000000 woodcut-0.6.0/woodcut.egg-info/requires.txt
+-rw-r--r--   0 luke       (501) staff       (20)        8 2023-08-07 16:02:48.000000 woodcut-0.6.0/woodcut.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `woodcut-0.5.0/PKG-INFO` & `woodcut-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: woodcut
-Version: 0.5.0
+Version: 0.6.0
 Summary: Minimalist content management system for static websites.
 Home-page: http://wiki.github.com/lukecyca/woodcut
 Author: Luke Cyca
 Author-email: me@lukecyca.com
 License: MIT
-Description: Woodcut is a system for building static websites from Mako source files. It will walk your source directory, process any templates it finds, and produce a complete website in the build directory, ready to rsync to your webserver.
 Keywords: mako template static web development
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Text Processing :: Markup
+License-File: LICENSE
+
+Woodcut is a system for building static websites from Mako source files. It will walk your source directory, process any templates it finds, and produce a complete website in the build directory, ready to rsync to your webserver.
```

### Comparing `woodcut-0.5.0/setup.py` & `woodcut-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from setuptools import setup
 
 setup(
     name="woodcut",
-    version="0.5.0",
+    version="0.6.0",
     author="Luke Cyca",
     author_email="me@lukecyca.com",
     description="Minimalist content management system for static websites.",
     license="MIT",
     keywords="mako template static web development",
     url="http://wiki.github.com/lukecyca/woodcut",
     long_description="Woodcut is a system for building static websites from Mako source files. It will walk your source directory, process any templates it finds, and produce a complete website in the build directory, ready to rsync to your webserver.",
     classifiers=[
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.6",
-        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Natural Language :: English",
         "Topic :: Internet :: WWW/HTTP :: Site Management",
         "Topic :: Text Processing :: Markup",
     ],
 
     packages=['woodcut'],
-    install_requires=["Mako>=0.4.2"],
+    install_requires=["Mako>=1.2.4"],
 
     entry_points={
         'console_scripts': [
             'woodcut = woodcut:main',
         ]
     }
 )
```

### Comparing `woodcut-0.5.0/woodcut/__init__.py` & `woodcut-0.6.0/woodcut/__init__.py`

 * *Files identical despite different names*

### Comparing `woodcut-0.5.0/woodcut/project.py` & `woodcut-0.6.0/woodcut/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,23 @@
         return AttributeDict(metadata)
 
     def build_template(self, root_relative_src_path):
         """Builds a single template"""
 
         def relative_path(path):
             """Translates a root-relative path to a path relative to this file"""
-            backout_path = os.path.relpath('.', os.path.dirname(root_relative_src_path))
+            backout_path = os.path.relpath(
+                '.', os.path.dirname(root_relative_src_path))
             return os.path.normpath(os.path.join(backout_path, path))
 
         # Absolute paths to source and build objects
-        src_path = os.path.normpath(os.path.join(self.src_root, root_relative_src_path))
-        build_path = os.path.normpath(os.path.join(self.build_root, root_relative_src_path))
+        src_path = os.path.normpath(os.path.join(
+            self.src_root, root_relative_src_path))
+        build_path = os.path.normpath(os.path.join(
+            self.build_root, root_relative_src_path))
 
         if os.path.exists(build_path):
             os.unlink(build_path)
 
         extension = os.path.splitext(src_path)[1]
 
         # Skip non-templates, and just link them to the source file
@@ -101,21 +104,22 @@
                 os.symlink(src_path, build_path)
             return
 
         # Determine output filename
         build_path = build_path.replace('.mako', '')
 
         # Render the template to the output path
-        logger.info("Rendering %s" % root_relative_src_path.replace('.mako', ''))
+        logger.info("Rendering %s" %
+                    root_relative_src_path.replace('.mako', ''))
 
         # Find this template's metadata
         (md,) = [t for t in self.templates
                  if t['src_path'] == os.path.normpath(root_relative_src_path)]
 
-        with open(build_path, 'w') as fh:
+        with open(build_path, 'wb') as fh:
             mako_src = self.lookup.get_template(root_relative_src_path)
             fh.write(mako_src.render(
                 relative_path=relative_path,
                 templates=self.templates,
                 articles=self.articles,
                 meta=md,
             ))
@@ -179,15 +183,16 @@
                 elif not os.path.exists(os.path.join(self.build_root, path, d)):
                     os.mkdir(os.path.join(self.build_root, path, d))
             for f in files:
                 if not any([ignore.search(os.path.join(path, f)) for ignore in IGNORE_PATTERNS]):
                     try:
                         self.build_template(os.path.join(path, f))
                     except Exception:
-                        logger.exception('Exception in {0}'.format(os.path.join(path, f)))
+                        logger.exception(
+                            'Exception in {0}'.format(os.path.join(path, f)))
                 else:
                     logger.debug("Ignoring {0}".format(os.path.join(path, f)))
 
         logger.info("Build complete")
 
     def clean(self):
         """Delete everything in the build directory"""
```

### Comparing `woodcut-0.5.0/woodcut.egg-info/PKG-INFO` & `woodcut-0.6.0/woodcut.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: woodcut
-Version: 0.5.0
+Version: 0.6.0
 Summary: Minimalist content management system for static websites.
 Home-page: http://wiki.github.com/lukecyca/woodcut
 Author: Luke Cyca
 Author-email: me@lukecyca.com
 License: MIT
-Description: Woodcut is a system for building static websites from Mako source files. It will walk your source directory, process any templates it finds, and produce a complete website in the build directory, ready to rsync to your webserver.
 Keywords: mako template static web development
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Text Processing :: Markup
+License-File: LICENSE
+
+Woodcut is a system for building static websites from Mako source files. It will walk your source directory, process any templates it finds, and produce a complete website in the build directory, ready to rsync to your webserver.
```

