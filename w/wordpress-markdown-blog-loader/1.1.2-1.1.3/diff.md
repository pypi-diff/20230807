# Comparing `tmp/wordpress-markdown-blog-loader-1.1.2.tar.gz` & `tmp/wordpress-markdown-blog-loader-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordpress-markdown-blog-loader-1.1.2.tar", last modified: Mon Aug  7 07:40:51 2023, max compression
+gzip compressed data, was "wordpress-markdown-blog-loader-1.1.3.tar", last modified: Mon Aug  7 08:10:50 2023, max compression
```

## Comparing `wordpress-markdown-blog-loader-1.1.2.tar` & `wordpress-markdown-blog-loader-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:40:51.510221 wordpress-markdown-blog-loader-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 07:40:51.510221 wordpress-markdown-blog-loader-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 07:40:51.510221 wordpress-markdown-blog-loader-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:40:51.506220 wordpress-markdown-blog-loader-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:40:51.506220 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/check_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/name_to_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/remove_newlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:40:51.510221 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 07:40:51.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-07 07:40:51.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:40:51.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 07:40:51.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:40:25.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-07 07:40:51.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 07:40:51.000000 wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:40:51.510221 wordpress-markdown-blog-loader-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-07 07:40:04.000000 wordpress-markdown-blog-loader-1.1.2/tests/test_blog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.739639 wordpress-markdown-blog-loader-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/check_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/name_to_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/remove_newlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 08:10:21.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/tests/test_blog.py
```

### Comparing `wordpress-markdown-blog-loader-1.1.2/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-markdown-blog-loader
-Version: 1.1.2
+Version: 1.1.3
 Summary: load markdown blogs into wordpress
 Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: APL2
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -75,15 +75,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.2
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.3
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.2/README.md` & `wordpress-markdown-blog-loader-1.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.2
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.3
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.2/setup.py` & `wordpress-markdown-blog-loader-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="wordpress-markdown-blog-loader",
-    version="1.1.2",
+    version="1.1.3",
     url="https://github.com/binxio/wordpress-markdown-blog-loader",
     license="APL2",
     author="Mark van Holsteijn",
     author_email="markvanholsteijn@binx.io",
     description="load markdown blogs into wordpress",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/__main__.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/__main__.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/api.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/api.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/blog.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/blog.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/check_links.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/check_links.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/download.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/download.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/name_to_email.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/name_to_email.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/new.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/new.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/remove_newlines.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/remove_newlines.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader/upload.py` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/upload.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-markdown-blog-loader
-Version: 1.1.2
+Version: 1.1.3
 Summary: load markdown blogs into wordpress
 Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: APL2
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -75,15 +75,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.2
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.3
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.2/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt` & `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.2/tests/test_blog.py` & `wordpress-markdown-blog-loader-1.1.3/tests/test_blog.py`

 * *Files identical despite different names*

