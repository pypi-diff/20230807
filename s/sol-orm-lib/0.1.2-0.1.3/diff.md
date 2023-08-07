# Comparing `tmp/sol_orm_lib-0.1.2.tar.gz` & `tmp/sol_orm_lib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sol_orm_lib-0.1.2.tar", max compression
+gzip compressed data, was "sol_orm_lib-0.1.3.tar", max compression
```

## Comparing `sol_orm_lib-0.1.2.tar` & `sol_orm_lib-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      684 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/README.md
--rw-r--r--   0        0        0      511 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/sol_orm_lib/__init__.py
--rw-r--r--   0        0        0     2742 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/sol_orm_lib/models.py
--rw-r--r--   0        0        0     4646 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/sol_orm_lib/sol_orm.py
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 sol_orm_lib-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      684 2023-08-07 01:25:59.639219 sol_orm_lib-0.1.3/README.md
+-rw-r--r--   0        0        0      511 2023-08-07 01:25:59.639219 sol_orm_lib-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 01:25:59.639219 sol_orm_lib-0.1.3/sol_orm_lib/__init__.py
+-rw-r--r--   0        0        0     2753 2023-08-07 01:25:59.639219 sol_orm_lib-0.1.3/sol_orm_lib/models.py
+-rw-r--r--   0        0        0     5646 2023-08-07 01:25:59.639219 sol_orm_lib-0.1.3/sol_orm_lib/sol_orm.py
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 sol_orm_lib-0.1.3/PKG-INFO
```

### Comparing `sol_orm_lib-0.1.2/README.md` & `sol_orm_lib-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sol_orm_lib-0.1.2/sol_orm_lib/models.py` & `sol_orm_lib-0.1.3/sol_orm_lib/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 #  MeasuredWeather
 # =========================================================================== #
 class MeasuredWeather(BaseModel):
     rad_ar: float
     temp_ar: float
     wind_ar: float
     timestamp: int
-    storeTimestamp: Optional[float] = None
+    storeTimestamp: Optional[int] = None
 
 # =========================================================================== #
 #  MeasuredWeatherTIC
 # =========================================================================== #
 class MeasuredWeatherTIC(BaseModel):
     k: int
     rad_ar: float
     temp_ar: float
     wind_ar: float
-    measuredTimestamp: float
-    storeTimestamp: float
+    measuredTimestamp: int
+    storeTimestamp: Optional[int] = None
 
 # =========================================================================== #
 #  OptimizationParameter
 # =========================================================================== #
 class OptimizationParameter(BaseModel):
     name: str
     value: float
```

### Comparing `sol_orm_lib-0.1.2/sol_orm_lib/sol_orm.py` & `sol_orm_lib-0.1.3/sol_orm_lib/sol_orm.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
            format="<le>[{time:DD-MM-YYYY HH:mm:ss}]</le> <lvl>[{level}]: {message}</lvl>", 
            level="INFO")
 
 
 class SolORM:
     base_url = None
 
+    verify_ssl_certificates = True
+
     # Add Methods
     add_paths = {
         TIC.__name__: "TICs/add",
         TAC.__name__: "TACs/add",
         SpotPublishedTIC.__name__: "SpotPublishedTICs/add",
         SpotEstimatedTIC.__name__: "SpotEstimatedTICs/add",
         ReceivedForecast.__name__: "ReceivedForecasts/add",
@@ -39,14 +41,18 @@
         ReceivedForecast.__name__ : "ReceivedForecasts",
         SAMParameter.__name__: "SAMParameters",
         OptimizationParameter.__name__: "OptimizationParameters",
         MeasuredWeather.__name__:"MeasuredWeathers",
         MeasuredWeatherTIC.__name__: "MeasuredWeatherTICs"
     }
 
+    # Util Methods
+    util_paths = {
+        'CreateTICsAndTACs': "Utilities/CreateTICsAndTACs"
+    }
 
     def __init__(self, base_url=None, debug=False):
         if base_url is not None:
             self.base_url = base_url
         else:
             self.base_url = os.getenv("DB_API_URL")
             if self.base_url is None:
@@ -61,52 +67,67 @@
         return urllib.parse.urljoin(self.base_url, path)
     
     def add_entity(self, entity):
         headers = {'Accept': 'text/plain', 'Content-Type': 'application/json'}
         response = requests.post(
             self.get_url(
                 self.add_paths[entity.__class__.__name__]),
-                json.dumps(entity.dict(exclude_none=True)), headers=headers)
+                json.dumps(entity.dict(exclude_none=True)), headers=headers, verify = self.verify_ssl_certificates)
         
         if response.status_code == 201:
             logger.debug("Request successful")
             return json.loads(response.text)
         else:
             logger.debug(f"{response.status_code}-{response.reason}\n{response.text}")
             raise Exception(f"Request failed with status {response.status_code}")
     
     def get_entity(self, entity_name, id, id2=None):
         headers = {'Accept': 'text/plain', 'Content-Type': 'application/json'}
         endpoint = self.get_url(self.get_paths[entity_name]) + "/" + str(id) + ("/" + str(id2) if id2 is not None else "")        
-        response = requests.get(endpoint, headers=headers)
+        response = requests.get(endpoint, headers=headers, verify = self.verify_ssl_certificates)
         
         if response.status_code == 200:
             logger.debug("Request successful")
             return json.loads(response.text)
         else:
             logger.debug(f"{response.status_code}-{response.reason}\n{response.text}")
             raise Exception(f"Request failed with status {response.status_code}")
     
     def get_last_entity(self, entity_name, number=1):
         headers = {'Accept': 'text/plain', 'Content-Type': 'application/json'}
         endpoint = self.get_url(self.get_paths[entity_name]) + "/getLast/" + str(number)
-        response = requests.get(endpoint, headers=headers)
+        response = requests.get(endpoint, headers=headers, verify = self.verify_ssl_certificates)
         
         if response.status_code == 200:
             logger.debug("Request successful")
             return json.loads(response.text)
         else:
             logger.debug(f"{response.status_code}-{response.reason}\n{response.text}")
             raise Exception(f"Request failed with status {response.status_code}")
     
     def get_since_entity(self, entity_name, since, number=10):
         headers = {'Accept': 'text/plain', 'Content-Type': 'application/json'}
         endpoint = self.get_url(self.get_paths[entity_name]) + "/getSince/" + str(since) + "/" + str(number)
-        response = requests.get(endpoint, headers=headers)
+        response = requests.get(endpoint, headers=headers, verify = self.verify_ssl_certificates)
         
         if response.status_code == 200:
             logger.debug("Request successful")
             return json.loads(response.text)
         else:
             logger.debug(f"{response.status_code}-{response.reason}\n{response.text}")
             raise Exception(f"Request failed with status {response.status_code}")
+        
+    def util_create_TIC_TACs(self, years = 1):
+        headers = {'Accept': 'text/plain', 'Content-Type': 'application/json'}
+        endpoint = self.get_url(self.util_paths['CreateTICsAndTACs'])
+
+        response = requests.post(
+            endpoint,
+            json.dumps({"years": years}), headers=headers, verify = self.verify_ssl_certificates)
+        
+        if response.status_code == 201:
+            logger.debug("Request successful")
+            return json.loads(response.text)
+        else:
+            logger.debug(f"{response.status_code}-{response.reason}\n{response.text}")
+            raise Exception(f"Request failed with status {response.status_code}")
```

### Comparing `sol_orm_lib-0.1.2/PKG-INFO` & `sol_orm_lib-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sol-orm-lib
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/idener/SOL-Python-ORM-Library
 Author: Antonio Gomez
 Author-email: antonio.gomez@idener.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

