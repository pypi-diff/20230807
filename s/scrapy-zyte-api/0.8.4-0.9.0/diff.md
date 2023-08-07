# Comparing `tmp/scrapy-zyte-api-0.8.4.tar.gz` & `tmp/scrapy-zyte-api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-zyte-api-0.8.4.tar", last modified: Fri May 26 09:15:17 2023, max compression
+gzip compressed data, was "scrapy-zyte-api-0.9.0.tar", last modified: Tue Jun 13 09:42:35 2023, max compression
```

## Comparing `scrapy-zyte-api-0.8.4.tar` & `scrapy-zyte-api-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28637 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:15:17.078590 scrapy-zyte-api-0.8.4/scrapy_zyte_api/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_downloader_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_request_fingerprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:35.166797 scrapy-zyte-api-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-06-13 09:42:35.166797 scrapy-zyte-api-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:35.162798 scrapy-zyte-api-0.9.0/scrapy_zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/_downloader_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/_request_fingerprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:35.166797 scrapy-zyte-api-0.9.0/scrapy_zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-06-13 09:42:35.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-13 09:42:35.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:42:35.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 09:42:35.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 09:42:35.000000 scrapy-zyte-api-0.9.0/scrapy_zyte_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 09:42:35.166797 scrapy-zyte-api-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 09:42:21.000000 scrapy-zyte-api-0.9.0/setup.py
```

### Comparing `scrapy-zyte-api-0.8.4/LICENSE.txt` & `scrapy-zyte-api-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.4/PKG-INFO` & `scrapy-zyte-api-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: scrapy-zyte-api
-Version: 0.8.4
-Summary: Client library to process URLs through Zyte API
-Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
-Author: Zyte Group Ltd
-Author-email: info@zyte.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
 ===============
 scrapy-zyte-api
 ===============
 
 .. image:: https://img.shields.io/pypi/v/scrapy-zyte-api.svg
    :target: https://pypi.python.org/pypi/scrapy-zyte-api
    :alt: PyPI Version
@@ -618,14 +597,17 @@
 of which parameters you define through ``ZYTE_API_AUTOMAP_PARAMS``. In
 transparent mode, all Scrapy requests go through Zyte API, even requests that
 Scrapy sends automatically, such as those for ``robots.txt`` files when
 ROBOTSTXT_OBEY_ is ``True``, or those for sitemaps when using a `sitemap
 spider`_. Certain parameters, like ``browserHtml`` or ``screenshot``, are not
 meant to be used for every single request.
 
+If the ``zyte_api_default_params`` request meta key is set to ``False``, the
+value of the ``ZYTE_API_DEFAULT_PARAMS`` setting for this request is ignored.
+
 .. _ROBOTSTXT_OBEY: https://docs.scrapy.org/en/latest/topics/settings.html#robotstxt-obey
 .. _sitemap spider: https://docs.scrapy.org/en/latest/topics/spiders.html#sitemapspider
 
 
 Customizing the retry policy
 ============================
 
@@ -808,7 +790,69 @@
 For example::
 
    Sending Zyte API extract request: {"url": "https://example.com", "httpResponseBody": true}
 
 The ``ZYTE_API_LOG_REQUESTS_TRUNCATE``, 64 by default, determines the maximum
 length of any string value in the logged JSON object, excluding object keys. To
 disable truncation, set it to 0.
+
+
+scrapy-poet integration
+=======================
+
+``scrapy-zyte-api`` includes a `scrapy-poet provider`_ that you can use to get
+data from Zyte API in page objects. Enable it in the Scrapy settings::
+
+    SCRAPY_POET_PROVIDERS = {
+        ZyteApiProvider: 1100,
+    }
+
+Request some supported dependencies in the page object::
+
+    @attrs.define
+    class ProductPage(BasePage):
+        response: BrowserResponse
+        product: Product
+
+
+    class ZyteApiSpider(scrapy.Spider):
+        ...
+
+        def parse_page(self, response: DummyResponse, page: ProductPage):
+            ...
+
+Or request them directly in the callback::
+
+    class ZyteApiSpider(scrapy.Spider):
+        ...
+
+        def parse_page(self,
+                       response: DummyResponse,
+                       browser_response: BrowserResponse,
+                       product: Product,
+                       ):
+            ...
+
+The currently supported dependencies are:
+
+* ``web_poet.BrowserHtml``
+* ``web_poet.BrowserResponse``
+* ``zyte_common_items.Product``
+
+The provider will make a request to Zyte API using the ``ZYTE_API_KEY`` and
+``ZYTE_API_URL`` settings. It will ignore the transparent mode and parameter
+mapping settings.
+
+Note that the built-in ``scrapy_poet.page_input_providers.ItemProvider`` has a
+priority of 1000, so when you have page objects producing
+``zyte_common_items.Product`` items you should use higher values for
+``ZyteApiProvider`` if you want these items to come from these page objects,
+and lower values if you want them to come from Zyte API.
+
+Currently, when ``ItemProvider`` is used together with ``ZyteApiProvider``,
+it may make more requests than is optimal: the normal Scrapy response will be
+always requested even when using a ``DummyResponse`` annotation, and in some
+dependency combinations two Zyte API requests will be made for the same page.
+We are planning to solve these problems in the future releases of
+``scrapy-poet`` and ``scrapy-zyte-api``.
+
+.. _scrapy-poet provider: https://scrapy-poet.readthedocs.io/en/stable/providers.html
```

### Comparing `scrapy-zyte-api-0.8.4/README.rst` & `scrapy-zyte-api-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: scrapy-zyte-api
+Version: 0.9.0
+Summary: Client library to process URLs through Zyte API
+Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
+Author: Zyte Group Ltd
+Author-email: info@zyte.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 ===============
 scrapy-zyte-api
 ===============
 
 .. image:: https://img.shields.io/pypi/v/scrapy-zyte-api.svg
    :target: https://pypi.python.org/pypi/scrapy-zyte-api
    :alt: PyPI Version
@@ -597,14 +618,17 @@
 of which parameters you define through ``ZYTE_API_AUTOMAP_PARAMS``. In
 transparent mode, all Scrapy requests go through Zyte API, even requests that
 Scrapy sends automatically, such as those for ``robots.txt`` files when
 ROBOTSTXT_OBEY_ is ``True``, or those for sitemaps when using a `sitemap
 spider`_. Certain parameters, like ``browserHtml`` or ``screenshot``, are not
 meant to be used for every single request.
 
+If the ``zyte_api_default_params`` request meta key is set to ``False``, the
+value of the ``ZYTE_API_DEFAULT_PARAMS`` setting for this request is ignored.
+
 .. _ROBOTSTXT_OBEY: https://docs.scrapy.org/en/latest/topics/settings.html#robotstxt-obey
 .. _sitemap spider: https://docs.scrapy.org/en/latest/topics/spiders.html#sitemapspider
 
 
 Customizing the retry policy
 ============================
 
@@ -787,7 +811,69 @@
 For example::
 
    Sending Zyte API extract request: {"url": "https://example.com", "httpResponseBody": true}
 
 The ``ZYTE_API_LOG_REQUESTS_TRUNCATE``, 64 by default, determines the maximum
 length of any string value in the logged JSON object, excluding object keys. To
 disable truncation, set it to 0.
+
+
+scrapy-poet integration
+=======================
+
+``scrapy-zyte-api`` includes a `scrapy-poet provider`_ that you can use to get
+data from Zyte API in page objects. Enable it in the Scrapy settings::
+
+    SCRAPY_POET_PROVIDERS = {
+        ZyteApiProvider: 1100,
+    }
+
+Request some supported dependencies in the page object::
+
+    @attrs.define
+    class ProductPage(BasePage):
+        response: BrowserResponse
+        product: Product
+
+
+    class ZyteApiSpider(scrapy.Spider):
+        ...
+
+        def parse_page(self, response: DummyResponse, page: ProductPage):
+            ...
+
+Or request them directly in the callback::
+
+    class ZyteApiSpider(scrapy.Spider):
+        ...
+
+        def parse_page(self,
+                       response: DummyResponse,
+                       browser_response: BrowserResponse,
+                       product: Product,
+                       ):
+            ...
+
+The currently supported dependencies are:
+
+* ``web_poet.BrowserHtml``
+* ``web_poet.BrowserResponse``
+* ``zyte_common_items.Product``
+
+The provider will make a request to Zyte API using the ``ZYTE_API_KEY`` and
+``ZYTE_API_URL`` settings. It will ignore the transparent mode and parameter
+mapping settings.
+
+Note that the built-in ``scrapy_poet.page_input_providers.ItemProvider`` has a
+priority of 1000, so when you have page objects producing
+``zyte_common_items.Product`` items you should use higher values for
+``ZyteApiProvider`` if you want these items to come from these page objects,
+and lower values if you want them to come from Zyte API.
+
+Currently, when ``ItemProvider`` is used together with ``ZyteApiProvider``,
+it may make more requests than is optimal: the normal Scrapy response will be
+always requested even when using a ``DummyResponse`` annotation, and in some
+dependency combinations two Zyte API requests will be made for the same page.
+We are planning to solve these problems in the future releases of
+``scrapy-poet`` and ``scrapy-zyte-api``.
+
+.. _scrapy-poet provider: https://scrapy-poet.readthedocs.io/en/stable/providers.html
```

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_cookies.py` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api/_cookies.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_downloader_middleware.py` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api/_downloader_middleware.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_params.py` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api/_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,18 +587,19 @@
             self._warn_on_cookies = settings.getbool("COOKIES_ENABLED")
         self._max_cookies = settings.getint("ZYTE_API_MAX_COOKIES", 100)
         self._crawler = crawler
         self._cookie_jars = None
 
     def parse(self, request):
         dont_merge_cookies = request.meta.get("dont_merge_cookies", False)
+        use_default_params = request.meta.get("zyte_api_default_params", True)
         cookies_enabled = self._cookies_enabled and not dont_merge_cookies
         params = _get_api_params(
             request,
-            default_params=self._default_params,
+            default_params=self._default_params if use_default_params else {},
             transparent_mode=self._transparent_mode,
             automap_params=self._automap_params,
             skip_headers=self._skip_headers,
             browser_headers=self._browser_headers,
             job_id=self._job_id,
             cookies_enabled=cookies_enabled,
             cookie_jars=self._cookie_jars,
```

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_request_fingerprinter.py` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api/_request_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api/handler.py` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api/handler.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api/responses.py` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api/responses.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api/utils.py` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/PKG-INFO` & `scrapy-zyte-api-0.9.0/scrapy_zyte_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-api
-Version: 0.8.4
+Version: 0.9.0
 Summary: Client library to process URLs through Zyte API
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -618,14 +618,17 @@
 of which parameters you define through ``ZYTE_API_AUTOMAP_PARAMS``. In
 transparent mode, all Scrapy requests go through Zyte API, even requests that
 Scrapy sends automatically, such as those for ``robots.txt`` files when
 ROBOTSTXT_OBEY_ is ``True``, or those for sitemaps when using a `sitemap
 spider`_. Certain parameters, like ``browserHtml`` or ``screenshot``, are not
 meant to be used for every single request.
 
+If the ``zyte_api_default_params`` request meta key is set to ``False``, the
+value of the ``ZYTE_API_DEFAULT_PARAMS`` setting for this request is ignored.
+
 .. _ROBOTSTXT_OBEY: https://docs.scrapy.org/en/latest/topics/settings.html#robotstxt-obey
 .. _sitemap spider: https://docs.scrapy.org/en/latest/topics/spiders.html#sitemapspider
 
 
 Customizing the retry policy
 ============================
 
@@ -808,7 +811,69 @@
 For example::
 
    Sending Zyte API extract request: {"url": "https://example.com", "httpResponseBody": true}
 
 The ``ZYTE_API_LOG_REQUESTS_TRUNCATE``, 64 by default, determines the maximum
 length of any string value in the logged JSON object, excluding object keys. To
 disable truncation, set it to 0.
+
+
+scrapy-poet integration
+=======================
+
+``scrapy-zyte-api`` includes a `scrapy-poet provider`_ that you can use to get
+data from Zyte API in page objects. Enable it in the Scrapy settings::
+
+    SCRAPY_POET_PROVIDERS = {
+        ZyteApiProvider: 1100,
+    }
+
+Request some supported dependencies in the page object::
+
+    @attrs.define
+    class ProductPage(BasePage):
+        response: BrowserResponse
+        product: Product
+
+
+    class ZyteApiSpider(scrapy.Spider):
+        ...
+
+        def parse_page(self, response: DummyResponse, page: ProductPage):
+            ...
+
+Or request them directly in the callback::
+
+    class ZyteApiSpider(scrapy.Spider):
+        ...
+
+        def parse_page(self,
+                       response: DummyResponse,
+                       browser_response: BrowserResponse,
+                       product: Product,
+                       ):
+            ...
+
+The currently supported dependencies are:
+
+* ``web_poet.BrowserHtml``
+* ``web_poet.BrowserResponse``
+* ``zyte_common_items.Product``
+
+The provider will make a request to Zyte API using the ``ZYTE_API_KEY`` and
+``ZYTE_API_URL`` settings. It will ignore the transparent mode and parameter
+mapping settings.
+
+Note that the built-in ``scrapy_poet.page_input_providers.ItemProvider`` has a
+priority of 1000, so when you have page objects producing
+``zyte_common_items.Product`` items you should use higher values for
+``ZyteApiProvider`` if you want these items to come from these page objects,
+and lower values if you want them to come from Zyte API.
+
+Currently, when ``ItemProvider`` is used together with ``ZyteApiProvider``,
+it may make more requests than is optimal: the normal Scrapy response will be
+always requested even when using a ``DummyResponse`` annotation, and in some
+dependency combinations two Zyte API requests will be made for the same page.
+We are planning to solve these problems in the future releases of
+``scrapy-poet`` and ``scrapy-zyte-api``.
+
+.. _scrapy-poet provider: https://scrapy-poet.readthedocs.io/en/stable/providers.html
```

### Comparing `scrapy-zyte-api-0.8.4/setup.py` & `scrapy-zyte-api-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import setuptools
 
 setuptools.setup(
     name="scrapy-zyte-api",
-    version="0.8.4",
+    version="0.9.0",
     description="Client library to process URLs through Zyte API",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     author="Zyte Group Ltd",
     author_email="info@zyte.com",
     url="https://github.com/scrapy-plugins/scrapy-zyte-api",
     packages=["scrapy_zyte_api"],
     install_requires=[
-        "packaging>=14.0",
+        "packaging>=20.0",
         "scrapy>=2.0.1",
+        "scrapy-poet>=0.9.0",
+        "web-poet>=0.13.0",
         "zyte-api>=0.4.0",
+        "zyte-common-items",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

