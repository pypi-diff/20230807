# Comparing `tmp/hydroloader-0.1.8.tar.gz` & `tmp/hydroloader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroloader-0.1.8.tar", last modified: Tue Jul 25 16:42:05 2023, max compression
+gzip compressed data, was "hydroloader-0.1.9.tar", last modified: Tue Jul 25 17:43:28 2023, max compression
```

## Comparing `hydroloader-0.1.8.tar` & `hydroloader-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.676277 hydroloader-0.1.8/
--rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.8/LICENSE.txt
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-07-25 16:42:05.676345 hydroloader-0.1.8/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.8/README.md
--rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.8/pyproject.toml
--rw-r--r--   0 klippold   (501) staff       (20)      378 2023-07-25 16:42:05.676654 hydroloader-0.1.8/setup.cfg
--rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.8/setup.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.673361 hydroloader-0.1.8/src/
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.675111 hydroloader-0.1.8/src/hydroloader/
--rw-r--r--   0 klippold   (501) staff       (20)      396 2023-06-26 22:58:34.000000 hydroloader-0.1.8/src/hydroloader/__init__.py
--rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.8/src/hydroloader/exceptions.py
--rw-r--r--   0 klippold   (501) staff       (20)    15536 2023-06-30 05:21:23.000000 hydroloader-0.1.8/src/hydroloader/main.py
--rw-r--r--   0 klippold   (501) staff       (20)     7973 2023-07-25 16:37:24.000000 hydroloader-0.1.8/src/hydroloader/models.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.675941 hydroloader-0.1.8/src/hydroloader.egg-info/
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)      391 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/SOURCES.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/dependency_links.txt
--rw-r--r--   0 klippold   (501) staff       (20)      124 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/requires.txt
--rw-r--r--   0 klippold   (501) staff       (20)       12 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/top_level.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.8/src/hydroloader.egg-info/zip-safe
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 17:43:28.659288 hydroloader-0.1.9/
+-rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.9/LICENSE.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-07-25 17:43:28.659334 hydroloader-0.1.9/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.9/README.md
+-rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.9/pyproject.toml
+-rw-r--r--   0 klippold   (501) staff       (20)      378 2023-07-25 17:43:28.659563 hydroloader-0.1.9/setup.cfg
+-rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.9/setup.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 17:43:28.656936 hydroloader-0.1.9/src/
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 17:43:28.658130 hydroloader-0.1.9/src/hydroloader/
+-rw-r--r--   0 klippold   (501) staff       (20)      396 2023-06-26 22:58:34.000000 hydroloader-0.1.9/src/hydroloader/__init__.py
+-rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.9/src/hydroloader/exceptions.py
+-rw-r--r--   0 klippold   (501) staff       (20)    15533 2023-07-25 17:30:41.000000 hydroloader-0.1.9/src/hydroloader/main.py
+-rw-r--r--   0 klippold   (501) staff       (20)     7973 2023-07-25 16:37:24.000000 hydroloader-0.1.9/src/hydroloader/models.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 17:43:28.658952 hydroloader-0.1.9/src/hydroloader.egg-info/
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-07-25 17:43:28.000000 hydroloader-0.1.9/src/hydroloader.egg-info/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)      391 2023-07-25 17:43:28.000000 hydroloader-0.1.9/src/hydroloader.egg-info/SOURCES.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-07-25 17:43:28.000000 hydroloader-0.1.9/src/hydroloader.egg-info/dependency_links.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      124 2023-07-25 17:43:28.000000 hydroloader-0.1.9/src/hydroloader.egg-info/requires.txt
+-rw-r--r--   0 klippold   (501) staff       (20)       12 2023-07-25 17:43:28.000000 hydroloader-0.1.9/src/hydroloader.egg-info/top_level.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.9/src/hydroloader.egg-info/zip-safe
```

### Comparing `hydroloader-0.1.8/LICENSE.txt` & `hydroloader-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydroloader-0.1.8/src/hydroloader/main.py` & `hydroloader-0.1.9/src/hydroloader/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         datastream IDs in the conf file.
 
         :param self: Bind the method to an object
         :return: A dictionary of datastreams
         """
 
         for datastream in self.conf.datastreams:
-            request_url = f'{self.service}/Datastreams({datastream.datastream_id})'
+            request_url = f'{self.service}/Datastreams({datastream.id})'
 
             try:
                 raw_response = self.client.get(request_url)
             except requests.exceptions.RequestException as e:
                 logger.error(
                     'Failed to make request to "' + request_url + '" with error: ' + str(e)
                 )
@@ -85,24 +85,24 @@
             except ValueError as e:
                 logger.error(
                     'Failed to parse SensorThings response from "' + request_url + '" with error: ' + str(e)
                 )
                 continue
 
             try:
-                if self.datastreams.get(str(datastream.datastream_id)):
-                    self.datastreams[str(datastream.datastream_id)].value_count = response['properties']['valueCount']
-                    self.datastreams[str(datastream.datastream_id)].result_time = datetime.strptime(
+                if self.datastreams.get(str(datastream.id)):
+                    self.datastreams[str(datastream.id)].value_count = response['properties']['valueCount']
+                    self.datastreams[str(datastream.id)].result_time = datetime.strptime(
                         response['resultTime'].split('/')[1].replace('Z', '+0000'), '%Y-%m-%dT%H:%M:%S%z'
                     ) if response['resultTime'] else None
-                    self.datastreams[str(datastream.datastream_id)].phenomenon_time = datetime.strptime(
+                    self.datastreams[str(datastream.id)].phenomenon_time = datetime.strptime(
                         response['phenomenonTime'].split('/')[1].replace('Z', '+0000'), '%Y-%m-%dT%H:%M:%S%z'
                     ) if response['phenomenonTime'] else None
                 else:
-                    self.datastreams[str(datastream.datastream_id)] = HydroLoaderDatastream(
+                    self.datastreams[str(datastream.id)] = HydroLoaderDatastream(
                         id=response['@iot.id'],
                         value_count=response['properties']['valueCount'],
                         result_time=datetime.strptime(
                             response['resultTime'].split('/')[1].replace('Z', '+0000'), '%Y-%m-%dT%H:%M:%S%z'
                         ) if response['resultTime'] else None,
                         phenomenon_time=datetime.strptime(
                             response['phenomenonTime'].split('/')[1].replace('Z', '+0000'), '%Y-%m-%dT%H:%M:%S%z'
@@ -128,33 +128,33 @@
 
         if len(self.datastreams.keys()) == 0:
             self.get_datastreams()
 
         if not self.conf.file_access.path:
             return
 
+        message = None
+
         with open(self.conf.file_access.path) as data_file:
             data_reader = csv.reader(data_file, delimiter=self.conf.file_access.delimiter)
             file_parsing_error = False
             failed_datastreams = []
             for i, row in enumerate(data_reader):
                 try:
                     self.parse_data_file_row(i + 1, row)
                 except HeaderParsingError as e:
-                    logger.error(
-                        f'Failed to parse data file headers for "{self.conf.file_access.path}" ' +
+                    message = f'Failed to parse data file headers for "{self.conf.file_access.path}" ' + \
                         f'with error: {str(e)}'
-                    )
+                    logger.error(message)
                     file_parsing_error = True
                     break
                 except TimestampParsingError as e:
-                    logger.error(
-                        f'Failed to parse timestamp on row {i + 1} for "{self.conf.file_access.path}" ' +
+                    message = f'Failed to parse timestamp on row {i + 1} for "{self.conf.file_access.path}" ' + \
                         f'with error: {str(e)}'
-                    )
+                    logger.error(message)
                     file_parsing_error = True
                     break
                 if i > 0 and i % self.chunk_size == 0:
                     responses = self.post_observations(
                         skip_datastreams=failed_datastreams
                     )
                     failed_datastreams = self.handle_post_responses(
@@ -166,17 +166,21 @@
                     skip_datastreams=failed_datastreams
                 )
                 self.handle_post_responses(
                     responses=responses,
                     failed_datastreams=failed_datastreams
                 )
 
+        if not message and len(failed_datastreams) > 0:
+            message = 'One or more datastreams failed to sync with HydroServer.'
+
         return {
             'data_thru': getattr(self, 'file_result_timestamp', None),
-            'success': len(failed_datastreams) == 0 and file_parsing_error is False
+            'success': len(failed_datastreams) == 0 and file_parsing_error is False,
+            'message': message
         }
 
     @staticmethod
     def handle_post_responses(responses, failed_datastreams):
         """
         The handle_post_responses function takes a list of responses from SensorThings observations POST requests and
         a list of datastreams that have failed to post observations. It iterates through each response,
@@ -259,15 +263,15 @@
         return responses
 
     def parse_data_file_row(self, index, row):
         """
         The parse_data_file_row function is used to parse the data file row by row. The function takes in two
         arguments: index and row. The index argument is the current line number of the data file, and it's used to
         determine if we are at a header or not (if so, then we need to determine the column index for each named
-        column). The second argument is a list containing all of the values for each column on that particular line. If
+        column). The second argument is a list containing all the values for each column on that particular line. If
         this isn't a header, then we check if there are any observations with timestamps later than the latest
         timestamp for the associated datastream; if so, then add them into our observation_bodies to be posted.
 
         :param self: Refer to the object itself
         :param index: Keep track of the row number in the file
         :param row: Access the row of data in the csv file
         :return: A list of datetime and value pairs for each datastream
@@ -283,15 +287,15 @@
                     for datastream in self.conf.datastreams
                 }
                 self.timestamp_column_index = row.index(self.conf.file_timestamp.column) \
                     if isinstance(self.conf.file_timestamp.column, str) else self.conf.file_timestamp.column - 1
                 if max(self.datastream_column_indexes.values()) > len(row) or self.timestamp_column_index > len(row):
                     raise ValueError
             except ValueError as e:
-                raise HeaderParsingError from e
+                raise HeaderParsingError(str(e)) from e
 
         if index < self.conf.file_access.data_start_row:
             return
 
         try:
             if self.conf.file_timestamp.format == 'iso':
                 timestamp = isoparse(
@@ -299,38 +303,38 @@
                 )
             else:
                 timestamp = datetime.strptime(
                     row[self.timestamp_column_index],
                     self.conf.file_timestamp.format
                 )
         except ValueError as e:
-            raise TimestampParsingError from e
+            raise TimestampParsingError(str(e)) from e
 
         if timestamp.tzinfo is None:
             if not self.conf.file_timestamp.offset:
                 timestamp = timestamp.replace(
                     tzinfo=timezone.utc
                 )
 
         self.file_result_timestamp = timestamp
 
         for datastream in [
-            ds for ds in self.conf.datastreams if str(ds.datastream_id) in self.datastreams.keys()
+            ds for ds in self.conf.datastreams if str(ds.id) in self.datastreams.keys()
         ]:
-            ds_timestamp = self.datastreams[str(datastream.datastream_id)].result_time
+            ds_timestamp = self.datastreams[str(datastream.id)].result_time
 
-            if not self.datastreams[str(datastream.datastream_id)].file_row_start_index:
+            if not self.datastreams[str(datastream.id)].file_row_start_index:
                 if ds_timestamp is None or timestamp > ds_timestamp:
-                    self.datastreams[str(datastream.datastream_id)].file_row_start_index = index
+                    self.datastreams[str(datastream.id)].file_row_start_index = index
 
-            if self.datastreams[str(datastream.datastream_id)].file_row_start_index and \
-                    self.datastreams[str(datastream.datastream_id)].file_row_start_index <= index:
-                if str(datastream.datastream_id) not in self.observation_bodies.keys():
-                    self.observation_bodies[str(datastream.datastream_id)] = []
-
-                if not self.datastreams[str(datastream.datastream_id)].chunk_result_start_time:
-                    self.datastreams[str(datastream.datastream_id)].chunk_result_start_time = timestamp
-                self.datastreams[str(datastream.datastream_id)].chunk_result_end_time = timestamp
+            if self.datastreams[str(datastream.id)].file_row_start_index and \
+                    self.datastreams[str(datastream.id)].file_row_start_index <= index:
+                if str(datastream.id) not in self.observation_bodies.keys():
+                    self.observation_bodies[str(datastream.id)] = []
+
+                if not self.datastreams[str(datastream.id)].chunk_result_start_time:
+                    self.datastreams[str(datastream.id)].chunk_result_start_time = timestamp
+                self.datastreams[str(datastream.id)].chunk_result_end_time = timestamp
 
-                self.observation_bodies[str(datastream.datastream_id)].append([
+                self.observation_bodies[str(datastream.id)].append([
                     timestamp.strftime('%Y-%m-%dT%H:%M:%S%z'), row[self.datastream_column_indexes[datastream.column]]
                 ])
```

### Comparing `hydroloader-0.1.8/src/hydroloader/models.py` & `hydroloader-0.1.9/src/hydroloader/models.py`

 * *Files identical despite different names*

