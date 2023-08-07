# Comparing `tmp/kctools-0.2.3.tar.gz` & `tmp/kctools-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kctools-0.2.3.tar", last modified: Sat Dec 17 18:28:35 2022, max compression
+gzip compressed data, was "kctools-0.23.8.tar", last modified: Mon Aug  7 20:13:14 2023, max compression
```

## Comparing `kctools-0.2.3.tar` & `kctools-0.23.8.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2022-12-17 18:28:35.594830 kctools-0.2.3/
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1061 2022-01-22 01:49:58.000000 kctools-0.2.3/LICENSE
--rw-rw-r--   0 kcs       (1000) kcs       (1000)      513 2022-12-17 18:28:35.594830 kctools-0.2.3/PKG-INFO
--rw-r--r--   0 kcs       (1000) kcs       (1000)       63 2022-01-22 01:52:01.000000 kctools-0.2.3/README.md
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2022-12-17 18:28:35.582828 kctools-0.2.3/kctools/
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1389 2022-06-20 16:46:36.000000 kctools-0.2.3/kctools/__init__.py
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2022-12-17 18:28:35.590829 kctools-0.2.3/kctools/classes/
--rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-0.2.3/kctools/classes/__init__.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1027 2022-12-17 18:05:40.000000 kctools-0.2.3/kctools/classes/cuke.py
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2022-12-17 18:28:35.594830 kctools-0.2.3/kctools/classes/data/
--rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-0.2.3/kctools/classes/data/__init__.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     3024 2022-09-09 16:54:23.000000 kctools-0.2.3/kctools/classes/data/config.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1537 2022-12-17 18:07:26.000000 kctools-0.2.3/kctools/classes/dicts.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1334 2022-09-30 00:15:37.000000 kctools-0.2.3/kctools/classes/lock.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     3936 2022-01-29 17:28:35.000000 kctools-0.2.3/kctools/classes/map.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     2419 2022-09-20 10:42:16.000000 kctools-0.2.3/kctools/classes/reg.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)    14889 2022-12-17 18:12:07.000000 kctools-0.2.3/kctools/classes/sub.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     3648 2022-09-30 00:11:29.000000 kctools-0.2.3/kctools/classes/vec.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)    10078 2022-11-29 00:54:25.000000 kctools-0.2.3/kctools/kctools.py
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2022-12-17 18:28:35.586829 kctools-0.2.3/kctools.egg-info/
--rw-r--r--   0 kcs       (1000) kcs       (1000)      513 2022-12-17 18:28:35.000000 kctools-0.2.3/kctools.egg-info/PKG-INFO
--rw-r--r--   0 kcs       (1000) kcs       (1000)      476 2022-12-17 18:28:35.000000 kctools-0.2.3/kctools.egg-info/SOURCES.txt
--rw-r--r--   0 kcs       (1000) kcs       (1000)        1 2022-12-17 18:28:35.000000 kctools-0.2.3/kctools.egg-info/dependency_links.txt
--rw-r--r--   0 kcs       (1000) kcs       (1000)       30 2022-12-17 18:28:35.000000 kctools-0.2.3/kctools.egg-info/requires.txt
--rw-r--r--   0 kcs       (1000) kcs       (1000)        8 2022-12-17 18:28:35.000000 kctools-0.2.3/kctools.egg-info/top_level.txt
--rw-rw-r--   0 kcs       (1000) kcs       (1000)       38 2022-12-17 18:28:35.594830 kctools-0.2.3/setup.cfg
--rw-r--r--   0 kcs       (1000) kcs       (1000)      892 2022-11-29 00:52:50.000000 kctools-0.2.3/setup.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1061 2022-01-22 01:49:58.000000 kctools-0.23.8/LICENSE
+-rw-rw-r--   0 kcs       (1000) kcs       (1000)      514 2023-08-07 20:13:14.312344 kctools-0.23.8/PKG-INFO
+-rw-r--r--   0 kcs       (1000) kcs       (1000)       63 2022-01-22 01:52:01.000000 kctools-0.23.8/README.md
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1416 2023-08-04 18:10:16.000000 kctools-0.23.8/kctools/__init__.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools/classes/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-0.23.8/kctools/classes/__init__.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1027 2022-12-17 18:05:40.000000 kctools-0.23.8/kctools/classes/cuke.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools/classes/data/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-0.23.8/kctools/classes/data/__init__.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     3033 2023-03-04 23:53:30.000000 kctools-0.23.8/kctools/classes/data/config.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1537 2022-12-17 18:07:26.000000 kctools-0.23.8/kctools/classes/dicts.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1334 2022-09-30 00:15:37.000000 kctools-0.23.8/kctools/classes/lock.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     3936 2022-01-29 17:28:35.000000 kctools-0.23.8/kctools/classes/map.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     2897 2023-08-04 21:28:02.000000 kctools-0.23.8/kctools/classes/reg.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)    15102 2023-08-04 18:45:06.000000 kctools-0.23.8/kctools/classes/sub.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     3992 2023-08-05 19:32:57.000000 kctools-0.23.8/kctools/classes/vec.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)    12361 2023-08-06 14:56:18.000000 kctools-0.23.8/kctools/kctools.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools.egg-info/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)      514 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/PKG-INFO
+-rw-r--r--   0 kcs       (1000) kcs       (1000)      446 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/SOURCES.txt
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        1 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/dependency_links.txt
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        8 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/top_level.txt
+-rw-rw-r--   0 kcs       (1000) kcs       (1000)       38 2023-08-07 20:13:14.312344 kctools-0.23.8/setup.cfg
+-rw-r--r--   0 kcs       (1000) kcs       (1000)      797 2023-08-04 19:12:30.000000 kctools-0.23.8/setup.py
```

### Comparing `kctools-0.2.3/LICENSE` & `kctools-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kctools-0.2.3/PKG-INFO` & `kctools-0.23.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kctools
-Version: 0.2.3
+Version: 0.23.8
 Summary: miscellaneous elves
 Home-page: https://github.com/kcstokely/kctools
 Author: kevin c. stokely
 Author-email: kcstokely@gmail.com
 License: MIT
 Description: # kctools
```

### Comparing `kctools-0.2.3/kctools/__init__.py` & `kctools-0.23.8/kctools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 from .kctools import only_one
 from .kctools import split_into_rows
 from .kctools import split_into_chunks
 from .kctools import flatten
 from .kctools import gram_getter
 from .kctools import where_in_thing
 from .kctools import autovivify
+from .kctools import vivify
 from .kctools import mortify
 from .kctools import dict_update
 from .kctools import setup_logger
-from .kctools import coalesce
 from .kctools import mround
-
+from .kctools import coalesce
 from .kctools import normalize
 from .kctools import is_diagonal
 from .kctools import kpow
 from .kctools import kcos
 from .kctools import bin_entropy
 from .kctools import mod_entropy
 from .kctools import lower_conf_bound
```

### Comparing `kctools-0.2.3/kctools/classes/cuke.py` & `kctools-0.23.8/kctools/classes/cuke.py`

 * *Files identical despite different names*

### Comparing `kctools-0.2.3/kctools/classes/data/config.py` & `kctools-0.23.8/kctools/classes/data/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'maj7 b5':       (0, 4, 6, 11),
     'dom7 #5':       (0, 4, 8, 10),
     'dom7 b5':       (0, 4, 6, 10),
     'mma7 #5':       (0, 3, 8, 11),
     'mma7 b5':       (0, 3, 6, 11),
     'min7 #5':       (0, 3, 8, 10),
     'min7 b5':       (0, 3, 6, 10),
-    'dim7':          (0, 3, 6, 9),
+    'dim7':          (0, 3, 6,  9),
     'maj7 sus4':     (0, 5, 7, 11),
     'maj7 #5 sus4':  (0, 5, 8, 11),
     'maj7 b5 sus4':  (0, 5, 6, 11),
     'min7 sus4':     (0, 5, 7, 10),
     'min7 #5 sus4':  (0, 5, 8, 10),
     'min7 b5 sus4':  (0, 5, 6, 10),
     'maj7 sus2':     (0, 2, 7, 11),
@@ -46,15 +46,15 @@
     'min7 sus2':     (0, 2, 7, 10),
     'min7 #5 sus2':  (0, 2, 8, 10),
     'min7 b5 sus2':  (0, 2, 6, 10),
     'maj7 ##5':      (0, 4, 9, 11),
     'maj7 ##5 sus4': (0, 5, 9, 11),
 
     # PENTADS
-    'major pentatonic':      (0, 2, 4, 7, 9),
+    'major pentatonic':      (0, 2, 4, 7,  9),
     'fucked-up pentatonic':  (0, 3, 6, 8, 10),
     
     # HEXADS
     'whole tone':            (0, 2, 4, 6, 8, 10),
     'augmented':             (0, 3, 4, 7, 8, 11),
     
     # SEPTADS
@@ -68,21 +68,21 @@
     'dim7 / dim (R)':        (0, 2, 3, 5, 6, 9, 11),
     'dom7 #5 / aug (L)':     (0, 3, 4, 5, 7, 8, 11),
     'dom7 #5 / aug (R)':     (0, 3, 4, 6, 7, 8, 11),
     'neapolitan minor (R)':  (0, 1, 3, 5, 7, 8, 11),
     'neapolitan minor (L)':  (0, 2, 4, 6, 7, 8, 11),
 
     # OCTADS
-    'dim7 / dim7':           (0, 2, 3, 5, 6, 8, 9, 11),
-    'min6 / dim7':           (0, 2, 3, 5, 7, 8, 9, 11),
-    'maj6 / dim7':           (0, 2, 4, 5, 7, 8, 9, 11),
+    'dim7 / dim7':           (0, 2, 3, 5, 6, 8,  9, 11),
+    'min6 / dim7':           (0, 2, 3, 5, 7, 8,  9, 11),
+    'maj6 / dim7':           (0, 2, 4, 5, 7, 8,  9, 11),
     'dom7 / dim7':           (0, 2, 4, 5, 7, 8, 10, 11),
     'dom7 b5 / dim7':        (0, 2, 4, 5, 6, 8, 10, 11),
-    'whole tone / maj':      (0, 1, 3, 4, 5, 7, 9, 11),
-    'augmented / P4':        (0, 1, 3, 4, 6, 7, 8, 11),
-    'augmented / maj (L)':   (0, 1, 3, 4, 5, 7, 8, 11),
-    'augmented / maj (R)':   (0, 1, 3, 4, 5, 8, 9, 11)
+    'whole tone / maj':      (0, 1, 3, 4, 5, 7,  9, 11),
+    'augmented / P4':        (0, 1, 3, 4, 6, 7,  8, 11),
+    'augmented / maj (L)':   (0, 1, 3, 4, 5, 7,  8, 11),
+    'augmented / maj (R)':   (0, 1, 3, 4, 5, 8,  9, 11)
     
 }
```

### Comparing `kctools-0.2.3/kctools/classes/dicts.py` & `kctools-0.23.8/kctools/classes/dicts.py`

 * *Files identical despite different names*

### Comparing `kctools-0.2.3/kctools/classes/lock.py` & `kctools-0.23.8/kctools/classes/lock.py`

 * *Files identical despite different names*

### Comparing `kctools-0.2.3/kctools/classes/map.py` & `kctools-0.23.8/kctools/classes/map.py`

 * *Files identical despite different names*

### Comparing `kctools-0.2.3/kctools/classes/sub.py` & `kctools-0.23.8/kctools/classes/sub.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 ################################################
 
 from collections import Counter
 
-import numpy as np
-import pandas as pd
-
 from ..kctools import endify as _e
+from ..kctools import is_np, is_pd
+from ..kctools import np_check, pd_check
+
+if is_np:
+    import numpy as np
+    
+if is_np and is_pd:
+    import pandas as pd
+
 from .data.config import conf as cf
 
 ################################################
 
+@np_check
 class N():
     
     '''
         This class represents one or more
           objects in the power-set 2**L.
 
         It has methods that are useful
           for exploring the properties
           of collections of notes from 
           an L-tone musical scale.
           
         So generally, L will be twelve.
 
-        All data is stored in self._hot:
+        All data:
+          - kept in self._hot
           - it is an np.ndarray
           - it will either be 1-D or 2-D
           - if 1-D it is a 1-hot vector
           - if 2-D it is N 1-hot vectors,
           -   unique and sorted.
 
-        All methods rely only on self._hot:
+        All methods:
+          - rely only on self._hot
           - written to act on 1-D array
           - wrappers extend to act on 2-D
-
-        Most methods mutate self:
-          - use .copy() to protect self
     '''
 
+    ############ CONFIG   
+    
     _L = 12 # overwrite to warp spacetime
     _conf = cf # overwrite to name things
     _cmap = {v: k for k, v in cf.items()}
     
     ############ BIRTH
     
     def __init__(self, inp = []):
 
-        if isinstance(inp, str):
-            ndxs = N._conf[inp]
-        elif isinstance(inp, int):
-            ndxs = np.where([ int(x) for x in list(f'{int(bin(inp)[2:]):0{N._L}d}') ])[0]
-        elif len(inp) == N._L:
-            ndxs = np.where(inp)[0]
+        if isinstance(inp, N):
+            self._hot = N._hot
         else:
-            ndxs = inp
+            
+            if isinstance(inp, str):
+                ndxs = N._conf[inp]
+            elif isinstance(inp, int):
+                ndxs = np.where([ int(x) for x in list(f'{int(bin(inp)[2:]):0{N._L}d}') ])[0]
+            elif len(inp) == N._L:
+                ndxs = np.where(inp)[0]
+            else:
+                ndxs = inp
 
-        self._hot = np.zeros(N._L, dtype=bool)
-        self._hot[[ ndx%N._L for ndx in ndxs ]] = 1
+            self._hot = np.zeros(N._L, dtype=bool)
+            self._hot[[ ndx%N._L for ndx in ndxs ]] = 1
     
-    ###
+    ############ WHAT
     
     def __len__(self):
         return self._hot.shape[0] if self._hot.ndim > 1 else 1
 
     def __iter__(self):
         return (x for x in self._hot) if self._hot.ndim > 1 else self._hot
     
     def __repr__(self):
-        return str(self.copy()._hot.astype(int))
-
-    ############ EXTEND
+        return str(N(self)._hot.astype(int))
 
-    def copy(self):
-        return N(self._hot)
+    ############ ORGANIZE
     
     def crush(self):
         # keeps 2-D arrays unique and sorted
         if self._hot.ndim > 1:
             assert self._hot.ndim == 2
             self._hot = np.unique(self._hot, axis=0)
             if self._hot.shape[0] == 1:
@@ -102,16 +111,172 @@
         # extends bool/int/tuple methods to act on 2-D arrays
         def wrapped(self, *args, **kwargs):
             if self._hot.ndim == 1:
                 return method(self, *args, **kwargs)
             else:
                 return [ method(N(x), *args, **kwargs) for x in self._hot ]
         return wrapped
-        
-    ############ MUTATE (alter)
+
+    ############ REVEAL (UNIQUE IDENTIFIERS)
+
+    @tuple_mapper
+    def hot(self):
+        return tuple(int(x) for x in self._hot)
+
+    @tuple_mapper
+    def index(self):
+        return int(''.join(map(str, N(self).compose().hot())), 2)
+    
+    @tuple_mapper
+    def notes(self):
+        return tuple(np.where(self._hot)[0])
+
+    @tuple_mapper
+    def string(self):
+        return ''.join([ 'x' if x else '_' for x in self.hot() ])
+    
+    @tuple_mapper
+    def forte(self):
+        x = self.num()
+        y = 1 + N(self).modes()._hot.tolist().index(N(self).canonical())
+        return (x, y)
+    
+    @tuple_mapper
+    def forte_string(self):
+        x = self.num()
+        y = 1 + N(self).modes()._hot.tolist().index(N(self).canonical())
+        return '-'.join(self.forte())
+    
+    @tuple_mapper
+    def diff(self):
+        return tuple(np.diff(list(self.notes())+[N._L+self.notes()[0]])) if self.notes() else ()
+    
+    @tuple_mapper
+    def lookup(self):
+        name = N._cmap.get(self.notes(), '')
+        if not name:
+            modes = N(self).modes()
+            for mode in modes._hot:
+                mode = N(mode)
+                name = N._cmap.get(mode.notes())
+                if name:
+                    if not self._hot[0]:
+                        name = f'disp. mode of {name}'
+                    else:
+                        for mdx in range(self.num()):
+                            if (self._hot == N(mode).roll(mdx)._hot).all():
+                                name = f'{_e(mdx+1)} mode of {name}'
+                                break
+                    break
+        return name
+    
+    @tuple_mapper
+    def harmonize(self, n_max = 4):
+        chords = ( N(self).roll(mdx).chord(n_max).hot() for mdx in range(self.num()) )
+        return tuple(zip(self.notes(), chords))
+    
+    ############ CALCULATE (NON-UNIQUE VALUES)
+    
+    @tuple_mapper
+    def num(self):
+        return self._hot.sum()
+    
+    @tuple_mapper
+    def spin(self):
+        return self.handedness() * self.symmetry()
+
+    @tuple_mapper
+    def symmetry(self):
+        for m in range(1, 1 + N._L):
+            if not N._L % m:
+                l = N._L // m
+                tiled = np.reshape(self._hot, (m, l))
+                if (tiled == tiled[0]).all():
+                    sym = m
+        return sym
+
+    @tuple_mapper
+    def handedness(self):
+        if (N(self).canonical()._hot == N(self).rev().canonical()._hot).all():
+            h = 0
+        elif (N(self).canonical()._hot == N(self).ext_canonical()._hot).all():
+            h = -1
+        else:
+            h = 1
+        return h
+
+    @tuple_mapper
+    def is_canon(self):
+        return (self._hot == N(self).canonical()._hot).all()
+    
+    @tuple_mapper
+    def is_ext_canon(self):
+        return (self._hot == N(self).ext_canonical()._hot).all()
+    
+    @tuple_mapper
+    def energy(self, norm = False, ref = False):
+        e, r = 0, 0
+        for idx, a in enumerate(self.notes()):
+            for jdx, b in enumerate(self.notes()):
+                if jdx > idx:
+                    e += (b-a)**2
+                    e += (N._L-(b-a))**2
+                    r += (N._L/self.num()*(jdx-idx))**2
+                    r += (N._L-N._L/self.num()*(jdx-idx))**2
+        return 1 if ref and norm else r if ref else e/r if norm else e
+    
+    @tuple_mapper
+    def gaps(self):
+        return tuple(sorted(Counter(self.diff()).most_common())[::-1])
+
+    @tuple_mapper
+    def runs(self):
+        runs = []
+        run = 0
+        for gap in self.diff():
+            if gap == 1:
+                run += 1
+            elif run:
+                runs.append(1+run)
+                run = 0
+        if run:
+            if runs:
+                if self.diff()[0] == 1:
+                    runs[0] = runs[0] + run
+                else:
+                    runs.append(1+run)
+            else:
+                runs.append(1+run)
+        return tuple(sorted(Counter(runs).most_common())[::-1])
+    
+    ### COMPARE
+    
+    @tuple_mapper
+    def contains(self, other):
+        return N(other)._hot == (N(self).compose()._hot * N(other)._hot)
+
+    @tuple_mapper
+    def contained(self, other):
+        return other.contains(self)
+
+    ############ MUTATE  (PRESERVE)    
+    
+    @array_mapper
+    def compose(self):
+        self._hot = self._hot.astype(bool)
+        return self
+
+    @array_mapper
+    def decompose(self):
+        self.compose()
+        self._hot = self._hot.astype(int)
+        self._hot += N(self).compliment()._hot
+        return self  
+    
+    ############ MUTATE  (PRESERVE / ONE-TO-ONE)
     
     @array_mapper
     def inv(self):
         self.compose()
         self._hot = np.invert(self._hot)
         return self
 
@@ -154,16 +319,16 @@
                 mdx -= 1
             self._hot[mdx] = 0
             mdx -= 1
             while self._hot[mdx]:
                 mdx -= 1
             self._hot[mdx] = 1
         return self
-
-    ############ MUTATE (one-way)
+    
+    ############ MUTATE (PRESERVE / MANY-TO-ONE)
     
     @array_mapper
     def canonical(self):
         self.compose().modes()
         if self._hot.ndim > 1:
             self._hot = self._hot[-1, :]
             self.roll(1)
@@ -173,57 +338,57 @@
     def ext_canonical(self):
         self.compose().ext_modes()
         if self._hot.ndim > 1:
             self._hot = self._hot[-1, :]
             self.roll(1)
         return self
     
-    ############ MUTATE (restrict)
+    ############ MUTATE (RESTRICTT)
     
     @array_mapper
     def chord(self, n_max = None):
         n_max = n_max if n_max else N._L
         n_max = max(n_max, self.num()//2 + self.num()%2)
         notes = self.notes()[::2][:n_max]
         self._hot = N(notes)._hot
         return self
 
     @array_mapper
     def compliment(self, n_max = None):
         n_max = n_max if n_max else N._L
-        chord = self.copy().chord().notes()
+        chord = N(self).chord().notes()
         notes = [ n for n in self.notes() if n not in chord ][:n_max]
         self._hot = N(notes)._hot
-        return self
-
-   ############ MUTATE (extend)
+        return self  
+    
+   ############ MUTATE (EXPAND)
 
     @array_mapper
     def modes(self):
         if self.num():
-            self._hot = np.array([ self.copy().roll(mdx)._hot for mdx in range(self.num()) ])
+            self._hot = np.array([ N(self).roll(mdx)._hot for mdx in range(self.num()) ])
         return self.crush()
 
     @array_mapper
     def ext_modes(self):
-        x = self.copy().modes()._hot
-        y = self.copy().rev().modes()._hot
+        x = N(self).modes()._hot
+        y = N(self).rev().modes()._hot
         if x.ndim > 1:
             assert y.ndim > 1
             self._hot = np.concatenate((x, y), 0)
         else:
             assert y.ndim == 1
             self._hot = np.array([x, y])
         return self.crush()
     
     @array_mapper
     def parents(self):
         self.compose()
         if not self._hot.sum() == N._L:
-            zdxs = list(enumerate(self.copy().inv().notes()))
+            zdxs = list(enumerate(N(self).inv().notes()))
             self._hot = np.tile(self._hot, len(zdxs))
             self._hot = self._hot.reshape((len(zdxs), N._L))
             for i, j in zdxs:
                 self._hot[i, j] = 1
         return self.crush()
 
     @array_mapper
@@ -239,196 +404,43 @@
     
     @array_mapper
     def universe(self):
         self._hot = np.zeros((2**N._L, N._L), dtype=bool)
         for idx in range(2**N._L):
             self._hot[idx, :] = N(idx)._hot
         return self
-    
-    ############ PERSIST
-    
-    @array_mapper
-    def compose(self):
-        self._hot = self._hot.astype(bool)
-        return self
-
-    @array_mapper
-    def decompose(self):
-        self.compose()
-        self._hot = self._hot.astype(int)
-        self._hot += self.copy().compliment()._hot
-        return self
 
-    ############ REVEAL
-
-    @tuple_mapper
-    def hot(self):
-        return tuple(int(x) for x in self._hot)
-
-    @tuple_mapper
-    def index(self):
-        return int(''.join(map(str, self.copy().compose().hot())), 2)
-    
-    @tuple_mapper
-    def notes(self):
-        return tuple(np.where(self._hot)[0])
-
-    @tuple_mapper
-    def string(self):
-        return ''.join([ 'x' if x else '_' for x in self.hot() ])
+    def uv(self):
+        return self.universe()
     
-    @tuple_mapper
-    def forte(self):
-        x = self.num()
-        y = 1 + self.copy().modes()._hot.tolist().index(self.copy().canonical())
-        return (x, y)
-    
-    @tuple_mapper
-    def forte_string(self):
-        x = self.num()
-        y = 1 + self.copy().modes()._hot.tolist().index(self.copy().canonical())
-        return '-'.join(self.forte())
-    
-    @tuple_mapper
-    def diff(self):
-        return tuple(np.diff(list(self.notes())+[N._L+self.notes()[0]])) if self.notes() else ()
-    
-    @tuple_mapper
-    def lookup(self):
-        name = N._cmap.get(self.notes())
-        if not name:
-            modes = self.copy().modes()
-            for mode in modes._hot:
-                mode = N(mode)
-                name = N._cmap.get(mode.notes())
-                if name:
-                    if not self._hot[0]:
-                        name = f'disp. mode of {name}'
-                    else:
-                        for mdx in range(self.num()):
-                            if (self._hot == mode.copy().roll(mdx)._hot).all():
-                                name = f'{_e(mdx+1)} mode of {name}'
-                                break
-                    break
-        return name if name else ''
-    
-    ############ SUMMARIZE
-    
-    @tuple_mapper
-    def num(self):
-        return self._hot.sum()
-    
-    @tuple_mapper
-    def spin(self):
-        return self.handedness() * self.symmetry()
-
-    @tuple_mapper
-    def symmetry(self):
-        for m in range(1, 1 + N._L):
-            if not N._L % m:
-                l = N._L // m
-                tiled = np.reshape(self._hot, (m, l))
-                if (tiled == tiled[0]).all():
-                    sym = m
-        return sym
-
-    @tuple_mapper
-    def handedness(self):
-        if (self.copy().canonical()._hot == self.copy().rev().canonical()._hot).all():
-            h = 0
-        elif (self.copy().canonical()._hot == self.copy().ext_canonical()._hot).all():
-            h = -1
-        else:
-            h = 1
-        return h
-
-    @tuple_mapper
-    def is_canon(self):
-        return (self._hot == self.copy().canonical()._hot).all()
-    
-    @tuple_mapper
-    def is_ext_canon(self):
-        return (self._hot == self.copy().ext_canonical()._hot).all()
-    
-    @tuple_mapper
-    def energy(self, norm = False, ref = False):
-        e, r = 0, 0
-        for idx, a in enumerate(self.notes()):
-            for jdx, b in enumerate(self.notes()):
-                if jdx > idx:
-                    e += (b-a)**2
-                    e += (N._L-(b-a))**2
-                    r += (N._L/self.num()*(jdx-idx))**2
-                    r += (N._L-N._L/self.num()*(jdx-idx))**2
-        return 1 if ref and norm else r if ref else e/r if norm else e
-    
-    @tuple_mapper
-    def gaps(self):
-        return tuple(sorted(Counter(self.diff()).most_common())[::-1])
-
-    @tuple_mapper
-    def runs(self):
-        runs = []
-        run = 0
-        for gap in self.diff():
-            if gap == 1:
-                run += 1
-            elif run:
-                runs.append(1+run)
-                run = 0
-        if run:
-            if runs:
-                if self.diff()[0] == 1:
-                    runs[0] = runs[0] + run
-                else:
-                    runs.append(1+run)
-            else:
-                runs.append(1+run)
-        return tuple(sorted(Counter(runs).most_common())[::-1])
-    
-    ### HARMONIZE
-    
-    @tuple_mapper
-    def harmonize(self, n_max = 4):
-        chords = ( self.copy().roll(mdx).chord(n_max).hot() for mdx in range(self.num()) )
-        return tuple(zip(self.notes(), chords))
-    
-    ### COMPARE
-    
-    @tuple_mapper
-    def contains(self, other):
-        if not isinstance(other, N):
-            other = N(other)
-        return other.copy()._hot == (self.copy().compose()._hot * other.copy()._hot)
-
-    @tuple_mapper
-    def contained(self, other):
-        if not isinstance(other, N):
-            other = N(other)
-        return other.contains(self)
+    ### WE LOVE TO SPREADSHEET
     
-    ### UNIVERSE
+    @pd_check
+    def df(self, filt = None):
+        return self.dataframe(filt)
     
+    @pd_check
     def dataframe(self, filt = None):
 
         '''
             Creates a panda of all 2**L sequences, or
               optionally filtered down to a musically
               relevant subset.
         '''
         
         if isinstance(filt, str):
             assert filt in ['hot', 'canon', 'ext_canon']
 
+        hots  = self._hot if self._hot.ndim > 1 else [self._hot]    
+            
         cols  = ['hot', 'num', 'energy', 'symmetry']
         cols += ['ext_canonical', 'runs', 'gaps']
         cols += ['canonical', 'handedness', 'string', 'lookup']
 
         rows = []
-        hots = self._hot if self._hot.ndim > 1 else [self._hot]
         for hot in hots:
             row = []
             for col in cols:
                 value = getattr(N(hot), col)()
                 value = value.hot() if isinstance(value, N) else value
                 row.append(value)
             rows.append(row)
@@ -476,8 +488,8 @@
 
         return df
 
 ################################################
 
 if __name__ == '__main__':    
     n  = N()
-    df = n.universe().dataframe()
+    df = n.uv().df()
```

### Comparing `kctools-0.2.3/kctools/classes/vec.py` & `kctools-0.23.8/kctools/classes/vec.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,94 +3,106 @@
 from .map import Map
 
 ################################################
 
 class Vector():
     
     '''
-        A Vector() is a class that keeps track of things in a map.
+        A Vector is a class that keeps track of attributes in a Map.
         
-        Can zero, set, add, and multiply with each other or dicts.
+        It can zero itself, or set, add, or multiply with other Vectors,
+          or dicts.
     '''
 
     def __init__(self, inp = {}):
         self._map = Map()
         self.set(inp, True)
+        self.snap()
 
     def __repr__(self):
         return str(list(self.items()))
-        
+    
     def keys(self):
         return ( x for x in self._map.keys() )
     
     def values(self):
         return ( getattr(self, x) for x in self._map.keys() )
     
     def items(self):
         return ( (x, getattr(self, x)) for x in self._map.keys() )
     
+    def snap(self):
+        self._snap = self.values()
+        
+    def recall(self):
+        return self._snap
+    
     ###
     
     def nullify(self):
         '''
             set all attributes to 'zero', by:
             self.attr = 0
         '''
-        for attr in self._map:
-            setattr(self, attr, type(getattr(self, attr))())
+        for attr, value in self._map.items():
+            setattr(self, attr, type(value)())
         return self
     
     ###
 
     def set(self, inp, add_new = False):
+        assert type(inp) in [dict, Vector]
         '''
             set all attributes (found in 'inp'), by:
             self.attr = inp.attr
-        '''         
+        '''
         for attr, value in inp.items():
             if attr in self._map or add_new:
                 self._map.add(attr)
                 setattr(self, attr, value)
         return self
     
     ###
     
     def add(self, inp, add_new = False):
+        assert type(inp) in [dict, Vector]
         '''
             set all attributes (found in 'inp'), by:
             self.attr = self.attr + inp.attr
         '''
         for attr, value in inp.items():
             if attr in self._map:
                 if type(value) in [set, dict]:
                     value.update(inp)
                 else:
                     setattr(self, attr, getattr(self, attr) + value)
             elif add_new:
-                # unsafe!
+                # unsafe! ??
                 self._map.add(attr)
                 setattr(self, attr, value)
         return self
     
     ###
     
     def mul(self, inp, add_new = False):
+        assert type(inp) in [dict, Vector]
         '''
             set all attributes (found in 'inp', if inp.attr is numeric), by:
             self.attr = self.attr * inp.attr
         '''
         for attr, value in inp.items():
             if type(value) in [int, float, complex]:
                 if attr in self._map:
                     setattr(self, attr, getattr(self, attr) * value)
         return self
     
     ###
     
     def apply(self, inp, func, add_new = False):
+        assert type(inp) in [dict, Vector]
         '''
             set all attributes (found in 'inp'), by:
             self.attr = func(self.attr, inp.attr)
         '''
         for attr, value in inp.items():
             if attr in self._map:
                 setattr(self, attr, func(getattr(self, attr), value))
@@ -99,50 +111,47 @@
         return self
     
 ################################################
 
 class VecSet(Vector):
     
     '''
-        A VecSet() extends Vector():
-          other Vectors can be loaded
-            (or unloaded) from a named
-            key, and attributes may be
-            reset to the sum of these
-            named keys.
+        A VecSet is a Vector that is also the
+          sum of a collection of other Vectors,
+          which may be loaded or unloaded with
+          a named key.
     '''
 
     def __init__(self):
         Vector.__init__(self)
-        self._slots = []
+        self._slots = {}
 
     ###
 
     def _reset(self):
-        for attr, value in self._map:
-            setattr(self, attr, type(value)())
-        for slot, vecset in self._slots:
-            self.add(vecset, True)
+        self.nullify()
+        for key, value in self._slots.items():
+            self.add(value, True)
 
     ###
-    
-    def load(self, inp):
-        self._slots.update(inp)
+
+    def load(self, key, value):
+        assert type(value) in [dict, Vector]
+        if isinstance(value, dict):
+            value = Vector(value)
+        self._slots.update({key: value})
         self._reset()
 
     ###
     
     def unload(self, key):
         if key in self._slots:
             del self._slots[key]
             self._reset()
 
 ################################################
-
-
-
```

### Comparing `kctools-0.2.3/kctools/kctools.py` & `kctools-0.23.8/kctools/kctools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,84 @@
 ########################################################################
 
-import logging, math, os, re, string, sys
 import datetime as dt
+import logging, math, os, re, string, sys
 
 from copy        import deepcopy
-from collections import *
+from collections import defaultdict
+from importlib   import util
+
+
+is_np  = util.find_spec('numpy') is not None
+is_pd  = util.find_spec('pandas') is not None
+is_sci = util.find_spec('scipy') is not None
+is_mpl = util.find_spec('matplotlib') is not None
 
-import numpy  as np
-import pandas as pd
+if is_np:
+    import numpy  as np
 
-from scipy.stats import beta
-from matplotlib  import pyplot as plt
+if is_pd:    
+    import pandas as pd
+    
+if is_sci:    
+    from scipy.stats import beta
+      
+if is_mpl:
+    from matplotlib import pyplot as plt
+
+    
+def np_check(method):
+    def wrapped(*args, **kwargs):
+        if is_np:
+            return method(*args, **kwargs)
+        else:
+            raise Exception('Please install numpy.')
+    return wrapped
 
+
+def pd_check(method):
+    def wrapped(*args, **kwargs):
+        if is_pd:
+            return method(*args, **kwargs)
+        else:
+            raise Exception('Please install pandas.')
+    return wrapped
+
+
+def sci_check(method):
+    def wrapped(*args, **kwargs):
+        if is_sci:
+            return method(*args, **kwargs)
+        else:
+            raise Exception('Please install scipy.')
+    return wrapped
+
+                            
+def mpl_check(method):
+    def wrapped(*args, **kwargs):
+        if is_mpl:
+            return method(*args, **kwargs)
+        else:
+            raise Exception('Please install matplotlib.')
+    return wrapped
+
+########################################################################
 ########################################################################
 ### FILES:
 
 def lsdashr(tdir, absolute = False):
     sdx = 0 if absolute else len(tdir)
     return [ os.path.join(dp, f)[sdx:] for dp, dn, fn in os.walk(tdir) for f in fn ]
 
 def readlines(fname, mode = 'r'):
     with open(fname, mode) as fp:
         return [ line.strip() for line in fp.readlines() ]
 
 ########################################################################
+########################################################################
 ### STRINGS:
 
 def lpad(text, x = 2):
     return '\n'.join([ ''.join([' '] * x + list(line)) for line in text.split('\n') ])
 
 ###########################
 
@@ -77,14 +128,15 @@
     c = {0: '', 3: 'k', 6: 'M', 9: 'B', 12: 'T'}[d]
     l = min(e+1, l)
     r = mround(m, 10**(max(e-l+1, 0)))/(10**d)
     r = int(r) if (e-d+1 >= l) else r
     return f'{"-" if n < 0 else ""}{r}{" " if space else ""}{c}'
 
 ########################################################################
+########################################################################
 ### LISTS:
 
 def only_one(inlist):
     return sum(map(bool, inlist)) == 1
 
 ###########################
 
@@ -131,34 +183,40 @@
     while(found):
         answers.append(ans)
         ans, found = get_next_idxs_in_thing(test, thing, already = answers)
     
     return answers
 
 ########################################################################
+########################################################################
 ### DICTS:
 
-def autovivify(levels = 2, final = int):
+def autovivify():
+    '''thanks eu'''
+    return defaultdict(lambda: autovivify())
+
+def vivify(levels = 2, final = int):
     '''thanks bert'''
-    return defaultdict(final) if levels==1 else defaultdict(lambda: autovivify(levels-1, final))
+    return defaultdict(final) if levels==1 else defaultdict(lambda: vivify(levels-1, final))
 
 def mortify(inp):
     return { k: mortify(v) for k, v in inp.items() } if isinstance(inp, dict) else inp
 
-def dict_update(A, B, new = False):
-    if new:
+def dict_update(A, B, inplace = False):
+    if not inplace:
         A = deepcopy(A)
     for key, value in B.items():
         if key in A and isinstance(value, dict):
             A[key] = dict_update(A[key], value)
         else:
             A[key] = value
     return A
 
 ########################################################################
+########################################################################
 ### LOGGING:
 
 def setup_logger(
         name,
         path    = '',
         mode    = 'a',
         level   = 'debug',
@@ -188,98 +246,122 @@
         f_handler.setLevel(f_level)
         f_handler.setFormatter(logging.Formatter(fmt=fmt, datefmt=datefmt))
         logger.addHandler(f_handler)
     
     return logger
 
 ########################################################################
+########################################################################
 ### NUMBERS: 
 
 def mround(x, m):
     return int(m * round(float(x)/m))
 
 def coalesce(*values):
     y = 0
     for x in values:
         y = y + x + y*x
     return y
 
 ########################################################################
+########################################################################
 ### NUMPY:
 
+@np_check
 def normalize(arr):
     return np.nan_to_num(np.divide(arr, np.sum(arr)))
 
 ###########################
 
+@np_check
 def is_diagonal(mtx):
     return not np.count_nonzero(mtx - np.diag(np.diagonal(mtx)))
 
 ###########################
 
+@np_check
 def kpow(x, p):
     return np.power(np.power(x, 1/p).mean(), p)
 
+@np_check
 def kcos(a, b):
     return np.nan_to_num(np.divide(np.dot(a, b), np.multiply(np.sqrt(np.square(a).sum()), np.sqrt(np.square(b).sum()))), copy=False)
 
 ###########################
 
+@np_check
 def bin_entropy(true, pred, eps = 0.0000001):
     return -np.sum( true * np.log(pred+eps) + (1-true) * np.log(1-pred+eps) )
 
+@np_check
 def mod_entropy(true, pred, mod = 2., eps = 0.0000001):
     return -np.sum( true * np.log(pred+eps) + (1-true) * (mod * pred) * np.log(1-pred+eps) )
 
 ###########################
 
+@np_check
 def pargsort(arr, n):
     idxs = np.argpartition(arr, n)[:n]
     return idxs[np.argsort(arr[idxs])][:n]
 
+@np_check
 def psort(arr, n):
     return arr[pargsort(arr, n)]
 
 ###########################
 
+@np_check
 def rchoice(*args, **kwargs):
     try:
         return np.random.choice(*args, **kwargs)
     except ValueError:
-        size = kwargs.get('size') or args[1] or 1
+        size = kwargs.get('size')
+        if not size:
+            if len(args) > 1:
+                size = args[1]
+            else:
+                size = 1
         if size < 2:
             return None
         else:
             return np.array([], dtype = object)
 
-###########################
-### SCIPY
+########################################################################
+########################################################################
+### SCIPY:
 
+@sci_check
 def lower_conf_bound(ups, downs, conf = 0.683):
     return beta.ppf((1.-conf)/2., 1+ups, 1+downs)
 
+@sci_check
 def upper_conf_bound(ups, downs, conf = 0.683):
     return beta.ppf(1.-(1.-conf)/2., 1+ups, 1+downs)
 
+@sci_check
 def conf_bounds(ups, downs, conf = 0.683):
     return (lower_conf_bound(ups, downs, conf), upper_conf_bound(ups, downs, conf))
 
 ########################################################################
+########################################################################
 ### PANDAS:
 
+@pd_check
 def rename_dup_df_cols(df, sep = '.'):
     names = pd.Series(df.columns)
     for dup in df.columns.get_duplicates():
         d_mask = df.columns.get_loc(dup)
         names[d_mask] = [ f'{dup}{sep}{ddx}' for ddx in range(d_mask.sum()) ]
     df.columns = names
 
 ########################################################################
+########################################################################
 ### MATPLOTLIB:
 
+@mpl_check
 def make_heatmap(
             data,
             xlabels  = None,
             ylabels  = None,
             annotate = True,
             title    = None,
             subtitle = None,
```

### Comparing `kctools-0.2.3/kctools.egg-info/PKG-INFO` & `kctools-0.23.8/kctools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kctools
-Version: 0.2.3
+Version: 0.23.8
 Summary: miscellaneous elves
 Home-page: https://github.com/kcstokely/kctools
 Author: kevin c. stokely
 Author-email: kcstokely@gmail.com
 License: MIT
 Description: # kctools
```

### Comparing `kctools-0.2.3/setup.py` & `kctools-0.23.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,21 @@
 
 with open('README.md', 'r') as fp:
     long_description = fp.read()
     long_description_content_type = 'text/markdown'
 
 setuptools.setup(
     name             = 'kctools',
-    version          = '0.2.3',
+    version          = '0.23.8',
     author           = 'kevin c. stokely',
     author_email     = 'kcstokely@gmail.com',
     description      = 'miscellaneous elves',
     url              = 'https://github.com/kcstokely/kctools',
     packages         = setuptools.find_packages(),
-    install_requires = [
-        'matplotlib',
-        'numpy',
-        'pandas',
-        'scipy'
-    ],
-    license = 'MIT',
+    license          = 'MIT',
     classifiers = [
          'Operating System :: OS Independent',
          'Programming Language :: Python :: 3',
          'License :: OSI Approved :: MIT License'
     ],
     long_description              = long_description,
     long_description_content_type = long_description_content_type
```

