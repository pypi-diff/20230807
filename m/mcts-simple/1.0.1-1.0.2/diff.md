# Comparing `tmp/mcts-simple-1.0.1.tar.gz` & `tmp/mcts-simple-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\USER\OneDrive\Desktop\MACHINE LEARNING\mcts_simple\dist\.tmp-1xubisio\mcts-simple-1.0.1.tar", last modified: Sun Feb 26 03:52:44 2023, max compression
+gzip compressed data, was "C:\Users\USER\OneDrive\Desktop\MACHINE LEARNING\mcts_simple\dist\.tmp-vd2g0lvy\mcts-simple-1.0.2.tar", last modified: Mon Aug  7 12:45:15 2023, max compression
```

## Comparing `mcts-simple-1.0.1.tar` & `mcts-simple-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/
--rw-rw-rw-   0        0        0     1087 2022-02-19 09:40:27.000000 mcts-simple-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     8828 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7971 2023-02-26 03:52:11.000000 mcts-simple-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple/
--rw-rw-rw-   0        0        0      173 2023-02-26 03:43:04.000000 mcts-simple-1.0.1/mcts_simple/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple/mcts/
--rw-rw-rw-   0        0        0     1787 2023-02-25 13:57:15.000000 mcts-simple-1.0.1/mcts_simple/mcts/game.py
--rw-rw-rw-   0        0        0     6328 2023-02-25 12:03:08.000000 mcts-simple-1.0.1/mcts_simple/mcts/mcts.py
--rw-rw-rw-   0        0        0     2708 2023-02-25 10:38:48.000000 mcts-simple-1.0.1/mcts_simple/mcts/open_loop_mcts.py
--rw-rw-rw-   0        0        0     1739 2023-02-26 01:04:22.000000 mcts-simple-1.0.1/mcts_simple/mcts/open_loop_uct.py
--rw-rw-rw-   0        0        0     2600 2023-02-25 08:51:30.000000 mcts-simple-1.0.1/mcts_simple/mcts/uct.py
-drwxrwxrwx   0        0        0        0 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple.egg-info/
--rw-rw-rw-   0        0        0     8828 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/mcts_simple.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2023-02-26 02:57:27.000000 mcts-simple-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-26 03:52:44.000000 mcts-simple-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1420 2023-02-26 03:50:13.000000 mcts-simple-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2022-02-19 09:40:27.000000 mcts-simple-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     8828 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7971 2023-02-26 03:52:11.000000 mcts-simple-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple/
+-rw-rw-rw-   0        0        0      173 2023-08-07 12:29:39.000000 mcts-simple-1.0.2/mcts_simple/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple/mcts/
+-rw-rw-rw-   0        0        0     1787 2023-02-25 13:57:15.000000 mcts-simple-1.0.2/mcts_simple/mcts/game.py
+-rw-rw-rw-   0        0        0     6327 2023-08-07 12:24:09.000000 mcts-simple-1.0.2/mcts_simple/mcts/mcts.py
+-rw-rw-rw-   0        0        0     2708 2023-02-25 10:38:48.000000 mcts-simple-1.0.2/mcts_simple/mcts/open_loop_mcts.py
+-rw-rw-rw-   0        0        0     1739 2023-02-26 01:04:22.000000 mcts-simple-1.0.2/mcts_simple/mcts/open_loop_uct.py
+-rw-rw-rw-   0        0        0     2600 2023-02-25 08:51:30.000000 mcts-simple-1.0.2/mcts_simple/mcts/uct.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple.egg-info/
+-rw-rw-rw-   0        0        0     8828 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/mcts_simple.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2023-02-26 02:57:27.000000 mcts-simple-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 12:45:15.000000 mcts-simple-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1420 2023-08-07 12:27:16.000000 mcts-simple-1.0.2/setup.py
```

### Comparing `mcts-simple-1.0.1/LICENSE` & `mcts-simple-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcts-simple-1.0.1/PKG-INFO` & `mcts-simple-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcts-simple
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package that helps to quickly implement MCTS to solve reinforcement learning problems.
 Home-page: https://github.com/DenseLance/mcts-simple
 Author: Lance Chin
 Author-email: denselance@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DenseLance/mcts-simple/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mcts-simple-1.0.1/README.md` & `mcts-simple-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mcts-simple-1.0.1/mcts_simple/mcts/game.py` & `mcts-simple-1.0.2/mcts_simple/mcts/game.py`

 * *Files identical despite different names*

### Comparing `mcts-simple-1.0.1/mcts_simple/mcts/mcts.py` & `mcts-simple-1.0.2/mcts_simple/mcts/mcts.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             else:
                 self.children[action] = Node(next_player, next_state, prev_node = self)
 
     def choose_best_action(self, training: bool) -> int:
         return max(self.children, key = lambda action: self.children[action].eval(training))
 
     def choose_random_action(self) -> int:
-        return random.sample(self.children.keys(), 1)[0]
+        return random.sample(list(self.children), 1)[0]
 
 class MCTS:
     def __init__(self, game: Game, allow_transpositions: bool = True, training: bool = True):
         self.game = game
         self.copied_game = deepcopy(self.game)
 
         self.transposition_table = dict() if allow_transpositions is True else None
```

### Comparing `mcts-simple-1.0.1/mcts_simple/mcts/open_loop_mcts.py` & `mcts-simple-1.0.2/mcts_simple/mcts/open_loop_mcts.py`

 * *Files identical despite different names*

### Comparing `mcts-simple-1.0.1/mcts_simple/mcts/open_loop_uct.py` & `mcts-simple-1.0.2/mcts_simple/mcts/open_loop_uct.py`

 * *Files identical despite different names*

### Comparing `mcts-simple-1.0.1/mcts_simple/mcts/uct.py` & `mcts-simple-1.0.2/mcts_simple/mcts/uct.py`

 * *Files identical despite different names*

### Comparing `mcts-simple-1.0.1/mcts_simple.egg-info/PKG-INFO` & `mcts-simple-1.0.2/mcts_simple.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcts-simple
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package that helps to quickly implement MCTS to solve reinforcement learning problems.
 Home-page: https://github.com/DenseLance/mcts-simple
 Author: Lance Chin
 Author-email: denselance@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DenseLance/mcts-simple/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mcts-simple-1.0.1/setup.py` & `mcts-simple-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 import setuptools
 
 # METADATA
 NAME = "mcts-simple"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 AUTHOR = "Lance Chin"
 EMAIL = "denselance@gmail.com"
 DESCRIPTION = "Python package that helps to quickly implement MCTS to solve reinforcement learning problems."
 URL = "https://github.com/DenseLance/mcts-simple"
 REQUIRES_PYTHON = ">=3.7.0"
 
 DEPENDENCIES = ["tqdm", "gymnasium"]
```

