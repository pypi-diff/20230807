# Comparing `tmp/smile_id_core-2.1.0.tar.gz` & `tmp/smile_id_core-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smile_id_core-2.1.0.tar", max compression
+gzip compressed data, was "smile_id_core-2.1.1.tar", max compression
```

## Comparing `smile_id_core-2.1.0.tar` & `smile_id_core-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/LICENSE
--rw-r--r--   0        0        0     3967 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/README.md
--rw-r--r--   0        0        0     2136 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3137 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/BusinessVerification.py
--rw-r--r--   0        0        0     3657 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/IdApi.py
--rw-r--r--   0        0        0      223 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/ServerError.py
--rw-r--r--   0        0        0     2369 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/Signature.py
--rw-r--r--   0        0        0    14727 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/Utilities.py
--rw-r--r--   0        0        0    12058 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/WebApi.py
--rw-r--r--   0        0        0      662 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/__init__.py
--rw-r--r--   0        0        0     1019 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/base.py
--rw-r--r--   0        0        0     2125 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/constants.py
--rw-r--r--   0        0        0     8523 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/image_upload.py
--rw-r--r--   0        0        0      811 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/types.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 smile_id_core-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3967 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/README.md
+-rw-r--r--   0        0        0     2185 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3137 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/BusinessVerification.py
+-rw-r--r--   0        0        0     3657 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/IdApi.py
+-rw-r--r--   0        0        0      223 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/ServerError.py
+-rw-r--r--   0        0        0     2369 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/Signature.py
+-rw-r--r--   0        0        0    14727 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/Utilities.py
+-rw-r--r--   0        0        0    12058 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/WebApi.py
+-rw-r--r--   0        0        0      662 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/__init__.py
+-rw-r--r--   0        0        0     1019 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/base.py
+-rw-r--r--   0        0        0     2125 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/constants.py
+-rw-r--r--   0        0        0     8523 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/image_upload.py
+-rw-r--r--   0        0        0      811 2023-08-07 13:50:56.679613 smile_id_core-2.1.1/smile_id_core/types.py
+-rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 smile_id_core-2.1.1/PKG-INFO
```

### Comparing `smile_id_core-2.1.0/LICENSE` & `smile_id_core-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/README.md` & `smile_id_core-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/pyproject.toml` & `smile_id_core-2.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smile-id-core"
-version = "2.1.0"
+version = "2.1.1"
 description = "The official Smile Identity package exposes four classes namely; the WebApi class, the IDApi class, the Signature class and the Utilities class."
 license = "MIT"
 authors = ["Smile Identity <support@smileidentity.com>"]
 readme = "README.md"
 homepage = "https://github.com/smileidentity/smile-identity-core-python-3"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -20,34 +20,36 @@
 exclude = ["tests/**/*"]
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-pycryptodome = "^3.15.0"
+pycryptodome = "^3.0.0"
 python = "^3.7"
-requests = "^2.27.1"
-typing-extensions = "4.7.1"
-types-requests = "^2.28.11.5"
+requests = "^2.0.0"
+typing-extensions = "4.2.0"
+types-requests = "^2.0.0.0"
 
 [tool.poetry.group.dev]
 optional = true
 [tool.poetry.group.dev.dependencies]
 black = ">=22.8,<24.0"
 coverage = "7.2.7"
 isort = "^5.10.1"
+keepachangelog-manager = ">=3.3.1"
 mock = ">=4.0.3,<6.0.0"
 mypy = "1.4.1"
+pydocstyle = "^6.3.0"
 pylint = "2.13.9"
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
-pydocstyle = "^6.3.0"
 pytest-xdist = "^3.0.2"
 responses = ">=0.17,<0.24"
+ruff = "^0.0.282"
 types-mock = ">=4.0.15.2,<6.0.0.0"
 
 [tool.poetry.group.github-actions]
 optional = true
 [tool.poetry.group.github-actions.dependencies]
 pytest-github-actions-annotate-failures = ">=0.1.7,<0.3.0"
```

### Comparing `smile_id_core-2.1.0/smile_id_core/BusinessVerification.py` & `smile_id_core-2.1.1/smile_id_core/BusinessVerification.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/IdApi.py` & `smile_id_core-2.1.1/smile_id_core/IdApi.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/Signature.py` & `smile_id_core-2.1.1/smile_id_core/Signature.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/Utilities.py` & `smile_id_core-2.1.1/smile_id_core/Utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,35 +255,35 @@
             raise ServerError(
                 f"Failed to get to /services, status={response.status_code},"
                 f" response={response.json()}"
             )
         response_json = response.json()
         if job_type == JobType.DOCUMENT_VERIFICATION:
             doc_verification = response_json["hosted_web"]["doc_verification"]
-            if not id_info_params["country"] in doc_verification:
+            if id_info_params["country"] not in doc_verification:
                 raise ValueError(
                     f"country {id_info_params['country']} is invalid"
                 )
             selected_country = doc_verification[id_info_params["country"]][
                 "id_types"
             ]
-            if not id_info_params["id_type"] in selected_country:
+            if id_info_params["id_type"] not in selected_country:
                 raise ValueError(
                     f"id_type {id_info_params['id_type']} is invalid"
                 )
         else:
             id_types_by_country = response_json["id_types"]
-            if not id_info_params["country"] in id_types_by_country:
+            if id_info_params["country"] not in id_types_by_country:
                 raise ValueError(
                     f"country {id_info_params['country']} is invalid"
                 )
             selected_country = response_json["id_types"][
                 id_info_params["country"]
             ]
-            if not id_info_params["id_type"] in selected_country:
+            if id_info_params["id_type"] not in selected_country:
                 raise ValueError(
                     f"id_type {id_info_params['id_type']} is invalid"
                 )
             id_params = selected_country[id_info_params["id_type"]]
             for key in id_params:
                 if key not in id_info_params and key not in partner_params:
                     raise ValueError(f"key {key} is required")
```

### Comparing `smile_id_core-2.1.0/smile_id_core/WebApi.py` & `smile_id_core-2.1.1/smile_id_core/WebApi.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/__init__.py` & `smile_id_core-2.1.1/smile_id_core/__init__.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/base.py` & `smile_id_core-2.1.1/smile_id_core/base.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/constants.py` & `smile_id_core-2.1.1/smile_id_core/constants.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/image_upload.py` & `smile_id_core-2.1.1/smile_id_core/image_upload.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/smile_id_core/types.py` & `smile_id_core-2.1.1/smile_id_core/types.py`

 * *Files identical despite different names*

### Comparing `smile_id_core-2.1.0/PKG-INFO` & `smile_id_core-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: smile-id-core
-Version: 2.1.0
+Version: 2.1.1
 Summary: The official Smile Identity package exposes four classes namely; the WebApi class, the IDApi class, the Signature class and the Utilities class.
 Home-page: https://github.com/smileidentity/smile-identity-core-python-3
 License: MIT
 Author: Smile Identity
 Author-email: support@smileidentity.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: types-requests (>=2.28.11.5,<3.0.0.0)
-Requires-Dist: typing-extensions (==4.7.1)
+Requires-Dist: pycryptodome (>=3.0.0,<4.0.0)
+Requires-Dist: requests (>=2.0.0,<3.0.0)
+Requires-Dist: types-requests (>=2.0.0.0,<3.0.0.0)
+Requires-Dist: typing-extensions (==4.2.0)
 Description-Content-Type: text/markdown
 
 # Smile Identity Python Server Side SDK
 
 Smile Identity provides the best solutions for real time Digital KYC, Identity Verification, User Onboarding, and User Authentication across Africa. Our server side libraries make it easy to integrate us on the server-side. Since the library is server-side, you will be required to pass the images (if required) to the library.
 
 If you haven’t already, [sign up for a free Smile Identity account](https://www.smileidentity.com/schedule-a-demo/), which comes with Sandbox access.
```

