# Comparing `tmp/btgsolutions-dataservices-python-client-0.5.tar.gz` & `tmp/btgsolutions-dataservices-python-client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/btgsolutions-dataservices-python-client-0.5.tar", last modified: Fri Aug  4 22:05:43 2023, max compression
+gzip compressed data, was "dist/btgsolutions-dataservices-python-client-0.5.1.tar", last modified: Mon Aug  7 15:38:54 2023, max compression
```

## Comparing `btgsolutions-dataservices-python-client-0.5.tar` & `btgsolutions-dataservices-python-client-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1642 2023-08-04 21:57:33.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/config.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/exceptions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      168 2023-08-04 19:36:26.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1363 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/authenticator.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2646 2023-08-04 22:05:02.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/bulk_data.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3001 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/historical_candles.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/intraday_candles.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7985 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/websocket_client.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/websocket_default_functions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      885 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       67 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/setup.cfg
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-08-04 22:05:30.000000 btgsolutions-dataservices-python-client-0.5/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 15:38:54.000000 btgsolutions-dataservices-python-client-0.5.1/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2375 2023-08-07 15:38:54.000000 btgsolutions-dataservices-python-client-0.5.1/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1594 2023-08-07 15:36:28.000000 btgsolutions-dataservices-python-client-0.5.1/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 15:38:54.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1642 2023-08-04 21:57:33.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/config.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/exceptions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 15:38:54.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      168 2023-08-04 19:36:26.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1363 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/authenticator.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3000 2023-08-07 15:38:42.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/bulk_data.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3001 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/historical_candles.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/intraday_candles.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 15:38:54.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/websocket/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/websocket/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7985 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/websocket/websocket_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/websocket/websocket_default_functions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 15:38:54.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2375 2023-08-07 15:38:53.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      885 2023-08-07 15:38:53.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-08-07 15:38:53.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       83 2023-08-07 15:38:53.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-08-07 15:38:53.000000 btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       82 2023-08-07 15:36:17.000000 btgsolutions-dataservices-python-client-0.5.1/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-08-07 15:38:54.000000 btgsolutions-dataservices-python-client-0.5.1/setup.cfg
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-08-07 15:38:05.000000 btgsolutions-dataservices-python-client-0.5.1/setup.py
```

### Comparing `btgsolutions-dataservices-python-client-0.5/PKG-INFO` & `btgsolutions-dataservices-python-client-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 0.5
+Version: 0.5.1
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # BTG Solutions - Data Service
         
         It's a Python library to get Brazilian Financial Market Data.
@@ -36,12 +36,20 @@
         ```
         ## Example - Plot HistoricalCandles
         ```python
         import btgsolutions_dataservices as btg
         hist_candles = btg.HistoricalCandles(api_key='YOUR_API_KEY')
         hist_candles.get_historical_candles(ticker='PETR4', lookback='5D', mode='absolute').plot(x='date', y='close_price', kind='scatter')
         ```
+        
+        ## Example - BulkData
+        ```python
+        import btgsolutions_dataservices as btg
+        bulk_data = btg.BulkData(api_key='YOUR_API_KEY')
+        bulk_data.get_data(ticker='PETR4', date='2023-07-03', data_type='trades')
+        ```
+        
         ## Documentation
         The official documentation is hosted at https://python-client-docs.dataservices.btgpactualsolutions.com/
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `btgsolutions-dataservices-python-client-0.5/README.md` & `btgsolutions-dataservices-python-client-0.5.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -29,9 +29,17 @@
 ```
 ## Example - Plot HistoricalCandles
 ```python
 import btgsolutions_dataservices as btg
 hist_candles = btg.HistoricalCandles(api_key='YOUR_API_KEY')
 hist_candles.get_historical_candles(ticker='PETR4', lookback='5D', mode='absolute').plot(x='date', y='close_price', kind='scatter')
 ```
+
+## Example - BulkData
+```python
+import btgsolutions_dataservices as btg
+bulk_data = btg.BulkData(api_key='YOUR_API_KEY')
+bulk_data.get_data(ticker='PETR4', date='2023-07-03', data_type='trades')
+```
+
 ## Documentation
 The official documentation is hosted at https://python-client-docs.dataservices.btgpactualsolutions.com/
```

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/config.py` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/config.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/exceptions.py` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/exceptions.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/authenticator.py` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/authenticator.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/bulk_data.py` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/bulk_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Optional
 from ..exceptions import BadResponse
 import requests
 from ..config import url_api_v1
 from .authenticator import Authenticator
 import json
 import pandas as pd
+from io import BytesIO
+import pyarrow.parquet as pq
 
 class BulkData:
     """
     This class provides market data by ticker and date, in .csv format
 
     * Main use case:
 
@@ -65,21 +67,29 @@
         """     
         url = f"{url_api_v1}/marketdata/bulkdata/{data_type}?ticker={ticker}&date={date}"
 
         response = requests.request("GET", url,  headers=self.headers)
         if response.status_code == 200:
 
             try:
-                content_disposition = response.headers.get('Content-Disposition', '')
-                filename = content_disposition.split('filename=')[1]
 
-                # Write the content to a file
-                with open(filename, 'wb') as file:
-                    file.write(response.content)
-                return None
+                if raw_data == False:
+                    parquet_buffer = BytesIO(response.content)
+                    parquet_file = pq.ParquetFile(parquet_buffer)
+                    df = parquet_file.read().to_pandas()
+                    return df
+
+                else:
+                    content_disposition = response.headers.get('Content-Disposition', '')
+                    filename = content_disposition.split('filename=')[1]
+
+                    # Write the content to a file
+                    with open(filename, 'wb') as file:
+                        file.write(response.content)
+                    return None
                 
             except Exception as e:
                 print(f'error while trying to retrieve file:\n{e}')
                 return None
 
         response = json.loads(response.text)
         raise BadResponse(f'Error: {response.get("ApiClientError", "")}.\n{response.get("SuggestedAction", "")}')
```

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/historical_candles.py` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/historical_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/intraday_candles.py` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/rest/intraday_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/websocket_client.py` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/PKG-INFO` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 0.5
+Version: 0.5.1
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # BTG Solutions - Data Service
         
         It's a Python library to get Brazilian Financial Market Data.
@@ -36,12 +36,20 @@
         ```
         ## Example - Plot HistoricalCandles
         ```python
         import btgsolutions_dataservices as btg
         hist_candles = btg.HistoricalCandles(api_key='YOUR_API_KEY')
         hist_candles.get_historical_candles(ticker='PETR4', lookback='5D', mode='absolute').plot(x='date', y='close_price', kind='scatter')
         ```
+        
+        ## Example - BulkData
+        ```python
+        import btgsolutions_dataservices as btg
+        bulk_data = btg.BulkData(api_key='YOUR_API_KEY')
+        bulk_data.get_data(ticker='PETR4', date='2023-07-03', data_type='trades')
+        ```
+        
         ## Documentation
         The official documentation is hosted at https://python-client-docs.dataservices.btgpactualsolutions.com/
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt` & `btgsolutions-dataservices-python-client-0.5.1/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.5/setup.py` & `btgsolutions-dataservices-python-client-0.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open(requirementPath) as f:
             install_requires = f.read().splitlines()
 
 description = "Python package containing several classes and data for extracting and manipulating market and trading data."
 
 setup(
     name='btgsolutions-dataservices-python-client',
-    version='0.5',
+    version='0.5.1',
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="BTG Solutions Data Services powered by BTG Pactual Solutions",
     packages=find_packages(),
     url="https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client",
     install_requires=install_requires,
```

