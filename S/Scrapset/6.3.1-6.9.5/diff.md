# Comparing `tmp/Scrapset-6.3.1.tar.gz` & `tmp/Scrapset-6.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-6.3.1.tar", last modified: Mon Aug  7 15:52:36 2023, max compression
+gzip compressed data, was "Scrapset-6.9.5.tar", last modified: Mon Aug  7 17:11:56 2023, max compression
```

## Comparing `Scrapset-6.3.1.tar` & `Scrapset-6.9.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 15:52:36.244523 Scrapset-6.3.1/
--rw-rw-rw-   0        0        0     8461 2023-08-07 15:52:36.244523 Scrapset-6.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     8230 2023-08-07 15:49:33.000000 Scrapset-6.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 15:52:36.212992 Scrapset-6.3.1/Scrapset/
--rw-rw-rw-   0        0        0    12991 2023-08-07 15:41:44.000000 Scrapset-6.3.1/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       81 2023-08-07 15:52:26.000000 Scrapset-6.3.1/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 15:52:36.243526 Scrapset-6.3.1/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     8461 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-07-30 04:41:08.000000 Scrapset-6.3.1/licence.txt
--rw-rw-rw-   0        0        0      158 2023-08-07 15:52:36.252033 Scrapset-6.3.1/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-08-07 15:36:08.000000 Scrapset-6.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:11:56.819665 Scrapset-6.9.5/
+-rw-rw-rw-   0        0        0     8276 2023-08-07 17:11:56.820662 Scrapset-6.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8045 2023-08-07 16:27:51.000000 Scrapset-6.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 17:11:56.786642 Scrapset-6.9.5/Scrapset/
+-rw-rw-rw-   0        0        0    12999 2023-08-07 17:09:52.000000 Scrapset-6.9.5/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       81 2023-08-07 15:52:26.000000 Scrapset-6.9.5/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:11:56.818665 Scrapset-6.9.5/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     8276 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-07-30 04:41:08.000000 Scrapset-6.9.5/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-08-07 17:11:56.823188 Scrapset-6.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-08-07 17:11:41.000000 Scrapset-6.9.5/setup.py
```

### Comparing `Scrapset-6.3.1/PKG-INFO` & `Scrapset-6.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 6.3.1
+Version: 6.9.5
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
@@ -120,15 +120,15 @@
 
 df = m.imdb()
 data = df.comments('https://www.imdb.com/title/tt0111161/reviews')
 ```
 
 Please note that you should replace the URL `'https://www.imdb.com/title/tt0111161/reviews'` with the IMDb movie page URL you want to scrape comments from. 
 
-Sure! Let's continue with the documentation for the `VesselFinder` class:
+
 
 # VesselFinder Class
 
 The VesselFinder class facilitates scraping vessel details and locations.
 
 ## Methods
 
@@ -160,15 +160,14 @@
     Returns:
         List[str]: A list containing the scraped vessel locations.
     """
 ```
 
 ## Example Code
 
-Here's an example code demonstrating how to use the VesselFinder class to scrape vessel details and locations:
 
 ```python
 import scrapset as m
 
 df = m.VesselFinder()
 
 # Scrape vessel details
```

### Comparing `Scrapset-6.3.1/README.md` & `Scrapset-6.9.5/Scrapset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: Scrapset
+Version: 6.9.5
+Summary: DataScraper: Effortless Dataset Extraction
+Author: Ibrahim
+Author-email: string2025@gmail.com
+Description-Content-Type: text/markdown
+License-File: licence.txt
+
 # Dataset Scraper (Scrapset)
 
 
 
 Scrapset is a Python module specifically created for web scraping data from websites like Kaggle and Data.gov. It simplifies the task of extracting dataset information such as titles, upvotes (for Kaggle), and recent views (for Data.gov).
 
 By utilizing the Scrapset module, you can automate the retrieval of dataset details from these platforms. This can be beneficial for various purposes such as data analysis, research, or developing machine learning models. The module employs the Selenium library to interact with the websites and extract the desired data.
@@ -111,15 +120,15 @@
 
 df = m.imdb()
 data = df.comments('https://www.imdb.com/title/tt0111161/reviews')
 ```
 
 Please note that you should replace the URL `'https://www.imdb.com/title/tt0111161/reviews'` with the IMDb movie page URL you want to scrape comments from. 
 
-Sure! Let's continue with the documentation for the `VesselFinder` class:
+
 
 # VesselFinder Class
 
 The VesselFinder class facilitates scraping vessel details and locations.
 
 ## Methods
 
@@ -151,15 +160,14 @@
     Returns:
         List[str]: A list containing the scraped vessel locations.
     """
 ```
 
 ## Example Code
 
-Here's an example code demonstrating how to use the VesselFinder class to scrape vessel details and locations:
 
 ```python
 import scrapset as m
 
 df = m.VesselFinder()
 
 # Scrape vessel details
```

### Comparing `Scrapset-6.3.1/Scrapset/Scrapset.py` & `Scrapset-6.9.5/Scrapset/Scrapset.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,34 +249,34 @@
         try:
             driver=webdriver.Chrome()
             c=1
             text=list()
             while c<=200:
                 driver.get(url+f'/vessels?page={c}')
                 time.sleep(0.8)
-                cards=driver.find_elements(By.XPATH,'/html/body/div[1]/div/main/div/table')
-
+                cards=driver.find_elements(By.XPATH,'/html/body/div[1]/div/main/div/table/tbody/tr')
                 for card in cards:
                     text.append(card.text+'<>')
                 c=c+1
             driver.quit()
             return text
         except:
             driver.quit()
             logging.error('Invalid Url')
     def vessel_location(self,url):
         try:
             driver=webdriver.Chrome()
             c=1
             text=list()
-            while c<=293:
+            while c<=10:
                 driver.get(url+f'/ports?page={c}')
                 time.sleep(0.4)
                 cards=driver.find_elements(By.XPATH,'/html/body/div[1]/div/main/div[1]/table/tbody/tr')
                 for card in cards:
                     text.append(card.text+'<>')
                 c=c+1
             driver.quit()
             return text
         except:
             driver.quit()
             logging.error('Invalid Url')
+
```

### Comparing `Scrapset-6.3.1/Scrapset.egg-info/PKG-INFO` & `Scrapset-6.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: Scrapset
-Version: 6.3.1
-Summary: DataScraper: Effortless Dataset Extraction
-Author: Ibrahim
-Author-email: string2025@gmail.com
-Description-Content-Type: text/markdown
-License-File: licence.txt
-
 # Dataset Scraper (Scrapset)
 
 
 
 Scrapset is a Python module specifically created for web scraping data from websites like Kaggle and Data.gov. It simplifies the task of extracting dataset information such as titles, upvotes (for Kaggle), and recent views (for Data.gov).
 
 By utilizing the Scrapset module, you can automate the retrieval of dataset details from these platforms. This can be beneficial for various purposes such as data analysis, research, or developing machine learning models. The module employs the Selenium library to interact with the websites and extract the desired data.
@@ -120,15 +111,15 @@
 
 df = m.imdb()
 data = df.comments('https://www.imdb.com/title/tt0111161/reviews')
 ```
 
 Please note that you should replace the URL `'https://www.imdb.com/title/tt0111161/reviews'` with the IMDb movie page URL you want to scrape comments from. 
 
-Sure! Let's continue with the documentation for the `VesselFinder` class:
+
 
 # VesselFinder Class
 
 The VesselFinder class facilitates scraping vessel details and locations.
 
 ## Methods
 
@@ -160,15 +151,14 @@
     Returns:
         List[str]: A list containing the scraped vessel locations.
     """
 ```
 
 ## Example Code
 
-Here's an example code demonstrating how to use the VesselFinder class to scrape vessel details and locations:
 
 ```python
 import scrapset as m
 
 df = m.VesselFinder()
 
 # Scrape vessel details
```

### Comparing `Scrapset-6.3.1/licence.txt` & `Scrapset-6.9.5/licence.txt`

 * *Files identical despite different names*

