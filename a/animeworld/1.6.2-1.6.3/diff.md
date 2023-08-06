# Comparing `tmp/animeworld-1.6.2.tar.gz` & `tmp/animeworld-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animeworld-1.6.2.tar", last modified: Wed Jul 26 21:52:28 2023, max compression
+gzip compressed data, was "animeworld-1.6.3.tar", last modified: Sun Aug  6 21:57:22 2023, max compression
```

## Comparing `animeworld-1.6.2.tar` & `animeworld-1.6.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.860119 animeworld-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 21:52:18.000000 animeworld-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-26 21:52:28.860119 animeworld-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-26 21:52:18.000000 animeworld-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.856119 animeworld-1.6.2/animeworld/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/episodio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.860119 animeworld-1.6.2/animeworld/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/AnimeWorld_Server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/Streamtape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/YouTube.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.856119 animeworld-1.6.2/animeworld.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:52:28.860119 animeworld-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-26 21:52:18.000000 animeworld-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:57:22.227125 animeworld-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-06 21:57:13.000000 animeworld-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-06 21:57:22.223125 animeworld-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-08-06 21:57:13.000000 animeworld-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:57:22.219125 animeworld-1.6.3/animeworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/episodio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:57:22.223125 animeworld-1.6.3/animeworld/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/servers/AnimeWorld_Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/servers/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/servers/Streamtape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/servers/YouTube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-08-06 21:57:13.000000 animeworld-1.6.3/animeworld/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:57:22.223125 animeworld-1.6.3/animeworld.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-06 21:57:22.000000 animeworld-1.6.3/animeworld.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-06 21:57:22.000000 animeworld-1.6.3/animeworld.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:57:22.000000 animeworld-1.6.3/animeworld.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 21:57:22.000000 animeworld-1.6.3/animeworld.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 21:57:22.000000 animeworld-1.6.3/animeworld.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:57:22.227125 animeworld-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-06 21:57:14.000000 animeworld-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:57:22.223125 animeworld-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:57:14.000000 animeworld-1.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-06 21:57:14.000000 animeworld-1.6.3/tests/test_animeworld.py
```

### Comparing `animeworld-1.6.2/LICENSE` & `animeworld-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.2/PKG-INFO` & `animeworld-1.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animeworld
-Version: 1.6.2
+Version: 1.6.3
 Summary: AnimeWorld UNOFFICIAL API
 Home-page: https://mainkronos.github.io/AnimeWorld-API/
 Author: MainKronos
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animeworld-1.6.2/README.md` & `animeworld-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.2/animeworld/anime.py` & `animeworld-1.6.3/animeworld/anime.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.2/animeworld/episodio.py` & `animeworld-1.6.3/animeworld/episodio.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.2/animeworld/exceptions.py` & `animeworld-1.6.3/animeworld/exceptions.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.2/animeworld/servers/AnimeWorld_Server.py` & `animeworld-1.6.3/animeworld/servers/AnimeWorld_Server.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.2/animeworld/servers/Server.py` & `animeworld-1.6.3/animeworld/servers/Server.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     
     def _fileInfoIn(self) -> Dict[str,str]:
         """
         Recupera le informazioni del file dell'episodio usando httpx.
         """
         url = self.fileLink()
 
-        r = SES.head(url)
+        r = SES.head(url, follow_redirects=True)
         r.raise_for_status()
 
         return {
             "content_type": r.headers['content-type'],
             "total_bytes": int(r.headers['Content-Length']),
             "last_modified": datetime.strptime(r.headers['Last-Modified'], "%a, %d %b %Y %H:%M:%S %Z"),
             "server_name": self.name,
```

### Comparing `animeworld-1.6.2/animeworld/servers/Streamtape.py` & `animeworld-1.6.3/animeworld/servers/Streamtape.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         Example:
           ```py
           return str # Link del file
           ```
         """
         
-        sb_get = SES.get(self.link)
+        sb_get = SES.get(self.link, follow_redirects=True)
 
         if sb_get.status_code == 200:
             soupeddata = BeautifulSoup(sb_get.content, "html.parser")
 
             raw_link = re.search(r"document\.getElementById\('ideoooolink'\)\.innerHTML = (\".*'\))", soupeddata.prettify()).group(1)
 
             raw_link = raw_link.replace('"', '').replace("'", "").replace('+', '')
```

### Comparing `animeworld-1.6.2/animeworld/servers/YouTube.py` & `animeworld-1.6.3/animeworld/servers/YouTube.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.2/animeworld/utility.py` & `animeworld-1.6.3/animeworld/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,29 +111,32 @@
           "malVote": float, # Valutazione di MyanimeList
           "trailer": str # Link del trailer dell'anime
         }
       ]
       ```
     """
 
-    locale.setlocale(locale.LC_TIME, "it_IT.UTF-8")
+    try:
+        locale.setlocale(locale.LC_TIME, "it_IT.UTF-8")
+    except locale.Error:
+        pass
+
     res = SES.post("https://www.animeworld.so/api/search/v2?", params = {"keyword": keyword}, follow_redirects=True)
 
     data = res.json()
     if "error" in data: return []
     data = data["animes"]
 
     for elem in data:
         for k in elem:
             if elem[k] == "??":
                 elem[k] = None
-        if elem["release"].find("??") != -1:
+        if elem["release"] and elem["release"].find("??") != -1:
             elem["release"] = elem["release"].replace("??", "1")
 
-
     data.sort(key=lambda a: a["dub"])
 
     return [
         {
         "id": elem["id"],
         "name": elem["name"],
         "jtitle": elem["jtitle"],
```

### Comparing `animeworld-1.6.2/animeworld.egg-info/PKG-INFO` & `animeworld-1.6.3/animeworld.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animeworld
-Version: 1.6.2
+Version: 1.6.3
 Summary: AnimeWorld UNOFFICIAL API
 Home-page: https://mainkronos.github.io/AnimeWorld-API/
 Author: MainKronos
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animeworld-1.6.2/setup.py` & `animeworld-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="animeworld",
-    version="1.6.2",
+    version="1.6.3",
     author="MainKronos",
     description="AnimeWorld UNOFFICIAL API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mainkronos.github.io/AnimeWorld-API/",
     packages=setuptools.find_packages(),
     install_requires=['httpx', 'httpx[http2]', 'youtube_dl', 'beautifulsoup4'],
```

