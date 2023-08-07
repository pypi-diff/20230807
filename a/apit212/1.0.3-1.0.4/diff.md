# Comparing `tmp/apit212-1.0.3.tar.gz` & `tmp/apit212-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-1.0.3.tar", last modified: Sat Aug  5 11:41:07 2023, max compression
+gzip compressed data, was "apit212-1.0.4.tar", last modified: Mon Aug  7 03:23:46 2023, max compression
```

## Comparing `apit212-1.0.3.tar` & `apit212-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 11:41:07.258344 apit212-1.0.3/
--rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     9396 2023-08-05 11:41:07.255802 apit212-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8629 2023-08-05 08:54:08.000000 apit212-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 11:41:07.204880 apit212-1.0.3/apit212/
--rw-rw-rw-   0        0        0    41429 2023-08-05 11:34:45.000000 apit212-1.0.3/apit212/Apit212.py
--rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.3/apit212/__init__.py
--rw-rw-rw-   0        0        0     1254 2023-08-05 10:09:12.000000 apit212-1.0.3/apit212/apitconstant.py
--rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.3/apit212/cfdScrape.py
-drwxrwxrwx   0        0        0        0 2023-08-05 11:41:07.254791 apit212-1.0.3/apit212.egg-info/
--rw-rw-rw-   0        0        0     9396 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      839 2023-08-05 11:38:51.000000 apit212-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 11:41:07.258344 apit212-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-08-05 10:40:41.000000 apit212-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:23:46.485903 apit212-1.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    11137 2023-08-07 03:23:46.484454 apit212-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10370 2023-08-07 03:22:14.000000 apit212-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 03:23:46.443155 apit212-1.0.4/apit212/
+-rw-rw-rw-   0        0        0    46709 2023-08-07 03:23:06.000000 apit212-1.0.4/apit212/Apit212.py
+-rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.4/apit212/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-08-05 10:09:12.000000 apit212-1.0.4/apit212/apitconstant.py
+-rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.4/apit212/cfdScrape.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:23:46.482462 apit212-1.0.4/apit212.egg-info/
+-rw-rw-rw-   0        0        0    11137 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2023-08-07 02:59:38.000000 apit212-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 03:23:46.488590 apit212-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-08-07 02:59:34.000000 apit212-1.0.4/setup.py
```

### Comparing `apit212-1.0.3/LICENSE` & `apit212-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-1.0.3/PKG-INFO` & `apit212-1.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: apit212
-Version: 1.0.3
-Summary: Unofficial trading212 API
-Home-page: https://github.com/Flock92/aPit212
-Author: Flock92
-Author-email: Flock92 <stuwe_3000@outlook.com>
-Maintainer-email: Flock92 <stuwe_3000@outlook.com>
-License: MIT
-Project-URL: Homepage, https://github.com/Flock92/apit212
-Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
-Keywords: trading,trading212,api,trade,flock92
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires: requests
-Requires: selenium
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
 I will continue to work on this project and would appriciate any feedback. 
 
 ## Requirments
 
@@ -259,36 +237,121 @@
 'open': {'unfilteredCount': 1, 'items': [{'positionId': '********-****-****-****-************', 'humanId': '********',
 'created': '2023-07-03T18:17:46.563+03:00', 'averagePrice': 192.25, 'averagePriceConverted': 150.73025341182984,
 'currentPrice': 192.2, 'value': 1054.82, 'investment': 1055.11, 'code': 'AAPL', 'margin': 212.02, 'ppl': -0.28,
 'quantity': 7, 'maxBuy': 9.0, 'maxSell': 7, 'maxOpenBuy': 2033.0, 'maxOpenSell': 2040.0, 'swap': -1.06, 'frontend': 'WC4'}]}
 
 ```
 
-### Get Ask Price
+### Get live Price
+
+The *live_price* function will return the current ask price for the passed instrument.
+
+```py
+
+ticker = ["TSLA","AAPL","GOOG"]
+
+live_price = client.live_price(instruments=ticker)
+
+print(live_price)
+
+
+```
+
+#### console:
+
+```bash
+
+[{'ticker': 'TSLA', 'price': 253.49}, {'ticker': 'AAPL', 'price': 182.08}, {'ticker': 'GOOG', 'price': 128.44}]
+
+
+```
+
+### Get fast price
+
+The *fast_price* function will return the last qouted chart price as a float
+
+```py
+
+price = client.fast_price(instrument="TSLA")
+
+print(price)
+
+
+```
+
+#### console:
+
+```bash
+
+253.49
+
+```
+
+### Get chart data
+
+the *chart_data* function will return the lastest chart data for passed instrument
+
+```py
+
+chart = client.chart_data(instrument="TSLA")
+
+print(chart)
+
+```
+
+#### console:
+
+```bash
+
+[{'request': {'ticker': 'TSLA', 'period': 'ONE_MINUTE', 'size': 500, 'useAskPrice': False}, 'response': {'candles': [[1691152740000, 259.6, 259.97, 259.43, 259.49, 47], [1691152800000, 259.38, 259.94, 259.17, 259.56, 58], [1691152860000, 259.62, 260.34, 259.62, 260.19, 42]
+
+```
+
+### Get price deviations
 
-The *get_ask* function will return the current ask price for the passed instrument.
+The *get_deviations* function will return price deviations
 
 ```py
 
+ticker = ["TSLA","AAPL","GOOG"]
+
+deviations = client.get_deviations(instruments=ticker)
+
+print(deviations)
 
-ask_price = client.get_ask("TSLA")[0]['response']['price']
+```
+
+#### console:
+
+```bash
 
+[{'request': {'ticker': 'TSLA', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 259.38, 'period': 'd1'}}, {'request': {'ticker': 'AAPL', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 188.99, 'period': 'd1'}}, {'request': {'ticker': 'GOOG', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 129.05, 'period': 'd1'}}]
 
 ```
 
 ### Get Companies
 
 The *get_companies* function will return companies currently listed on T212 & their respective isin ID.
 
 
 ```py
 
 
 companies = client.get_companies()
 
+print(companies)
+
+
+```
+
+#### console:
+
+```bash
+
+[{'ticker': 'SIGTl_EQ', 'isin': 'GB0008769993'}, {'ticker': 'PDYPY_US_EQ', 'isin': 'US3440441026'}...]
 
 ```
 
 ### Limit Order
 The *limit_order* function submit a limit order and takes quantity, target_price, take_profit & stop_loss parms.
 
 ```py
```

### Comparing `apit212-1.0.3/README.md` & `apit212-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: apit212
+Version: 1.0.4
+Summary: Unofficial trading212 API
+Home-page: https://github.com/Flock92/aPit212
+Author: Flock92
+Author-email: Flock92 <stuwe_3000@outlook.com>
+Maintainer-email: Flock92 <stuwe_3000@outlook.com>
+License: MIT
+Project-URL: Homepage, https://github.com/Flock92/apit212
+Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
+Keywords: trading,trading212,api,trade,flock92
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires: requests
+Requires: selenium
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
 I will continue to work on this project and would appriciate any feedback. 
 
 ## Requirments
 
@@ -237,36 +259,121 @@
 'open': {'unfilteredCount': 1, 'items': [{'positionId': '********-****-****-****-************', 'humanId': '********',
 'created': '2023-07-03T18:17:46.563+03:00', 'averagePrice': 192.25, 'averagePriceConverted': 150.73025341182984,
 'currentPrice': 192.2, 'value': 1054.82, 'investment': 1055.11, 'code': 'AAPL', 'margin': 212.02, 'ppl': -0.28,
 'quantity': 7, 'maxBuy': 9.0, 'maxSell': 7, 'maxOpenBuy': 2033.0, 'maxOpenSell': 2040.0, 'swap': -1.06, 'frontend': 'WC4'}]}
 
 ```
 
-### Get Ask Price
+### Get live Price
+
+The *live_price* function will return the current ask price for the passed instrument.
+
+```py
+
+ticker = ["TSLA","AAPL","GOOG"]
+
+live_price = client.live_price(instruments=ticker)
+
+print(live_price)
+
+
+```
+
+#### console:
+
+```bash
+
+[{'ticker': 'TSLA', 'price': 253.49}, {'ticker': 'AAPL', 'price': 182.08}, {'ticker': 'GOOG', 'price': 128.44}]
+
+
+```
+
+### Get fast price
+
+The *fast_price* function will return the last qouted chart price as a float
+
+```py
+
+price = client.fast_price(instrument="TSLA")
+
+print(price)
+
+
+```
+
+#### console:
+
+```bash
+
+253.49
+
+```
+
+### Get chart data
+
+the *chart_data* function will return the lastest chart data for passed instrument
+
+```py
+
+chart = client.chart_data(instrument="TSLA")
+
+print(chart)
+
+```
+
+#### console:
+
+```bash
+
+[{'request': {'ticker': 'TSLA', 'period': 'ONE_MINUTE', 'size': 500, 'useAskPrice': False}, 'response': {'candles': [[1691152740000, 259.6, 259.97, 259.43, 259.49, 47], [1691152800000, 259.38, 259.94, 259.17, 259.56, 58], [1691152860000, 259.62, 260.34, 259.62, 260.19, 42]
+
+```
+
+### Get price deviations
 
-The *get_ask* function will return the current ask price for the passed instrument.
+The *get_deviations* function will return price deviations
 
 ```py
 
+ticker = ["TSLA","AAPL","GOOG"]
+
+deviations = client.get_deviations(instruments=ticker)
+
+print(deviations)
 
-ask_price = client.get_ask("TSLA")[0]['response']['price']
+```
+
+#### console:
+
+```bash
 
+[{'request': {'ticker': 'TSLA', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 259.38, 'period': 'd1'}}, {'request': {'ticker': 'AAPL', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 188.99, 'period': 'd1'}}, {'request': {'ticker': 'GOOG', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 129.05, 'period': 'd1'}}]
 
 ```
 
 ### Get Companies
 
 The *get_companies* function will return companies currently listed on T212 & their respective isin ID.
 
 
 ```py
 
 
 companies = client.get_companies()
 
+print(companies)
+
+
+```
+
+#### console:
+
+```bash
+
+[{'ticker': 'SIGTl_EQ', 'isin': 'GB0008769993'}, {'ticker': 'PDYPY_US_EQ', 'isin': 'US3440441026'}...]
 
 ```
 
 ### Limit Order
 The *limit_order* function submit a limit order and takes quantity, target_price, take_profit & stop_loss parms.
 
 ```py
```

### Comparing `apit212-1.0.3/apit212/Apit212.py` & `apit212-1.0.4/apit212/Apit212.py`

 * *Files 3% similar despite different names*

```diff
@@ -309,39 +309,111 @@
         except requests.exceptions.HTTPError as em:
             return {"code": "HTTPError", "message": em}
         except requests.exceptions.RequestException as em:
             return {"code": "Unknown", "message": em}
 
         return r.json()
     
+    def fast_price(self, instrument: str, _useaskprice: str = "false") -> float:
+        """
+        :param instrument:
+        :return: float
+
+        """
+        payload = {"candles":[{"ticker": f"{instrument}", "useAskPrice": _useaskprice, 
+                                 "period": "ONE_MINUTE", "size": 1}]}
+        try:
+            r = requests.put(f'{self.url}/charting/v3/candles', headers=self.headers,
+                             data=json.dumps(payload))
+        except requests.exceptions.ConnectionError as em:
+            return {"code":"connectionError", "message":em}
+        except requests.exceptions.Timeout as em:
+            return {"code": "requestTimeout", "message": em}
+        except requests.exceptions.HTTPError as em:
+            return {"code": "HTTPError", "message": em}
+        except requests.exceptions.RequestException as em:
+            return {"code": "Unknown", "message": em}
+        
+        price = r.json()
+        result = float(price[0]["response"]["candles"][0][-2])
+
+        return result
+        
+    # GET CHART DATA
+    def chart_data(self, instrument: str, _useaskprice: str = "false", 
+                   period: str = "ONE_MINUTE", size: int = 500) -> list:
+        """
+        :param instruments:
+        :param period: ONE_MINUTE, FIVE_MINUTES, TEN_MINUTES, ONE_MONTH
+        :param _useaskprice:
+        :param size:
+        :return: [{'request': {'ticker': 'TSLA', 'period': 'ONE_MINUTE', 'size': 500, 
+            'useAskPrice': False}, 'response': {'candles': [[1691152740000, 259.6, 259.97, 
+            259.43, 259.49, 47], [1691152800000, 259.38, 259.94, 259.17, 259.56, 58], 
+            [1691152860000, 259.62, 260.34, 259.62, 260.19, 42]
+
+        """
+        payload = {"candles":[{"ticker": f"{instrument}", "useAskPrice": _useaskprice, 
+                                 "period": f"{period}", "size": size}]}
+        
+        try:
+            r = requests.put(f'{self.url}/charting/v3/candles', headers=self.headers,
+                             data=json.dumps(payload))
+        except requests.exceptions.ConnectionError as em:
+            return {"code":"connectionError", "message":em}
+        except requests.exceptions.Timeout as em:
+            return {"code": "requestTimeout", "message": em}
+        except requests.exceptions.HTTPError as em:
+            return {"code": "HTTPError", "message": em}
+        except requests.exceptions.RequestException as em:
+            return {"code": "Unknown", "message": em}
+        
+        return r.json()
+    
     # GET THE CURRENT PRICE
-    def live_price(self, instruments: list, _useaskprice: str = "false"):
+    def live_price(self, instruments: list, 
+                   _useaskprice: str = "false") -> dict:
         """
         :param instruments:
-        :return: 
+        :param _useaskprice:
+        :return: [{'ticker': 'TSLA', 'price': 253.49}, 
+            {'ticker': 'AAPL', 'price': 182.08}, 
+            {'ticker': 'GOOG', 'price': 128.44}]
 
         """
-        payload = []
+        if isinstance(instruments, str) == True:
+            instruments = [f"{instruments}"]
+        else:
+            pass
+        
+        payload = {"candles":[]}
 
         for instrument in instruments:
-            payload.append(dict({"ticker": f"{instrument}", "useAskPrice": f"{_useaskprice}"}))
-
+            payload["candles"].append(dict({"ticker": f"{instrument}", "useAskPrice": _useaskprice, 
+                                 "period": "ONE_MINUTE", "size": 1}))
+       
         try:
-            r = requests.put(f'{self.url}/charting/v1/watchlist/batch/deviations', headers=self.headers,
+            r = requests.put(f'{self.url}/charting/v3/candles', headers=self.headers,
                              data=json.dumps(payload))
         except requests.exceptions.ConnectionError as em:
             return {"code":"connectionError", "message":em}
         except requests.exceptions.Timeout as em:
             return {"code": "requestTimeout", "message": em}
         except requests.exceptions.HTTPError as em:
             return {"code": "HTTPError", "message": em}
         except requests.exceptions.RequestException as em:
             return {"code": "Unknown", "message": em}
+        
+        result = []
+        data = r.json()
+        
+        for i in enumerate(data):
+            result.append(dict({"ticker":data[i[0]]["request"]["ticker"], "price": float(data[i[0]]["response"]["candles"][0][-2])}))
                          
-        return r.json()
+        return result
 
     # GET AUTH VALIDATE
     def auth_validate(self) -> dict:
         """
         :return: {'id': '********-****-****-****-************', 'accountId': ********, 'customerId': ********,
         'tradingType': 'CFD', 'customerUuid': '********-****-****-****-************', 'frontend': 'WC4',
         'readyToTrade': True, 'deviceUuid': ''}
@@ -616,24 +688,33 @@
             return {"code": "HTTPError", "message": em}
         except requests.exceptions.RequestException as em:
             return {"code": "Unknown", "message": em}
         
         return r.json()
 
     # GET ASK PRICE FOR INSTRUMENT
-    def get_deviations(self, instrument: str, _useaskprice: str = "false") -> list:
+    def get_deviations(self, instruments: list, _useaskprice: str = "false") -> list:
         """
 
         :param instrument:
         :param _useaskprice:
         :return: [{'request': {'ticker': '****', 'useAskPrice': False}, 'response':
         {'timestamp': 1687852810000, 'price': 250.37, 'period': 'd1'}}]
         """
 
-        payload = [{"ticker": f"{instrument}", "useAskPrice": f"{_useaskprice}"}]
+        if isinstance(instruments, str) == True:
+            instruments = [f"{instruments}"]
+        else:
+            pass
+        
+
+        payload = []
+
+        for instrument in instruments:
+            payload.append(dict({"ticker": f"{instrument}", "useAskPrice": f"{_useaskprice}"}))
 
         try:
             r = requests.put(f'{self.url}charting/v1/watchlist/batch/deviations',
                              headers=self.headers, data=json.dumps(payload))
         except requests.exceptions.ConnectionError as em:
             return {"code":"connectionError", "message":em}
         except requests.exceptions.Timeout as em:
@@ -946,14 +1027,15 @@
     # VALIDATE SESSION
     def validate_session(self):
         """
         :return: {'id': '*****-********-********-******', 'accountId': **********, 
                 'customerId': *********, 'tradingType': 'CFD', 
                 'customerUuid': '*****-********-********-******', 'frontend': 'WC4', 
                 'readyToTrade': True, 'deviceUuid': ''}
+
         """
         try:
             r = requests.get(f"{self.url}validate-session", headers=self.headers)
         except requests.exceptions.ConnectionError as em:
             return {"code":"connectionError", "message":em}
         except requests.exceptions.Timeout as em:
             return {"code": "requestTimeout", "message": em}
@@ -974,14 +1056,15 @@
         return r
     
     def settings(self, instrument: str):
         """
         :param instrument:
         :return: [{'code': 'TSLA', 'maxBuy': 4.7, 'maxMarketOrderBuy': 1.8, 'maxSell': 4.7, 
                 'maxOpenBuy': 1200.0, 'maxOpenSell': 1200.0, 'suspended': False, 'minTrade': 0.1}]
+
         """
 
         payload = [instrument]
 
         try:
             r = requests.post(f"{self.url}/rest/v2/account/instruments/settings", headers=self.headers,
                               data=json.dumps(payload))
@@ -991,14 +1074,61 @@
             return {"code": "requestTimeout", "message": em}
         except requests.exceptions.HTTPError as em:
             return {"code": "HTTPError", "message": em}
         except requests.exceptions.RequestException as em:
             return {"code": "Unknown", "message": em}
     
         return r.json()
+    
+    def additional_info(self, instrument: str):
+        """
+
+        :param instrument:
+        :return: {code: "STLD_US_CFD", type: "STOCK", margin: 0.2, shortPositionSwap: -0.026087881955975,…}
+
+        """
+
+        params = instrument
+
+        try:
+            r = requests.get(f"{self.url}/rest/v2/instruments/additional-info/", 
+                             headers=self.headers, params=params)
+        except requests.exceptions.ConnectionError as em:
+            return {"code":"connectionError", "message":em}
+        except requests.exceptions.Timeout as em:
+            return {"code": "requestTimeout", "message": em}
+        except requests.exceptions.HTTPError as em:
+            return {"code": "HTTPError", "message": em}
+        except requests.exceptions.RequestException as em:
+            return {"code": "Unknown", "message": em}
+        
+        return r.json()
+    
+    def high_low(self, instrument: str):
+        """
+        :param instrument:
+        :return: {request: {ticker: "EURUSD"}, result: {high: 1.10339, low: 1.10002}}
+        
+        """
+
+        payload = {"ticker": f"{instrument}"}
+
+        try:
+            r = requests.post(f"{self.url}/charting/v2/batch/high-low",
+                              headers=self.headers, data=json.dumps(payload))
+        except requests.exceptions.ConnectionError as em:
+            return {"code":"connectionError", "message":em}
+        except requests.exceptions.Timeout as em:
+            return {"code": "requestTimeout", "message": em}
+        except requests.exceptions.HTTPError as em:
+            return {"code": "HTTPError", "message": em}
+        except requests.exceptions.RequestException as em:
+            return {"code": "Unknown", "message": em}
+        
+        return r.json()
 
     def profit_losses(self, instrument: str):
         """
         :param instrument:
         :return: {'data': [{'profit': 1.28223115578, 'loss': 1.267194029851}], 
                 'size': 1, 'positiveSum': 0, 'negativeSum': 0}
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apit212-1.0.3/apit212/apitconstant.py` & `apit212-1.0.4/apit212/apitconstant.py`

 * *Files identical despite different names*

### Comparing `apit212-1.0.3/apit212/cfdScrape.py` & `apit212-1.0.4/apit212/cfdScrape.py`

 * *Files identical despite different names*

### Comparing `apit212-1.0.3/apit212.egg-info/PKG-INFO` & `apit212-1.0.4/apit212.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
@@ -259,36 +259,121 @@
 'open': {'unfilteredCount': 1, 'items': [{'positionId': '********-****-****-****-************', 'humanId': '********',
 'created': '2023-07-03T18:17:46.563+03:00', 'averagePrice': 192.25, 'averagePriceConverted': 150.73025341182984,
 'currentPrice': 192.2, 'value': 1054.82, 'investment': 1055.11, 'code': 'AAPL', 'margin': 212.02, 'ppl': -0.28,
 'quantity': 7, 'maxBuy': 9.0, 'maxSell': 7, 'maxOpenBuy': 2033.0, 'maxOpenSell': 2040.0, 'swap': -1.06, 'frontend': 'WC4'}]}
 
 ```
 
-### Get Ask Price
+### Get live Price
 
-The *get_ask* function will return the current ask price for the passed instrument.
+The *live_price* function will return the current ask price for the passed instrument.
 
 ```py
 
+ticker = ["TSLA","AAPL","GOOG"]
 
-ask_price = client.get_ask("TSLA")[0]['response']['price']
+live_price = client.live_price(instruments=ticker)
 
+print(live_price)
+
+
+```
+
+#### console:
+
+```bash
+
+[{'ticker': 'TSLA', 'price': 253.49}, {'ticker': 'AAPL', 'price': 182.08}, {'ticker': 'GOOG', 'price': 128.44}]
+
+
+```
+
+### Get fast price
+
+The *fast_price* function will return the last qouted chart price as a float
+
+```py
+
+price = client.fast_price(instrument="TSLA")
+
+print(price)
+
+
+```
+
+#### console:
+
+```bash
+
+253.49
+
+```
+
+### Get chart data
+
+the *chart_data* function will return the lastest chart data for passed instrument
+
+```py
+
+chart = client.chart_data(instrument="TSLA")
+
+print(chart)
+
+```
+
+#### console:
+
+```bash
+
+[{'request': {'ticker': 'TSLA', 'period': 'ONE_MINUTE', 'size': 500, 'useAskPrice': False}, 'response': {'candles': [[1691152740000, 259.6, 259.97, 259.43, 259.49, 47], [1691152800000, 259.38, 259.94, 259.17, 259.56, 58], [1691152860000, 259.62, 260.34, 259.62, 260.19, 42]
+
+```
+
+### Get price deviations
+
+The *get_deviations* function will return price deviations
+
+```py
+
+ticker = ["TSLA","AAPL","GOOG"]
+
+deviations = client.get_deviations(instruments=ticker)
+
+print(deviations)
+
+```
+
+#### console:
+
+```bash
+
+[{'request': {'ticker': 'TSLA', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 259.38, 'period': 'd1'}}, {'request': {'ticker': 'AAPL', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 188.99, 'period': 'd1'}}, {'request': {'ticker': 'GOOG', 'useAskPrice': False}, 'response': {'timestamp': 1691136010000, 'price': 129.05, 'period': 'd1'}}]
 
 ```
 
 ### Get Companies
 
 The *get_companies* function will return companies currently listed on T212 & their respective isin ID.
 
 
 ```py
 
 
 companies = client.get_companies()
 
+print(companies)
+
+
+```
+
+#### console:
+
+```bash
+
+[{'ticker': 'SIGTl_EQ', 'isin': 'GB0008769993'}, {'ticker': 'PDYPY_US_EQ', 'isin': 'US3440441026'}...]
 
 ```
 
 ### Limit Order
 The *limit_order* function submit a limit order and takes quantity, target_price, take_profit & stop_loss parms.
 
 ```py
```

### Comparing `apit212-1.0.3/pyproject.toml` & `apit212-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
 { name= "Flock92", email= "stuwe_3000@outlook.com" },
 ]
 
 maintainers = [
   {name = "Flock92", email = "stuwe_3000@outlook.com"}
 ]
```

### Comparing `apit212-1.0.3/setup.py` & `apit212-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """This is an unofficial API use to interact with the trading212 platform. It is still currently in
                    it's testing stages I created this API to challenge myself and also start creating a portfolio of
                    work that i can showcase to employers"""
 
 setup(
     name="apit212",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     requires=[
         'requests',
         'selenium',
     ],
     author="Flock92",
     author_email="stuwe_3000@outlook.com",
```

