# Comparing `tmp/amazondata-0.0.7.tar.gz` & `tmp/amazondata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazondata-0.0.7.tar", last modified: Sun Oct 23 15:04:31 2022, max compression
+gzip compressed data, was "amazondata-0.0.8.tar", last modified: Mon Aug  7 21:07:10 2023, max compression
```

## Comparing `amazondata-0.0.7.tar` & `amazondata-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anupkumarpanwar   (501) staff       (20)        0 2022-10-23 15:04:31.690197 amazondata-0.0.7/
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1059 2022-10-22 09:27:08.000000 amazondata-0.0.7/LICENSE.txt
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1865 2022-10-23 15:04:31.690065 amazondata-0.0.7/PKG-INFO
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1375 2022-10-23 14:57:39.000000 amazondata-0.0.7/README.md
-drwxr-xr-x   0 anupkumarpanwar   (501) staff       (20)        0 2022-10-23 15:04:31.689103 amazondata-0.0.7/amazondata/
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)      155 2022-10-23 13:45:51.000000 amazondata-0.0.7/amazondata/__init__.py
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     9442 2022-10-23 15:03:35.000000 amazondata-0.0.7/amazondata/product_details_extractor.py
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     3744 2022-10-23 14:20:08.000000 amazondata-0.0.7/amazondata/search_result_extractor.py
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     6795 2022-10-23 12:16:51.000000 amazondata-0.0.7/amazondata/user_agents.py
-drwxr-xr-x   0 anupkumarpanwar   (501) staff       (20)        0 2022-10-23 15:04:31.689889 amazondata-0.0.7/amazondata.egg-info/
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1865 2022-10-23 15:04:31.000000 amazondata-0.0.7/amazondata.egg-info/PKG-INFO
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)      326 2022-10-23 15:04:31.000000 amazondata-0.0.7/amazondata.egg-info/SOURCES.txt
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)        1 2022-10-23 15:04:31.000000 amazondata-0.0.7/amazondata.egg-info/dependency_links.txt
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)       21 2022-10-23 15:04:31.000000 amazondata-0.0.7/amazondata.egg-info/requires.txt
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)       11 2022-10-23 15:04:31.000000 amazondata-0.0.7/amazondata.egg-info/top_level.txt
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)       38 2022-10-23 15:04:31.690249 amazondata-0.0.7/setup.cfg
--rw-r--r--   0 anupkumarpanwar   (501) staff       (20)      850 2022-10-23 15:04:24.000000 amazondata-0.0.7/setup.py
+drwxr-xr-x   0 anupkumarpanwar   (501) staff       (20)        0 2023-08-07 21:07:10.140270 amazondata-0.0.8/
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1059 2023-08-07 21:05:31.000000 amazondata-0.0.8/LICENSE.txt
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1865 2023-08-07 21:07:10.140106 amazondata-0.0.8/PKG-INFO
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1375 2022-10-23 14:57:39.000000 amazondata-0.0.8/README.md
+drwxr-xr-x   0 anupkumarpanwar   (501) staff       (20)        0 2023-08-07 21:07:10.139309 amazondata-0.0.8/amazondata/
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)      155 2022-10-23 13:45:51.000000 amazondata-0.0.8/amazondata/__init__.py
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)    10061 2023-08-07 20:59:56.000000 amazondata-0.0.8/amazondata/product_details_extractor.py
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     3744 2022-10-23 14:20:08.000000 amazondata-0.0.8/amazondata/search_result_extractor.py
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     6795 2022-10-23 12:16:51.000000 amazondata-0.0.8/amazondata/user_agents.py
+drwxr-xr-x   0 anupkumarpanwar   (501) staff       (20)        0 2023-08-07 21:07:10.139901 amazondata-0.0.8/amazondata.egg-info/
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)     1865 2023-08-07 21:07:10.000000 amazondata-0.0.8/amazondata.egg-info/PKG-INFO
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)      326 2023-08-07 21:07:10.000000 amazondata-0.0.8/amazondata.egg-info/SOURCES.txt
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)        1 2023-08-07 21:07:10.000000 amazondata-0.0.8/amazondata.egg-info/dependency_links.txt
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)       21 2023-08-07 21:07:10.000000 amazondata-0.0.8/amazondata.egg-info/requires.txt
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)       11 2023-08-07 21:07:10.000000 amazondata-0.0.8/amazondata.egg-info/top_level.txt
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)       38 2023-08-07 21:07:10.140397 amazondata-0.0.8/setup.cfg
+-rw-r--r--   0 anupkumarpanwar   (501) staff       (20)      850 2023-08-07 21:07:04.000000 amazondata-0.0.8/setup.py
```

### Comparing `amazondata-0.0.7/LICENSE.txt` & `amazondata-0.0.8/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 Anup Kumar Panwar
+Copyright © 2023 Anup Kumar Panwar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `amazondata-0.0.7/PKG-INFO` & `amazondata-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazondata
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to get amazon product and search data in json form. The package does not require any API keys as it works by scraping the amazon page.
 Home-page: https://github.com/AnupKumarPanwar/amazondata
 Download-URL: https://pypi.org/project/amazondata/
 Author: Anup Kumar Panwar
 Author-email: 1anuppanwar@gmail.com
 License: MIT
 Keywords: Amazon,Scraper
```

### Comparing `amazondata-0.0.7/README.md` & `amazondata-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `amazondata-0.0.7/amazondata/product_details_extractor.py` & `amazondata-0.0.8/amazondata/product_details_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,24 +103,37 @@
 class ProductDetailsExtractor:
     def __init__(self):
         self._amazon_product_extractor = Extractor.from_yaml_string(
             YAML_STRING)
 
     def __scrape(self, url):
         headers = {
-            'dnt': '1',
-            'upgrade-insecure-requests': '1',
-            'user-agent': random.choice(user_agents.USER_AGENTS),
-            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-            'sec-fetch-site': 'same-origin',
-            'sec-fetch-mode': 'navigate',
-            'sec-fetch-user': '?1',
-            'sec-fetch-dest': 'document',
-            'referer': 'www.amazon.in',
-            'accept-language': 'en-GB,en-US;q=0.9,en;q=0.8',
+            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,/;q=0.8,application/signed-exchange;v=b3;q=0.7',
+            'Accept-Language': 'en-US,en;q=0.9',
+            'Cache-Control': 'max-age=0',
+            'Connection': 'keep-alive',
+            'Sec-Fetch-Dest': 'document',
+            'Sec-Fetch-Mode': 'navigate',
+            'Sec-Fetch-Site': 'same-origin',
+            'Sec-Fetch-User': '?1',
+            'Upgrade-Insecure-Requests': '1',
+            'User-Agent': 'Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Mobile Safari/537.36',
+            'device-memory': '8',
+            'downlink': '10',
+            'dpr': '2',
+            'ect': '4g',
+            'rtt': '250',
+            'sec-ch-device-memory': '8',
+            'sec-ch-dpr': '2',
+            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
+            'sec-ch-ua-mobile': '?1',
+            'sec-ch-ua-platform': '"Android"',
+            'sec-ch-ua-platform-version': '"6.0"',
+            'sec-ch-viewport-width': '400',
+            'viewport-width': '400'
         }
 
         r = requests.get(url, headers=headers)
 
         if r.status_code > 500:
             raise Exception(
                 "Page %s was blocked by Amazon. Please try using better proxies." % url)
```

### Comparing `amazondata-0.0.7/amazondata/search_result_extractor.py` & `amazondata-0.0.8/amazondata/search_result_extractor.py`

 * *Files identical despite different names*

### Comparing `amazondata-0.0.7/amazondata/user_agents.py` & `amazondata-0.0.8/amazondata/user_agents.py`

 * *Files identical despite different names*

### Comparing `amazondata-0.0.7/amazondata.egg-info/PKG-INFO` & `amazondata-0.0.8/amazondata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazondata
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to get amazon product and search data in json form. The package does not require any API keys as it works by scraping the amazon page.
 Home-page: https://github.com/AnupKumarPanwar/amazondata
 Download-URL: https://pypi.org/project/amazondata/
 Author: Anup Kumar Panwar
 Author-email: 1anuppanwar@gmail.com
 License: MIT
 Keywords: Amazon,Scraper
```

### Comparing `amazondata-0.0.7/setup.py` & `amazondata-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='amazondata',
-    version='0.0.7',
+    version='0.0.8',
     description='A python package to get amazon product and search data in json form. The package does not require any API keys as it works by scraping the amazon page.',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Anup Kumar Panwar',
     author_email='1anuppanwar@gmail.com',
```

