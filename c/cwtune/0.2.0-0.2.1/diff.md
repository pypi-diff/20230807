# Comparing `tmp/cwtune-0.2.0.tar.gz` & `tmp/cwtune-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwtune-0.2.0.tar", last modified: Thu Aug  3 10:14:49 2023, max compression
+gzip compressed data, was "cwtune-0.2.1.tar", last modified: Mon Aug  7 16:05:26 2023, max compression
```

## Comparing `cwtune-0.2.0.tar` & `cwtune-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-03 10:14:49.644513 cwtune-0.2.0/
--rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.2.0/LICENSE
--rw-r--r--   0 arran      (501) staff       (20)     3206 2023-08-03 10:14:49.644723 cwtune-0.2.0/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)     2535 2023-08-03 09:01:39.000000 cwtune-0.2.0/README.md
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-03 10:14:49.629230 cwtune-0.2.0/cwtune/
--rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.2.0/cwtune/__init__.py
--rw-r--r--   0 arran      (501) staff       (20)     8949 2023-08-03 09:45:53.000000 cwtune-0.2.0/cwtune/analyze.py
--rw-r--r--   0 arran      (501) staff       (20)     4987 2023-08-03 09:46:34.000000 cwtune-0.2.0/cwtune/aws.py
--rw-r--r--   0 arran      (501) staff       (20)     2694 2023-08-02 14:44:19.000000 cwtune-0.2.0/cwtune/cli.py
--rw-r--r--   0 arran      (501) staff       (20)     5116 2023-08-02 13:44:14.000000 cwtune-0.2.0/cwtune/timeseries.py
--rw-r--r--   0 arran      (501) staff       (20)     2836 2023-08-01 12:29:11.000000 cwtune-0.2.0/cwtune/utils.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-03 10:14:49.643873 cwtune-0.2.0/cwtune.egg-info/
--rw-r--r--   0 arran      (501) staff       (20)     3206 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      349 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/SOURCES.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/dependency_links.txt
--rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/entry_points.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/not-zip-safe
--rw-r--r--   0 arran      (501) staff       (20)      109 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/requires.txt
--rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/top_level.txt
--rw-r--r--   0 arran      (501) staff       (20)      423 2023-08-03 10:14:49.646009 cwtune-0.2.0/setup.cfg
--rw-r--r--   0 arran      (501) staff       (20)     1336 2023-08-03 10:14:44.000000 cwtune-0.2.0/setup.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-07 16:05:26.056497 cwtune-0.2.1/
+-rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.2.1/LICENSE
+-rw-r--r--   0 arran      (501) staff       (20)     3206 2023-08-07 16:05:26.056788 cwtune-0.2.1/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)     2535 2023-08-03 09:01:39.000000 cwtune-0.2.1/README.md
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-07 16:05:25.739257 cwtune-0.2.1/cwtune/
+-rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.2.1/cwtune/__init__.py
+-rw-r--r--   0 arran      (501) staff       (20)     8813 2023-08-07 15:59:55.000000 cwtune-0.2.1/cwtune/analyze.py
+-rw-r--r--   0 arran      (501) staff       (20)     4987 2023-08-03 09:46:34.000000 cwtune-0.2.1/cwtune/aws.py
+-rw-r--r--   0 arran      (501) staff       (20)     2694 2023-08-02 14:44:19.000000 cwtune-0.2.1/cwtune/cli.py
+-rw-r--r--   0 arran      (501) staff       (20)     5501 2023-08-04 11:40:10.000000 cwtune-0.2.1/cwtune/timeseries.py
+-rw-r--r--   0 arran      (501) staff       (20)     2836 2023-08-01 12:29:11.000000 cwtune-0.2.1/cwtune/utils.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-07 16:05:25.855885 cwtune-0.2.1/cwtune.egg-info/
+-rw-r--r--   0 arran      (501) staff       (20)     3206 2023-08-07 16:05:23.000000 cwtune-0.2.1/cwtune.egg-info/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      349 2023-08-07 16:05:24.000000 cwtune-0.2.1/cwtune.egg-info/SOURCES.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-07 16:05:23.000000 cwtune-0.2.1/cwtune.egg-info/dependency_links.txt
+-rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-07 16:05:23.000000 cwtune-0.2.1/cwtune.egg-info/entry_points.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-07 16:05:23.000000 cwtune-0.2.1/cwtune.egg-info/not-zip-safe
+-rw-r--r--   0 arran      (501) staff       (20)      109 2023-08-07 16:05:23.000000 cwtune-0.2.1/cwtune.egg-info/requires.txt
+-rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-07 16:05:23.000000 cwtune-0.2.1/cwtune.egg-info/top_level.txt
+-rw-r--r--   0 arran      (501) staff       (20)      423 2023-08-07 16:05:26.208085 cwtune-0.2.1/setup.cfg
+-rw-r--r--   0 arran      (501) staff       (20)     1336 2023-08-07 16:04:41.000000 cwtune-0.2.1/setup.py
```

### Comparing `cwtune-0.2.0/LICENSE` & `cwtune-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cwtune-0.2.0/PKG-INFO` & `cwtune-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.2.0/README.md` & `cwtune-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cwtune-0.2.0/cwtune/analyze.py` & `cwtune-0.2.1/cwtune/analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,33 +61,32 @@
     click.echo(f"Padded data to {len(data)} data points.")
     return data, start, end
 
 
 def calculate_threshold_and_breaches(data, alarm_type, window_size, max_alerts):
     """Calculates threshold and breaches for the given data."""
     # Initial values
-    threshold = 1 if alarm_type.is_lt() else 0
-    breaches = get_breaches(data, threshold, alarm_type,
-                            window_size, math.ceil(window_size / 2))
-
     values = [value for timestamp, value in data]
     sum_values = sum(values)
     std_dev = sum([abs(value - sum_values / len(values))
-                  for value in values]) / len(values)
+            for value in values]) / len(values)
+
+    if alarm_type.is_gt():
+        threshold = math.ceil(sum_values / len(values) + 5 * std_dev)
+    elif alarm_type.is_lt():
+        threshold = max(math.ceil(sum_values / len(values) - 5 * std_dev), 1)
+
+    breaches = get_breaches(data, threshold, alarm_type,
+                            window_size, math.ceil(window_size / 2))
+
 
     # Threshold search when breaches are too many or too long
     if len(breaches) > max_alerts or longest_breach(breaches) > timedelta(days=2):
         click.echo('Starting binary search for threshold.')
 
-        # mean +/- 5 standard deviations depending on the alarm type
-        if alarm_type.is_gt():
-            threshold = math.ceil(sum_values / len(values) + 5 * std_dev)
-        elif alarm_type.is_lt():
-            threshold = max(math.ceil(sum_values / len(values) - 5 * std_dev), 1)
-
         min_threshold = min(values)
         max_threshold = max(values) * 2
 
         for i in range(MAX_ITERATIONS):
             click.echo(
                 f"Iteration {i + 1}. Evaluating threshold of {threshold}.")
             threshold = math.ceil((min_threshold + max_threshold) / 2)
@@ -180,15 +179,15 @@
     if click.confirm('Create/Update an alarm for this metric?', default=True):
         create_cloudwatch_alarm(
             metric['MetricName'], metric['Namespace'], metric['Dimensions'], threshold, alarm_type,
             client, statistic=statistic, period=period, window_size=window_size
         )
 
 
-def run(alarm_type, aws_profile=None, period=5, statistic='Sum', region='us-east-1', window_size=5, max_alerts=5, client=None):
+def run(alarm_type, aws_profile=None, period=5, statistic='Sum', region='us-east-1', window_size=5, max_alerts=11, client=None):
     """Select threshold for CloudWatch metrics."""
 
     if not client:
         client = cw_client(aws_profile, region)
 
     try:
         metrics = list_metrics(client)
```

### Comparing `cwtune-0.2.0/cwtune/aws.py` & `cwtune-0.2.1/cwtune/aws.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.2.0/cwtune/cli.py` & `cwtune-0.2.1/cwtune/cli.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.2.0/cwtune/timeseries.py` & `cwtune-0.2.1/cwtune/timeseries.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,50 +23,56 @@
 def eval(value, threshold, alarm_type):
     """Evaluate the value against the threshold."""
     if alarm_type.is_gt():
         return value > threshold
     elif alarm_type.is_lt():
         return value < threshold
 
+from collections import deque
+import logging
 
 def get_breaches(data, threshold, alarm_type, window_size, time_threshold):
     """Identify the start and end of each continuous breach of the threshold."""
-
     # iterate over the data using a sliding window
     breaches = []
-    window = []
+    window = deque()
 
     for timestamp, value in data:
         window.append((timestamp, value))
 
         # remove values that are outside of the window
-        while window and window[0][0] < timestamp - timedelta(minutes=window_size):
-            window.pop(0)
-
+        while window and window[0][0] < timestamp - timedelta(minutes=window_size - 1):
+            window.popleft()
         # check if the window contains more than time_threshold breaches
-        num_breaches = 0
-        for w in window:
-            if eval(w[1], threshold, alarm_type):
-                num_breaches += 1
+        num_breaches = sum(eval(w[1], threshold, alarm_type) for w in window)
 
         if num_breaches >= time_threshold:
+            logging.debug(f"num_breaches: {num_breaches}")
+            logging.debug(f"time_threshold: {time_threshold}")
+            logging.debug(f"window: {[w[1] for w in window]}")
             # check if we are already in a breach
             if breaches and breaches[-1]['status'] == 'open':
                 breaches[-1]['end'] = timestamp
                 breaches[-1]['values'].append(value)
             else:
                 breaches.append({'start': timestamp, 'end': timestamp, 'status': 'open', 'values': [value]})
         else:
             # check if we are already in a breach
             if breaches and breaches[-1]['status'] == 'open':
                 breaches[-1]['end'] = timestamp
                 breaches[-1]['status'] = 'closed'
 
+    # Ensure last breach is closed
+    if breaches and breaches[-1]['status'] == 'open':
+        breaches[-1]['end'] = data[-1][0]  # Last timestamp in data
+        breaches[-1]['status'] = 'closed'
+
     return breaches
 
+
 def longest_breach(breaches):
     """Return the length of the longest breach."""
     longest_breach = timedelta(seconds=0)
     for breach in breaches:
         if breach['end'] - breach['start'] > longest_breach:
             longest_breach = breach['end'] - breach['start']
     return longest_breach
```

### Comparing `cwtune-0.2.0/cwtune/utils.py` & `cwtune-0.2.1/cwtune/utils.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.2.0/cwtune.egg-info/PKG-INFO` & `cwtune-0.2.1/cwtune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.2.0/setup.py` & `cwtune-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords='cwtune',
     name='cwtune',
     packages=find_packages(include=['cwtune', 'cwtune.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/availabl-co/cwtune',
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```

