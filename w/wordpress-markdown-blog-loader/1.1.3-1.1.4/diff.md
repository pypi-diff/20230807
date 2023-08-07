# Comparing `tmp/wordpress-markdown-blog-loader-1.1.3.tar.gz` & `tmp/wordpress-markdown-blog-loader-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordpress-markdown-blog-loader-1.1.3.tar", last modified: Mon Aug  7 08:10:50 2023, max compression
+gzip compressed data, was "wordpress-markdown-blog-loader-1.1.4.tar", last modified: Mon Aug  7 10:09:14 2023, max compression
```

## Comparing `wordpress-markdown-blog-loader-1.1.3.tar` & `wordpress-markdown-blog-loader-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.739639 wordpress-markdown-blog-loader-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/check_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/name_to_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/remove_newlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 08:10:21.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 08:10:50.000000 wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:10:50.743639 wordpress-markdown-blog-loader-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-07 08:09:50.000000 wordpress-markdown-blog-loader-1.1.3/tests/test_blog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:09:14.900396 wordpress-markdown-blog-loader-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-08-07 10:09:14.900396 wordpress-markdown-blog-loader-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:09:14.900396 wordpress-markdown-blog-loader-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:09:14.896396 wordpress-markdown-blog-loader-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:09:14.900396 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15163 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/check_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/name_to_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/remove_newlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:09:14.900396 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-08-07 10:09:14.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-07 10:09:14.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:09:14.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 10:09:14.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:08:52.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-07 10:09:14.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 10:09:14.000000 wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:09:14.900396 wordpress-markdown-blog-loader-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-07 10:08:38.000000 wordpress-markdown-blog-loader-1.1.4/tests/test_blog.py
```

### Comparing `wordpress-markdown-blog-loader-1.1.3/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-markdown-blog-loader
-Version: 1.1.3
+Version: 1.1.4
 Summary: load markdown blogs into wordpress
 Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: APL2
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -38,14 +38,20 @@
 ## required Wordpress Plugins
 
 - [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/)
 - [REST API Meta Support](https://wordpress.org/plugins/rest-api-meta-support/)
 
 Furthermore, you have to enable the Rest API for the [Custom Field Group](https://www.advancedcustomfields.com/resources/wp-rest-api-integration/#enabling-the-rest-api-for-your-acf-fields) for the field `show_header_image`.
 
+## Installation
+Install it with [pipx](https://pypa.github.io/pipx/) or use Docker (see below):
+```shell
+pipx install wordpress-markdown-blog-loader
+```
+
 ## configuration
 to configure the access credentials, you need to add your WordPress application password to the file `~/.wordpress.ini`  
 and add a section for your Wordpress installation:
 
 ```
 [DEFAULT]
 host = xebia.com
@@ -75,15 +81,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.3
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.4
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.3/README.md` & `wordpress-markdown-blog-loader-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 ## required Wordpress Plugins
 
 - [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/)
 - [REST API Meta Support](https://wordpress.org/plugins/rest-api-meta-support/)
 
 Furthermore, you have to enable the Rest API for the [Custom Field Group](https://www.advancedcustomfields.com/resources/wp-rest-api-integration/#enabling-the-rest-api-for-your-acf-fields) for the field `show_header_image`.
 
+## Installation
+Install it with [pipx](https://pypa.github.io/pipx/) or use Docker (see below):
+```shell
+pipx install wordpress-markdown-blog-loader
+```
+
 ## configuration
 to configure the access credentials, you need to add your WordPress application password to the file `~/.wordpress.ini`  
 and add a section for your Wordpress installation:
 
 ```
 [DEFAULT]
 host = xebia.com
@@ -54,15 +60,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.3
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.4
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.3/setup.py` & `wordpress-markdown-blog-loader-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="wordpress-markdown-blog-loader",
-    version="1.1.3",
+    version="1.1.4",
     url="https://github.com/binxio/wordpress-markdown-blog-loader",
     license="APL2",
     author="Mark van Holsteijn",
     author_email="markvanholsteijn@binx.io",
     description="load markdown blogs into wordpress",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/__main__.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/__main__.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/api.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,18 @@
         return self.get("permalink_template")
 
     @permalink_template.setter
     def permalink_template(self, template: str):
         self["permalink_template"] = template
 
 
+class PermissionDenied(Exception):
+    def __init__(self, msg):
+        super().__init__(msg)
+
 class Wordpress(object):
     def __init__(self, host: Optional[str] = None):
         self.endpoint = WordpressEndpoint.load(host)
 
         self._media: List[Medium] = {}
         self._categories: Dict[str, int] = {}
         self.headers = {
@@ -264,16 +268,20 @@
             )
             if response.status_code == 200:
                 for object in response.json():
                     yield object
                 total_pages = int(response.headers["X-WP-TotalPages"])
                 page = page + 1
             else:
-                print(f"failed to get all {resource}: {response.text}")
-                exit(1)
+                msg = f"failed to get all {resource}: {response.status_code}, {response.text}"
+                if response.status_code in [401,403]:
+                    raise PermissionDenied(msg)
+                else:
+                    print(msg)
+                    exit(1)
 
         return None
 
     def users(self, query: dict = None) -> List["User"]:
         return list(map(lambda u: User(u), self.get_all("users", query)))
 
     def get_user_by_id(self, resource_id: int) -> "User":
@@ -281,15 +289,22 @@
 
     def get_unique_user_by_name(self, name: str, email: Optional[str]) -> "User":
 
         user = self.get_user_by_id("me")
         if user and user.name == name:
             return user
 
-        users = self.users({"context": "edit", "search": name})
+
+        users = []
+        try:
+            users = self.users({"context": "edit", "search": name})
+        except PermissionDenied as error:
+            logging.error("You have no permission to search for other users.\n        Make sure your author name '%s' matches your WP display name '%s' or visa versa", name, user.name)
+            exit(1)
+
         if len(users) == 0:
             raise ValueError(f"author '{name}' not found on {self.endpoint.host}")
         elif len(users) > 1:
             user = next(filter(lambda u: email and u.email == email, users), None)
             if not user:
                 raise ValueError(
                     f"Multiple authors named '{name}' found, none with email {email}"
```

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/blog.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/blog.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/check_links.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/check_links.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/download.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/download.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/name_to_email.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/name_to_email.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/new.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/new.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/remove_newlines.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/remove_newlines.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader/upload.py` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader/upload.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-markdown-blog-loader
-Version: 1.1.3
+Version: 1.1.4
 Summary: load markdown blogs into wordpress
 Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: APL2
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -38,14 +38,20 @@
 ## required Wordpress Plugins
 
 - [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/)
 - [REST API Meta Support](https://wordpress.org/plugins/rest-api-meta-support/)
 
 Furthermore, you have to enable the Rest API for the [Custom Field Group](https://www.advancedcustomfields.com/resources/wp-rest-api-integration/#enabling-the-rest-api-for-your-acf-fields) for the field `show_header_image`.
 
+## Installation
+Install it with [pipx](https://pypa.github.io/pipx/) or use Docker (see below):
+```shell
+pipx install wordpress-markdown-blog-loader
+```
+
 ## configuration
 to configure the access credentials, you need to add your WordPress application password to the file `~/.wordpress.ini`  
 and add a section for your Wordpress installation:
 
 ```
 [DEFAULT]
 host = xebia.com
@@ -75,15 +81,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.3
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.4
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.3/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt` & `wordpress-markdown-blog-loader-1.1.4/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.3/tests/test_blog.py` & `wordpress-markdown-blog-loader-1.1.4/tests/test_blog.py`

 * *Files identical despite different names*

