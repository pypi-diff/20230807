# Comparing `tmp/openi-beta-2.0.7.tar.gz` & `tmp/openi-beta-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-2.0.7.tar", last modified: Sun Jul 30 16:02:07 2023, max compression
+gzip compressed data, was "openi-beta-2.0.8.tar", last modified: Mon Aug  7 01:56:15 2023, max compression
```

## Comparing `openi-beta-2.0.7.tar` & `openi-beta-2.0.8.tar`

### file list

```diff
@@ -1,39 +1,28 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.940656 openi-beta-2.0.7/
--rw-r--r--   0 jochen10518   (501) staff       (20)     5256 2023-07-30 16:02:07.940488 openi-beta-2.0.7/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     4630 2023-07-30 16:01:55.000000 openi-beta-2.0.7/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-07-30 16:02:07.940703 openi-beta-2.0.7/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1255 2023-07-30 16:01:59.000000 openi-beta-2.0.7/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.935610 openi-beta-2.0.7/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.936781 openi-beta-2.0.7/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)      184 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     6284 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/apis.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     5070 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/cli.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.937508 openi-beta-2.0.7/src/openi/cloudbrain/
--rw-r--r--   0 jochen10518   (501) staff       (20)       81 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/cloudbrain/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     1544 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/cloudbrain/env_check.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     5154 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/cloudbrain/helper.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     1510 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/cloudbrain/minio_operate.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     2806 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/cloudbrain/obs_operate.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.938152 openi-beta-2.0.7/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)      106 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     2660 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/dataset/dataset_file.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     2587 2023-07-30 15:53:14.000000 openi-beta-2.0.7/src/openi/dataset/download.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     4270 2023-07-30 16:00:53.000000 openi-beta-2.0.7/src/openi/dataset/upload.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     2949 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/login.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.938459 openi-beta-2.0.7/src/openi/path/
--rw-r--r--   0 jochen10518   (501) staff       (20)       20 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/path/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     2326 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/path/path.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     3972 2023-07-30 16:01:11.000000 openi-beta-2.0.7/src/openi/settings.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.938875 openi-beta-2.0.7/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/utils/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     1346 2023-07-30 16:00:47.000000 openi-beta-2.0.7/src/openi/utils/file_utils.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      691 2023-07-29 06:56:39.000000 openi-beta-2.0.7/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.939962 openi-beta-2.0.7/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     5256 2023-07-30 16:02:07.000000 openi-beta-2.0.7/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      787 2023-07-30 16:02:07.000000 openi-beta-2.0.7/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-07-30 16:02:07.000000 openi-beta-2.0.7/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       41 2023-07-30 16:02:07.000000 openi-beta-2.0.7/src/openi_beta.egg-info/entry_points.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       20 2023-07-30 16:02:07.000000 openi-beta-2.0.7/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-07-30 16:02:07.000000 openi-beta-2.0.7/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-07-30 16:02:07.940198 openi-beta-2.0.7/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)     5669 2023-06-20 08:41:55.000000 openi-beta-2.0.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.343454 openi-beta-2.0.8/
+-rw-rw-rw-   0        0        0     2086 2023-08-07 01:56:15.342449 openi-beta-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2023-08-07 01:38:11.000000 openi-beta-2.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 01:56:15.343454 openi-beta-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-08-07 01:39:47.000000 openi-beta-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.307411 openi-beta-2.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.312202 openi-beta-2.0.8/src/openi/
+-rw-rw-rw-   0        0        0      194 2023-08-07 01:38:11.000000 openi-beta-2.0.8/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-08-07 01:38:11.000000 openi-beta-2.0.8/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-08-07 01:38:11.000000 openi-beta-2.0.8/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.314327 openi-beta-2.0.8/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2752 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2671 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4392 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3029 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/login.py
+-rw-rw-rw-   0        0        0     4078 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.316939 openi-beta-2.0.8/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1400 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.342449 openi-beta-2.0.8/src/openi_beta.egg-info/
+-rw-rw-rw-   0        0        0     2086 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/top_level.txt
```

### Comparing `openi-beta-2.0.7/setup.py` & `openi-beta-2.0.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# python setup.py sdist bdist_wheel
-# twine upload dist/*
-# twine upload --repository testpypi dist/*
-# pip install -i https://test.pypi.org/pypi/ --extra-index-url https://pypi.org/simple <your_package_in_testpypi>
-
-from setuptools import find_packages, setup
-
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
-
-setup(
-    name="openi-beta",
-    version="2.0.7",
-    description="Beta package for openi pypi",
-    package_dir={"": "src"},
-    packages=find_packages("src"),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
-    author="chenzh05",
-    author_email="chenzh.ds@outlook.com",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Build Tools",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Operating System :: OS Independent",
-    ],
-    entry_points={"console_scripts": ["openi = openi.cli:main"]},
-    install_requires=["requests", "tqdm", "emoji"],
-    python_requires=">=3.6",
-)
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
+# twine upload --repository testpypi dist/*
+# pip install -i https://test.pypi.org/pypi/ --extra-index-url https://pypi.org/simple <your_package_in_testpypi>
+
+from setuptools import find_packages, setup
+
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+
+setup(
+    name="openi-beta",
+    version="2.0.8",
+    description="Beta package for openi pypi",
+    package_dir={"": "src"},
+    packages=find_packages("src"),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
+    author="chenzh05",
+    author_email="chenzh.ds@outlook.com",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Operating System :: OS Independent",
+    ],
+    entry_points={"console_scripts": ["openi = openi.cli:main"]},
+    install_requires=["requests", "tqdm", "emoji"],
+    python_requires=">=3.6",
+)
```

### Comparing `openi-beta-2.0.7/src/openi/apis.py` & `openi-beta-2.0.8/src/openi/apis.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-import logging
-
-import requests
-from openi.settings import *
-from openi.utils import file_utils
-
-"""
-APIS
-"""
-
-
-class OpeniAPI:
-    def __init__(self, endpoint: str = None, token: str = None):
-        self.baseURL = (
-            file_utils.get_token()["endpoint"] if endpoint is None else endpoint
-        )
-        self.endpoint = self.baseURL + API.VERSION
-        self.token = file_utils.get_token()["token"] if token is None else token
-
-    def catch_auth_error(self, x):
-        if x.status_code == 401:
-            msg = f"❌ {x} {x.reason} - failed to connecting OPENI, please check your `token` or permssion."
-            logging.error(msg)
-            raise PermissionError(msg)
-        if x.status_code == 404:
-            msg = f"❌ {x} {x.reason} - failed to connecting OPENI, either incorrect `owner/repo` or `endpoint`."
-            logging.error(msg)
-            raise ConnectionError(msg)
-        if x.raise_for_status():
-            logging.error(x.raise_for_status())
-            x.raise_for_status()
-
-    def login_check(self) -> str:
-        params = {"access_token": self.token}
-        x = requests.get(f"{self.endpoint}/user", params=params)
-        logging.info(f"GET {x.url}")
-        self.catch_auth_error(x)
-        logging.info(f"{x} {x.url} {x.json()}")
-        return x.json()["username"]
-
-    def get_dataset(self, repo_id):
-        params = {"access_token": self.token}
-        x = requests.get(f"{self.endpoint}/datasets/{repo_id}", params=params)
-        logging.info(f"GET {x.url}")
-        self.catch_auth_error(x)
-        logging.info(f"{x} {x.url} {x.json()}")
-        return x.json()["data"]
-
-    def get_dataset_attachment(self, repo_id: str, upload_type: str):
-        params = {"access_token": self.token, "type": upload_type}
-        x = requests.get(
-            f"{self.endpoint}/datasets/{repo_id}/current_repo", params=params
-        )
-        logging.info(f"GET {x.url}")
-        self.catch_auth_error(x)
-        logging.info(f"{x} {x.url} {x.json()}")
-        return x.json()
-
-    def get_chunks(self, _file):
-        params = {
-            "access_token": self.token,
-            "dataset_id": _file["dataset_id"],
-            "md5": _file["md5"],
-            "file_name": _file["filename"],
-            "type": _file["upload_type"],
-        }
-        x = requests.get(f"{self.endpoint}/attachments/get_chunks", params=params)
-        logging.info(f"GET {x.url}")
-        if x.ok:
-            logging.info(f"{x} {x.url} {x.json()}")
-            return x.json()
-        else:
-            msg = f"❌ {x} {x.reason} {x.text}"
-            logging.error(msg)
-            raise ConnectionRefusedError(msg)
-
-    def get_multipart_url(self, chunk_number: int, chunk_size: int, _file: dict):
-        params = {
-            "access_token": self.token,
-            "dataset_id": _file["dataset_id"],
-            "file_name": _file["filename"],
-            "type": _file["upload_type"],
-            "chunkNumber": chunk_number,
-            "size": chunk_size,
-            "uploadID": _file["upload_id"],
-            "uuid": _file["uuid"],
-        }
-        x = requests.get(
-            f"{self.endpoint}/attachments/get_multipart_url", params=params
-        )
-        logging.info(f"GET {x.url}")
-        if x.ok:
-            logging.info(f"{x} {x.url} {x.json()}")
-            return x.json()["url"]
-        else:
-            msg = f"❌ {x} {x.reason}"
-            logging.error(msg)
-            raise ConnectionRefusedError(msg)
-
-    def put_upload(self, url, data, upload_type):
-        headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
-        x = requests.put(url, data=data, headers=headers)
-        logging.info(f"PUT {x.url}")
-        try:
-            logging.info(f"{x} {x.url} {x.headers}")
-            return x.headers["ETag"]
-        except:
-            msg = f"❌ {x} {x.reason} {x.text}"
-            logging.error(msg)
-            raise ConnectionRefusedError(msg)
-
-    def new_multipart(self, _file):
-        params = {
-            "access_token": self.token,
-            "dataset_id": _file["dataset_id"],
-            "md5": _file["md5"],
-            "file_name": _file["filename"],
-            "type": _file["upload_type"],
-            "totalChunkCounts": _file["total_chunks_count"],
-            "size": _file["size"],
-        }
-        x = requests.get(f"{self.endpoint}/attachments/new_multipart", params=params)
-        logging.info(f"GET {x.url}")
-        if x.ok:
-            if x.json()["result_code"] == "0":
-                logging.info(f"{x} {x.url} {x.json()}")
-                return x.json()["uuid"], x.json()["uploadID"]
-            else:
-                logging.error(f"❌ {x} {x.reason} {x.json()}")
-                raise ConnectionRefusedError(f'❌ {x} {x.reason} {x.json()["msg"]}')
-        else:
-            msg = f"❌ {x} {x.reason}"
-            logging.error(msg)
-            raise ConnectionRefusedError(msg)
-
-    def complete_multipart(self, _file):
-        params = {
-            "access_token": self.token,
-            "dataset_id": _file["dataset_id"],
-            "file_name": _file["filename"],
-            "type": _file["upload_type"],
-            "size": _file["size"],
-            "uploadID": _file["upload_id"],
-            "uuid": _file["uuid"],
-        }
-        x = requests.post(
-            f"{self.endpoint}/attachments/complete_multipart", params=params
-        )
-        logging.info(f"POST {x.url}")
-        if x.ok:
-            if x.json()["result_code"] == "-1":
-                logging.error(f"❌ {x} {x.reason} {x.json()}")
-                raise ConnectionRefusedError(f'❌ {x} {x.reason} {x.json()["msg"]}')
-            else:
-                logging.info(f"{x} {x.url} {x.json()}")
-        else:
-            msg = f"❌ {x} {x.reason} {x.text}"
-            logging.error(msg)
-            raise ConnectionRefusedError(msg)
-
-    def download_attachments(self, uuid: str, upload_type: int):
-        params = {"access_token": self.token, "type": upload_type}
-        x = requests.get(
-            f"{self.endpoint}/attachments/{uuid}",
-            params=params,
-            allow_redirects=True,
-            stream=True,
-        )
-        logging.info(f"GET {x.url}")
-        self.catch_auth_error(x)
-        logging.info(f"{x} {x.url}")
-        return x
+import logging
+
+import requests
+from openi.settings import *
+from openi.utils import file_utils
+
+"""
+APIS
+"""
+
+
+class OpeniAPI:
+    def __init__(self, endpoint: str = None, token: str = None):
+        self.baseURL = (
+            file_utils.get_token()["endpoint"] if endpoint is None else endpoint
+        )
+        self.endpoint = self.baseURL + API.VERSION
+        self.token = file_utils.get_token()["token"] if token is None else token
+
+    def catch_auth_error(self, x):
+        if x.status_code == 401:
+            msg = f"❌ {x} {x.reason} - failed to connecting OPENI, please check your `token` or permssion."
+            logging.error(msg)
+            raise PermissionError(msg)
+        if x.status_code == 404:
+            msg = f"❌ {x} {x.reason} - failed to connecting OPENI, either incorrect `owner/repo` or `endpoint`."
+            logging.error(msg)
+            raise ConnectionError(msg)
+        if x.raise_for_status():
+            logging.error(x.raise_for_status())
+            x.raise_for_status()
+
+    def login_check(self) -> str:
+        params = {"access_token": self.token}
+        x = requests.get(f"{self.endpoint}/user", params=params)
+        logging.info(f"GET {x.url}")
+        self.catch_auth_error(x)
+        logging.info(f"{x} {x.url} {x.json()}")
+        return x.json()["username"]
+
+    def get_dataset(self, repo_id):
+        params = {"access_token": self.token}
+        x = requests.get(f"{self.endpoint}/datasets/{repo_id}", params=params)
+        logging.info(f"GET {x.url}")
+        self.catch_auth_error(x)
+        logging.info(f"{x} {x.url} {x.json()}")
+        return x.json()["data"]
+
+    def get_dataset_attachment(self, repo_id: str, upload_type: str):
+        params = {"access_token": self.token, "type": upload_type}
+        x = requests.get(
+            f"{self.endpoint}/datasets/{repo_id}/current_repo", params=params
+        )
+        logging.info(f"GET {x.url}")
+        self.catch_auth_error(x)
+        logging.info(f"{x} {x.url} {x.json()}")
+        return x.json()
+
+    def get_chunks(self, _file):
+        params = {
+            "access_token": self.token,
+            "dataset_id": _file["dataset_id"],
+            "md5": _file["md5"],
+            "file_name": _file["filename"],
+            "type": _file["upload_type"],
+        }
+        x = requests.get(f"{self.endpoint}/attachments/get_chunks", params=params)
+        logging.info(f"GET {x.url}")
+        if x.ok:
+            logging.info(f"{x} {x.url} {x.json()}")
+            return x.json()
+        else:
+            msg = f"❌ {x} {x.reason} {x.text}"
+            logging.error(msg)
+            raise ConnectionRefusedError(msg)
+
+    def get_multipart_url(self, chunk_number: int, chunk_size: int, _file: dict):
+        params = {
+            "access_token": self.token,
+            "dataset_id": _file["dataset_id"],
+            "file_name": _file["filename"],
+            "type": _file["upload_type"],
+            "chunkNumber": chunk_number,
+            "size": chunk_size,
+            "uploadID": _file["upload_id"],
+            "uuid": _file["uuid"],
+        }
+        x = requests.get(
+            f"{self.endpoint}/attachments/get_multipart_url", params=params
+        )
+        logging.info(f"GET {x.url}")
+        if x.ok:
+            logging.info(f"{x} {x.url} {x.json()}")
+            return x.json()["url"]
+        else:
+            msg = f"❌ {x} {x.reason}"
+            logging.error(msg)
+            raise ConnectionRefusedError(msg)
+
+    def put_upload(self, url, data, upload_type):
+        headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
+        x = requests.put(url, data=data, headers=headers)
+        logging.info(f"PUT {x.url}")
+        try:
+            logging.info(f"{x} {x.url} {x.headers}")
+            return x.headers["ETag"]
+        except:
+            msg = f"❌ {x} {x.reason} {x.text}"
+            logging.error(msg)
+            raise ConnectionRefusedError(msg)
+
+    def new_multipart(self, _file):
+        params = {
+            "access_token": self.token,
+            "dataset_id": _file["dataset_id"],
+            "md5": _file["md5"],
+            "file_name": _file["filename"],
+            "type": _file["upload_type"],
+            "totalChunkCounts": _file["total_chunks_count"],
+            "size": _file["size"],
+        }
+        x = requests.get(f"{self.endpoint}/attachments/new_multipart", params=params)
+        logging.info(f"GET {x.url}")
+        if x.ok:
+            if x.json()["result_code"] == "0":
+                logging.info(f"{x} {x.url} {x.json()}")
+                return x.json()["uuid"], x.json()["uploadID"]
+            else:
+                logging.error(f"❌ {x} {x.reason} {x.json()}")
+                raise ConnectionRefusedError(f'❌ {x} {x.reason} {x.json()["msg"]}')
+        else:
+            msg = f"❌ {x} {x.reason}"
+            logging.error(msg)
+            raise ConnectionRefusedError(msg)
+
+    def complete_multipart(self, _file):
+        params = {
+            "access_token": self.token,
+            "dataset_id": _file["dataset_id"],
+            "file_name": _file["filename"],
+            "type": _file["upload_type"],
+            "size": _file["size"],
+            "uploadID": _file["upload_id"],
+            "uuid": _file["uuid"],
+        }
+        x = requests.post(
+            f"{self.endpoint}/attachments/complete_multipart", params=params
+        )
+        logging.info(f"POST {x.url}")
+        if x.ok:
+            if x.json()["result_code"] == "-1":
+                logging.error(f"❌ {x} {x.reason} {x.json()}")
+                raise ConnectionRefusedError(f'❌ {x} {x.reason} {x.json()["msg"]}')
+            else:
+                logging.info(f"{x} {x.url} {x.json()}")
+        else:
+            msg = f"❌ {x} {x.reason} {x.text}"
+            logging.error(msg)
+            raise ConnectionRefusedError(msg)
+
+    def download_attachments(self, uuid: str, upload_type: int):
+        params = {"access_token": self.token, "type": upload_type}
+        x = requests.get(
+            f"{self.endpoint}/attachments/{uuid}",
+            params=params,
+            allow_redirects=True,
+            stream=True,
+        )
+        logging.info(f"GET {x.url}")
+        self.catch_auth_error(x)
+        logging.info(f"{x} {x.url}")
+        return x
```

### Comparing `openi-beta-2.0.7/src/openi/cli.py` & `openi-beta-2.0.8/src/openi/cli.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-import argparse
-from .login import login, logout, whoami
-import openi.dataset as dataset
-from .settings import *
-import textwrap
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-        usage=CLI.usage,
-        description=CLI.banner,
-    )
-    parser._action_groups.pop()
-    subparsers = parser.add_subparsers(title="commands", dest="commands")
-    subparsers.required = False
-    # subparsers.choices = Help.openi_choices
-    parse_login(subparsers)
-    parse_logout(subparsers)
-    parse_whoami(subparsers)
-    parse_dataset(subparsers)
-    args = parser.parse_args()
-    if not hasattr(args, "func"):
-        parser.print_help()
-        exit(1)
-
-    command_args = {}
-    command_args.update(vars(args))
-    del command_args["func"]
-    del command_args["commands"]
-    error = False
-    try:
-        out = args.func(**command_args)
-    except Exception as e:
-        print(e)
-        out = None
-        error = True
-    except ValueError as e:
-        print(e)
-        out = None
-        error = True
-    except KeyboardInterrupt:
-        print("User cancelled operation")
-        out = None
-    if out is not None:
-        print(out, end="")
-
-    # This is so that scripts that pick up on error codes can tell when there was a failure
-    if error:
-        exit(1)
-
-
-def parse_login(subparsers):
-    parse_login = subparsers.add_parser(
-        "login",
-        description=CLI.command_login,
-        usage=CLI.login_usage,
-        help=CLI.command_login,
-    )
-    parse_login.add_argument(
-        "-e",  # '--endpoint',
-        dest="endpoint",
-        default=API.ENDPOINT,
-        required=False,
-        help=CLI.param_endpoint,
-    )
-    parse_login.add_argument(
-        "-t",  # '--token',
-        dest="token",
-        default=None,
-        required=False,
-        help=CLI.param_token,
-    )
-    parse_login.set_defaults(func=login)
-
-
-def parse_logout(subparsers):
-    parse_logout = subparsers.add_parser(
-        "logout",
-        description=CLI.command_logout,
-        usage="openi logout [-h]",
-        help=CLI.command_logout,
-    )
-    parse_logout.set_defaults(func=logout)
-
-
-def parse_whoami(subparsers):
-    parse_whoami = subparsers.add_parser(
-        "whoami",
-        description=CLI.command_whoami,
-        usage="openi whoami [-h]",
-        help=CLI.command_whoami,
-    )
-    parse_whoami.set_defaults(func=whoami)
-
-
-def parse_dataset(subparsers):
-    parser_dataset = subparsers.add_parser(
-        "dataset", usage=CLI.dataset_usage, help=CLI.command_dataset, aliases=["d"]
-    )
-    parser_dataset._action_groups.pop()
-    subparsers_dataset = parser_dataset.add_subparsers(
-        title="commands", dest="commands"
-    )
-    subparsers_dataset.required = True
-
-    # dataset upload
-    parser_dataset_upload = subparsers_dataset.add_parser(
-        "upload",
-        description=CLI.command_dataset_upload,
-        usage=CLI.dataset_upload_usage,
-        help=CLI.dataset_upload_help,
-        # epilog=CLI.dataset_upload_epilog,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_dataset_upload._action_groups.pop()
-    parser_dataset_upload_args = parser_dataset_upload.add_argument_group("arguments")
-    parser_dataset_upload_args.add_argument(
-        "-f", dest="file", required=True, help=CLI.dataset_upload_param_file
-    )
-    parser_dataset_upload_args.add_argument(
-        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
-    )
-    parser_dataset_upload_args.add_argument(
-        "-c",
-        dest="cluster",
-        required=False,
-        default="NPU",
-        choices=["gpu", "npu"],
-        help=CLI.dataset_upload_param_cluster,
-    )
-    parser_dataset_upload.set_defaults(func=dataset.upload_file)
-
-    # dataset download
-    parser_dataset_download = subparsers_dataset.add_parser(
-        "download",
-        description=CLI.command_dataset_download,
-        usage=CLI.dataset_download_usage,
-        help=CLI.dataset_download_help,
-        # epilog = CLI.dataset_download_epilog,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_dataset_download._action_groups.pop()
-    parser_dataset_download_args = parser_dataset_download.add_argument_group(
-        "arguments"
-    )
-    parser_dataset_download_args.add_argument(
-        "-f", dest="file", required=True, help=CLI.dataset_download_param_file
-    )
-    parser_dataset_download_args.add_argument(
-        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
-    )
-    parser_dataset_download_args.add_argument(
-        "-c",  #'--cluster',
-        dest="cluster",
-        required=False,
-        default="NPU",
-        choices=["gpu", "npu"],
-        help=CLI.dataset_upload_param_cluster,
-    )
-    parser_dataset_download_args.add_argument(
-        "-p",  #'--save_path',
-        dest="save_path",
-        required=False,
-        default=PATH.SAVE_PATH,
-        help=CLI.dataset_download_param_save_path,
-    )
-    parser_dataset_download.set_defaults(func=dataset.download_file)
+import argparse
+from .login import login, logout, whoami
+import openi.dataset as dataset
+from .settings import *
+import textwrap
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        usage=CLI.usage,
+        description=CLI.banner,
+    )
+    parser._action_groups.pop()
+    subparsers = parser.add_subparsers(title="commands", dest="commands")
+    subparsers.required = False
+    # subparsers.choices = Help.openi_choices
+    parse_login(subparsers)
+    parse_logout(subparsers)
+    parse_whoami(subparsers)
+    parse_dataset(subparsers)
+    args = parser.parse_args()
+    if not hasattr(args, "func"):
+        parser.print_help()
+        exit(1)
+
+    command_args = {}
+    command_args.update(vars(args))
+    del command_args["func"]
+    del command_args["commands"]
+    error = False
+    try:
+        out = args.func(**command_args)
+    except Exception as e:
+        print(e)
+        out = None
+        error = True
+    except ValueError as e:
+        print(e)
+        out = None
+        error = True
+    except KeyboardInterrupt:
+        print("User cancelled operation")
+        out = None
+    if out is not None:
+        print(out, end="")
+
+    # This is so that scripts that pick up on error codes can tell when there was a failure
+    if error:
+        exit(1)
+
+
+def parse_login(subparsers):
+    parse_login = subparsers.add_parser(
+        "login",
+        description=CLI.command_login,
+        usage=CLI.login_usage,
+        help=CLI.command_login,
+    )
+    parse_login.add_argument(
+        "-e",  # '--endpoint',
+        dest="endpoint",
+        default=API.ENDPOINT,
+        required=False,
+        help=CLI.param_endpoint,
+    )
+    parse_login.add_argument(
+        "-t",  # '--token',
+        dest="token",
+        default=None,
+        required=False,
+        help=CLI.param_token,
+    )
+    parse_login.set_defaults(func=login)
+
+
+def parse_logout(subparsers):
+    parse_logout = subparsers.add_parser(
+        "logout",
+        description=CLI.command_logout,
+        usage="openi logout [-h]",
+        help=CLI.command_logout,
+    )
+    parse_logout.set_defaults(func=logout)
+
+
+def parse_whoami(subparsers):
+    parse_whoami = subparsers.add_parser(
+        "whoami",
+        description=CLI.command_whoami,
+        usage="openi whoami [-h]",
+        help=CLI.command_whoami,
+    )
+    parse_whoami.set_defaults(func=whoami)
+
+
+def parse_dataset(subparsers):
+    parser_dataset = subparsers.add_parser(
+        "dataset", usage=CLI.dataset_usage, help=CLI.command_dataset, aliases=["d"]
+    )
+    parser_dataset._action_groups.pop()
+    subparsers_dataset = parser_dataset.add_subparsers(
+        title="commands", dest="commands"
+    )
+    subparsers_dataset.required = True
+
+    # dataset upload
+    parser_dataset_upload = subparsers_dataset.add_parser(
+        "upload",
+        description=CLI.command_dataset_upload,
+        usage=CLI.dataset_upload_usage,
+        help=CLI.dataset_upload_help,
+        # epilog=CLI.dataset_upload_epilog,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_dataset_upload._action_groups.pop()
+    parser_dataset_upload_args = parser_dataset_upload.add_argument_group("arguments")
+    parser_dataset_upload_args.add_argument(
+        "-f", dest="file", required=True, help=CLI.dataset_upload_param_file
+    )
+    parser_dataset_upload_args.add_argument(
+        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
+    )
+    parser_dataset_upload_args.add_argument(
+        "-c",
+        dest="cluster",
+        required=False,
+        default="NPU",
+        choices=["gpu", "npu"],
+        help=CLI.dataset_upload_param_cluster,
+    )
+    parser_dataset_upload.set_defaults(func=dataset.upload_file)
+
+    # dataset download
+    parser_dataset_download = subparsers_dataset.add_parser(
+        "download",
+        description=CLI.command_dataset_download,
+        usage=CLI.dataset_download_usage,
+        help=CLI.dataset_download_help,
+        # epilog = CLI.dataset_download_epilog,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_dataset_download._action_groups.pop()
+    parser_dataset_download_args = parser_dataset_download.add_argument_group(
+        "arguments"
+    )
+    parser_dataset_download_args.add_argument(
+        "-f", dest="file", required=True, help=CLI.dataset_download_param_file
+    )
+    parser_dataset_download_args.add_argument(
+        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
+    )
+    parser_dataset_download_args.add_argument(
+        "-c",  #'--cluster',
+        dest="cluster",
+        required=False,
+        default="NPU",
+        choices=["gpu", "npu"],
+        help=CLI.dataset_upload_param_cluster,
+    )
+    parser_dataset_download_args.add_argument(
+        "-p",  #'--save_path',
+        dest="save_path",
+        required=False,
+        default=PATH.SAVE_PATH,
+        help=CLI.dataset_download_param_save_path,
+    )
+    parser_dataset_download.set_defaults(func=dataset.download_file)
```

### Comparing `openi-beta-2.0.7/src/openi/dataset/dataset_file.py` & `openi-beta-2.0.8/src/openi/dataset/dataset_file.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from openi.utils import file_utils, logger
-from openi.settings import *
-import os
-import logging
-
-logger.setup_logger()
-
-
-"""
-Dataset File class
-"""
-
-
-class DatasetFile:
-    """
-    File object in a dataset from https://openi.pcl.ac.cn/
-
-    Attributes:
-        filepath (`str`):
-            filepath on local machine
-        owner (`str`):
-            username of target repo owner
-        repository (`str`):
-            repository name to which the dataset file is uploaded
-        upload_type (`str`, [`0`,`1`], defaults to `1`):
-            cloud storage type, `0` for GPU and `1` for NPU
-
-        filename (`str`):
-            filepath on local machine
-        size (`str`):
-            filepath on local machine
-        upload_id (`str`):
-            filepath on local machine
-        uuid (`str`):
-            filepath on local machine
-        token (`str`):
-            filepath on local machine
-    """
-
-    def __init__(self, file: str, repo_id: str, cluster: str, **kwargs):
-        self.filepath = os.path.abspath(file)
-        self.filename = os.path.basename(file)
-        self.size = os.path.getsize(file)
-
-        self.owner, self.repository = get_owner_repo(repo_id)
-        self.upload_type, self.cluster = get_upload_type(cluster)
-
-        self.chunk_size = (
-            DATASET.SMALL_FILE_CHUNK_SIZE
-            if self.size < DATASET.SMALL_FILE_LIMIT
-            else DATASET.LARGE_FILE_CHUNK_SIZE
-        )
-        self.total_chunks_count = file_utils.get_file_chunk(
-            chunk_size=self.chunk_size, filesize=self.size
-        )
-
-        self.uuid = None
-        self.md5 = None
-        self.upload_id = None
-        self.dataset_id = None
-
-    def upload_size_check(self):
-        if self.size == 0:
-            msg = f"❌ `{self.filename}` file size is 0"
-            logging.error(msg)
-            raise ValueError(msg)
-        if self.size > DATASET.MAX_FILE_SIZE:
-            msg = f"❌ `{self.filename}` file size exceeds {DATASET.MAX_FILE_SIZE_GB}GB"
-            logging.error(msg)
-            raise ValueError(msg)
-
-
-def get_owner_repo(repo_id: str):
-    try:
-        owner = repo_id.split("/")[0]
-        repository = repo_id.split("/")[1]
-        return owner, repository
-    except:
-        msg = f"❌ argument `repo_id` must be in the form of `owner/repo`"
-        logging.error(msg)
-        raise ValueError(msg)
-
-
-def get_upload_type(cluster: str):
-    try:
-        upload_type = DATASET.SOTRAGE_TYPE[cluster]
-        cluster = cluster
-        return upload_type, cluster
-    except:
-        msg = f"❌ argument `cluster` must be either `GPU` or `NPU`"
-        logging.error(msg)
-        raise ValueError(msg)
+from openi.utils import file_utils, logger
+from openi.settings import *
+import os
+import logging
+
+logger.setup_logger()
+
+
+"""
+Dataset File class
+"""
+
+
+class DatasetFile:
+    """
+    File object in a dataset from https://openi.pcl.ac.cn/
+
+    Attributes:
+        filepath (`str`):
+            filepath on local machine
+        owner (`str`):
+            username of target repo owner
+        repository (`str`):
+            repository name to which the dataset file is uploaded
+        upload_type (`str`, [`0`,`1`], defaults to `1`):
+            cloud storage type, `0` for GPU and `1` for NPU
+
+        filename (`str`):
+            filepath on local machine
+        size (`str`):
+            filepath on local machine
+        upload_id (`str`):
+            filepath on local machine
+        uuid (`str`):
+            filepath on local machine
+        token (`str`):
+            filepath on local machine
+    """
+
+    def __init__(self, file: str, repo_id: str, cluster: str, **kwargs):
+        self.filepath = os.path.abspath(file)
+        self.filename = os.path.basename(file)
+        self.size = os.path.getsize(file)
+
+        self.owner, self.repository = get_owner_repo(repo_id)
+        self.upload_type, self.cluster = get_upload_type(cluster)
+
+        self.chunk_size = (
+            DATASET.SMALL_FILE_CHUNK_SIZE
+            if self.size < DATASET.SMALL_FILE_LIMIT
+            else DATASET.LARGE_FILE_CHUNK_SIZE
+        )
+        self.total_chunks_count = file_utils.get_file_chunk(
+            chunk_size=self.chunk_size, filesize=self.size
+        )
+
+        self.uuid = None
+        self.md5 = None
+        self.upload_id = None
+        self.dataset_id = None
+
+    def upload_size_check(self):
+        if self.size == 0:
+            msg = f"❌ `{self.filename}` file size is 0"
+            logging.error(msg)
+            raise ValueError(msg)
+        if self.size > DATASET.MAX_FILE_SIZE:
+            msg = f"❌ `{self.filename}` file size exceeds {DATASET.MAX_FILE_SIZE_GB}GB"
+            logging.error(msg)
+            raise ValueError(msg)
+
+
+def get_owner_repo(repo_id: str):
+    try:
+        owner = repo_id.split("/")[0]
+        repository = repo_id.split("/")[1]
+        return owner, repository
+    except:
+        msg = f"❌ argument `repo_id` must be in the form of `owner/repo`"
+        logging.error(msg)
+        raise ValueError(msg)
+
+
+def get_upload_type(cluster: str):
+    try:
+        upload_type = DATASET.SOTRAGE_TYPE[cluster]
+        cluster = cluster
+        return upload_type, cluster
+    except:
+        msg = f"❌ argument `cluster` must be either `GPU` or `NPU`"
+        logging.error(msg)
+        raise ValueError(msg)
```

### Comparing `openi-beta-2.0.7/src/openi/dataset/download.py` & `openi-beta-2.0.8/src/openi/dataset/download.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from openi.apis import OpeniAPI
-from .dataset_file import *
-from openi.utils import file_utils, logger
-from openi.settings import *
-from pathlib import Path
-from tqdm import tqdm
-import requests
-import os
-import logging
-
-logger.setup_logger()
-
-
-def download_with_tqdm(response: requests.Response, save_path: str, file: str):
-    """
-    Download file with tqdm progress bar
-    """
-    file_size = int(response.headers.get("content-length", 0))
-    block_size = 1024  # 1 KB
-
-    if not os.path.exists(save_path):
-        os.makedirs(save_path)
-    outfile = os.path.join(save_path, file)
-    if os.path.exists(outfile):
-        outfile = file_utils.rename_existing_file(outfile)
-
-    with tqdm(
-        total=file_size,
-        leave=True,
-        unit="B",
-        unit_scale=True,
-        unit_divisor=1000,
-        bar_format="{desc}{percentage:3.0f}%|{bar}{r_bar}",
-        desc=f"{logger.get_time()} - Downloading: ",
-        dynamic_ncols=True,
-    ) as pbar:
-        with open(outfile, "wb") as f:
-            for data in response.iter_content(block_size):
-                pbar.update(len(data))
-                f.write(data)
-    print(f"{logger.get_time()} - 🎉 Download complete! file was saved to `{outfile}`")
-
-
-def download_file(
-    file: str,
-    repo_id: str,
-    cluster: str = "NPU",
-    save_path: str = PATH.SAVE_PATH,
-    endpoint: str = None,
-    token: str = None,
-):
-    """
-    Download file from dataset
-    """
-
-    _, repo = get_owner_repo(repo_id)
-    upload_type, cluster = get_upload_type(cluster.upper())
-
-    print(f"{logger.get_time()} - `{file}`({cluster}) preprocessing...")
-    outfile = os.path.join(save_path, file)
-
-    api = OpeniAPI(endpoint=endpoint, token=token)
-
-    _datasets = api.get_dataset_attachment(repo_id=repo_id, upload_type=upload_type)
-    if _datasets["data"] is not None:
-        _dataset_info = next(
-            (d for d in _datasets["data"] if d["repo"]["name"] == repo), None
-        )
-    if _datasets["count"] == 0 or _dataset_info is None:
-        raise ValueError(
-            f"❌ `{repo_id}`: dataset not created OR no zipfile({cluster.upper()}) found."
-        )
-    if _dataset_info["attachments"] is not None:
-        _attachment = next(
-            (d for d in _dataset_info["attachments"] if d["name"] == file), None
-        )
-    if _attachment is None:
-        raise ValueError(
-            f"❌ `{file}`({cluster.upper()}): file not found in `{repo_id}`"
-        )
-    uuid = _attachment["uuid"]
-
-    response = api.download_attachments(uuid, upload_type)
-    download_with_tqdm(response, save_path, file)
+from openi.apis import OpeniAPI
+from .dataset_file import *
+from openi.utils import file_utils, logger
+from openi.settings import *
+from pathlib import Path
+from tqdm import tqdm
+import requests
+import os
+import logging
+
+logger.setup_logger()
+
+
+def download_with_tqdm(response: requests.Response, save_path: str, file: str):
+    """
+    Download file with tqdm progress bar
+    """
+    file_size = int(response.headers.get("content-length", 0))
+    block_size = 1024  # 1 KB
+
+    if not os.path.exists(save_path):
+        os.makedirs(save_path)
+    outfile = os.path.join(save_path, file)
+    if os.path.exists(outfile):
+        outfile = file_utils.rename_existing_file(outfile)
+
+    with tqdm(
+        total=file_size,
+        leave=True,
+        unit="B",
+        unit_scale=True,
+        unit_divisor=1000,
+        bar_format="{desc}{percentage:3.0f}%|{bar}{r_bar}",
+        desc=f"{logger.get_time()} - Downloading: ",
+        dynamic_ncols=True,
+    ) as pbar:
+        with open(outfile, "wb") as f:
+            for data in response.iter_content(block_size):
+                pbar.update(len(data))
+                f.write(data)
+    print(f"{logger.get_time()} - 🎉 Download complete! file was saved to `{outfile}`")
+
+
+def download_file(
+    file: str,
+    repo_id: str,
+    cluster: str = "NPU",
+    save_path: str = PATH.SAVE_PATH,
+    endpoint: str = None,
+    token: str = None,
+):
+    """
+    Download file from dataset
+    """
+
+    _, repo = get_owner_repo(repo_id)
+    upload_type, cluster = get_upload_type(cluster.upper())
+
+    print(f"{logger.get_time()} - `{file}`({cluster}) preprocessing...")
+    outfile = os.path.join(save_path, file)
+
+    api = OpeniAPI(endpoint=endpoint, token=token)
+
+    _datasets = api.get_dataset_attachment(repo_id=repo_id, upload_type=upload_type)
+    if _datasets["data"] is not None:
+        _dataset_info = next(
+            (d for d in _datasets["data"] if d["repo"]["name"] == repo), None
+        )
+    if _datasets["count"] == 0 or _dataset_info is None:
+        raise ValueError(
+            f"❌ `{repo_id}`: dataset not created OR no zipfile({cluster.upper()}) found."
+        )
+    if _dataset_info["attachments"] is not None:
+        _attachment = next(
+            (d for d in _dataset_info["attachments"] if d["name"] == file), None
+        )
+    if _attachment is None:
+        raise ValueError(
+            f"❌ `{file}`({cluster.upper()}): file not found in `{repo_id}`"
+        )
+    uuid = _attachment["uuid"]
+
+    response = api.download_attachments(uuid, upload_type)
+    download_with_tqdm(response, save_path, file)
```

### Comparing `openi-beta-2.0.7/src/openi/login.py` & `openi-beta-2.0.8/src/openi/login.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import os
-import json
-from getpass import getpass
-from pathlib import Path
-from openi.apis import OpeniAPI
-from .settings import *
-from openi.utils.file_utils import get_token
-from openi.utils import logger
-import logging
-
-logger.setup_logger()
-
-
-def login(token: str = None, endpoint: str = API.ENDPOINT) -> None:
-    print(
-        """\n
-             ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
-            ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
-            ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
-            ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
-            ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
-             ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝\n
-         """
-    )
-    endpoint = endpoint[:-1] if endpoint[-1] == "/" else endpoint
-
-    if token is None:
-        print(f"点击链接获取令牌并复制粘贴到下列输入栏 {endpoint}/user/settings/applications \n")
-        print(
-            f"[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖 \n"
-            "          若粘贴时切换了本窗口，请先按 退格键⇦ 删除多余空格\n"
-        )
-        token = getpass(prompt="  🔒 token: ")
-    _login(token=token, endpoint=endpoint)
-
-
-def _login(token: str, endpoint: str) -> None:
-    try:
-        api = OpeniAPI(endpoint, token)
-        valid_user = api.login_check()
-
-        if not os.path.exists(PATH.OPENI_FOLDER):
-            os.mkdir(PATH.OPENI_FOLDER)
-        Path(PATH.TOKEN_PATH).write_text(
-            json.dumps({"endpoint": endpoint, "token": token, "username": valid_user})
-        )
-        msg = (
-            f"\n  Your token was saved to `{PATH.TOKEN_PATH}`\n"
-            f"  Successfully logged in as `{valid_user}` @{endpoint}!\n"
-        )
-        logging.info(msg)
-        print(msg)
-    except:
-        raise ValueError("\n  ❌ login failed: invalid token or endpoint!\n")
-
-
-def whoami() -> None:
-    try:
-        api = OpeniAPI()
-        valid_user = api.login_check()
-        msg = f"\n`{valid_user}` @{api.baseURL}\n"
-        logging.info(msg)
-        print(msg)
-    except:
-        msg = f"\nCurrently not logged in.\n"
-        logging.info(msg)
-        print(msg)
-
-
-def logout() -> None:
-    try:
-        valid_user = get_token()["username"]
-        os.remove(PATH.TOKEN_PATH)
-        msg = f"\n`{valid_user}` successfully logged out.\n"
-        logging.info(msg)
-        print(msg)
-    except:
-        msg = "\nCurrently not logged in.\n"
-        logging.info(msg)
-        print(msg)
+import os
+import json
+from getpass import getpass
+from pathlib import Path
+from openi.apis import OpeniAPI
+from .settings import *
+from openi.utils.file_utils import get_token
+from openi.utils import logger
+import logging
+
+logger.setup_logger()
+
+
+def login(token: str = None, endpoint: str = API.ENDPOINT) -> None:
+    print(
+        """\n
+             ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
+            ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
+            ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
+            ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
+            ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
+             ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝\n
+         """
+    )
+    endpoint = endpoint[:-1] if endpoint[-1] == "/" else endpoint
+
+    if token is None:
+        print(f"点击链接获取令牌并复制粘贴到下列输入栏 {endpoint}/user/settings/applications \n")
+        print(
+            f"[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖 \n"
+            "          若粘贴时切换了本窗口，请先按 退格键⇦ 删除多余空格\n"
+        )
+        token = getpass(prompt="  🔒 token: ")
+    _login(token=token, endpoint=endpoint)
+
+
+def _login(token: str, endpoint: str) -> None:
+    try:
+        api = OpeniAPI(endpoint, token)
+        valid_user = api.login_check()
+
+        if not os.path.exists(PATH.OPENI_FOLDER):
+            os.mkdir(PATH.OPENI_FOLDER)
+        Path(PATH.TOKEN_PATH).write_text(
+            json.dumps({"endpoint": endpoint, "token": token, "username": valid_user})
+        )
+        msg = (
+            f"\n  Your token was saved to `{PATH.TOKEN_PATH}`\n"
+            f"  Successfully logged in as `{valid_user}` @{endpoint}!\n"
+        )
+        logging.info(msg)
+        print(msg)
+    except:
+        raise ValueError("\n  ❌ login failed: invalid token or endpoint!\n")
+
+
+def whoami() -> None:
+    try:
+        api = OpeniAPI()
+        valid_user = api.login_check()
+        msg = f"\n`{valid_user}` @{api.baseURL}\n"
+        logging.info(msg)
+        print(msg)
+    except:
+        msg = f"\nCurrently not logged in.\n"
+        logging.info(msg)
+        print(msg)
+
+
+def logout() -> None:
+    try:
+        valid_user = get_token()["username"]
+        os.remove(PATH.TOKEN_PATH)
+        msg = f"\n`{valid_user}` successfully logged out.\n"
+        logging.info(msg)
+        print(msg)
+    except:
+        msg = "\nCurrently not logged in.\n"
+        logging.info(msg)
+        print(msg)
```

### Comparing `openi-beta-2.0.7/src/openi/settings.py` & `openi-beta-2.0.8/src/openi/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import os
-
-# import textwrap
-
-"""
-File PATHs
-"""
-
-
-class PATH(object):
-    OPENI_FOLDER = os.path.join(
-        os.path.expanduser("~"), ".openi"
-    )  # os.path.expanduser('~'), os.getcwd()
-    TOKEN_PATH = os.path.join(OPENI_FOLDER, "token.json")
-    SAVE_PATH = os.path.join(os.getcwd(), "dataset")
-    LOG_PATH = os.path.join(OPENI_FOLDER, "openi.log")
-    TOKEN_PATTERN = r"^[0-9a-fA-F]{40}$"
-
-
-"""
-API
-"""
-
-
-class API(object):
-    ENDPOINT = "https://openi.pcl.ac.cn"
-    VERSION = "/api/v1"
-
-
-"""
-Datasets
-"""
-
-
-class DATASET(object):
-    SOTRAGE_TYPE = {"GPU": 0, "NPU": 1}
-    MAX_FILE_SIZE_GB = 200
-    SMALL_FILE_CHUNK_SIZE = 1024 * 1024 * 8
-    LARGE_FILE_CHUNK_SIZE = 1024 * 1024 * 64
-
-    MAX_CHUNKS = 10000
-    MAX_FILE_SIZE = 1024 * 1024 * 1024 * MAX_FILE_SIZE_GB
-    SMALL_FILE_LIMIT = 1024 * 1024 * 8 * MAX_CHUNKS
-
-
-"""
-CLI help 
-"""
-
-
-class CLI(object):
-    # main help page
-    banner = "OpenI command line tool 启智AI协作平台命令行工具"
-
-    usage = "openi {login, whoami, dataset, ...} [<args>] [-h]"
-    command_login = "使用令牌登录启智并保存到本机"
-    command_logout = "登出当前用户并删除本地令牌文件"
-    command_whoami = "查询当前登录用户"
-    command_dataset = "{upload,download} 上传/下载启智AI协作平台的数据集 "
-
-    # Login
-    login_usage = "openi login [-t token] [-e endpoint] [-h]"
-    param_token = (
-        "选填: 替代命令行输入，启智账号令牌，https://openi.pcl.ac.cn/user/settings/applications"
-    )
-    param_endpoint = "选填: 仅内部使用"
-
-    # Dataset
-    dataset_choices = ["upload", "download"]
-    dataset_usage = "openi dataset {upload,download} [<args>] [-h]"
-
-    command_dataset_upload = "上传数据集文件，需指定文件名,仓库路径及存储类型"
-    dataset_upload_help = "上传数据集文件, openi dataset upload -h 查看更多说明"
-    dataset_upload_usage = (
-        "openi dataset upload [-f file] [-r repo_id] [-c cluster] [-h]"
-    )
-    dataset_upload_param_file = "本地文件名称，包含文件路径"
-    dataset_upload_param_repo_id = "所在仓库路径，格式为`拥有者/仓库名`，登录用户需要拥有此仓库权限"
-    dataset_upload_param_cluster = "选填: 文件的存储集群，不区分大小写，默认为`NPU`"
-    # dataset_upload_epilog = textwrap.dedent(
-    #     """
-    #     用法说明：\n
-    #     登录用户为user1，并且为user2/repo2仓库的协作者 \n
-    #     用法一: openi dataset upload data1.zip user1/repo1 gpu
-    #     上传本地文件`data1.zip`到repo1仓库数据集，存储类型为GPU \n
-    #     用法二: openi d upload localDir/data2.zip user2/repo2
-    #     上传本地文件`./localDir/data2.zip`到协作仓库user2/repo2，存储类型为NPU \n
-    #     """)
-
-    command_dataset_download = "下载数据集文件，需指定文件名,仓库路径及存储类型"
-    dataset_download_help = "下载数据集文件, openi dataset download -h 查看更多说明"
-    dataset_download_usage = (
-        "openi dataset download "
-        "[-f file] [-r repo_id] "
-        "[-c cluster] [-p save_path] [-h]"
-    )
-    dataset_download_param_file = "网页端数据集文件名称，只能下载`.zip`或`.tar.gz`格式的文件"
-    dataset_download_param_save_path = "选填: 本地的保存路径，默认为在当前路径下创建`dataset`目录"
-    # dataset_download_epilog = textwrap.dedent(
-    #     """
-    #     用法说明： \n
-    #     登录用户为user1，并且为user2/repo2仓库的协作者\n
-    #     用法一: openi dataset download data1.zip user1/repo1 gpu -p /downloads
-    #     从repo1仓库下载`data1.zip`(GPU)数据集文件，并存到本地`/downloads/data1.zip`\n
-    #     用法二: openi d download data2.zip user2/repo2
-    #     从协作仓库user2/repo2下载`data2.zip`(NPU)数据集文件，并存到本地`./dataset/data2.zip`\n
-    #     """)
-
-    param_default = "TODO"
+import os
+
+# import textwrap
+
+"""
+File PATHs
+"""
+
+
+class PATH(object):
+    OPENI_FOLDER = os.path.join(
+        os.path.expanduser("~"), ".openi"
+    )  # os.path.expanduser('~'), os.getcwd()
+    TOKEN_PATH = os.path.join(OPENI_FOLDER, "token.json")
+    SAVE_PATH = os.path.join(os.getcwd(), "dataset")
+    LOG_PATH = os.path.join(OPENI_FOLDER, "openi.log")
+    TOKEN_PATTERN = r"^[0-9a-fA-F]{40}$"
+
+
+"""
+API
+"""
+
+
+class API(object):
+    ENDPOINT = "https://openi.pcl.ac.cn"
+    VERSION = "/api/v1"
+
+
+"""
+Datasets
+"""
+
+
+class DATASET(object):
+    SOTRAGE_TYPE = {"GPU": 0, "NPU": 1}
+    MAX_FILE_SIZE_GB = 200
+    SMALL_FILE_CHUNK_SIZE = 1024 * 1024 * 8
+    LARGE_FILE_CHUNK_SIZE = 1024 * 1024 * 64
+
+    MAX_CHUNKS = 10000
+    MAX_FILE_SIZE = 1024 * 1024 * 1024 * MAX_FILE_SIZE_GB
+    SMALL_FILE_LIMIT = 1024 * 1024 * 8 * MAX_CHUNKS
+
+
+"""
+CLI help 
+"""
+
+
+class CLI(object):
+    # main help page
+    banner = "OpenI command line tool 启智AI协作平台命令行工具"
+
+    usage = "openi {login, whoami, dataset, ...} [<args>] [-h]"
+    command_login = "使用令牌登录启智并保存到本机"
+    command_logout = "登出当前用户并删除本地令牌文件"
+    command_whoami = "查询当前登录用户"
+    command_dataset = "{upload,download} 上传/下载启智AI协作平台的数据集 "
+
+    # Login
+    login_usage = "openi login [-t token] [-e endpoint] [-h]"
+    param_token = (
+        "选填: 替代命令行输入，启智账号令牌，https://openi.pcl.ac.cn/user/settings/applications"
+    )
+    param_endpoint = "选填: 仅内部使用"
+
+    # Dataset
+    dataset_choices = ["upload", "download"]
+    dataset_usage = "openi dataset {upload,download} [<args>] [-h]"
+
+    command_dataset_upload = "上传数据集文件，需指定文件名,仓库路径及存储类型"
+    dataset_upload_help = "上传数据集文件, openi dataset upload -h 查看更多说明"
+    dataset_upload_usage = (
+        "openi dataset upload [-f file] [-r repo_id] [-c cluster] [-h]"
+    )
+    dataset_upload_param_file = "本地文件名称，包含文件路径"
+    dataset_upload_param_repo_id = "所在仓库路径，格式为`拥有者/仓库名`，登录用户需要拥有此仓库权限"
+    dataset_upload_param_cluster = "选填: 文件的存储集群，仅支持小写，默认为`npu`"
+    # dataset_upload_epilog = textwrap.dedent(
+    #     """
+    #     用法说明：\n
+    #     登录用户为user1，并且为user2/repo2仓库的协作者 \n
+    #     用法一: openi dataset upload data1.zip user1/repo1 gpu
+    #     上传本地文件`data1.zip`到repo1仓库数据集，存储类型为GPU \n
+    #     用法二: openi d upload localDir/data2.zip user2/repo2
+    #     上传本地文件`./localDir/data2.zip`到协作仓库user2/repo2，存储类型为NPU \n
+    #     """)
+
+    command_dataset_download = "下载数据集文件，需指定文件名,仓库路径及存储类型"
+    dataset_download_help = "下载数据集文件, openi dataset download -h 查看更多说明"
+    dataset_download_usage = (
+        "openi dataset download "
+        "[-f file] [-r repo_id] "
+        "[-c cluster] [-p save_path] [-h]"
+    )
+    dataset_download_param_file = "网页端数据集文件名称，只能下载`.zip`或`.tar.gz`格式的文件"
+    dataset_download_param_save_path = "选填: 本地的保存路径，默认为在当前路径下创建`dataset`目录"
+    # dataset_download_epilog = textwrap.dedent(
+    #     """
+    #     用法说明： \n
+    #     登录用户为user1，并且为user2/repo2仓库的协作者\n
+    #     用法一: openi dataset download data1.zip user1/repo1 gpu -p /downloads
+    #     从repo1仓库下载`data1.zip`(GPU)数据集文件，并存到本地`/downloads/data1.zip`\n
+    #     用法二: openi d download data2.zip user2/repo2
+    #     从协作仓库user2/repo2下载`data2.zip`(NPU)数据集文件，并存到本地`./dataset/data2.zip`\n
+    #     """)
+
+    param_default = "TODO"
```

### Comparing `openi-beta-2.0.7/src/openi/utils/file_utils.py` & `openi-beta-2.0.8/src/openi/utils/file_utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import hashlib
-import math
-import json
-from datetime import datetime
-from pathlib import Path
-from openi.settings import *
-
-
-def calculateMD5(filepath: str = None) -> str:
-    """
-    计算文件的完整md5
-    :param self.filepath:
-    :return:
-    """
-    m = hashlib.md5()  # 创建md5对象
-    with open(filepath, "rb") as f:
-        while True:
-            data = f.read(4096)
-            if not data:
-                break
-            m.update(data)  # 更新md5对象
-    return m.hexdigest()  # 返回md5对象
-
-
-def read_file_chunk(
-    filepath: str = None, start_position: int = 0, chunk_size: int = None
-):
-    with open(filepath, "rb") as file:
-        file.seek(start_position)
-        chunk = file.read(chunk_size)
-        return chunk
-
-
-def get_file_chunk(chunk_size: int, filesize: int = 0) -> dict:
-    total_chunks_count = math.ceil(filesize / chunk_size)
-    return total_chunks_count
-
-
-def get_token() -> str:
-    return json.loads(Path(PATH.TOKEN_PATH).read_text())
-
-
-def rename_existing_file(filepath):
-    if "tar.gz" in filepath:
-        path = filepath.replace(".tar.gz", "")
-        suffix = ".tar.gz"
-    else:
-        path, suffix = os.path.splitext(filepath)
-
-    counter = 1
-    while os.path.exists(filepath):
-        filepath = "{}({}){}".format(path, counter, suffix)
-        counter += 1
-    return filepath
+import hashlib
+import math
+import json
+from datetime import datetime
+from pathlib import Path
+from openi.settings import *
+
+
+def calculateMD5(filepath: str = None) -> str:
+    """
+    计算文件的完整md5
+    :param self.filepath:
+    :return:
+    """
+    m = hashlib.md5()  # 创建md5对象
+    with open(filepath, "rb") as f:
+        while True:
+            data = f.read(4096)
+            if not data:
+                break
+            m.update(data)  # 更新md5对象
+    return m.hexdigest()  # 返回md5对象
+
+
+def read_file_chunk(
+    filepath: str = None, start_position: int = 0, chunk_size: int = None
+):
+    with open(filepath, "rb") as file:
+        file.seek(start_position)
+        chunk = file.read(chunk_size)
+        return chunk
+
+
+def get_file_chunk(chunk_size: int, filesize: int = 0) -> dict:
+    total_chunks_count = math.ceil(filesize / chunk_size)
+    return total_chunks_count
+
+
+def get_token() -> str:
+    return json.loads(Path(PATH.TOKEN_PATH).read_text())
+
+
+def rename_existing_file(filepath):
+    if "tar.gz" in filepath:
+        path = filepath.replace(".tar.gz", "")
+        suffix = ".tar.gz"
+    else:
+        path, suffix = os.path.splitext(filepath)
+
+    counter = 1
+    while os.path.exists(filepath):
+        filepath = "{}({}){}".format(path, counter, suffix)
+        counter += 1
+    return filepath
```

### Comparing `openi-beta-2.0.7/src/openi/utils/logger.py` & `openi-beta-2.0.8/src/openi/utils/logger.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import logging
-import os
-from ..settings import *
-from datetime import datetime
-
-
-def setup_logger():
-    if not os.path.exists(PATH.OPENI_FOLDER):
-        os.mkdir(PATH.OPENI_FOLDER)
-    LOG_FORMAT = "%(asctime)s [%(levelname)s] - %(filename)s %(funcName)s() %(message)s"
-    DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
-    logging.basicConfig(
-        filename=PATH.LOG_PATH,
-        level=logging.INFO,
-        format=LOG_FORMAT,
-        datefmt=DATE_FORMAT,
-    )
-
-
-def get_time():
-    return datetime.now().strftime("%H:%M:%S")
-
-
-def debug(ob):
-    if type(ob) == dict:
-        import json
-
-        print(json.dumps(ob, indent=4))
-    else:
-        print(ob)
-    print("Debug stop!")
-    exit(1)
+import logging
+import os
+from ..settings import *
+from datetime import datetime
+
+
+def setup_logger():
+    if not os.path.exists(PATH.OPENI_FOLDER):
+        os.mkdir(PATH.OPENI_FOLDER)
+    LOG_FORMAT = "%(asctime)s [%(levelname)s] - %(filename)s %(funcName)s() %(message)s"
+    DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
+    logging.basicConfig(
+        filename=PATH.LOG_PATH,
+        level=logging.INFO,
+        format=LOG_FORMAT,
+        datefmt=DATE_FORMAT,
+    )
+
+
+def get_time():
+    return datetime.now().strftime("%H:%M:%S")
+
+
+def debug(ob):
+    if type(ob) == dict:
+        import json
+
+        print(json.dumps(ob, indent=4))
+    else:
+        print(ob)
+    print("Debug stop!")
+    exit(1)
```

### Comparing `openi-beta-2.0.7/src/openi_beta.egg-info/SOURCES.txt` & `openi-beta-2.0.8/src/openi_beta.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 README.md
 setup.py
 src/openi/__init__.py
 src/openi/apis.py
 src/openi/cli.py
 src/openi/login.py
 src/openi/settings.py
-src/openi/cloudbrain/__init__.py
-src/openi/cloudbrain/env_check.py
-src/openi/cloudbrain/helper.py
-src/openi/cloudbrain/minio_operate.py
-src/openi/cloudbrain/obs_operate.py
 src/openi/dataset/__init__.py
 src/openi/dataset/dataset_file.py
 src/openi/dataset/download.py
 src/openi/dataset/upload.py
-src/openi/path/__init__.py
-src/openi/path/path.py
 src/openi/utils/__init__.py
 src/openi/utils/file_utils.py
 src/openi/utils/logger.py
 src/openi_beta.egg-info/PKG-INFO
 src/openi_beta.egg-info/SOURCES.txt
 src/openi_beta.egg-info/dependency_links.txt
 src/openi_beta.egg-info/entry_points.txt
 src/openi_beta.egg-info/requires.txt
-src/openi_beta.egg-info/top_level.txt
-test/test.py
+src/openi_beta.egg-info/top_level.txt
```

