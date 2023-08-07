# Comparing `tmp/lesaviezvous-0.2.5.tar.gz` & `tmp/lesaviezvous-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.2.5.tar", last modified: Mon Jul 10 19:42:00 2023, max compression
+gzip compressed data, was "lesaviezvous-0.2.6.tar", last modified: Mon Aug  7 11:03:51 2023, max compression
```

## Comparing `lesaviezvous-0.2.5.tar` & `lesaviezvous-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.2.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1539 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      670 2023-07-10 19:41:27.000000 lesaviezvous-0.2.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-10 19:26:59.000000 lesaviezvous-0.2.5/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79538 2023-07-10 19:25:06.000000 lesaviezvous-0.2.5/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1539 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      239 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 lesaviezvous-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 19:41:38.000000 lesaviezvous-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-07 11:03:51.134368 lesaviezvous-0.2.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2735 2023-08-07 11:03:51.134368 lesaviezvous-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1634 2023-08-07 11:01:49.000000 lesaviezvous-0.2.6/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-07 11:03:51.130367 lesaviezvous-0.2.6/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-10 19:26:59.000000 lesaviezvous-0.2.6/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79817 2023-08-07 10:38:37.000000 lesaviezvous-0.2.6/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-07 11:03:51.134368 lesaviezvous-0.2.6/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2735 2023-08-07 11:03:50.000000 lesaviezvous-0.2.6/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      239 2023-08-07 11:03:50.000000 lesaviezvous-0.2.6/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-07 11:03:50.000000 lesaviezvous-0.2.6/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-08-07 11:03:50.000000 lesaviezvous-0.2.6/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 lesaviezvous-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-08-07 11:03:51.134368 lesaviezvous-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-08-07 10:41:33.000000 lesaviezvous-0.2.6/setup.py
```

### Comparing `lesaviezvous-0.2.5/LICENSE` & `lesaviezvous-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.2.5/lesaviezvous/lesaviezvous.py` & `lesaviezvous-0.2.6/lesaviezvous/lesaviezvous.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-facts = [
+faits = [
   "La Terre est la seule planète connue à abriter la vie.",
   "Les abeilles communiquent en dansant.",
   "Le cerveau humain pèse environ 1,4 kilogramme.",
   "Les éléphants sont les seuls animaux à se reconnaître dans un miroir.",
   "Les dauphins dorment avec un œil ouvert.",
   "Les grenouilles boivent par leur peau.",
   "Les girafes ont le même nombre de vertèbres cervicales que les humains (sept).",
@@ -573,10 +573,22 @@
   "La préservation du Coran dans sa forme originale depuis plus de 1400 ans est considérée comme un miracle en soi.",
   "Le Coran offre une guidance morale et spirituelle, et ses enseignements ont eu un impact profond sur la vie de millions de personnes à travers les siècles.",
   "La beauté littéraire et les récits narratifs du Coran ont influencé la poésie et la littérature arabes, et ont été une source d'inspiration pour de nombreux écrivains et penseurs.",
   "Les miracles du Coran sont souvent cités comme une preuve de l'authenticité de la religion de l'islam et de la prophétie de Muhammad, paix soit sur lui.",
   "Les miracles du Coran sont considérés comme une manifestation du pouvoir et de la sagesse divines, et sont vus comme des signes de la vérité et de la perfection du message coranique."
 ]
 
-def faits():
-    fact = random.choice(facts)
-    return fact
+faits_utilises = []
+
+def obtenir_fait():
+    global faits_utilises
+
+    if len(faits_utilises) == len(faits):
+        faits_utilises = []
+
+    fait = random.sample(set(faits) - set(faits_utilises), 1)[0]
+    faits_utilises.append(fait)
+    return fait
+
+def reinitialiser_faits_utilises():
+    global faits_utilises
+    faits_utilises = []
```

### Comparing `lesaviezvous-0.2.5/pyproject.toml` & `lesaviezvous-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.2.5/setup.py` & `lesaviezvous-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = ""
 with open('README.md', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name="lesaviezvous",
-    version="0.2.5",
+    version="0.2.6",
     author="Coding Team",
     author_email="codingteam@telegmail.com",
     license='MIT',
     description='Un package Python pour obtenir des informations intéressantes du monde.',
     long_description=render(long_description),
     long_description_content_type="text/markdown",
     url="https://github.com/codingtuto/lesaviezvouspkg/",
```

