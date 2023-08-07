# Comparing `tmp/tictectoc-0.1.4-py3-none-any.whl.zip` & `tmp/tictectoc-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3170 bytes, number of entries: 7
--rw-r--r--  2.0 unx       41 b- defN 22-Jul-16 09:08 tictectoc/__init__.py
--rw-r--r--  2.0 unx     2474 b- defN 22-Jul-16 08:59 tictectoc/tictectoc.py
--rw-r--r--  2.0 unx     1066 b- defN 22-Jul-16 09:10 tictectoc-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1289 b- defN 22-Jul-16 09:10 tictectoc-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-16 09:10 tictectoc-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Jul-16 09:10 tictectoc-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      551 b- defN 22-Jul-16 09:10 tictectoc-0.1.4.dist-info/RECORD
-7 files, 5523 bytes uncompressed, 2192 bytes compressed:  60.3%
+Zip file size: 3728 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       41 b- defN 23-Aug-04 08:38 tictectoc/__init__.py
+-rw-rw-r--  2.0 unx     3509 b- defN 23-Aug-04 10:23 tictectoc/tictectoc.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Aug-07 01:03 tictectoc-0.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3420 b- defN 23-Aug-07 01:03 tictectoc-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-07 01:03 tictectoc-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Aug-07 01:03 tictectoc-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      551 b- defN 23-Aug-07 01:03 tictectoc-0.2.0.dist-info/RECORD
+7 files, 8689 bytes uncompressed, 2750 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: tictectoc/__init__.py
 Comment: 
 
 Filename: tictectoc/tictectoc.py
 Comment: 
 
-Filename: tictectoc-0.1.4.dist-info/LICENSE
+Filename: tictectoc-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: tictectoc-0.1.4.dist-info/METADATA
+Filename: tictectoc-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: tictectoc-0.1.4.dist-info/WHEEL
+Filename: tictectoc-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: tictectoc-0.1.4.dist-info/top_level.txt
+Filename: tictectoc-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tictectoc-0.1.4.dist-info/RECORD
+Filename: tictectoc-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tictectoc/tictectoc.py

```diff
@@ -1,30 +1,42 @@
 from timeit import default_timer
 from datetime import timedelta
+from typing import Union, Optional
+
 
 class TicTecToc:
     MSG = '[TTT:{}] Elapsed time is'
     Temp_MSG = '[TTT:{}] Temp Elapsed time is'
     _timestamps: dict = None
 
-    def __init__(self):
+    def __init__(self, name: Union[str, int] = 'default'):
         self._timestamps = dict()
+        self._name = name
 
-    def tic(self, name: str = 'default'):
+    def tic(self, name: Optional[Union[str, int]] = None):
         '''Start.'''
+        if name is None:
+            name = self._name
+        name = str(name)
         if name not in self._timestamps:
             self._timestamps[name] = {
                 'start': default_timer(),
                 'elapsed': 0.
             }
         else: 
             self._timestamps[name]['start'] = default_timer()
 
-    def tec(self, name: str = 'default', msg: str = None, tmp_msg: str = None, verbose: int = 0):
+    def i(self,*args, **kwargs):
+        self.tic(*args, **kwargs)
+
+    def tec(self, name: Optional[Union[str, int]] = None, msg: str = None, tmp_msg: str = None, verbose: int = 0):
         '''End temp.'''
+        if name is None:
+            name = self._name
+        name = str(name)
         if name not in self._timestamps:
             return None
         if self._timestamps[name] is None:
             return None
         if self._timestamps[name]['start'] is None:
             return None
         if msg is None:
@@ -46,17 +58,23 @@
         if verbose == 2: 
             print(msg.format+ timedelta(seconds=elapsed))
 
         if verbose == 3: 
             print(tmp_msg.format(name), timedelta(seconds=temp_elapsed))
 
         return temp_elapsed, elapsed
+    
+    def e(self,*args, **kwargs):
+        return self.tec(*args, **kwargs)
 
-    def toc(self, name: str = "default", msg: str = None, verbose: int = 1):
+    def toc(self, name: Optional[Union[str, int]] = None, msg: str = None, verbose: int = 1):
         '''End.'''
+        if name is None:
+            name = self._name
+        name = str(name)
         if name not in self._timestamps:
             return None
         if self._timestamps[name]['start'] is not None:
             self.tec(name)
         if msg is None:
             msg = TicTecToc.MSG
 
@@ -64,15 +82,43 @@
         if verbose == 1:
             print(msg.format(name), timedelta(seconds=elapsed))
 
         del self._timestamps[name]
 
         return elapsed
 
+    def o(self,*args, **kwargs):
+        return self.toc(*args, **kwargs)
+
     def __enter__(self):
-        self.start = default_timer()
+        """Start the timer when using TicToc in a context manager."""
+        self.tic()
     
     def __exit__(self, *args):
-        msg = TicTecToc.MSG.replace(':{}','')
-        self.end = default_timer()
-        self.elapsed = self.end - self.start
-        print(msg, timedelta(seconds=self.elapsed))
+        """On exit, pring time elapsed since entering context manager."""
+        self.toc()
+
+    
+    # decorator
+    def dec(self, argument):
+        def decorator(func):
+            def wrapper(*args, **kwargs):
+                self.tic(argument)
+                result = func(*args, **kwargs)
+                self.toc(argument)
+                return result
+            return wrapper
+        return decorator
+    
+
+# init
+ttt = TicTecToc()
+
+
+# global func with abbreviation
+tic = i = ttt.tic
+tec = e = ttt.tec
+toc = o = ttt.toc
+
+dec = ttt.dec
+
+
```

## Comparing `tictectoc-0.1.4.dist-info/LICENSE` & `tictectoc-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

