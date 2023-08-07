# Comparing `tmp/dapplooker-0.0.3.tar.gz` & `tmp/dapplooker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapplooker-0.0.3.tar", last modified: Sat Jul 22 21:00:35 2023, max compression
+gzip compressed data, was "dapplooker-0.0.4.tar", last modified: Mon Aug  7 20:39:26 2023, max compression
```

## Comparing `dapplooker-0.0.3.tar` & `dapplooker-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 21:00:35.275759 dapplooker-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-07-22 20:42:35.000000 dapplooker-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3646 2023-07-22 21:00:35.272740 dapplooker-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3317 2023-07-22 20:39:31.000000 dapplooker-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 21:00:35.174742 dapplooker-0.0.3/dapplooker/
--rw-rw-rw-   0        0        0       50 2023-07-22 20:07:29.000000 dapplooker-0.0.3/dapplooker/__init__.py
--rw-rw-rw-   0        0        0      456 2023-07-22 17:10:42.000000 dapplooker-0.0.3/dapplooker/chart_constants.py
--rw-rw-rw-   0        0        0     1918 2023-07-22 20:18:31.000000 dapplooker-0.0.3/dapplooker/dapplooker_charts.py
--rw-rw-rw-   0        0        0      747 2023-07-22 17:12:39.000000 dapplooker-0.0.3/dapplooker/interface.py
-drwxrwxrwx   0        0        0        0 2023-07-22 21:00:35.268738 dapplooker-0.0.3/dapplooker.egg-info/
--rw-rw-rw-   0        0        0     3646 2023-07-22 21:00:33.000000 dapplooker-0.0.3/dapplooker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-22 19:56:55.000000 dapplooker-0.0.3/dapplooker.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 21:00:35.277753 dapplooker-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-07-22 21:00:11.000000 dapplooker-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:39:26.110468 dapplooker-0.0.4/
+-rw-rw-rw-   0        0        0     3305 2023-08-07 20:39:26.094823 dapplooker-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3027 2023-08-07 20:24:56.000000 dapplooker-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 20:39:26.025794 dapplooker-0.0.4/dapplooker/
+-rw-rw-rw-   0        0        0       52 2023-08-07 20:25:21.000000 dapplooker-0.0.4/dapplooker/__init__.py
+-rw-rw-rw-   0        0        0      456 2023-08-07 20:24:56.000000 dapplooker-0.0.4/dapplooker/chart_constants.py
+-rw-rw-rw-   0        0        0     2904 2023-08-07 20:36:22.000000 dapplooker-0.0.4/dapplooker/dapplooker_charts.py
+-rw-rw-rw-   0        0        0      747 2023-08-07 20:36:43.000000 dapplooker-0.0.4/dapplooker/interface.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:39:26.094823 dapplooker-0.0.4/dapplooker.egg-info/
+-rw-rw-rw-   0        0        0     3305 2023-08-07 20:39:25.000000 dapplooker-0.0.4/dapplooker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-08-07 20:39:25.000000 dapplooker-0.0.4/dapplooker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 20:39:25.000000 dapplooker-0.0.4/dapplooker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 20:39:25.000000 dapplooker-0.0.4/dapplooker.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-08-07 20:39:25.000000 dapplooker-0.0.4/dapplooker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 20:39:25.000000 dapplooker-0.0.4/dapplooker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 20:39:26.110468 dapplooker-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-08-07 20:37:03.000000 dapplooker-0.0.4/setup.py
```

### Comparing `dapplooker-0.0.3/PKG-INFO` & `dapplooker-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dapplooker
-Version: 0.0.3
+Version: 0.0.4
 Summary: A minimal, complete, python API for DappLooker
 Home-page: https://github.com/0xSumitBanik/dapplooker-py-sdk
 Author: Sumit Banik
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # DappLooker Python SDK
 
 ![DappLooker Logo](https://d2yxqfr8upg55w.cloudfront.net/npm-package-images/DLLogo1800x400.png)
 
 Discover blockchain insights effortlessly with the DappLooker Python SDK. Access reliable Web3 data and popular Dapp charts via the DappLooker Analytics platform. Enhance your Python projects with seamless integration.
 
-**Heavily inspired by [DappLooker SDK](https://github.com/dapplooker/dapplooker-sdk/)**
+
+[![Downloads](https://pepy.tech/badge/dapplooker)](https://pepy.tech/project/dapplooker)
+
 
 ## Introduction
 
 DappLooker Python SDK provides developers with programmatic access to comprehensive blockchain data in the Web3 environment. With this SDK, you can easily retrieve popular charts data for your decentralized applications (Dapps). The DappLooker Analytics platform offers a no-code, community-driven analytics and visualization platform for blockchain networks and Dapps.
 
 ## Features
 
@@ -77,19 +77,8 @@
 
 - **[DappLooker Website](https://dapplooker.com/)** - To discover our product and analytics platform.
 - **[DappLooker SDK Repository](https://github.com/dapplooker/dapplooker-sdk/)** - To explore the inspiration for this Python SDK.
 - **[DappLooker Documentation](https://docs.dapplooker.com)** - For comprehensive documentation on the SDK and analytics platform.
 
 ## Contributing
 
-We welcome contributions from the community to improve the DappLooker Python SDK. If you find any issues, have suggestions for new features, or want to help with bug fixes, feel free to submit a pull request or create an issue on the [GitHub repository](https://github.com/0xSumitBanik/dapplooker-py-sdk).
-
-## License
-
-The DappLooker Python SDK is licensed under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use and modify it in your projects.
-
-## Contact
-
-For any questions or support, 
-
-Let's enhance blockchain analytics together with DappLooker Python SDK ðŸš€
-
+We welcome contributions from the community to improve the DappLooker Python SDK. If you find any issues, have suggestions for new features, or want to help with bug fixes, feel free to submit a pull request or create an issue on the [GitHub repository](https://github.com/dapplooker/dapplooker-sdk/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dapplooker-0.0.3/README.md` & `dapplooker-0.0.4/dapplooker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+Metadata-Version: 2.1
+Name: dapplooker
+Version: 0.0.4
+Summary: A minimal, complete, python API for DappLooker
+Home-page: https://github.com/0xSumitBanik/dapplooker-py-sdk
+Author: Sumit Banik
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # DappLooker Python SDK
 
 ![DappLooker Logo](https://d2yxqfr8upg55w.cloudfront.net/npm-package-images/DLLogo1800x400.png)
 
 Discover blockchain insights effortlessly with the DappLooker Python SDK. Access reliable Web3 data and popular Dapp charts via the DappLooker Analytics platform. Enhance your Python projects with seamless integration.
 
-**Heavily inspired by [DappLooker SDK](https://github.com/dapplooker/dapplooker-sdk/)**
+
+[![Downloads](https://pepy.tech/badge/dapplooker)](https://pepy.tech/project/dapplooker)
+
 
 ## Introduction
 
 DappLooker Python SDK provides developers with programmatic access to comprehensive blockchain data in the Web3 environment. With this SDK, you can easily retrieve popular charts data for your decentralized applications (Dapps). The DappLooker Analytics platform offers a no-code, community-driven analytics and visualization platform for blockchain networks and Dapps.
 
 ## Features
 
@@ -65,18 +77,8 @@
 
 - **[DappLooker Website](https://dapplooker.com/)** - To discover our product and analytics platform.
 - **[DappLooker SDK Repository](https://github.com/dapplooker/dapplooker-sdk/)** - To explore the inspiration for this Python SDK.
 - **[DappLooker Documentation](https://docs.dapplooker.com)** - For comprehensive documentation on the SDK and analytics platform.
 
 ## Contributing
 
-We welcome contributions from the community to improve the DappLooker Python SDK. If you find any issues, have suggestions for new features, or want to help with bug fixes, feel free to submit a pull request or create an issue on the [GitHub repository](https://github.com/0xSumitBanik/dapplooker-py-sdk).
-
-## License
-
-The DappLooker Python SDK is licensed under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use and modify it in your projects.
-
-## Contact
-
-For any questions or support, 
-
-Let's enhance blockchain analytics together with DappLooker Python SDK 🚀
+We welcome contributions from the community to improve the DappLooker Python SDK. If you find any issues, have suggestions for new features, or want to help with bug fixes, feel free to submit a pull request or create an issue on the [GitHub repository](https://github.com/dapplooker/dapplooker-sdk/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dapplooker-0.0.3/dapplooker/interface.py` & `dapplooker-0.0.4/dapplooker/interface.py`

 * *Files identical despite different names*

### Comparing `dapplooker-0.0.3/dapplooker.egg-info/PKG-INFO` & `dapplooker-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,16 @@
-Metadata-Version: 2.1
-Name: dapplooker
-Version: 0.0.3
-Summary: A minimal, complete, python API for DappLooker
-Home-page: https://github.com/0xSumitBanik/dapplooker-py-sdk
-Author: Sumit Banik
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DappLooker Python SDK
 
 ![DappLooker Logo](https://d2yxqfr8upg55w.cloudfront.net/npm-package-images/DLLogo1800x400.png)
 
 Discover blockchain insights effortlessly with the DappLooker Python SDK. Access reliable Web3 data and popular Dapp charts via the DappLooker Analytics platform. Enhance your Python projects with seamless integration.
 
-**Heavily inspired by [DappLooker SDK](https://github.com/dapplooker/dapplooker-sdk/)**
+
+[![Downloads](https://pepy.tech/badge/dapplooker)](https://pepy.tech/project/dapplooker)
+
 
 ## Introduction
 
 DappLooker Python SDK provides developers with programmatic access to comprehensive blockchain data in the Web3 environment. With this SDK, you can easily retrieve popular charts data for your decentralized applications (Dapps). The DappLooker Analytics platform offers a no-code, community-driven analytics and visualization platform for blockchain networks and Dapps.
 
 ## Features
 
@@ -77,19 +67,8 @@
 
 - **[DappLooker Website](https://dapplooker.com/)** - To discover our product and analytics platform.
 - **[DappLooker SDK Repository](https://github.com/dapplooker/dapplooker-sdk/)** - To explore the inspiration for this Python SDK.
 - **[DappLooker Documentation](https://docs.dapplooker.com)** - For comprehensive documentation on the SDK and analytics platform.
 
 ## Contributing
 
-We welcome contributions from the community to improve the DappLooker Python SDK. If you find any issues, have suggestions for new features, or want to help with bug fixes, feel free to submit a pull request or create an issue on the [GitHub repository](https://github.com/0xSumitBanik/dapplooker-py-sdk).
-
-## License
-
-The DappLooker Python SDK is licensed under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use and modify it in your projects.
-
-## Contact
-
-For any questions or support, 
-
-Let's enhance blockchain analytics together with DappLooker Python SDK ðŸš€
-
+We welcome contributions from the community to improve the DappLooker Python SDK. If you find any issues, have suggestions for new features, or want to help with bug fixes, feel free to submit a pull request or create an issue on the [GitHub repository](https://github.com/dapplooker/dapplooker-sdk/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dapplooker-0.0.3/setup.py` & `dapplooker-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # read the contents of  README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="dapplooker",
-    version="0.0.3",
+    version="0.0.4",
     description="A minimal, complete, python API for DappLooker",
     long_description=long_description,
     url="https://github.com/0xSumitBanik/dapplooker-py-sdk",
     long_description_content_type="text/markdown",
     author="Sumit Banik",
     license="MIT",
     packages=[
         "dapplooker"
     ],
     python_requires='>=3.8',
     install_requires=["requests"],
     include_package_data=True,
     zip_safe=False,
-)
+)
```

