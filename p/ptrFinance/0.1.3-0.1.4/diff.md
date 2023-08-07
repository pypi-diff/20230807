# Comparing `tmp/ptrFinance-0.1.3.tar.gz` & `tmp/ptrFinance-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptrFinance-0.1.3.tar", last modified: Sun May 28 02:10:52 2023, max compression
+gzip compressed data, was "ptrFinance-0.1.4.tar", last modified: Mon Aug  7 00:16:43 2023, max compression
```

## Comparing `ptrFinance-0.1.3.tar` & `ptrFinance-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.433061 ptrFinance-0.1.3/
--rw-rw-rw-   0        0        0     2645 2023-05-28 02:09:26.000000 ptrFinance-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-02-08 18:15:55.000000 ptrFinance-0.1.3/LICENCE.txt
--rw-rw-rw-   0        0        0       39 2023-02-14 00:15:14.000000 ptrFinance-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3624 2023-05-28 02:10:52.433061 ptrFinance-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-03-19 01:05:14.000000 ptrFinance-0.1.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.416984 ptrFinance-0.1.3/ptrFinance/
--rw-rw-rw-   0        0        0    23005 2023-05-27 15:19:31.000000 ptrFinance-0.1.3/ptrFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.432041 ptrFinance-0.1.3/ptrFinance/__pycache__/
--rw-rw-rw-   0        0        0     1374 2023-02-13 23:43:16.000000 ptrFinance-0.1.3/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc
--rw-rw-rw-   0        0        0       38 2023-02-14 11:26:40.000000 ptrFinance-0.1.3/ptrFinance/repetitionCSV.csv
-drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.426537 ptrFinance-0.1.3/ptrFinance.egg-info/
--rw-rw-rw-   0        0        0     3624 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-05-28 02:10:52.000000 ptrFinance-0.1.3/ptrFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 02:10:52.434425 ptrFinance-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-05-28 02:09:08.000000 ptrFinance-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:16:43.849149 ptrFinance-0.1.4/
+-rw-rw-rw-   0        0        0     2844 2023-08-07 00:06:55.000000 ptrFinance-0.1.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-02-08 18:15:55.000000 ptrFinance-0.1.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       39 2023-02-14 00:15:14.000000 ptrFinance-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3823 2023-08-07 00:16:43.849149 ptrFinance-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-03-19 01:05:14.000000 ptrFinance-0.1.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 00:16:43.838146 ptrFinance-0.1.4/ptrFinance/
+-rw-rw-rw-   0        0        0    24790 2023-08-07 00:01:03.000000 ptrFinance-0.1.4/ptrFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:16:43.848148 ptrFinance-0.1.4/ptrFinance/__pycache__/
+-rw-rw-rw-   0        0        0     1374 2023-02-13 23:43:16.000000 ptrFinance-0.1.4/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc
+-rw-rw-rw-   0        0        0       38 2023-02-14 11:26:40.000000 ptrFinance-0.1.4/ptrFinance/repetitionCSV.csv
+drwxrwxrwx   0        0        0        0 2023-08-07 00:16:43.843147 ptrFinance-0.1.4/ptrFinance.egg-info/
+-rw-rw-rw-   0        0        0     3823 2023-08-07 00:16:43.000000 ptrFinance-0.1.4/ptrFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-08-07 00:16:43.000000 ptrFinance-0.1.4/ptrFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 00:16:43.000000 ptrFinance-0.1.4/ptrFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-07 00:16:43.000000 ptrFinance-0.1.4/ptrFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 00:16:43.000000 ptrFinance-0.1.4/ptrFinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 00:16:43.850149 ptrFinance-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-08-07 00:07:11.000000 ptrFinance-0.1.4/setup.py
```

### Comparing `ptrFinance-0.1.3/CHANGELOG.txt` & `ptrFinance-0.1.4/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Change Log
 ==========
-Version "0.1.2" (2/30/2023)
+Version "0.1.4" (8/7/2023)
+Stock volatility given a specific time period function added (NO MORE THAN 4 MONTHS)
+Will change to selenium for it later on, and add another function for custom data
+
+Version "0.1.3" (5/28/2023)
 getLiveValues function added
 
 Version "0.1.2" (2/30/2023)
 returnDailyStockReviewArticle different companies bug fix
 
 Version "0.1.1" (2/30/2023)
 Bug Fix
```

### Comparing `ptrFinance-0.1.3/LICENCE.txt` & `ptrFinance-0.1.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ptrFinance-0.1.3/PKG-INFO` & `ptrFinance-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptrFinance
-Version: 0.1.3
+Version: 0.1.4
 Summary: Financial Web Scraping Library
 Home-page: 
 Author: Rocco Pio Maria Petruccio
 Author-email: whatsappbackuprocco@gmail.com
 License: MIT
 Keywords: Web Scraping,Finance
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,19 @@
 Documentation is the process of being created to improve the ease of use of the library.
 
 The GitHub repository is located at: https://github.com/123Rocco123/Web-Scraping-Pip-Library
 
 
 Change Log
 ==========
-Version "0.1.2" (2/30/2023)
+Version "0.1.4" (8/7/2023)
+Stock volatility given a specific time period function added (NO MORE THAN 4 MONTHS)
+Will change to selenium for it later on, and add another function for custom data
+
+Version "0.1.3" (5/28/2023)
 getLiveValues function added
 
 Version "0.1.2" (2/30/2023)
 returnDailyStockReviewArticle different companies bug fix
 
 Version "0.1.1" (2/30/2023)
 Bug Fix
```

### Comparing `ptrFinance-0.1.3/ptrFinance/__init__.py` & `ptrFinance-0.1.4/ptrFinance/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import time
 import os
 import csv
 # Used to search using our default webbrowser
 import webbrowser
 
 import pandas as pd
+import numpy as np
 
 from requests_html import HTMLSession
 from bs4 import BeautifulSoup
 from datetime import datetime
 from csv import writer
 
 # Class Variable
@@ -28,14 +29,16 @@
         soup = BeautifulSoup(stockValues, "html5lib")
 
         # Append the stock with the current value
         liveValues[x] = soup.find("fin-streamer", {"class" : "Fw(b) Fz(36px) Mb(-4px) D(ib)"}).text
 
     return liveValues
 
+#print(float(list(getLiveValues(["AMD"]).values())[0]))
+
 # Used for the whileTrueStock
 def repetitionsFunc(stockName, interval, repetitions):
     global previousVol
 
     session = HTMLSession()
     requests = session.get("https://finance.yahoo.com/quote/{stockName}/history?p={stockName}".format(stockName = stockName)).text
 
@@ -441,7 +444,47 @@
     # If-Else block used to return either a string or an array output
         # The string output is to format the volatility for the users
         # The array output gives the float values to allow users to add that information to their files or for calculations
     if stringOutput == True:
         return "Current Volatility: {volatilityPercent}\nPrevious Volatility: {previousVolatilityPercent}\nPercentage Difference: {percentageDifference}".format(volatilityPercent = volatilityPercent, previousVolatilityPercent = previousVolatilityPercent, percentageDifference = percentageDifference)
     else:
         return [float(volatilityPercent.replace("%", "")), float(previousVolatilityPercent), float(percentageDifference)]
+
+# Function used to return the volatility of a given time set
+def returnVolatilityGivenTime(stockName, numberOfDays):
+    # Requests is used to get the HTML page that we need to parse over
+    session = HTMLSession()
+    # Link used to contain the google finance page of the chosen stock
+    page = session.get("https://finance.yahoo.com/quote/{stockName}/history?p={stockName}".format(stockName = stockName)).text
+
+    soup = BeautifulSoup(page, "html5lib")
+    # Variable used to contain the table with the historic data
+    historicData = soup.find("table", {"class" : "W(100%) M(0)"}).findAll("tr")[1:]
+    # Array used to contain the closedValues
+    closedValues = []
+
+    print(historicData[len(historicData) - 2])
+
+    currentDays = 1
+    for x in historicData:
+        for dataPoints in x:
+            if (x.index(dataPoints) % 4 == 0 and x.index(dataPoints) != 0) and currentDays <= numberOfDays + 1:
+                closedValues.append(float(dataPoints.text))
+                currentDays += 1
+
+    # Memory Management
+    del session, page, soup, historicData, currentDays
+
+    # Used to calculate the daily returns of the stock over the week
+    dailyReturn = [closedValues[x] - closedValues[x - 1] for x in range(1, 8)]
+    # Contains the average daily return
+    averageReturn = np.average(dailyReturn)
+    # Contains the squared differences for each daily return
+    dailyReturn = [(x - averageReturn) ** 2 for x in dailyReturn]
+    # Save Memory
+    del averageReturn
+    # Contains the variance
+    varianceOfSquaredDiff = sum(dailyReturn) / 7
+    del dailyReturn
+
+    # Returns the volatility of the stock
+    return np.sqrt(varianceOfSquaredDiff)
```

### Comparing `ptrFinance-0.1.3/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc` & `ptrFinance-0.1.4/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ptrFinance-0.1.3/ptrFinance.egg-info/PKG-INFO` & `ptrFinance-0.1.4/ptrFinance.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptrFinance
-Version: 0.1.3
+Version: 0.1.4
 Summary: Financial Web Scraping Library
 Home-page: 
 Author: Rocco Pio Maria Petruccio
 Author-email: whatsappbackuprocco@gmail.com
 License: MIT
 Keywords: Web Scraping,Finance
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,19 @@
 Documentation is the process of being created to improve the ease of use of the library.
 
 The GitHub repository is located at: https://github.com/123Rocco123/Web-Scraping-Pip-Library
 
 
 Change Log
 ==========
-Version "0.1.2" (2/30/2023)
+Version "0.1.4" (8/7/2023)
+Stock volatility given a specific time period function added (NO MORE THAN 4 MONTHS)
+Will change to selenium for it later on, and add another function for custom data
+
+Version "0.1.3" (5/28/2023)
 getLiveValues function added
 
 Version "0.1.2" (2/30/2023)
 returnDailyStockReviewArticle different companies bug fix
 
 Version "0.1.1" (2/30/2023)
 Bug Fix
```

### Comparing `ptrFinance-0.1.3/setup.py` & `ptrFinance-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='ptrFinance',
-  version='0.1.3',
+  version='0.1.4',
   description='Financial Web Scraping Library',
   long_description= open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',
   author='Rocco Pio Maria Petruccio',
   author_email='whatsappbackuprocco@gmail.com',
   license='MIT',
   classifiers=classifiers,
   keywords=["Web Scraping", "Finance"],
   packages=find_packages(),
-  install_requires=['bs4', "requests_html", "requests", "pandas"]
+  install_requires=['bs4', "requests_html", "requests", "pandas", "numpy"]
 )
```

