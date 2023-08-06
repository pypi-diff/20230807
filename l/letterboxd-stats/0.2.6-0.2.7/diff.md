# Comparing `tmp/letterboxd_stats-0.2.6.tar.gz` & `tmp/letterboxd_stats-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.2.6.tar", last modified: Fri Aug  4 09:44:42 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.2.7.tar", last modified: Sun Aug  6 22:10:19 2023, max compression
```

## Comparing `letterboxd_stats-0.2.6.tar` & `letterboxd_stats-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.6/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.6/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-04 09:44:41.997653 letterboxd_stats-0.2.6/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1472 2023-07-30 11:28:06.000000 letterboxd_stats-0.2.6/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5609 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4574 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3074 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2958 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     6619 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      158 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      932 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-06 22:10:19.216074 letterboxd_stats-0.2.7/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.7/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-08-06 22:10:19.216074 letterboxd_stats-0.2.7/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.7/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-06 22:10:19.216074 letterboxd_stats-0.2.7/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1472 2023-07-30 11:28:06.000000 letterboxd_stats-0.2.7/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5609 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.7/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4574 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.7/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3074 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.7/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2958 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.7/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     6515 2023-08-06 22:06:09.000000 letterboxd_stats-0.2.7/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-06 22:10:19.216074 letterboxd_stats-0.2.7/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-08-06 22:10:19.000000 letterboxd_stats-0.2.7/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-08-06 22:10:19.000000 letterboxd_stats-0.2.7/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-08-06 22:10:19.000000 letterboxd_stats-0.2.7/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-08-06 22:10:19.000000 letterboxd_stats-0.2.7/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      158 2023-08-06 22:10:19.000000 letterboxd_stats-0.2.7/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-08-06 22:10:19.000000 letterboxd_stats-0.2.7/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      932 2023-08-06 09:47:19.000000 letterboxd_stats-0.2.7/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-08-06 22:10:19.216074 letterboxd_stats-0.2.7/setup.cfg
```

### Comparing `letterboxd_stats-0.2.6/LICENCE` & `letterboxd_stats-0.2.7/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.6/PKG-INFO` & `letterboxd_stats-0.2.7/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd_stats
-Version: 0.2.6
+Name: letterboxd-stats
+Version: 0.2.7
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.6/README.md` & `letterboxd_stats-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.6/letterboxd_stats/__init__.py` & `letterboxd_stats-0.2.7/letterboxd_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.6/letterboxd_stats/cli.py` & `letterboxd_stats-0.2.7/letterboxd_stats/cli.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.6/letterboxd_stats/data.py` & `letterboxd_stats-0.2.7/letterboxd_stats/data.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.6/letterboxd_stats/main.py` & `letterboxd_stats-0.2.7/letterboxd_stats/main.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.6/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.2.7/letterboxd_stats/tmdb.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.6/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.2.7/letterboxd_stats/web_scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,20 +109,21 @@
         raise ValueError("No Movie link found")
     id = tmdb_link[0].get("href").split("/")[-2]
     return int(id)
 
 
 def get_tmdb_id(link: str, is_diary=False):
     tmdb_id_cache = shelve.open(cache_path, writeback=False, protocol=5)
-    if link in tmdb_id_cache:
-        id = tmdb_id_cache[link]
+    key = link.split("/")[-1]
+    if key in tmdb_id_cache:
+        id = tmdb_id_cache[key]
     else:
         try:
             id = _get_tmdb_id_from_web(link, is_diary)
-            tmdb_id_cache[link] = id
+            tmdb_id_cache[key] = id
         except ValueError as e:
             print(e)
             id = None
     tmdb_id_cache.close()
     return id
 
 
@@ -136,21 +137,20 @@
     if res.status_code != 200:
         raise ConnectionError("It's been impossible to retireve the Letterboxd page")
     search_page = html.fromstring(res.text)
     if allow_selection:
         movie_list = search_page.xpath("//div[@class='film-detail-content']")
         if len(movie_list) == 0:
             raise ValueError(f"No film found with search query {title}")
-        titles = [movie.xpath("./h2/span/a")[0].text.rstrip() for movie in movie_list]
-        years = [
-            f"({year[0].text}) " if len(year := movie.xpath("./h2/span//small/a")) > 0 else "" for movie in movie_list
-        ]
-        directors = [director[0].text if len(director := movie.xpath("./p/a")) > 0 else "" for movie in movie_list]
-        links = [movie.xpath("./h2/span/a")[0].get("href") for movie in movie_list]
-        title_years_directors_links = {
-            f"{title} {year}- {director}": link for title, year, director, link in zip(titles, years, directors, links)
-        }
+        title_years_directors_links = {}
+        for movie in movie_list:
+            title = movie.xpath("./h2/span/a")[0].text.rstrip()
+            director = director[0].text if len(director := movie.xpath("./p/a")) > 0 else ""
+            year = f"({year[0].text}) " if len(year := movie.xpath("./h2/span//small/a")) > 0 else ""
+            link = movie.xpath("./h2/span/a")[0].get("href")
+            title_years_directors_links[f"{title} {year}- {director}"] = link
+
         selected_film = cli.select_value(list(title_years_directors_links.keys()), "Select your film")
         title_url = title_years_directors_links[selected_film].split("/")[-2]
     else:
         title_url = search_page.xpath("//span[@class='film-title-wrapper']/a")[0].get("href").split("/")[-2]
     return title_url
```

### Comparing `letterboxd_stats-0.2.6/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd-stats
-Version: 0.2.6
+Name: letterboxd_stats
+Version: 0.2.7
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.6/pyproject.toml` & `letterboxd_stats-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.2.6"
+version = "0.2.7"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

