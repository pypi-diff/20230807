# Comparing `tmp/aggregationslib-0.0.251.tar.gz` & `tmp/aggregationslib-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggregationslib-0.0.251.tar", last modified: Sun Aug 28 10:53:44 2022, max compression
+gzip compressed data, was "aggregationslib-0.0.26.tar", last modified: Mon Aug  7 10:11:18 2023, max compression
```

## Comparing `aggregationslib-0.0.251.tar` & `aggregationslib-0.0.26.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-08-28 10:53:44.449134 aggregationslib-0.0.251/
--rw-rw-rw-   0        0        0     1659 2022-08-28 10:53:44.446135 aggregationslib-0.0.251/PKG-INFO
--rw-rw-rw-   0        0        0     1275 2022-08-27 15:50:41.000000 aggregationslib-0.0.251/README.md
-drwxrwxrwx   0        0        0        0 2022-08-28 10:53:44.413183 aggregationslib-0.0.251/aggregationslib/
--rw-rw-rw-   0        0        0        0 2022-03-14 21:57:13.000000 aggregationslib-0.0.251/aggregationslib/__init__.py
--rw-rw-rw-   0        0        0     4645 2022-07-27 14:50:00.000000 aggregationslib-0.0.251/aggregationslib/aggregation.py
--rw-rw-rw-   0        0        0     5607 2022-08-28 10:09:52.000000 aggregationslib-0.0.251/aggregationslib/decimalaggregations.py
--rw-rw-rw-   0        0        0      157 2022-03-14 21:39:01.000000 aggregationslib-0.0.251/aggregationslib/example.py
--rw-rw-rw-   0        0        0      582 2022-08-27 15:02:34.000000 aggregationslib-0.0.251/aggregationslib/purepython.py
-drwxrwxrwx   0        0        0        0 2022-08-28 10:53:44.443095 aggregationslib-0.0.251/aggregationslib.egg-info/
--rw-rw-rw-   0        0        0     1659 2022-08-28 10:53:43.000000 aggregationslib-0.0.251/aggregationslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2022-08-28 10:53:43.000000 aggregationslib-0.0.251/aggregationslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-28 10:53:43.000000 aggregationslib-0.0.251/aggregationslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-08-28 10:53:43.000000 aggregationslib-0.0.251/aggregationslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-08-28 10:53:43.000000 aggregationslib-0.0.251/aggregationslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-28 10:53:44.450131 aggregationslib-0.0.251/setup.cfg
--rw-rw-rw-   0        0        0      920 2022-08-28 10:53:17.000000 aggregationslib-0.0.251/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:11:18.757120 aggregationslib-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-07 10:11:18.757120 aggregationslib-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:11:18.753120 aggregationslib-0.0.26/aggregationslib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/aggregationslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/aggregationslib/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/aggregationslib/decimalaggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/aggregationslib/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/aggregationslib/purepython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:11:18.757120 aggregationslib-0.0.26/aggregationslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-07 10:11:18.000000 aggregationslib-0.0.26/aggregationslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-07 10:11:18.000000 aggregationslib-0.0.26/aggregationslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:11:18.000000 aggregationslib-0.0.26/aggregationslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 10:11:18.000000 aggregationslib-0.0.26/aggregationslib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:11:18.757120 aggregationslib-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:11:18.757120 aggregationslib-0.0.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/tests/test_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-07 10:11:05.000000 aggregationslib-0.0.26/tests/test_decimal_exponential_mean.py
```

### Comparing `aggregationslib-0.0.251/PKG-INFO` & `aggregationslib-0.0.26/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,87 @@
-Metadata-Version: 2.1
-Name: aggregationslib
-Version: 0.0.251
-Summary: Python implementation of Arithmetic, quasi arithmetic and other aggregating functions
-Home-page: https://github.com/wgalka/Means
-Author: wgalka
-License: TO DOO
-Download-URL: https://github.com/wgalka/Means/archive/refs/tags/v0.0.251.tar.gz
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# Means
-Means, Aggregation functions...
-
-
-
-#### Example 1:
-Mix numpy and pure python example:
-```python
-import numpy as np
-t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
-t2 = [1 - x for x in t1]
-mean1 = np.mean(t1)
-mean2 = np.mean(t2)
-print(t1, mean1)
-print(t2, mean2)
-```
-In output we can see that returned value does not sum to 1. It have impact on comparasion
-```pycon
->>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
->>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.9800000000000001
-```
-
-
-#### Using 1:
-```python
-from aggregationslib.aggregation import arithmetic
-
-t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
-t2 = [1 - x for x in t1]
-mean1 = arithmetic_(t1)
-mean2 = arithmetic_(t2)
-print(t1, mean1)
-print(t2, mean2)
-```
-In implementation we obtain exact number:
-```pycon
->>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
->>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.98
-```
-
-`exponential(y, r=1)` is given by equation $A_6^{(r)}(x_1,...,x_n)= \frac{1}{r}\ln
-    \Big(\frac{1}{n} \sum \limits_{k=1}^{n} e^{rx_k}\Big)$, where
-    $r \in \mathbb{R}$, $r \neq 0$
-
-
-# 1
-arithmetic(y)
-
-# 2
-quadratic(y)
-
-# 3
-geometric(y)
-
-# 4
-harmonic(y)
-
-# 5
-power(y, r=1)
-
-# 6
-exponential(y, r=1)
-
-# 7
-lehmer(y, r=0)
-
-# 8
-arithmetic_min(y, p=0)
-
-# 9
-arithmetic_max(y, p=0)
-
-# 10
-median(y)
-
-# 11
-olimpic(y)
-
+Metadata-Version: 2.1
+Name: aggregationslib
+Version: 0.0.26
+Summary: Python implementation of Arithmetic, quasi arithmetic and other aggregating functions
+Home-page: https://github.com/wgalka/Means
+Download-URL: https://github.com/wgalka/Means/archive/refs/tags/v0.0.26.tar.gz
+Author: wgalka
+License: TO DOO
+Description-Content-Type: text/markdown
+
+# Means
+Means, Aggregation functions...
+
+
+
+#### Example 1:
+Mix numpy and pure python example:
+```python
+import numpy as np
+t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
+t2 = [1 - x for x in t1]
+mean1 = np.mean(t1)
+mean2 = np.mean(t2)
+print(t1, mean1)
+print(t2, mean2)
+```
+In output we can see that returned value does not sum to 1. It have impact on comparasion
+```pycon
+>>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
+>>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.9800000000000001
+```
+
+
+#### Using 1:
+```python
+from aggregationslib.aggregation import arithmetic
+
+t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
+t2 = [1 - x for x in t1]
+mean1 = arithmetic_(t1)
+mean2 = arithmetic_(t2)
+print(t1, mean1)
+print(t2, mean2)
+```
+In implementation we obtain exact number:
+```pycon
+>>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
+>>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.98
+```
+
+`exponential(y, r=1)` is given by equation $A_6^{(r)}(x_1,...,x_n)= \frac{1}{r}\ln
+    \Big(\frac{1}{n} \sum \limits_{k=1}^{n} e^{rx_k}\Big)$, where
+    $r \in \mathbb{R}$, $r \neq 0$
+
+
+# 1
+arithmetic(y)
+
+# 2
+quadratic(y)
+
+# 3
+geometric(y)
+
+# 4
+harmonic(y)
+
+# 5
+power(y, r=1)
+
+# 6
+exponential(y, r=1)
+
+# 7
+lehmer(y, r=0)
+
+# 8
+arithmetic_min(y, p=0)
+
+# 9
+arithmetic_max(y, p=0)
+
+# 10
+median(y)
+
+# 11
+olimpic(y)
```

### Comparing `aggregationslib-0.0.251/aggregationslib/purepython.py` & `aggregationslib-0.0.26/aggregationslib/purepython.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import math
-
-import numpy as np
-
-
-def exponential(y, r=1):
-    """
-    Mean is given by equation:
-    $A_6^{(r)}(x_1,...,x_n)= \frac{1}{r}\ln
-    \Big(\frac{1}{n} \sum \limits_{k=1}^{n} e^{rx_k}\Big)$, where
-    $r \in \mathbb{R}$, $r \neq 0$
-
-    :param y: array of values
-    :param r: r != 0
-    :return: value of exponential mean
-    """
-    size = len(y)
-    if r == 0:
-        raise ValueError("parameter r should be != 0 ")
-
-    _sum = 0
-    for idx, num in enumerate(y):
-        _sum += math.exp(num * r)
-
-    return (1 / r) * math.log(_sum / size)
+import math
+
+import numpy as np
+
+
+def exponential(y, r=1):
+    """
+    Mean is given by equation:
+    $A_6^{(r)}(x_1,...,x_n)= \frac{1}{r}\ln
+    \Big(\frac{1}{n} \sum \limits_{k=1}^{n} e^{rx_k}\Big)$, where
+    $r \in \mathbb{R}$, $r \neq 0$
+
+    :param y: array of values
+    :param r: r != 0
+    :return: value of exponential mean
+    """
+    size = len(y)
+    if r == 0:
+        raise ValueError("parameter r should be != 0 ")
+
+    _sum = 0
+    for idx, num in enumerate(y):
+        _sum += math.exp(num * r)
+
+    return (1 / r) * math.log(_sum / size)
```

### Comparing `aggregationslib-0.0.251/aggregationslib.egg-info/PKG-INFO` & `aggregationslib-0.0.26/aggregationslib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,87 @@
-Metadata-Version: 2.1
-Name: aggregationslib
-Version: 0.0.251
-Summary: Python implementation of Arithmetic, quasi arithmetic and other aggregating functions
-Home-page: https://github.com/wgalka/Means
-Author: wgalka
-License: TO DOO
-Download-URL: https://github.com/wgalka/Means/archive/refs/tags/v0.0.251.tar.gz
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# Means
-Means, Aggregation functions...
-
-
-
-#### Example 1:
-Mix numpy and pure python example:
-```python
-import numpy as np
-t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
-t2 = [1 - x for x in t1]
-mean1 = np.mean(t1)
-mean2 = np.mean(t2)
-print(t1, mean1)
-print(t2, mean2)
-```
-In output we can see that returned value does not sum to 1. It have impact on comparasion
-```pycon
->>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
->>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.9800000000000001
-```
-
-
-#### Using 1:
-```python
-from aggregationslib.aggregation import arithmetic
-
-t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
-t2 = [1 - x for x in t1]
-mean1 = arithmetic_(t1)
-mean2 = arithmetic_(t2)
-print(t1, mean1)
-print(t2, mean2)
-```
-In implementation we obtain exact number:
-```pycon
->>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
->>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.98
-```
-
-`exponential(y, r=1)` is given by equation $A_6^{(r)}(x_1,...,x_n)= \frac{1}{r}\ln
-    \Big(\frac{1}{n} \sum \limits_{k=1}^{n} e^{rx_k}\Big)$, where
-    $r \in \mathbb{R}$, $r \neq 0$
-
-
-# 1
-arithmetic(y)
-
-# 2
-quadratic(y)
-
-# 3
-geometric(y)
-
-# 4
-harmonic(y)
-
-# 5
-power(y, r=1)
-
-# 6
-exponential(y, r=1)
-
-# 7
-lehmer(y, r=0)
-
-# 8
-arithmetic_min(y, p=0)
-
-# 9
-arithmetic_max(y, p=0)
-
-# 10
-median(y)
-
-# 11
-olimpic(y)
-
+Metadata-Version: 2.1
+Name: aggregationslib
+Version: 0.0.26
+Summary: Python implementation of Arithmetic, quasi arithmetic and other aggregating functions
+Home-page: https://github.com/wgalka/Means
+Download-URL: https://github.com/wgalka/Means/archive/refs/tags/v0.0.26.tar.gz
+Author: wgalka
+License: TO DOO
+Description-Content-Type: text/markdown
+
+# Means
+Means, Aggregation functions...
+
+
+
+#### Example 1:
+Mix numpy and pure python example:
+```python
+import numpy as np
+t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
+t2 = [1 - x for x in t1]
+mean1 = np.mean(t1)
+mean2 = np.mean(t2)
+print(t1, mean1)
+print(t2, mean2)
+```
+In output we can see that returned value does not sum to 1. It have impact on comparasion
+```pycon
+>>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
+>>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.9800000000000001
+```
+
+
+#### Using 1:
+```python
+from aggregationslib.aggregation import arithmetic
+
+t1 = [0.0, 0.0, 0.0, 0.0, 0.1]
+t2 = [1 - x for x in t1]
+mean1 = arithmetic_(t1)
+mean2 = arithmetic_(t2)
+print(t1, mean1)
+print(t2, mean2)
+```
+In implementation we obtain exact number:
+```pycon
+>>> [0.0, 0.0, 0.0, 0.0, 0.1] 0.02
+>>> [1.0, 1.0, 1.0, 1.0, 0.9] 0.98
+```
+
+`exponential(y, r=1)` is given by equation $A_6^{(r)}(x_1,...,x_n)= \frac{1}{r}\ln
+    \Big(\frac{1}{n} \sum \limits_{k=1}^{n} e^{rx_k}\Big)$, where
+    $r \in \mathbb{R}$, $r \neq 0$
+
+
+# 1
+arithmetic(y)
+
+# 2
+quadratic(y)
+
+# 3
+geometric(y)
+
+# 4
+harmonic(y)
+
+# 5
+power(y, r=1)
+
+# 6
+exponential(y, r=1)
+
+# 7
+lehmer(y, r=0)
+
+# 8
+arithmetic_min(y, p=0)
+
+# 9
+arithmetic_max(y, p=0)
+
+# 10
+median(y)
+
+# 11
+olimpic(y)
```

