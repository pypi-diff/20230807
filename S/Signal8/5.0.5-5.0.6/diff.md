# Comparing `tmp/Signal8-5.0.5.tar.gz` & `tmp/Signal8-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-5.0.5.tar", last modified: Tue Jul 25 22:38:04 2023, max compression
+gzip compressed data, was "Signal8-5.0.6.tar", last modified: Mon Aug  7 19:26:20 2023, max compression
```

## Comparing `Signal8-5.0.5.tar` & `Signal8-5.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.857646 Signal8-5.0.5/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.5/LICENSE
--rw-rw-rw-   0        0        0     5300 2023-07-25 22:38:04.855641 Signal8-5.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4800 2023-07-22 22:09:51.000000 Signal8-5.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.762601 Signal8-5.0.5/Signal8/
--rw-rw-rw-   0        0        0    10063 2023-07-25 22:37:39.000000 Signal8-5.0.5/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.5/Signal8/__init__.py
--rw-rw-rw-   0        0        0     3288 2023-07-25 22:34:44.000000 Signal8-5.0.5/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.847641 Signal8-5.0.5/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.5/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.5/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     1208 2023-07-25 22:36:49.000000 Signal8-5.0.5/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.5/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.5/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.5/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.811641 Signal8-5.0.5/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5300 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 22:38:04.858640 Signal8-5.0.5/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-07-25 22:36:55.000000 Signal8-5.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:26:20.688620 Signal8-5.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5270 2023-08-07 19:26:20.675621 Signal8-5.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4770 2023-08-07 19:25:58.000000 Signal8-5.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 19:26:20.552621 Signal8-5.0.6/Signal8/
+-rw-rw-rw-   0        0        0    10076 2023-08-07 19:25:59.000000 Signal8-5.0.6/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.6/Signal8/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-08-07 18:43:42.000000 Signal8-5.0.6/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:26:20.666621 Signal8-5.0.6/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.6/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.6/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     1383 2023-08-07 19:25:59.000000 Signal8-5.0.6/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.6/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.6/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.6/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:26:20.617620 Signal8-5.0.6/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5270 2023-08-07 19:26:20.000000 Signal8-5.0.6/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-08-07 19:26:20.000000 Signal8-5.0.6/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 19:26:20.000000 Signal8-5.0.6/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 19:26:20.000000 Signal8-5.0.6/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 19:26:20.688620 Signal8-5.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-08-07 19:25:59.000000 Signal8-5.0.6/setup.py
```

### Comparing `Signal8-5.0.5/LICENSE` & `Signal8-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.5/PKG-INFO` & `Signal8-5.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.5
+Version: 5.0.6
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -44,25 +44,25 @@
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
-| :---------------: | :--------------------------------------------: |
-|    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
-|    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
-|   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
-|     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
-| ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
-|   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
-| ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
-| ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
+| :--------------: | :--------------------------------------------: |
+|    ``bisect``    | ![1691433763627](image/README/1691433763627.png) |
+|    ``circle``    | ![1691433778699](image/README/1691433778699.png) |
+|  ``corners``Â   | ![1691433832902](image/README/1691433832902.png) |
+|    ``cross``    | ![1691433961564](image/README/1691433961564.png) |
+|  ``staggered``  | ![1691433856331](image/README/1691433856331.png) |
+|   ``quarters``   | ![1691433864962](image/README/1691433864962.png) |
+|  ``stellaris``  | ![1691433878432](image/README/1691433878432.png) |
+|   ``scatter``   | ![1691433899914](image/README/1691433899914.png) |
 
-The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
+The red zones denote regions where large obstacles can be spawned, while the remaining space designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Contributing
 
 We welcome contributions to Signal8! If you're interested in contributing, you can do so in the following ways:
 
 * **Bug Reports** : If you discover a bug when using Signal8, please submit a report via the issues tab. When submitting an issue, please do your best to include a detailed description of the problem and a code sample, if applicable.
 * **Feature Requests** : If you have a great idea that you think would improve Signal8, don't hesitate to post your suggestions in the issues tab. Please be as detailed as possible in your explanation.
```

### Comparing `Signal8-5.0.5/README.md` & `Signal8-5.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,25 +32,25 @@
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
-| :---------------: | :--------------------------------------------: |
-|    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
-|    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
-|   ``corners``    | ![1686604788813](image/README/1686604788813.png) |
-|     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
-| ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
-|   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
-| ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
-| ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
+| :--------------: | :--------------------------------------------: |
+|    ``bisect``    | ![1691433763627](image/README/1691433763627.png) |
+|    ``circle``    | ![1691433778699](image/README/1691433778699.png) |
+|  ``corners``   | ![1691433832902](image/README/1691433832902.png) |
+|    ``cross``    | ![1691433961564](image/README/1691433961564.png) |
+|  ``staggered``  | ![1691433856331](image/README/1691433856331.png) |
+|   ``quarters``   | ![1691433864962](image/README/1691433864962.png) |
+|  ``stellaris``  | ![1691433878432](image/README/1691433878432.png) |
+|   ``scatter``   | ![1691433899914](image/README/1691433899914.png) |
 
-The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
+The red zones denote regions where large obstacles can be spawned, while the remaining space designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Contributing
 
 We welcome contributions to Signal8! If you're interested in contributing, you can do so in the following ways:
 
 * **Bug Reports** : If you discover a bug when using Signal8, please submit a report via the issues tab. When submitting an issue, please do your best to include a detailed description of the problem and a code sample, if applicable.
 * **Feature Requests** : If you have a great idea that you think would improve Signal8, don't hesitate to post your suggestions in the issues tab. Please be as detailed as possible in your explanation.
```

### Comparing `Signal8-5.0.5/Signal8/Signal8.py` & `Signal8-5.0.6/Signal8/Signal8.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         )
         return not within_constraints
 
     # Reset agents and goals to their initial positions
     def _reset_agents_and_goals(self, world, np_random):
         epsilon = world.agents[0].radius
         
-        if world.problem_instance in ['bisect', 'cross', 'quarters']:
+        if world.problem_instance in ['bisect', 'cross', 'staggered', 'quarters']:
             # Used for problem instances composed of rectangles
             x_constraints = [constr[0] for constr in world.instance_constr]
             y_constraints = [constr[1] for constr in world.instance_constr]
 
         for i, agent in enumerate(world.agents):
             agent.goal = world.goals[i]
```

### Comparing `Signal8-5.0.5/Signal8/main.py` & `Signal8-5.0.6/Signal8/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,21 +65,21 @@
     boundary = lines.convex_hull
     polygons = boundary.difference(lines)
     regions = [polygons] if polygons.geom_type == 'Polygon' else list(polygons.geoms)
     return regions
 
 
 env = signal8.env()
-problem_instance = 'stellaris'
+problem_instance = 'cross'
 
 agent_radius = env.unwrapped.world.agents[0].radius
 obstacle_radius = env.unwrapped.world.large_obstacles[0].radius
 
 start_time = time.time()
-for i in range(100):
+for i in range(1000):
     env.reset(options={'problem_instance': problem_instance})
     start_state = env.state()
     start = start_state[0:2]
     goal = start_state[2:4]
     obstacles = start_state[4:].reshape(-1, 2)
     
     agent_with_size = Point(start).buffer(agent_radius)
@@ -93,9 +93,9 @@
     plt.fill(*goal_with_size.exterior.xy, alpha=0.5, color='green')
 
 end_time = time.time()
 print(f'Elapsed time: {end_time - start_time}')
 
 plt.xlim(-1, 1)
 plt.ylim(-1, 1)
-plt.savefig('stellaris.png')
+plt.savefig('cross.png')
 a=3
```

### Comparing `Signal8-5.0.5/Signal8/utils/core.py` & `Signal8-5.0.6/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.5/Signal8/utils/problems.py` & `Signal8-5.0.6/Signal8/utils/problems.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,32 @@
 problems = {
     'bisect': [
         ((-1, -0), (-1, 1))
         ],
     'circle':  [
         ((0, 0), (0.5)),
         ],
-    'corners': [
-        ((1, 1), (0.40)),
-        ((1, -1), (0.40)),
-        ((-1, -1), (0.40)),
-        ((-1, 1), (0.40)),
-        ],
     'cross': [
         ((-0.25, 0.25), (0, 0.75)),
         ((-0.25, 0.25), (-0.75, 0)),
         ((-0.75, 0), (-0.25, 0.25)),
         ((0, 0.75), (-0.25, 0.25)),
         ],
+    'corners': [
+        ((1, 1), (0.40)),
+        ((1, -1), (0.40)),
+        ((-1, -1), (0.40)),
+        ((-1, 1), (0.40)),
+        ],
+    'staggered': [
+        ((-0.6, -0.4), (0.5, 1)),
+        ((-0.3, -0.1), (-1, -0.6)),
+        ((0.15, 0.35), (-0.15, 1)),
+        ((0.55, 0.75), (-1, -0.75)),
+    ],
     'quarters': [
         ((-1, -0.5), (-0.25, 0.25)),
         ((-0.25, 0.25), (0.5, 1)),
         ((0.5, 1), (-0.25, 0.25)),
         ((-0.25, 0.25), (-1, -0.5)),
         ],
     'scatter': [
```

### Comparing `Signal8-5.0.5/Signal8/utils/simple_env.py` & `Signal8-5.0.6/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.5/Signal8/utils/test_dynamic_obs.py` & `Signal8-5.0.6/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.5/Signal8.egg-info/PKG-INFO` & `Signal8-5.0.6/Signal8.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.5
+Version: 5.0.6
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -44,25 +44,25 @@
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
-| :---------------: | :--------------------------------------------: |
-|    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
-|    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
-|   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
-|     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
-| ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
-|   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
-| ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
-| ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
+| :--------------: | :--------------------------------------------: |
+|    ``bisect``    | ![1691433763627](image/README/1691433763627.png) |
+|    ``circle``    | ![1691433778699](image/README/1691433778699.png) |
+|  ``corners``Â   | ![1691433832902](image/README/1691433832902.png) |
+|    ``cross``    | ![1691433961564](image/README/1691433961564.png) |
+|  ``staggered``  | ![1691433856331](image/README/1691433856331.png) |
+|   ``quarters``   | ![1691433864962](image/README/1691433864962.png) |
+|  ``stellaris``  | ![1691433878432](image/README/1691433878432.png) |
+|   ``scatter``   | ![1691433899914](image/README/1691433899914.png) |
 
-The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
+The red zones denote regions where large obstacles can be spawned, while the remaining space designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Contributing
 
 We welcome contributions to Signal8! If you're interested in contributing, you can do so in the following ways:
 
 * **Bug Reports** : If you discover a bug when using Signal8, please submit a report via the issues tab. When submitting an issue, please do your best to include a detailed description of the problem and a code sample, if applicable.
 * **Feature Requests** : If you have a great idea that you think would improve Signal8, don't hesitate to post your suggestions in the issues tab. Please be as detailed as possible in your explanation.
```

### Comparing `Signal8-5.0.5/setup.py` & `Signal8-5.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="5.0.5",
+    version="5.0.6",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

