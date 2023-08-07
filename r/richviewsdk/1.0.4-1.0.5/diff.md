# Comparing `tmp/richviewsdk-1.0.4.tar.gz` & `tmp/richviewsdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richviewsdk-1.0.4.tar", last modified: Sun Aug  6 21:20:18 2023, max compression
+gzip compressed data, was "richviewsdk-1.0.5.tar", last modified: Mon Aug  7 07:05:52 2023, max compression
```

## Comparing `richviewsdk-1.0.4.tar` & `richviewsdk-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 21:20:18.331759 richviewsdk-1.0.4/
--rw-rw-rw-   0        0        0       55 2023-08-06 20:35:29.000000 richviewsdk-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2776 2023-08-06 21:20:18.329761 richviewsdk-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-06 21:20:18.290210 richviewsdk-1.0.4/richviewsdk/
--rw-rw-rw-   0        0        0    33298 2023-08-06 21:16:17.000000 richviewsdk-1.0.4/richviewsdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 21:20:18.325225 richviewsdk-1.0.4/richviewsdk.egg-info/
--rw-rw-rw-   0        0        0     2776 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 21:20:18.331759 richviewsdk-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      560 2023-08-06 21:19:54.000000 richviewsdk-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:05:52.608322 richviewsdk-1.0.5/
+-rw-rw-rw-   0        0        0       55 2023-08-06 20:35:29.000000 richviewsdk-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2776 2023-08-07 07:05:52.608322 richviewsdk-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 07:05:52.560260 richviewsdk-1.0.5/richviewsdk/
+-rw-rw-rw-   0        0        0    33938 2023-08-07 07:04:21.000000 richviewsdk-1.0.5/richviewsdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:05:52.608322 richviewsdk-1.0.5/richviewsdk.egg-info/
+-rw-rw-rw-   0        0        0     2776 2023-08-07 07:05:52.000000 richviewsdk-1.0.5/richviewsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-08-07 07:05:52.000000 richviewsdk-1.0.5/richviewsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:05:52.000000 richviewsdk-1.0.5/richviewsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-07 07:05:52.000000 richviewsdk-1.0.5/richviewsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-07 07:05:52.000000 richviewsdk-1.0.5/richviewsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:05:52.616283 richviewsdk-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-08-07 06:20:38.000000 richviewsdk-1.0.5/setup.py
```

### Comparing `richviewsdk-1.0.4/PKG-INFO` & `richviewsdk-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richviewsdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package to interact with RichView API.
 Home-page: https://therichview.com/
 Author: Daniel Vecera
 Author-email: daniel@therichview.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `richviewsdk-1.0.4/richviewsdk/__init__.py` & `richviewsdk-1.0.5/richviewsdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 URL = "https://api.therichview.com"
 
 import warnings
 
 import io
 
+import mergedeep
+
 
 # Moved the RichViewSession class to the top as it is used in other classes
 class RichViewSession:
     """
     A class used to represent a RichView Session.
 
     Attributes
@@ -177,26 +179,30 @@
 
     def update_block(self, **kwargs):
         url_ending = f"/report/{self.report_id}/block/{self.block_id}"
         for kwarg in kwargs.keys():
             assert hasattr(
                 self.data, kwarg
             ), f'Property {kwarg} is not valid for block type {self.block_type}, valid properties are {self.data._fields}'
-        new_data = self.data._asdict() | kwargs
+        new_data = mergedeep.merge({}, self.data._asdict(), kwargs)
         body = {"type": self.block_type, "data": new_data, "id": f"{self.block_id}"}
         response = self.session._put(url_ending, body=body)
         if not response.ok:
             raise Exception(f'Failed to update block: {response.status_code} {response.text}')
 
         self.synced_with_server = False
 
         return _convert_block(block_dict=response.json()['result'],
                               report_id=self.report_id,
                               session=self.session)
 
+    def update_online_version(self):
+        self.update_block(**self.data._asdict())
+        self.synced_with_server = True
+
     def get_online_version(self) -> RichViewBlock:
         if self.synced_with_server:
             warnings.warn('Online version is already synced with local version')
 
         url_ending = f"/report/{self.report_id}/block/{self.block_id}"
         response = self.session._get(url_ending)
         if not response.ok:
@@ -351,15 +357,15 @@
             _type_: _description_
         """
         url_ending = f"/report/{self.report_id}/chart/{self.block_id}"
 
         if not force:
             check_if_all_properties_exist(kwargs, self.chart_options_dict)
 
-        new_options = self.chart_options_dict | kwargs
+        new_options = mergedeep.merge({}, self.chart_options_dict, kwargs)
         body = {"data": {"chartOptions": json.dumps(new_options)}}
         response = self.session._put(url_ending, body=body)
         if not response.ok:
             raise Exception(
                 f'Failed to update chart options: {response.status_code} {response.text}')
         self.synced_with_server = False
         return _convert_block(block_dict=response.json()['result'],
@@ -526,15 +532,24 @@
     __repr__()
         Returns a string representation of the embed block
 
     """
     EmbedBlockData = recordclass('EmbedBlockData',
                                  ['service', 'source', 'embed', 'width', 'height', 'caption'])
 
-    def __init__(self, report_id: str, service: str, source: str, embed: str, width: int, height: int, session: RichViewSession, caption: str = '', id: str = None):
+    def __init__(self,
+                 report_id: str,
+                 service: str,
+                 source: str,
+                 embed: str,
+                 width: int,
+                 height: int,
+                 session: RichViewSession,
+                 caption: str = '',
+                 id: str = None):
         """
 
         """
         data = self.EmbedBlockData(service=service,
                                    source=source,
                                    embed=embed,
                                    width=width,
@@ -553,15 +568,20 @@
     Methods
     -------
     __repr__()
         Returns a string representation of the table block
     """
     TableBlockData = recordclass('TableBlockData', ['content', 'withHeadings'])
 
-    def __init__(self, report_id: str, content: list, withHeadings: bool, session: RichViewSession, id: str = None):
+    def __init__(self,
+                 report_id: str,
+                 content: list,
+                 withHeadings: bool,
+                 session: RichViewSession,
+                 id: str = None):
         """
         Attributes
         ----------
         report_id : str
             The ID of the report the table block belongs to
         content : list
             The content of the table block
@@ -601,15 +621,21 @@
     Methods
     -------
     __repr__()
         Returns a string representation of the code block
     """
     CodeBlockData = recordclass('CodeBlockData', ['code', 'language', 'showlinenumbers'])
 
-    def __init__(self, report_id: str, code: str, language: str, showlinenumbers: bool, session: RichViewSession, id: str = None):
+    def __init__(self,
+                 report_id: str,
+                 code: str,
+                 language: str,
+                 showlinenumbers: bool,
+                 session: RichViewSession,
+                 id: str = None):
         """
 
         """
         data = self.CodeBlockData(code=code, language=language, showlinenumbers=showlinenumbers)
         super().__init__(report_id=report_id, id=id, type='code', data=data, session=session)
 
     def __repr__(self):
@@ -636,15 +662,20 @@
     Methods
     -------
     __repr__()
         Returns a string representation of the list block
     """
     ListBlockData = recordclass('ListBlockData', ['style', 'items'])
 
-    def __init__(self, report_id: str, style: str, items: list, session: RichViewSession, id: str = None):
+    def __init__(self,
+                 report_id: str,
+                 style: str,
+                 items: list,
+                 session: RichViewSession,
+                 id: str = None):
         """
 
         """
         data = self.ListBlockData(style=style, items=items)
         super().__init__(report_id=report_id, id=id, type='list', data=data, session=session)
 
     def __repr__(self):
```

### Comparing `richviewsdk-1.0.4/richviewsdk.egg-info/PKG-INFO` & `richviewsdk-1.0.5/richviewsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richviewsdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package to interact with RichView API.
 Home-page: https://therichview.com/
 Author: Daniel Vecera
 Author-email: daniel@therichview.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `richviewsdk-1.0.4/setup.py` & `richviewsdk-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='richviewsdk',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     url='https://therichview.com/',
     author='Daniel Vecera',
     author_email='daniel@therichview.com',
     description='Package to interact with RichView API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     python_requires='>=3.9',
     install_requires=[
         "recordclass",
         "pandas>=1.2.0",
         "requests",
-        "shortuuid",    ],
+        "shortuuid",
+        "mergedeep"    ],
 )
```

