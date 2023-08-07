# Comparing `tmp/jfrog-client-0.0.2.tar.gz` & `tmp/jfrog-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jfrog-client-0.0.2.tar", last modified: Fri Aug  4 15:29:24 2023, max compression
+gzip compressed data, was "jfrog-client-0.1.0.tar", last modified: Mon Aug  7 15:37:00 2023, max compression
```

## Comparing `jfrog-client-0.0.2.tar` & `jfrog-client-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:24.511782 jfrog-client-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-04 15:29:24.511782 jfrog-client-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:24.507782 jfrog-client-0.0.2/jfrog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/jfrog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/jfrog/artifactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/jfrog/support.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/jfrog/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:24.511782 jfrog-client-0.0.2/jfrog_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-04 15:29:24.000000 jfrog-client-0.0.2/jfrog_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-04 15:29:24.000000 jfrog-client-0.0.2/jfrog_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:29:24.000000 jfrog-client-0.0.2/jfrog_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 15:29:24.000000 jfrog-client-0.0.2/jfrog_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 15:29:24.000000 jfrog-client-0.0.2/jfrog_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:29:24.511782 jfrog-client-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-04 15:28:54.000000 jfrog-client-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:00.474430 jfrog-client-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-08-07 15:37:00.474430 jfrog-client-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:00.470430 jfrog-client-0.1.0/jfrog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/jfrog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/jfrog/artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/jfrog/missioncontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/jfrog/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/jfrog/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/jfrog/xray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:00.474430 jfrog-client-0.1.0/jfrog_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-08-07 15:37:00.000000 jfrog-client-0.1.0/jfrog_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 15:37:00.000000 jfrog-client-0.1.0/jfrog_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:37:00.000000 jfrog-client-0.1.0/jfrog_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 15:37:00.000000 jfrog-client-0.1.0/jfrog_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 15:37:00.000000 jfrog-client-0.1.0/jfrog_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:37:00.474430 jfrog-client-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:00.474430 jfrog-client-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-07 15:36:37.000000 jfrog-client-0.1.0/tests/test_xray.py
```

### Comparing `jfrog-client-0.0.2/LICENSE` & `jfrog-client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jfrog-client-0.0.2/PKG-INFO` & `jfrog-client-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfrog-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: Package that creates simple APIs to interact with Jfrog
 Home-page: https://github.com/peterdeames/jfrog-client
 Keywords: jfrog
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
@@ -88,15 +88,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-This project is collection of API calls that interact with Jfrog to help maintain daily operations such as create projects, delete projects, rename projects.
+This project is collection of API calls that interact with the Jfrog Platform to help maintain daily operations such as checking the health, getting current version, getting storage usage, user details, create repos etc.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built With
 
@@ -142,18 +142,26 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p> -->
 
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] Create Repositories
-    - [ ] Create Local Repository
-    - [ ] Create Remote Repository
-    - [ ] Create Virtual Repository
+- [ ] Platform
+    - [X] Get Count of Users
+- [ ] Artifactory
+    - [x] Ping Artifactory Instance
+    - [x] Get Artifactory Version
+    - [x] Get Artifactory Licence Details
+    - [x] Get Count of Repositories
+- [ ] Mission Control
+    - [X] Ping Mission Control Instance
+- [ ] Xray
+    - [x] Ping Xray Instance
+    - [x] Get Xray Version
 
 
 See the [open issues](https://github.com/peterdeames/jfrog-client/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jfrog-client Version: 0.0.2 Summary: Package that
+Metadata-Version: 2.1 Name: jfrog-client Version: 0.1.0 Summary: Package that
 creates simple APIs to interact with Jfrog Home-page: https://github.com/
 peterdeames/jfrog-client Keywords: jfrog Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: System Administrators Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE
     [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
@@ -29,29 +29,32 @@
    3. Usage
    4. Roadmap
    5. Contributing
    6. License
    7. Contact
    8. Acknowledgments
   ## About The Project This project is collection of API calls that interact
-with Jfrog to help maintain daily operations such as create projects, delete
-projects, rename projects.
+with the Jfrog Platform to help maintain daily operations such as checking the
+health, getting current version, getting storage usage, user details, create
+repos etc.
                                                                   (back_to_top)
 ### Built With [![Python][Python.org]][Python-url]
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites This is an example of how to list things you
 need to use the software and how to install them. * python ### Installation 1.
 Clone the repo ```sh git clone https://github.com/peterdeames/jfrog-client.git
 ``` 2. Install Python packages ```sh pip install -r requirements.txt ```
                                                                   (back_to_top)
-   ## Roadmap - [ ] Create Repositories - [ ] Create Local Repository - [ ]
-Create Remote Repository - [ ] Create Virtual Repository See the [open issues]
-(https://github.com/peterdeames/jfrog-client/issues) for a full list of
-proposed features (and known issues).
+   ## Roadmap - [ ] Platform - [X] Get Count of Users - [ ] Artifactory - [x]
+Ping Artifactory Instance - [x] Get Artifactory Version - [x] Get Artifactory
+Licence Details - [x] Get Count of Repositories - [ ] Mission Control - [X]
+Ping Mission Control Instance - [ ] Xray - [x] Ping Xray Instance - [x] Get
+Xray Version See the [open issues](https://github.com/peterdeames/jfrog-client/
+issues) for a full list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `jfrog-client-0.0.2/README.md` & `jfrog-client-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-This project is collection of API calls that interact with Jfrog to help maintain daily operations such as create projects, delete projects, rename projects.
+This project is collection of API calls that interact with the Jfrog Platform to help maintain daily operations such as checking the health, getting current version, getting storage usage, user details, create repos etc.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built With
 
@@ -127,18 +127,26 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p> -->
 
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] Create Repositories
-    - [ ] Create Local Repository
-    - [ ] Create Remote Repository
-    - [ ] Create Virtual Repository
+- [ ] Platform
+    - [X] Get Count of Users
+- [ ] Artifactory
+    - [x] Ping Artifactory Instance
+    - [x] Get Artifactory Version
+    - [x] Get Artifactory Licence Details
+    - [x] Get Count of Repositories
+- [ ] Mission Control
+    - [X] Ping Mission Control Instance
+- [ ] Xray
+    - [x] Ping Xray Instance
+    - [x] Get Xray Version
 
 
 See the [open issues](https://github.com/peterdeames/jfrog-client/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -22,29 +22,32 @@
    3. Usage
    4. Roadmap
    5. Contributing
    6. License
    7. Contact
    8. Acknowledgments
   ## About The Project This project is collection of API calls that interact
-with Jfrog to help maintain daily operations such as create projects, delete
-projects, rename projects.
+with the Jfrog Platform to help maintain daily operations such as checking the
+health, getting current version, getting storage usage, user details, create
+repos etc.
                                                                   (back_to_top)
 ### Built With [![Python][Python.org]][Python-url]
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites This is an example of how to list things you
 need to use the software and how to install them. * python ### Installation 1.
 Clone the repo ```sh git clone https://github.com/peterdeames/jfrog-client.git
 ``` 2. Install Python packages ```sh pip install -r requirements.txt ```
                                                                   (back_to_top)
-   ## Roadmap - [ ] Create Repositories - [ ] Create Local Repository - [ ]
-Create Remote Repository - [ ] Create Virtual Repository See the [open issues]
-(https://github.com/peterdeames/jfrog-client/issues) for a full list of
-proposed features (and known issues).
+   ## Roadmap - [ ] Platform - [X] Get Count of Users - [ ] Artifactory - [x]
+Ping Artifactory Instance - [x] Get Artifactory Version - [x] Get Artifactory
+Licence Details - [x] Get Count of Repositories - [ ] Mission Control - [X]
+Ping Mission Control Instance - [ ] Xray - [x] Ping Xray Instance - [x] Get
+Xray Version See the [open issues](https://github.com/peterdeames/jfrog-client/
+issues) for a full list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `jfrog-client-0.0.2/jfrog/support.py` & `jfrog-client-0.1.0/jfrog/xray.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,77 @@
-""" functions to support the JFrog Platform """
+""" functions to manage Artifactory """
 
 import logging
 import requests
 from tabulate import tabulate
+from jfrog import utilities
 
 HEADERS = {'content-type': 'application/json'}
 
 # The different levels of logging, from highest urgency to lowest urgency, are:
 # CRITICAL | ERROR | WARNING | INFO | DEBUG
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
 )
 
 
-def artifactory_ping(url, token):
+def xray_ping(url, token):
     """
-    This function is intented to get the health info of Jfrog Platform
+    This function is intented to get the health info of Jfrog xray
 
     Parameters
     ----------
     arg1 : str
         base URL of JFrog Platform
     arg2 : str
         access or identity token of admin account
 
     Returns
     -------
     str
         reponse
     """
     HEADERS.update({"Authorization": "Bearer " + token})
-    urltopost = url + "/api/system/ping"
+    url = utilities.__validate_url(url)  # pylint: disable=W0212
+    urltopost = url + "/xray/api/v1/system/ping"
     response = requests.get(urltopost, headers=HEADERS, timeout=30)
     if response.ok:
-        logging.info("Your Artifactory Instance is currently healthy")
+        logging.info("Your Xray Instance is currently healthy")
     else:
-        logging.error("Your Artifactory Instance is not healthy")
-        logging.error(response.text)
+        logging.warning("Your Xray Instance may not be healthy")
+        try:
+            print(tabulate(response.json()))
+        except ValueError:
+            logging.warning("Please Xray is installed")
     return response
 
 
-def artifactory_version(url, token):
+def xray_version(url, token):
     """
-    This function is intented to get the version info of Jfrog Platform
+    This function is intented to get the version info of xray
 
     Parameters
     ----------
     arg1 : str
         base URL of Jfrog PLatform
     arg2 : str
         access or identity token of admin account
 
     Returns
     -------
     str
-        version of artifactory
+        version of xray
     """
     HEADERS.update({"Authorization": "Bearer " + token})
-    urltopost = url + "/api/system/version"
+    url = utilities.__validate_url(url)  # pylint: disable=W0212
+    urltopost = url + "/xray/api/v1/system/version"
     response = requests.get(urltopost, headers=HEADERS, timeout=30)
-    versioninfo = response.json()
     if response.ok:
+        versioninfo = response.json()
         logging.info(
-            "Your Artifactory Instance is currently running %s", versioninfo['version'])
+            "Your Xray Instance is currently running %s", versioninfo['xray_version'])
+        version = versioninfo['xray_version']
     else:
-        logging.error("Could not determin the Artifactory version")
-        logging.error(response.text)
-    return versioninfo['version']
-
-
-def xray_ping(url, token):
-    """
-    This function is intented to get the health info of Jfrog xray
-
-    Parameters
-    ----------
-    arg1 : str
-        base URL of JFrog Platform
-    arg2 : str
-        access or identity token of admin account
-
-    Returns
-    -------
-    str
-        reponse
-    """
-    HEADERS.update({"Authorization": "Bearer " + token})
-    urltopost = url + "/api/v1/system/ping"
-    response = requests.get(urltopost, headers=HEADERS, timeout=30)
-    if response.ok:
-        logging.info("Your Xray Instance is currently healthy")
-    else:
-        logging.error("Your Xray Instance is not healthy")
-        logging.error(response.text)
-    return response
-
-
-def get_license_details(url, token):
-    """
-    This function is intented to get the license info of Jfrog Platform
-
-    Parameters
-    ----------
-    arg1 : str
-        base URL of Jfrog Platform
-    arg2 : str
-        access or identity token of admin account
-
-    Returns
-    -------
-    dict
-        dictionary of license information
-
-    """
-    HEADERS.update({"Authorization": "Bearer " + token})
-    urltopost = url + "/api/system/license"
-    response = requests.get(urltopost, headers=HEADERS, timeout=30)
-    result = response.json()
-    print(tabulate(result.items()))
-    return result
+        logging.error("Could not determin the Xray version")
+        print(tabulate(response.json()))
+        version = 0.0
+    return version
```

### Comparing `jfrog-client-0.0.2/jfrog_client.egg-info/PKG-INFO` & `jfrog-client-0.1.0/jfrog_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfrog-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: Package that creates simple APIs to interact with Jfrog
 Home-page: https://github.com/peterdeames/jfrog-client
 Keywords: jfrog
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
@@ -88,15 +88,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-This project is collection of API calls that interact with Jfrog to help maintain daily operations such as create projects, delete projects, rename projects.
+This project is collection of API calls that interact with the Jfrog Platform to help maintain daily operations such as checking the health, getting current version, getting storage usage, user details, create repos etc.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built With
 
@@ -142,18 +142,26 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p> -->
 
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] Create Repositories
-    - [ ] Create Local Repository
-    - [ ] Create Remote Repository
-    - [ ] Create Virtual Repository
+- [ ] Platform
+    - [X] Get Count of Users
+- [ ] Artifactory
+    - [x] Ping Artifactory Instance
+    - [x] Get Artifactory Version
+    - [x] Get Artifactory Licence Details
+    - [x] Get Count of Repositories
+- [ ] Mission Control
+    - [X] Ping Mission Control Instance
+- [ ] Xray
+    - [x] Ping Xray Instance
+    - [x] Get Xray Version
 
 
 See the [open issues](https://github.com/peterdeames/jfrog-client/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jfrog-client Version: 0.0.2 Summary: Package that
+Metadata-Version: 2.1 Name: jfrog-client Version: 0.1.0 Summary: Package that
 creates simple APIs to interact with Jfrog Home-page: https://github.com/
 peterdeames/jfrog-client Keywords: jfrog Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: System Administrators Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE
     [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
@@ -29,29 +29,32 @@
    3. Usage
    4. Roadmap
    5. Contributing
    6. License
    7. Contact
    8. Acknowledgments
   ## About The Project This project is collection of API calls that interact
-with Jfrog to help maintain daily operations such as create projects, delete
-projects, rename projects.
+with the Jfrog Platform to help maintain daily operations such as checking the
+health, getting current version, getting storage usage, user details, create
+repos etc.
                                                                   (back_to_top)
 ### Built With [![Python][Python.org]][Python-url]
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites This is an example of how to list things you
 need to use the software and how to install them. * python ### Installation 1.
 Clone the repo ```sh git clone https://github.com/peterdeames/jfrog-client.git
 ``` 2. Install Python packages ```sh pip install -r requirements.txt ```
                                                                   (back_to_top)
-   ## Roadmap - [ ] Create Repositories - [ ] Create Local Repository - [ ]
-Create Remote Repository - [ ] Create Virtual Repository See the [open issues]
-(https://github.com/peterdeames/jfrog-client/issues) for a full list of
-proposed features (and known issues).
+   ## Roadmap - [ ] Platform - [X] Get Count of Users - [ ] Artifactory - [x]
+Ping Artifactory Instance - [x] Get Artifactory Version - [x] Get Artifactory
+Licence Details - [x] Get Count of Repositories - [ ] Mission Control - [X]
+Ping Mission Control Instance - [ ] Xray - [x] Ping Xray Instance - [x] Get
+Xray Version See the [open issues](https://github.com/peterdeames/jfrog-client/
+issues) for a full list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `jfrog-client-0.0.2/setup.py` & `jfrog-client-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='jfrog-client',
-    version='0.0.2',
+    version='0.1.0',
     description='Package that creates simple APIs to interact with Jfrog',
     packages=setuptools.find_packages(),
     url='https://github.com/peterdeames/jfrog-client',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='jfrog',
     classifiers=[
@@ -22,10 +22,11 @@
         'Intended Audience :: System Administrators',
         'Programming Language :: Python',
         'Topic :: Utilities',
         'Operating System :: OS Independent'
     ],
     install_requires=[
         'requests',
-        'tabulate'
+        'tabulate',
+        'logging'
     ]
 )
```

