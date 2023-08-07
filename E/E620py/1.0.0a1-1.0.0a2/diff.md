# Comparing `tmp/E620py-1.0.0a1.tar.gz` & `tmp/E620py-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E620py-1.0.0a1.tar", last modified: Fri Aug  4 08:48:47 2023, max compression
+gzip compressed data, was "E620py-1.0.0a2.tar", last modified: Mon Aug  7 17:42:30 2023, max compression
```

## Comparing `E620py-1.0.0a1.tar` & `E620py-1.0.0a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:47.580475 E620py-1.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 08:48:38.000000 E620py-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 08:48:47.580475 E620py-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-04 08:48:38.000000 E620py-1.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 08:48:38.000000 E620py-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:48:47.580475 E620py-1.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:47.580475 E620py-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:47.580475 E620py-1.0.0a1/src/E620py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 08:48:47.000000 E620py-1.0.0a1/src/E620py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-04 08:48:47.000000 E620py-1.0.0a1/src/E620py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:48:47.000000 E620py-1.0.0a1/src/E620py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 08:48:47.000000 E620py-1.0.0a1/src/E620py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 08:48:47.000000 E620py-1.0.0a1/src/E620py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-04 08:48:38.000000 E620py-1.0.0a1/src/boom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:47.580475 E620py-1.0.0a1/src/e620py/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-04 08:48:38.000000 E620py-1.0.0a1/src/e620py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-04 08:48:38.000000 E620py-1.0.0a1/src/e620py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-08-04 08:48:38.000000 E620py-1.0.0a1/src/e620py/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-04 08:48:38.000000 E620py-1.0.0a1/src/e620py/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-04 08:48:38.000000 E620py-1.0.0a1/src/e620py/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:30.222029 E620py-1.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 17:42:20.000000 E620py-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 17:42:30.222029 E620py-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-07 17:42:20.000000 E620py-1.0.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-07 17:42:20.000000 E620py-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 17:42:30.222029 E620py-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:30.222029 E620py-1.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:30.222029 E620py-1.0.0a2/src/E620py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 17:42:30.000000 E620py-1.0.0a2/src/E620py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-07 17:42:30.000000 E620py-1.0.0a2/src/E620py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:42:30.000000 E620py-1.0.0a2/src/E620py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 17:42:30.000000 E620py-1.0.0a2/src/E620py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 17:42:30.000000 E620py-1.0.0a2/src/E620py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-07 17:42:20.000000 E620py-1.0.0a2/src/boom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:30.222029 E620py-1.0.0a2/src/e620py/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-07 17:42:20.000000 E620py-1.0.0a2/src/e620py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-07 17:42:20.000000 E620py-1.0.0a2/src/e620py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-08-07 17:42:20.000000 E620py-1.0.0a2/src/e620py/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-07 17:42:20.000000 E620py-1.0.0a2/src/e620py/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-07 17:42:20.000000 E620py-1.0.0a2/src/e620py/utils.py
```

### Comparing `E620py-1.0.0a1/LICENSE` & `E620py-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `E620py-1.0.0a1/PKG-INFO` & `E620py-1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Project-URL: Repository, https://github.com/mrcrabs695/E620py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `E620py-1.0.0a1/pyproject.toml` & `E620py-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `E620py-1.0.0a1/src/E620py.egg-info/PKG-INFO` & `E620py-1.0.0a2/src/E620py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Project-URL: Repository, https://github.com/mrcrabs695/E620py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `E620py-1.0.0a1/src/boom.py` & `E620py-1.0.0a2/src/boom.py`

 * *Files identical despite different names*

### Comparing `E620py-1.0.0a1/src/e620py/handlers.py` & `E620py-1.0.0a2/src/e620py/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,23 +33,25 @@
             item = contained_item
         return item
         
     def get(self, get_options:dict, fetch_count:int = 320, return_request:bool = False) -> list | Response:
         """
         Retrieves up to 320 items from the fetcher specified endpoint
         """
+        logger.debug(f"get args: '{get_options}' fetch count: '{fetch_count}'")
         
         if fetch_count > 320:
             fetch_count = 320
             logger.debug("Fetch count over limit, reduced to 320")
         
         options = {**get_options, 'limit': fetch_count}
         
         try:
             request = self.session.get(url = self.endpoint, params = options)
+            logger.debug(f"request status {request.status_code}")
             request.raise_for_status()
         except HTTPError:
             logger.error("Network error occurred")
             raise NetworkError
         
         decoded_request = self.strip_dict_container(json.loads(request.text))
         if len(decoded_request) < 1:
@@ -86,15 +88,15 @@
             
             for item in loop_objects_list:
                 if len(objects_list) >= fetch_count and not fetch_all:
                     break
                 objects_list.append(item)
                 
             if len(objects_list) >= fetch_count and not fetch_all:
-                    break
+                break
         
         if fetch_all:
             logger.info(f"Fetched {len(objects_list)} {self.type_name}s")
         else:
             logger.info(f"Fetched {len(objects_list)} out of {fetch_count} {self.type_name}s")
         return objects_list 
     
@@ -135,19 +137,20 @@
 class PostHandler(Fetcher):
     def __init__(self, network_client = default_session):
         super().__init__(network_client)
         self.endpoint = "/posts.json"
         self.type_name = "post"
         
     def get_posts(self, tags:str, fetch_count:int = 320, fetch_all:bool = False):
+        logger.info(f"Fetching {fetch_count} posts with the tags: '{tags}'")
         if fetch_all or fetch_count <= 320:
             posts = self.get(get_options = {'tags': tags}, fetch_count = fetch_count)
         else:
             posts = self.looped_get(get_options = {'tags': tags}, fetch_count = fetch_count)
-        
+        logger.info("Fetch done")
         return posts
 
     def vote(self, post_id:int, vote:int) -> int:
         endpoint = f"/posts/{post_id}/votes.json"
         if vote not in [1, -1, 0]:
             logger.warn("Invalid vote, must be '1', '-1' or '0'")
             return 0
@@ -205,14 +208,15 @@
         
         try:
             request = self.session.patch(f"/posts/{post_id}.json", params=post_data)
             request.raise_for_status()
         except HTTPError:
             logger.error(f"A network error occurred. Request status code: {request.status_code}")
             raise NetworkError
+        logger.info(f"Edited post {post_id} successfully")
         return [self.strip_dict_container(json.loads(request.text))]
     
     def upload(self, 
                     tags:str, 
                     rating:str, 
                     source:str, 
                     description:str = None, 
@@ -331,27 +335,29 @@
                 "search[creator_name]": creator_name_search, 
                 "search[category]": search_category, 
                 "search[order]": search_order, 
                 "search[id]": pool_id, 
                 "search[creator_id]": creator_id,
                 "search[is_active]": is_active}
         
+        
         request_args = self.filter_args(request_args)
             
         if search_category not in self.categories and search_category != "":
             logger.warning(f"Search category invalid, must be one of the following {str(self.categories)}")
             raise InvalidArgs
         if search_order not in self.order and search_order != "":
             logger.warning(f"Search order invalid, must be one of the following {str(self.order)}")
             raise InvalidArgs
         
         if fetch_all or fetch_count <= 320:
             pools = self.get(get_options = request_args, fetch_count = fetch_count)
         else:
             pools = self.looped_get(get_options = request_args, fetch_count = fetch_count, fetch_all = fetch_all)
+        logger.info(f"{len(pools)} pools found")
         return pools
 
     def create(self, name:str, description:str, category:str, post_ids:list[int] = []):
         request_args = {"pool[name]": name, "pool[description]": description, "pool[category]": category}
         if post_ids != []:
             request_args = {**request_args, "pool[post_ids][]": post_ids}
         
@@ -370,15 +376,17 @@
                 except KeyError:
                     if status_message["creator"][0] == "have reached the hourly limit for this action":
                         logger.error("Rate limited, try again in an hour")
                         raise RateLimited
             else:
                 logger.error(f"Failed to create pool, a network error occurred. Request status code: {request.status_code}")
                 raise NetworkError
-        return self.strip_dict_container([json.loads(request.text)])
+        pool = self.strip_dict_container([json.loads(request.text)])
+        logger.info(f"Pool made successfully! id: {pool['id']}")
+        return pool
     
     def edit(self, id:int, name:str = None, description:str = None, post_ids:list[int] = None, is_active:bool = None, category:str = None):
         request_args = {"pool[description]": description, "pool[post_ids][]": post_ids, "pool[is_active]": is_active, "pool[category]": category}
         
         request_args = self.filter_args(request_args)
         self.validate_args(request_args)
         
@@ -386,20 +394,22 @@
             request = self.session.put(f"/pools/{id}.json", params = request_args)
             request.raise_for_status()
         except HTTPError:
             #! just going to spit out any errors that happen for now since the site i used to find out the error responses is down i think, i'll figure it out myself later
             logger.error("Unknown error occurred.")
             raise NetworkError(f"Raw response data: {request.text}")
         
+        logger.info(f"Edited pool {id} successfully")
         return self.get({"search[id]": id})
     
     def revert(self, id:int, version_id:int):
         """Revert pool to a previous state (may or may not work)"""
         try:
             request = self.session.put(f"/pools/{id}/revert.json", params = {"version_id": version_id})
             request.raise_for_status()
         except HTTPError:
             #! just going to spit out any errors that happen for now since the site i used to find out the error responses is down i think, i'll figure it out myself later
             logger.error("Unknown error occurred.")
             raise NetworkError(f"Raw response data: {request.text}")
         
+        logger.info(f"Reverted pool {id} to version {version_id}")
         return self.get({"search[id]": id})
```

### Comparing `E620py-1.0.0a1/src/e620py/networking.py` & `E620py-1.0.0a2/src/e620py/networking.py`

 * *Files identical despite different names*

