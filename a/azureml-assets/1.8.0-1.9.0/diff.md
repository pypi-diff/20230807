# Comparing `tmp/azureml-assets-1.8.0.tar.gz` & `tmp/azureml-assets-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.8.0.tar", last modified: Thu Jul 20 18:41:20 2023, max compression
+gzip compressed data, was "azureml-assets-1.9.0.tar", last modified: Thu Aug  3 17:26:54 2023, max compression
```

## Comparing `azureml-assets-1.8.0.tar` & `azureml-assets-1.9.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.746642 azureml-assets-1.8.0/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37800 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/copy_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/deployment_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17323 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13212 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15662 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17283 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 17:26:54.751595 azureml-assets-1.9.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-08-03 17:26:54.747595 azureml-assets-1.9.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 17:26:54.739595 azureml-assets-1.9.0/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 17:26:54.743595 azureml-assets-1.9.0/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    37971 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 17:26:54.743595 azureml-assets-1.9.0/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17323 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 17:26:54.747595 azureml-assets-1.9.0/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13212 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 17:26:54.747595 azureml-assets-1.9.0/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15662 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18268 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 17:26:54.747595 azureml-assets-1.9.0/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-08-03 17:26:54.000000 azureml-assets-1.9.0/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-08-03 17:26:54.000000 azureml-assets-1.9.0/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-03 17:26:54.000000 azureml-assets-1.9.0/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-08-03 17:26:54.000000 azureml-assets-1.9.0/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-08-03 17:26:54.000000 azureml-assets-1.9.0/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-03 17:26:54.751595 azureml-assets-1.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-08-03 17:26:13.000000 azureml-assets-1.9.0/setup.py
```

### Comparing `azureml-assets-1.8.0/PKG-INFO` & `azureml-assets-1.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.8.0
+Version: 1.9.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.8.0/azureml/assets/__init__.py` & `azureml-assets-1.9.0/azureml/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/asset_utils.py` & `azureml-assets-1.9.0/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/config.py` & `azureml-assets-1.9.0/azureml/assets/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,14 +635,19 @@
             return None
 
         image = f"{self.publish_visibility.value}/{self.image_name}"
         if tag:
             image += f":{tag}"
         return image
 
+    def get_dockerfile_contents(self) -> str:
+        """Dockerfile contents."""
+        with open(self.dockerfile_with_path, "r") as f:
+            return f.read()
+
     @property
     def _os(self) -> str:
         """Raw 'os' value."""
         return self._image.get('os')
 
     @property
     def os(self) -> Os:
```

### Comparing `azureml-assets-1.8.0/azureml/assets/copy_assets.py` & `azureml-assets-1.9.0/azureml/assets/copy_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/deployment_config.py` & `azureml-assets-1.9.0/azureml/assets/deployment_config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/environment/build.py` & `azureml-assets-1.9.0/azureml/assets/environment/build.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.9.0/azureml/assets/environment/pin_image_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.9.0/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.9.0/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.9.0/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.9.0/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/model/utils.py` & `azureml-assets-1.9.0/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/tag_released_assets.py` & `azureml-assets-1.9.0/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/update_assets.py` & `azureml-assets-1.9.0/azureml/assets/update_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/update_spec.py` & `azureml-assets-1.9.0/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/util/__init__.py` & `azureml-assets-1.9.0/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/util/logger.py` & `azureml-assets-1.9.0/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/util/template.py` & `azureml-assets-1.9.0/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/util/util.py` & `azureml-assets-1.9.0/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/azureml/assets/validate_assets.py` & `azureml-assets-1.9.0/azureml/assets/validate_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 ENVIRONMENT_NAME_FULL_PATTERN = re.compile("".join([
     FRAMEWORK_VERSION,
     f"(?:-{OPERATING_SYSTEM_VERSION})?",
     f"(?:-{PYTHON_VERSION})?",
     f"(?:-(?:{GPU_DRIVER_VERSION}|gpu))?",
 ]))
 
+# Dockerfile convention
+DOCKERFILE_IMAGE_PATTERN = re.compile(r"^FROM\s+mcr\.microsoft\.com/azureml/curated/", re.IGNORECASE | re.MULTILINE)
+
 # Image naming convention
 IMAGE_NAME_PATTERN = re.compile(r"^azureml/curated/(.+)")
 
 
 def _log_error(file: Path, error: str) -> None:
     """Log error.
 
@@ -141,14 +144,35 @@
     if frameworks_found and not ENVIRONMENT_NAME_FULL_PATTERN.search(asset_name):
         _log_error(asset_config.file_name_with_path, f"Name '{asset_name}' elements are out of order")
         error_count += 1
 
     return error_count
 
 
+def validate_dockerfile(environment_config: assets.EnvironmentConfig) -> int:
+    """Validate Dockerfile.
+
+    Args:
+        environment_config (EnvironmentConfig): Environment config.
+
+    Returns:
+        int: Number of errors.
+    """
+    error_count = 0
+    dockerfile = environment_config.get_dockerfile_contents()
+    dockerfile = dockerfile.replace("\r\n", "\n")
+
+    if DOCKERFILE_IMAGE_PATTERN.search(dockerfile):
+        _log_error(environment_config.dockerfile_with_path,
+                   "Referencing curated environment images in Dockerfile is not allowed")
+        error_count += 1
+
+    return error_count
+
+
 def validate_image_publishing(asset_config: assets.AssetConfig,
                               environment_config: assets.EnvironmentConfig = None) -> int:
     """Validate environment image publishing info.
 
     Args:
         asset_config (AssetConfig): Asset config.
         environment_config (EnvironmentConfig, optional): Environment config. Defaults to None.
@@ -324,14 +348,18 @@
             # Validate name
             if check_names:
                 if check_names_skip_pattern is None or not check_names_skip_pattern.fullmatch(asset_config.full_name):
                     error_count += validate_name(asset_config)
                 else:
                     logger.log_debug(f"Skipping name validation for {asset_config.full_name}")
 
+            # Validate Dockerfile
+            if asset_config.type == assets.AssetType.ENVIRONMENT:
+                error_count += validate_dockerfile(asset_config.extra_config_as_object())
+
             # Validate categories
             if check_categories:
                 error_count += validate_categories(asset_config)
 
             # Validate specific asset types
             if environment_config is not None:
                 if check_images:
```

### Comparing `azureml-assets-1.8.0/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.9.0/azureml_assets.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.8.0
+Version: 1.9.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.8.0/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.9.0/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.8.0/setup.py` & `azureml-assets-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.8.0",
+   version="1.9.0",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
```

