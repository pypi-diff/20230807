# Comparing `tmp/prelude-cli-1.3.2.tar.gz` & `tmp/prelude-cli-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.3.2.tar", last modified: Tue Aug  1 18:22:30 2023, max compression
+gzip compressed data, was "prelude-cli-1.3.3.tar", last modified: Mon Aug  7 20:24:12 2023, max compression
```

## Comparing `prelude-cli-1.3.2.tar` & `prelude-cli-1.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.960707 prelude-cli-1.3.2/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-08-01 18:22:30.960753 prelude-cli-1.3.2/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.3.2/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.956825 prelude-cli-1.3.2/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.3.2/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.3.2/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.957646 prelude-cli-1.3.2/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      263 2023-06-27 14:52:45.000000 prelude-cli-1.3.2/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.959254 prelude-cli-1.3.2/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4512 2023-07-26 15:41:33.000000 prelude-cli-1.3.2/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.3.2/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     8536 2023-07-31 17:07:15.000000 prelude-cli-1.3.2/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     4204 2023-07-26 15:41:33.000000 prelude-cli-1.3.2/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     3074 2023-07-26 15:41:33.000000 prelude-cli-1.3.2/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      658 2023-07-17 14:47:48.000000 prelude-cli-1.3.2/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.957455 prelude-cli-1.3.2/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-08-01 18:22:30.960968 prelude-cli-1.3.2/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:24:12.106328 prelude-cli-1.3.3/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.3.3/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.3.3/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-08-07 20:24:12.106375 prelude-cli-1.3.3/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.3.3/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:24:12.103501 prelude-cli-1.3.3/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.3/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.3.3/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.3.3/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:24:12.104376 prelude-cli-1.3.3/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.3/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      263 2023-06-27 14:52:45.000000 prelude-cli-1.3.3/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:24:12.105986 prelude-cli-1.3.3/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.3/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     4512 2023-07-26 15:41:33.000000 prelude-cli-1.3.3/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.3.3/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     9094 2023-08-07 19:56:56.000000 prelude-cli-1.3.3/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     4204 2023-07-26 15:41:33.000000 prelude-cli-1.3.3/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     3074 2023-07-26 15:41:33.000000 prelude-cli-1.3.3/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      658 2023-07-17 14:47:48.000000 prelude-cli-1.3.3/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:24:12.104186 prelude-cli-1.3.3/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-08-07 20:24:12.000000 prelude-cli-1.3.3/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-08-07 20:24:12.000000 prelude-cli-1.3.3/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-08-07 20:24:12.000000 prelude-cli-1.3.3/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-08-07 20:24:12.000000 prelude-cli-1.3.3/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-08-07 20:24:12.000000 prelude-cli-1.3.3/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-08-07 20:24:12.000000 prelude-cli-1.3.3/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.3.3/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-08-07 20:24:12.106582 prelude-cli-1.3.3/setup.cfg
```

### Comparing `prelude-cli-1.3.2/LICENSE` & `prelude-cli-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/PKG-INFO` & `prelude-cli-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.3.2
+Version: 1.3.3
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.3.2/prelude_cli/cli.py` & `prelude-cli-1.3.3/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/prelude_cli/views/build.py` & `prelude-cli-1.3.3/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/prelude_cli/views/configure.py` & `prelude-cli-1.3.3/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/prelude_cli/views/detect.py` & `prelude-cli-1.3.3/prelude_cli/views/detect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 import asyncio 
 
 from rich import print_json
 from pathlib import Path, PurePath
 from datetime import datetime, timedelta
 
-from prelude_sdk.models.codes import RunCode
+from prelude_sdk.models.codes import Control, RunCode
 from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.iam_controller import IAMController
 from prelude_sdk.controllers.detect_controller import DetectController
 
 
 @click.group()
 @click.pass_context
@@ -18,43 +18,49 @@
     ctx.obj = DetectController(account=ctx.obj)
 
 
 @detect.command('create-endpoint')
 @click.option('-h', '--host', help='hostname of this machine', type=str, required=True)
 @click.option('-s', '--serial_num', help='serial number of this machine', type=str, required=True)
 @click.option('-e', '--edr_id', help='EDR id', type=str, default='')
+@click.option('-p', '--partner', help='EDR partner',
+              type=click.Choice([c.name for c in Control], case_sensitive=False), default=Control.INVALID.name, show_default=False)
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default=None)
 @click.pass_obj
 @handle_api_error
-def register_endpoint(controller, host, serial_num, edr_id, tags):
+def register_endpoint(controller, host, serial_num, edr_id, partner, tags):
     """ Register a new endpoint """
     with Spinner(description='Registering endpoint'):
         token = controller.register_endpoint(
-            host=host, 
-            serial_num=serial_num, 
-            edr_id=edr_id, 
+            host=host,
+            serial_num=serial_num,
+            edr_id=edr_id,
+            partner_code=Control[partner.upper()].value,
             tags=tags
         )
     click.secho(token)
 
 
 @detect.command('update-endpoint')
 @click.argument('endpoint_id')
 @click.option('-h', '--host', help='hostname of this machine', type=str, default=None)
 @click.option('-e', '--edr_id', help='EDR id', type=str, default=None)
+@click.option('-p', '--partner', help='EDR partner',
+              type=click.Choice([c.name for c in Control] + ['None'], case_sensitive=False), default=Control.INVALID.name, show_default=False)
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default=None)
 @click.pass_obj
 @handle_api_error
-def update_endpoint(controller, endpoint_id, host, edr_id, tags):
+def update_endpoint(controller, endpoint_id, host, edr_id, partner, tags):
     """ Update an existing endpoint """
     with Spinner(description='Updating endpoint'):
         data = controller.update_endpoint(
             endpoint_id=endpoint_id,
             host=host,
             edr_id=edr_id,
+            partner_code=None if partner.upper() == 'NONE' else Control[partner.upper()].value,
             tags=tags
         )
     print_json(data=data)
 
 
 @detect.command('tests')
 @click.pass_obj
```

### Comparing `prelude-cli-1.3.2/prelude_cli/views/iam.py` & `prelude-cli-1.3.3/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/prelude_cli/views/partner.py` & `prelude-cli-1.3.3/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/prelude_cli/views/shared.py` & `prelude-cli-1.3.3/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.3.3/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.3.2
+Version: 1.3.3
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.3.2/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.3.3/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.2/setup.cfg` & `prelude-cli-1.3.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.3.2
+version = 1.3.3
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.3.4
+	prelude-sdk == 1.3.5
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

