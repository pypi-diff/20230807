# Comparing `tmp/utilities_hki-0.1.8.tar.gz` & `tmp/utilities_hki-0.1.9.tar.gz`

## Comparing `utilities_hki-0.1.8.tar` & `utilities_hki-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/.gitignore
--rwxr-xr-x   0        0        0    35182 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/LICENSE.txt
--rwxr-xr-x   0        0        0     4496 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/README.md
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/requirements.txt
--rwxr-xr-x   0        0        0   142321 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/dist/utilities_hki-0.1.3-py3-none-any.whl
--rwxr-xr-x   0        0        0   140729 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/dist/utilities_hki-0.1.3.tar.gz
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/__init__.py
--rwxr-xr-x   0        0        0    73470 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/analy_utils.py
--rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/db_utils.py
--rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/email_utils.py
--rwxr-xr-x   0        0        0     5420 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/fb_utils.py
--rwxr-xr-x   0        0        0     1344 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/test.py
--rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_2022-10-23.joblib
--rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_2023-04-02.joblib
--rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
--rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/.gitignore
+-rwxr-xr-x   0        0        0    35182 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/LICENSE.txt
+-rwxr-xr-x   0        0        0     4496 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/README.md
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/requirements.txt
+-rwxr-xr-x   0        0        0   142321 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/dist/utilities_hki-0.1.3-py3-none-any.whl
+-rwxr-xr-x   0        0        0   140729 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/dist/utilities_hki-0.1.3.tar.gz
+-rwxr-xr-x   0        0        0   148110 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/dist/utilities_hki-0.1.8-py3-none-any.whl
+-rwxr-xr-x   0        0        0   423078 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/dist/utilities_hki-0.1.8.tar.gz
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/__init__.py
+-rwxr-xr-x   0        0        0    73470 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/analy_utils.py
+-rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/db_utils.py
+-rwxr-xr-x   0        0        0     4993 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/email_utils.py
+-rwxr-xr-x   0        0        0     5420 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/fb_utils.py
+-rwxr-xr-x   0        0        0     1344 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/test.py
+-rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/data/gmm_2022-10-23.joblib
+-rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/data/gmm_2023-04-02.joblib
+-rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
+-rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 utilities_hki-0.1.9/PKG-INFO
```

### Comparing `utilities_hki-0.1.8/LICENSE.txt` & `utilities_hki-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/README.md` & `utilities_hki-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/pyproject.toml` & `utilities_hki-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "utilities_hki"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Francisco Pena" },
   { name="Colleen Treado" },
 ]
 description = "Global utilities for Humankind data science"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `utilities_hki-0.1.8/dist/utilities_hki-0.1.3-py3-none-any.whl` & `utilities_hki-0.1.9/dist/utilities_hki-0.1.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/dist/utilities_hki-0.1.3.tar.gz` & `utilities_hki-0.1.9/dist/utilities_hki-0.1.3.tar.gz`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/analy_utils.py` & `utilities_hki-0.1.9/src/utilities_hki/analy_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/db_utils.py` & `utilities_hki-0.1.9/src/utilities_hki/db_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/email_utils.py` & `utilities_hki-0.1.9/src/utilities_hki/email_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     port = credentials['port']
     
     # Create a multipart message
     msg = MIMEMultipart()
     msg['From'] = sender
     msg['To'] = receiver
     msg['Subject'] = subject
-    msg.attach(MIMEText(content))
+    msg.attach(MIMEText(content, _subtype='html'))
     msg.add_header('Content-Type', 'text/html')
         
     for path in attachment_paths:
         # Get the file name
         attachment_name = os.path.basename(path)
     
         # Read the attachment file
@@ -158,8 +158,7 @@
         # Add the attachment to the message
         msg.attach(attachment_part)
 
     with smtplib.SMTP('smtp.' + sender.split('@')[1], port) as server:
         server.starttls()
         server.login(sender, passw)
         server.send_message(msg)
-
```

### Comparing `utilities_hki-0.1.8/src/utilities_hki/fb_utils.py` & `utilities_hki-0.1.9/src/utilities_hki/fb_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/test.py` & `utilities_hki-0.1.9/src/utilities_hki/test.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/data/gmm_2022-10-23.joblib` & `utilities_hki-0.1.9/src/utilities_hki/data/gmm_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/data/gmm_2023-04-02.joblib` & `utilities_hki-0.1.9/src/utilities_hki/data/gmm_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib` & `utilities_hki-0.1.9/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib` & `utilities_hki-0.1.9/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.8/PKG-INFO` & `utilities_hki-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilities-hki
-Version: 0.1.8
+Version: 0.1.9
 Summary: Global utilities for Humankind data science
 Project-URL: Homepage, https://github.com/humankind-datascience/utilities-hki
 Author: Francisco Pena, Colleen Treado
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

