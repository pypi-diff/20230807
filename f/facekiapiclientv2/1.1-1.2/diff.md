# Comparing `tmp/facekiapiclientv2-1.1.tar.gz` & `tmp/facekiapiclientv2-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facekiapiclientv2-1.1.tar", last modified: Thu Jun 15 13:34:09 2023, max compression
+gzip compressed data, was "facekiapiclientv2-1.2.tar", last modified: Mon Aug  7 09:25:15 2023, max compression
```

## Comparing `facekiapiclientv2-1.1.tar` & `facekiapiclientv2-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:34:09.342960 facekiapiclientv2-1.1/
--rw-rw-rw-   0        0        0     3068 2023-06-15 13:34:09.339773 facekiapiclientv2-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2447 2023-06-15 13:26:07.000000 facekiapiclientv2-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 13:34:09.333724 facekiapiclientv2-1.1/faceki-kyc-python/
--rw-rw-rw-   0        0        0       72 2023-06-15 13:23:35.000000 facekiapiclientv2-1.1/faceki-kyc-python/__init__.py
--rw-rw-rw-   0        0        0     4534 2023-06-15 13:23:00.000000 facekiapiclientv2-1.1/faceki-kyc-python/client.py
--rw-rw-rw-   0        0        0      198 2023-06-14 13:21:15.000000 facekiapiclientv2-1.1/faceki-kyc-python/test.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:34:09.338765 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/
--rw-rw-rw-   0        0        0     3068 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 13:34:09.342960 facekiapiclientv2-1.1/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-06-15 13:33:59.000000 facekiapiclientv2-1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-07 09:25:15.718212 facekiapiclientv2-1.2/
+-rwxrwxrwx   0 root         (0) root         (0)     2923 2023-08-07 09:25:15.718002 facekiapiclientv2-1.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2447 2023-08-07 09:25:08.162448 facekiapiclientv2-1.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-07 09:25:15.715000 facekiapiclientv2-1.2/faceki-kyc-python/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-06-15 13:23:35.000000 facekiapiclientv2-1.2/faceki-kyc-python/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5974 2023-08-07 09:19:55.000000 facekiapiclientv2-1.2/faceki-kyc-python/client.py
+-rwxrwxrwx   0 root         (0) root         (0)      322 2023-08-07 09:23:20.000000 facekiapiclientv2-1.2/faceki-kyc-python/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-07 09:25:15.717436 facekiapiclientv2-1.2/facekiapiclientv2.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     2923 2023-08-07 09:25:15.000000 facekiapiclientv2-1.2/facekiapiclientv2.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      306 2023-08-07 09:25:15.000000 facekiapiclientv2-1.2/facekiapiclientv2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-07 09:25:15.000000 facekiapiclientv2-1.2/facekiapiclientv2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-08-07 09:25:15.000000 facekiapiclientv2-1.2/facekiapiclientv2.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-08-07 09:25:15.000000 facekiapiclientv2-1.2/facekiapiclientv2.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-07 09:25:15.718365 facekiapiclientv2-1.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      867 2023-08-07 09:24:54.000000 facekiapiclientv2-1.2/setup.py
```

### Comparing `facekiapiclientv2-1.1/PKG-INFO` & `facekiapiclientv2-1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,86 @@
-Metadata-Version: 2.1
-Name: facekiapiclientv2
-Version: 1.1
-Summary: FACEKI KYC Api Library
-Home-page: UNKNOWN
-Author: Faceki
-Author-email: haziq@faceki.com
-License: UNKNOWN
-Keywords: api,client,library
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
-# FacekiAPIClientV2
-
-The `FacekiAPIClientV2` is a Python client for interacting with the Faceki API. It provides methods to generate an access token, perform various KYC (Know Your Customer) operations, and retrieve KYC records.
-
-## Installation
-
-You can install `FacekiAPIClientV2` using pip:
-
-```
-pip install facekiapiclientv2
-```
-
-## Usage
-
-```python
-import requests
-from facekiapiclientv2 import FacekiAPIClientV2
-
-client_id = 'your_client_id'
-client_secret = 'your_client_secret'
-api_client = FacekiAPIClientV2(client_id, client_secret)
-
-# Generate an access token
-api_client.generate_token()
-
-# Get KYC rules
-kyc_rules = api_client.getKYCRules()
-
-# Perform a KYC verification
-selfie_image = 'path_to_selfie_image.jpg'
-id_front_image = 'path_to_id_front_image.jpg'
-id_back_image = 'path_to_id_back_image.jpg'
-dl_front_image = 'path_to_dl_front_image.jpg'
-dl_back_image = 'path_to_dl_back_image.jpg'
-pp_front_image = 'path_to_pp_front_image.jpg'
-pp_back_image = 'path_to_pp_back_image.jpg'
-
-result = api_client.requestKYC(selfie_image, id_front_image, id_back_image,
-                               dl_front_image, dl_back_image, pp_front_image,
-                               pp_back_image)
-
-# Get KYC verification summary
-kyc_summary = api_client.getKycSummary()
-
-# Generate a KYC verification link
-expire_time = 0
-application_id = 'your_application_id'
-
-link = api_client.generateKYCLink(expire_time, application_id)
-
-# Get KYC records
-link_id = 'your_link_id'
-kyc_records = api_client.getKYCrecords(link_id)
-
-# Perform a face check
-selfie_image = 'path_to_selfie_image.jpg'
-
-result = api_client.faceCheck(selfie_image)
-```
-
-## Exception Handling
-
-The `FacekiAPIClientV2` class may raise exceptions in case of errors. Ensure that you handle these exceptions appropriately in your code. Examples of possible exceptions include:
-
-- `requests.exceptions.RequestException`: Raised when there is an issue with making a request to the Faceki API.
-- `Exception`: Raised for various errors such as failed token generation or failed requests.
-
-## Disclaimer
-
-Please note that this client code is provided as a starting point and may require modifications or updates depending on the Faceki API's specific requirements or changes. Refer to the Faceki API documentation for detailed information about the API's endpoints, request/response structures, and authentication requirements.
-
+Metadata-Version: 2.1
+Name: facekiapiclientv2
+Version: 1.2
+Summary: FACEKI KYC Api Library
+Author: Faceki
+Author-email: haziq@faceki.com
+Keywords: api,client,library
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+
+# FacekiAPIClientV2
+
+The `FacekiAPIClientV2` is a Python client for interacting with the Faceki API. It provides methods to generate an access token, perform various KYC (Know Your Customer) operations, and retrieve KYC records.
+
+## Installation
+
+You can install `FacekiAPIClientV2` using pip:
+
+```
+pip install facekiapiclientv2
+```
+
+## Usage
+
+```python
+import requests
+from facekiapiclientv2 import FacekiAPIClientV2
+
+client_id = 'your_client_id'
+client_secret = 'your_client_secret'
+api_client = FacekiAPIClientV2(client_id, client_secret)
+
+# Generate an access token
+api_client.generate_token()
+
+# Get KYC rules
+kyc_rules = api_client.getKYCRules()
+
+# Perform a KYC verification
+selfie_image = 'path_to_selfie_image.jpg'
+id_front_image = 'path_to_id_front_image.jpg'
+id_back_image = 'path_to_id_back_image.jpg'
+dl_front_image = 'path_to_dl_front_image.jpg'
+dl_back_image = 'path_to_dl_back_image.jpg'
+pp_front_image = 'path_to_pp_front_image.jpg'
+pp_back_image = 'path_to_pp_back_image.jpg'
+
+result = api_client.requestKYC(selfie_image, id_front_image, id_back_image,
+                               dl_front_image, dl_back_image, pp_front_image,
+                               pp_back_image)
+
+# Get KYC verification summary
+kyc_summary = api_client.getKycSummary()
+
+# Generate a KYC verification link
+expire_time = 0
+application_id = 'your_application_id'
+
+link = api_client.generateKYCLink(expire_time, application_id)
+
+# Get KYC records
+link_id = 'your_link_id'
+kyc_records = api_client.getKYCrecords(link_id)
+
+# Perform a face check
+selfie_image = 'path_to_selfie_image.jpg'
+
+result = api_client.faceCheck(selfie_image)
+```
+
+## Exception Handling
+
+The `FacekiAPIClientV2` class may raise exceptions in case of errors. Ensure that you handle these exceptions appropriately in your code. Examples of possible exceptions include:
+
+- `requests.exceptions.RequestException`: Raised when there is an issue with making a request to the Faceki API.
+- `Exception`: Raised for various errors such as failed token generation or failed requests.
+
+## Disclaimer
+
+Please note that this client code is provided as a starting point and may require modifications or updates depending on the Faceki API's specific requirements or changes. Refer to the Faceki API documentation for detailed information about the API's endpoints, request/response structures, and authentication requirements.
```

### Comparing `facekiapiclientv2-1.1/README.md` & `facekiapiclientv2-1.2/README.md`

 * *Files identical despite different names*

### Comparing `facekiapiclientv2-1.1/faceki-kyc-python/client.py` & `facekiapiclientv2-1.2/faceki-kyc-python/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,14 @@
             'client_id': self.client_id,
             'client_secret': self.client_secret
         }
 
         response = requests.get(auth_url)
         if response.status_code == 200:
             resp = response.json()
-            print(resp)
             return resp["data"]["access_token"]
         else:
             raise Exception('Failed to generate token')
 
     def getKYCRules(self, params=None):
         headers = {
             'Authorization': f'Bearer {self.token}'
@@ -69,32 +68,35 @@
         response = requests.get(url, headers=headers)
 
         if response.status_code == 200:
             return response.json()
         else:
             raise Exception(f'Request failed with status code {response.status_code}')
         
-    def generateKYCLink(self,expireTime=0,applicationId=None):
+    def generateKYCLink(self,expireTime=0,applicationId=None,redirect_url=None,document_optional=None,require_additional_doc=None):
         headers = {
             'Authorization': f'Bearer {self.token}'
         }
         payload ={
             'expiryTime':expireTime,
-            'applicationId':applicationId
+            'applicationId':applicationId,
+            'redirect_url':redirect_url,
+            'document_optional':document_optional,
+            'require_additional_doc':require_additional_doc
         }
 
         url = f'{self.base_url}/kycverify/api/kycverify/kyc-verify-link'
         response = requests.post(url, headers=headers,json=payload)
 
-        if response.status_code == 200:
+        if response.status_code == 200 or response.status_code == 201 :
             return response.json()
         else:
             raise Exception(f'Request failed with status code {response.status_code}')
 
-    def getKYCrecords(self,linkId=None):
+    def getKYCrecordsByLink(self,linkId=None):
         headers = {
             'Authorization': f'Bearer {self.token}'
         }
         params = None
         if linkId != None:
             params ={
                 'linkId':linkId,
@@ -104,22 +106,58 @@
         response = requests.get(url, headers=headers,params=params)
 
         if response.status_code == 200:
             return response.json()
         else:
             raise Exception(f'Request failed with status code {response.status_code}')
 
-    def getKYCrecords(self,selfie_image):
+    def getKYCrecordsBySelfie(self,selfie_image):
         headers = {
             'Authorization': f'Bearer {self.token}'
         }
         files = {
         'selfie_image': ('selfie_image.jpg', open(selfie_image, 'rb'))
         }
 
         url = f'{self.base_url}/facelink/api/face-check'
         response = requests.post(url, headers=headers,files=files)
 
         if response.status_code == 200:
             return response.json()
         else:
+            raise Exception(f'Request failed with status code {response.status_code}')
+        
+    def getKYCRecordByRequestId(self,requestId):
+        headers = {
+            'Authorization': f'Bearer {self.token}'
+        }
+        params = None
+        if requestId != None:
+            params ={
+                'requestId':requestId,
+            }
+
+        url = f'{self.base_url}/kycverify/api/kycverify/records'
+        response = requests.get(url, headers=headers,params=params)
+
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise Exception(f'Request failed with status code {response.status_code}')
+
+    def getKYCRecordByReference(self,referenceId):
+        headers = {
+            'Authorization': f'Bearer {self.token}'
+        }
+        params = None
+        if referenceId != None:
+            params ={
+                'referenceId':referenceId,
+            }
+
+        url = f'{self.base_url}/kycverify/api/kycverify/reference'
+        response = requests.get(url, headers=headers,params=params)
+
+        if response.status_code == 200:
+            return response.json()
+        else:
             raise Exception(f'Request failed with status code {response.status_code}')
```

### Comparing `facekiapiclientv2-1.1/facekiapiclientv2.egg-info/PKG-INFO` & `facekiapiclientv2-1.2/facekiapiclientv2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,86 @@
-Metadata-Version: 2.1
-Name: facekiapiclientv2
-Version: 1.1
-Summary: FACEKI KYC Api Library
-Home-page: UNKNOWN
-Author: Faceki
-Author-email: haziq@faceki.com
-License: UNKNOWN
-Keywords: api,client,library
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
-# FacekiAPIClientV2
-
-The `FacekiAPIClientV2` is a Python client for interacting with the Faceki API. It provides methods to generate an access token, perform various KYC (Know Your Customer) operations, and retrieve KYC records.
-
-## Installation
-
-You can install `FacekiAPIClientV2` using pip:
-
-```
-pip install facekiapiclientv2
-```
-
-## Usage
-
-```python
-import requests
-from facekiapiclientv2 import FacekiAPIClientV2
-
-client_id = 'your_client_id'
-client_secret = 'your_client_secret'
-api_client = FacekiAPIClientV2(client_id, client_secret)
-
-# Generate an access token
-api_client.generate_token()
-
-# Get KYC rules
-kyc_rules = api_client.getKYCRules()
-
-# Perform a KYC verification
-selfie_image = 'path_to_selfie_image.jpg'
-id_front_image = 'path_to_id_front_image.jpg'
-id_back_image = 'path_to_id_back_image.jpg'
-dl_front_image = 'path_to_dl_front_image.jpg'
-dl_back_image = 'path_to_dl_back_image.jpg'
-pp_front_image = 'path_to_pp_front_image.jpg'
-pp_back_image = 'path_to_pp_back_image.jpg'
-
-result = api_client.requestKYC(selfie_image, id_front_image, id_back_image,
-                               dl_front_image, dl_back_image, pp_front_image,
-                               pp_back_image)
-
-# Get KYC verification summary
-kyc_summary = api_client.getKycSummary()
-
-# Generate a KYC verification link
-expire_time = 0
-application_id = 'your_application_id'
-
-link = api_client.generateKYCLink(expire_time, application_id)
-
-# Get KYC records
-link_id = 'your_link_id'
-kyc_records = api_client.getKYCrecords(link_id)
-
-# Perform a face check
-selfie_image = 'path_to_selfie_image.jpg'
-
-result = api_client.faceCheck(selfie_image)
-```
-
-## Exception Handling
-
-The `FacekiAPIClientV2` class may raise exceptions in case of errors. Ensure that you handle these exceptions appropriately in your code. Examples of possible exceptions include:
-
-- `requests.exceptions.RequestException`: Raised when there is an issue with making a request to the Faceki API.
-- `Exception`: Raised for various errors such as failed token generation or failed requests.
-
-## Disclaimer
-
-Please note that this client code is provided as a starting point and may require modifications or updates depending on the Faceki API's specific requirements or changes. Refer to the Faceki API documentation for detailed information about the API's endpoints, request/response structures, and authentication requirements.
-
+Metadata-Version: 2.1
+Name: facekiapiclientv2
+Version: 1.2
+Summary: FACEKI KYC Api Library
+Author: Faceki
+Author-email: haziq@faceki.com
+Keywords: api,client,library
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+
+# FacekiAPIClientV2
+
+The `FacekiAPIClientV2` is a Python client for interacting with the Faceki API. It provides methods to generate an access token, perform various KYC (Know Your Customer) operations, and retrieve KYC records.
+
+## Installation
+
+You can install `FacekiAPIClientV2` using pip:
+
+```
+pip install facekiapiclientv2
+```
+
+## Usage
+
+```python
+import requests
+from facekiapiclientv2 import FacekiAPIClientV2
+
+client_id = 'your_client_id'
+client_secret = 'your_client_secret'
+api_client = FacekiAPIClientV2(client_id, client_secret)
+
+# Generate an access token
+api_client.generate_token()
+
+# Get KYC rules
+kyc_rules = api_client.getKYCRules()
+
+# Perform a KYC verification
+selfie_image = 'path_to_selfie_image.jpg'
+id_front_image = 'path_to_id_front_image.jpg'
+id_back_image = 'path_to_id_back_image.jpg'
+dl_front_image = 'path_to_dl_front_image.jpg'
+dl_back_image = 'path_to_dl_back_image.jpg'
+pp_front_image = 'path_to_pp_front_image.jpg'
+pp_back_image = 'path_to_pp_back_image.jpg'
+
+result = api_client.requestKYC(selfie_image, id_front_image, id_back_image,
+                               dl_front_image, dl_back_image, pp_front_image,
+                               pp_back_image)
+
+# Get KYC verification summary
+kyc_summary = api_client.getKycSummary()
+
+# Generate a KYC verification link
+expire_time = 0
+application_id = 'your_application_id'
+
+link = api_client.generateKYCLink(expire_time, application_id)
+
+# Get KYC records
+link_id = 'your_link_id'
+kyc_records = api_client.getKYCrecords(link_id)
+
+# Perform a face check
+selfie_image = 'path_to_selfie_image.jpg'
+
+result = api_client.faceCheck(selfie_image)
+```
+
+## Exception Handling
+
+The `FacekiAPIClientV2` class may raise exceptions in case of errors. Ensure that you handle these exceptions appropriately in your code. Examples of possible exceptions include:
+
+- `requests.exceptions.RequestException`: Raised when there is an issue with making a request to the Faceki API.
+- `Exception`: Raised for various errors such as failed token generation or failed requests.
+
+## Disclaimer
+
+Please note that this client code is provided as a starting point and may require modifications or updates depending on the Faceki API's specific requirements or changes. Refer to the Faceki API documentation for detailed information about the API's endpoints, request/response structures, and authentication requirements.
```

### Comparing `facekiapiclientv2-1.1/setup.py` & `facekiapiclientv2-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='facekiapiclientv2',
-    version='1.1',
+    version='1.2',
     packages=find_packages(),
     install_requires=['requests'],
     description='FACEKI KYC Api Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Faceki',
     author_email='haziq@faceki.com',
```

