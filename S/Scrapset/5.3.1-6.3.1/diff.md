# Comparing `tmp/Scrapset-5.3.1.tar.gz` & `tmp/Scrapset-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-5.3.1.tar", last modified: Sun Jul 30 10:17:21 2023, max compression
+gzip compressed data, was "Scrapset-6.3.1.tar", last modified: Mon Aug  7 15:52:36 2023, max compression
```

## Comparing `Scrapset-5.3.1.tar` & `Scrapset-6.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 10:17:21.644474 Scrapset-5.3.1/
--rw-rw-rw-   0        0        0     4648 2023-07-30 10:17:21.652452 Scrapset-5.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4417 2023-07-30 04:41:08.000000 Scrapset-5.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 10:17:21.620477 Scrapset-5.3.1/Scrapset/
--rw-rw-rw-   0        0        0    11789 2023-07-30 10:13:44.000000 Scrapset-5.3.1/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       67 2023-07-30 10:14:01.000000 Scrapset-5.3.1/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 10:17:21.644474 Scrapset-5.3.1/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-07-30 04:41:08.000000 Scrapset-5.3.1/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-30 10:17:21.652452 Scrapset-5.3.1/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-07-30 10:16:56.000000 Scrapset-5.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:52:36.244523 Scrapset-6.3.1/
+-rw-rw-rw-   0        0        0     8461 2023-08-07 15:52:36.244523 Scrapset-6.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8230 2023-08-07 15:49:33.000000 Scrapset-6.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 15:52:36.212992 Scrapset-6.3.1/Scrapset/
+-rw-rw-rw-   0        0        0    12991 2023-08-07 15:41:44.000000 Scrapset-6.3.1/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       81 2023-08-07 15:52:26.000000 Scrapset-6.3.1/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:52:36.243526 Scrapset-6.3.1/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     8461 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 15:52:35.000000 Scrapset-6.3.1/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-07-30 04:41:08.000000 Scrapset-6.3.1/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-08-07 15:52:36.252033 Scrapset-6.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-08-07 15:36:08.000000 Scrapset-6.3.1/setup.py
```

### Comparing `Scrapset-5.3.1/Scrapset/Scrapset.py` & `Scrapset-6.3.1/Scrapset/Scrapset.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,8 +239,44 @@
                     time.sleep(1)  # Adjust this delay as needed
 
                 except:
                      break
             driver.quit()
             return corpus  
         except:
-                logging.error("Invalid url")
+                logging.error("Invalid url")
+class vesselfinder:
+    def vessel_details(self,url):
+        try:
+            driver=webdriver.Chrome()
+            c=1
+            text=list()
+            while c<=200:
+                driver.get(url+f'/vessels?page={c}')
+                time.sleep(0.8)
+                cards=driver.find_elements(By.XPATH,'/html/body/div[1]/div/main/div/table')
+
+                for card in cards:
+                    text.append(card.text+'<>')
+                c=c+1
+            driver.quit()
+            return text
+        except:
+            driver.quit()
+            logging.error('Invalid Url')
+    def vessel_location(self,url):
+        try:
+            driver=webdriver.Chrome()
+            c=1
+            text=list()
+            while c<=293:
+                driver.get(url+f'/ports?page={c}')
+                time.sleep(0.4)
+                cards=driver.find_elements(By.XPATH,'/html/body/div[1]/div/main/div[1]/table/tbody/tr')
+                for card in cards:
+                    text.append(card.text+'<>')
+                c=c+1
+            driver.quit()
+            return text
+        except:
+            driver.quit()
+            logging.error('Invalid Url')
```

### Comparing `Scrapset-5.3.1/licence.txt` & `Scrapset-6.3.1/licence.txt`

 * *Files identical despite different names*

