# Comparing `tmp/goosepaper-0.6.0.tar.gz` & `tmp/goosepaper-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goosepaper-0.6.0.tar", last modified: Sun Jun  5 20:44:35 2022, max compression
+gzip compressed data, was "goosepaper-0.7.0.tar", last modified: Mon Aug  7 19:02:50 2023, max compression
```

## Comparing `goosepaper-0.6.0.tar` & `goosepaper-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,44 @@
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-06-05 20:44:35.859728 goosepaper-0.6.0/
--rw-r--r--   0 mateljk1   (502) staff       (20)    11345 2022-01-13 14:30:43.000000 goosepaper-0.6.0/LICENSE
--rw-r--r--   0 mateljk1   (502) staff       (20)     7526 2022-06-05 20:44:35.859432 goosepaper-0.6.0/PKG-INFO
--rw-r--r--   0 mateljk1   (502) staff       (20)     6897 2022-06-05 19:56:36.000000 goosepaper-0.6.0/README.md
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-06-05 20:44:35.853257 goosepaper-0.6.0/goosepaper/
--rw-r--r--   0 mateljk1   (502) staff       (20)       66 2022-06-05 20:38:10.000000 goosepaper-0.6.0/goosepaper/__init__.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1985 2022-01-14 18:25:05.000000 goosepaper-0.6.0/goosepaper/__main__.py
--rw-r--r--   0 mateljk1   (502) staff       (20)      684 2022-01-13 15:33:14.000000 goosepaper-0.6.0/goosepaper/auth.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     8848 2022-06-05 20:44:00.000000 goosepaper-0.6.0/goosepaper/goosepaper.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     7670 2022-01-14 18:25:05.000000 goosepaper-0.6.0/goosepaper/multiparser.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1698 2022-01-13 14:30:43.000000 goosepaper-0.6.0/goosepaper/story.py
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-06-05 20:44:35.858899 goosepaper-0.6.0/goosepaper/storyprovider/
--rw-r--r--   0 mateljk1   (502) staff       (20)       48 2022-01-17 14:07:16.000000 goosepaper-0.6.0/goosepaper/storyprovider/__init__.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1599 2022-01-14 16:30:05.000000 goosepaper-0.6.0/goosepaper/storyprovider/reddit.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1840 2022-01-14 16:30:05.000000 goosepaper-0.6.0/goosepaper/storyprovider/rss.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     4189 2022-01-30 15:43:31.000000 goosepaper-0.6.0/goosepaper/storyprovider/storyprovider.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     3685 2022-01-14 16:30:05.000000 goosepaper-0.6.0/goosepaper/storyprovider/twitter.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     4293 2022-06-05 20:38:10.000000 goosepaper-0.6.0/goosepaper/storyprovider/weather.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1304 2022-01-14 16:30:05.000000 goosepaper-0.6.0/goosepaper/storyprovider/wikipedia.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     8404 2022-01-14 18:25:05.000000 goosepaper-0.6.0/goosepaper/styles.py
--rw-r--r--   0 mateljk1   (502) staff       (20)      706 2022-01-14 16:30:05.000000 goosepaper-0.6.0/goosepaper/test_goosepaper.py
--rw-r--r--   0 mateljk1   (502) staff       (20)      953 2022-01-13 15:33:14.000000 goosepaper-0.6.0/goosepaper/test_utils.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     6922 2022-01-13 15:33:14.000000 goosepaper-0.6.0/goosepaper/upload.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     2763 2022-06-05 20:38:10.000000 goosepaper-0.6.0/goosepaper/util.py
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-06-05 20:44:35.855726 goosepaper-0.6.0/goosepaper.egg-info/
--rw-r--r--   0 mateljk1   (502) staff       (20)     7526 2022-06-05 20:44:35.000000 goosepaper-0.6.0/goosepaper.egg-info/PKG-INFO
--rw-r--r--   0 mateljk1   (502) staff       (20)      740 2022-06-05 20:44:35.000000 goosepaper-0.6.0/goosepaper.egg-info/SOURCES.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)       98 2022-06-05 20:44:35.000000 goosepaper-0.6.0/goosepaper.egg-info/dependency_links.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)      105 2022-06-05 20:44:35.000000 goosepaper-0.6.0/goosepaper.egg-info/entry_points.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)       73 2022-06-05 20:44:35.000000 goosepaper-0.6.0/goosepaper.egg-info/requires.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)       11 2022-06-05 20:44:35.000000 goosepaper-0.6.0/goosepaper.egg-info/top_level.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)       38 2022-06-05 20:44:35.859854 goosepaper-0.6.0/setup.cfg
--rw-r--r--   0 mateljk1   (502) staff       (20)     1692 2022-06-05 20:44:12.000000 goosepaper-0.6.0/setup.py
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.281355 goosepaper-0.7.0/
+-rw-r--r--   0 mateljk1   (502) staff       (20)    11345 2022-01-13 14:30:43.000000 goosepaper-0.7.0/LICENSE
+-rw-r--r--   0 mateljk1   (502) staff       (20)       27 2023-04-28 11:49:38.000000 goosepaper-0.7.0/MANIFEST.in
+-rw-r--r--   0 mateljk1   (502) staff       (20)     7603 2023-08-07 19:02:50.280900 goosepaper-0.7.0/PKG-INFO
+-rw-r--r--   0 mateljk1   (502) staff       (20)     7013 2023-08-07 19:02:36.000000 goosepaper-0.7.0/README.md
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.270488 goosepaper-0.7.0/goosepaper/
+-rw-r--r--   0 mateljk1   (502) staff       (20)       66 2023-08-07 19:02:36.000000 goosepaper-0.7.0/goosepaper/__init__.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1985 2022-01-14 18:25:05.000000 goosepaper-0.7.0/goosepaper/__main__.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)      684 2022-01-13 15:33:14.000000 goosepaper-0.7.0/goosepaper/auth.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     8907 2023-04-28 11:49:38.000000 goosepaper-0.7.0/goosepaper/goosepaper.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     7670 2022-01-14 18:25:05.000000 goosepaper-0.7.0/goosepaper/multiparser.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1698 2022-01-13 14:30:43.000000 goosepaper-0.7.0/goosepaper/story.py
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.277403 goosepaper-0.7.0/goosepaper/storyprovider/
+-rw-r--r--   0 mateljk1   (502) staff       (20)       49 2023-04-28 11:49:38.000000 goosepaper-0.7.0/goosepaper/storyprovider/__init__.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1594 2023-08-07 18:53:17.000000 goosepaper-0.7.0/goosepaper/storyprovider/mastodon.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1599 2022-01-14 16:30:05.000000 goosepaper-0.7.0/goosepaper/storyprovider/reddit.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1901 2023-08-07 18:53:17.000000 goosepaper-0.7.0/goosepaper/storyprovider/rss.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     4189 2022-01-30 15:43:31.000000 goosepaper-0.7.0/goosepaper/storyprovider/storyprovider.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)      263 2023-08-07 19:02:36.000000 goosepaper-0.7.0/goosepaper/storyprovider/test_mastodon.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     4341 2022-07-15 19:15:59.000000 goosepaper-0.7.0/goosepaper/storyprovider/weather.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1304 2022-01-14 16:30:05.000000 goosepaper-0.7.0/goosepaper/storyprovider/wikipedia.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     4996 2023-04-28 11:49:38.000000 goosepaper-0.7.0/goosepaper/styles.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)      706 2022-01-14 16:30:05.000000 goosepaper-0.7.0/goosepaper/test_goosepaper.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1413 2023-08-07 19:02:36.000000 goosepaper-0.7.0/goosepaper/test_utils.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     6922 2022-01-13 15:33:14.000000 goosepaper-0.7.0/goosepaper/upload.py
+-rw-r--r--   0 mateljk1   (502) staff       (20)     2756 2023-08-07 19:02:36.000000 goosepaper-0.7.0/goosepaper/util.py
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.273360 goosepaper-0.7.0/goosepaper.egg-info/
+-rw-r--r--   0 mateljk1   (502) staff       (20)     7603 2023-08-07 19:02:50.000000 goosepaper-0.7.0/goosepaper.egg-info/PKG-INFO
+-rw-r--r--   0 mateljk1   (502) staff       (20)      953 2023-08-07 19:02:50.000000 goosepaper-0.7.0/goosepaper.egg-info/SOURCES.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)       32 2023-08-07 19:02:50.000000 goosepaper-0.7.0/goosepaper.egg-info/dependency_links.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)      104 2023-08-07 19:02:50.000000 goosepaper-0.7.0/goosepaper.egg-info/entry_points.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)       66 2023-08-07 19:02:50.000000 goosepaper-0.7.0/goosepaper.egg-info/requires.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)       11 2023-08-07 19:02:50.000000 goosepaper-0.7.0/goosepaper.egg-info/top_level.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)       38 2023-08-07 19:02:50.281483 goosepaper-0.7.0/setup.cfg
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1692 2023-08-07 19:02:36.000000 goosepaper-0.7.0/setup.py
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.261839 goosepaper-0.7.0/styles/
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.277941 goosepaper-0.7.0/styles/Academy/
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1462 2023-04-28 11:49:38.000000 goosepaper-0.7.0/styles/Academy/stylesheet.css
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.278898 goosepaper-0.7.0/styles/Autumn/
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1621 2023-04-28 11:49:38.000000 goosepaper-0.7.0/styles/Autumn/stylesheet.css
+-rw-r--r--   0 mateljk1   (502) staff       (20)      104 2023-04-28 11:49:38.000000 goosepaper-0.7.0/styles/Autumn/stylesheets.txt
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-08-07 19:02:50.280091 goosepaper-0.7.0/styles/FifthAvenue/
+-rw-r--r--   0 mateljk1   (502) staff       (20)     1672 2023-04-28 11:49:38.000000 goosepaper-0.7.0/styles/FifthAvenue/stylesheet.css
+-rw-r--r--   0 mateljk1   (502) staff       (20)      149 2023-04-28 11:49:38.000000 goosepaper-0.7.0/styles/FifthAvenue/stylesheets.txt
```

### Comparing `goosepaper-0.6.0/LICENSE` & `goosepaper-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/PKG-INFO` & `goosepaper-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: goosepaper
-Version: 0.6.0
+Version: 0.7.0
 Summary: Generate and deliver a daily newspaper PDF
-Home-page: UNKNOWN
+Download-URL: https://github.com/j6k4m8/goosepaper/tarball/0.7.0
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
 License: Apache 2.0
-Download-URL: https://github.com/j6k4m8/goosepaper/tarball/0.6.0
 Keywords: remarkable,tablet,pdf,news
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,23 +28,23 @@
   <a href="https://pypi.org/project/goosepaper/"><img alt="PyPI" src="https://img.shields.io/pypi/v/goosepaper?style=for-the-badge"></a>
 </p>
 <p align=center>
   <a href="https://hub.docker.com/repository/docker/j6k4m8/goosepaper"><img alt="Docker Hub Automated Build" src="https://img.shields.io/badge/DockerHub_image-automated-green?style=for-the-badge"></a>
   <a href="https://github.com/j6k4m8/goosepaper/pkgs/container/goosepaper"><img alt="GitHub Container Registry Automated build" src="https://img.shields.io/badge/GHCR.io_image-automated-green?style=for-the-badge"></a>
  </p>
  <p align=center>
-  <a href="https://github.com/j6k4m8/goosepaper/actions?query=workflow%3A%22Python+Tests%22"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/j6k4m8/goosepaper/Python%20Tests?label=GitHub%20Actions&style=for-the-badge"></a>
+  <a href="https://github.com/j6k4m8/goosepaper/actions?query=workflow%3A%22Python+Tests%22"><img alt="GitHub Workflow Status (with branch)" src="https://img.shields.io/github/actions/workflow/status/j6k4m8/goosepaper/python-package.yml?branch=master&style=for-the-badge"></a>
   <a href="https://codecov.io/gh/j6k4m8/goosepaper"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/j6k4m8/goosepaper?logo=codecov&style=for-the-badge"></a>
 </p>
 
 ## what's up
 
 goosepaper is a utility that delivers a daily newspaper to your remarkable tablet. that's cute!
 
-you can include RSS feeds, Twitter feeds, news articles, wikipedia articles-of-the-day, weather, and more. I read it when I wake up so that I can feel anxious without having to get my phone.
+you can include RSS feeds, Mastodon feeds, news articles, wikipedia articles-of-the-day, weather, and more. I read it when I wake up so that I can feel anxious without having to get my phone.
 
 ## survey
 
 **[New!]** In response to feedback, I'm collecting anonymous survey responses. Do you want a goosepaper delivered but without requiring any code? Please [let me know your thoughts!](https://forms.gle/t3PUp2TxDQnzzs8x9)
 
 ## get started with docker
 
@@ -127,15 +125,15 @@
 ---
 
 Check out [this example PDF](https://github.com/j6k4m8/goosepaper/blob/master/docs/Example-Nov-1-2020.pdf), generated on Nov 1 2020.
 
 ## existing story providers ([want to write your own?](https://github.com/j6k4m8/goosepaper/blob/master/CONTRIBUTING.md))
 
 -   [Wikipedia Top News / Current Events](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py)
--   [Tweets](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/twitter.py)
+-   [Mastodon Toots](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/mastodon.py)
 -   [Weather](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/weather.py). These stories appear in the "ear" of the front page, just like a regular ol' newspaper
 -   [RSS Feeds](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py)
 -   [Reddit Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/reddit.py)
 
 # More Questions, Infrequently Asked
 
 ### yes but pardon me — i haven't a remarkable tablet
@@ -150,15 +148,15 @@
 
 ### do all dogs' names start with the letter "B"?
 
 I do not think so, but it is a good question!
 
 ### may i use this to browse twitter?
 
-yes you may! you can add a list of usernames to the feed generator and it will make a print-ready version of twitter. this is helpful for when you are on twitter on your laptop but wish you had Other Twitter as well, in print form.
+~~yes you may! you can add a list of usernames to the feed generator and it will make a print-ready version of twitter. this is helpful for when you are on twitter on your laptop but wish you had Other Twitter as well, in print form.~~
+
+no! twitter has changed and now no one can play nicely with them. sorry! it is sad!
 
 # You May Also Like...
 
 -   [remailable](https://github.com/j6k4m8/remailable): Email PDF documents to your reMarkable tablet
 -   [rmapy fork](https://github.com/j6k4m8/rmapy): My fork of rmapy, with added features and bugfixes
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: goosepaper Version: 0.6.0 Summary: Generate and
-deliver a daily newspaper PDF Home-page: UNKNOWN Author: Jordan Matelsky
-Author-email: opensource@matelsky.com License: Apache 2.0 Download-URL: https:/
-/github.com/j6k4m8/goosepaper/tarball/0.6.0 Keywords:
-remarkable,tablet,pdf,news Platform: UNKNOWN Classifier: Development Status ::
-4 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
-text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: goosepaper Version: 0.7.0 Summary: Generate and
+deliver a daily newspaper PDF Download-URL: https://github.com/j6k4m8/
+goosepaper/tarball/0.7.0 Author: Jordan Matelsky Author-email:
+opensource@matelsky.com License: Apache 2.0 Keywords:
+remarkable,tablet,pdf,news Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+License-File: LICENSE
   [https://raw.githubusercontent.com/j6k4m8/goosepaper/master/docs/goose.svg]
            * a daily newsfeed delivered to your remarkable tablet *
 [https://img.shields.io/github/repo-size/j6k4m8/goosepaper?style=for-the-badge]
   [https://img.shields.io/github/last-commit/j6k4m8/goosepaper?style=for-the-
 badge] [https://img.shields.io/badge/pretty%20dope-%F0%9F%91%8C-blue?style=for-
                                   the-badge]
 [https://img.shields.io/github/license/j6k4m8/goosepaper?style=for-the-badge]
                                     [PyPI]
    [Docker_Hub_Automated_Build] [GitHub_Container_Registry_Automated_build]
-                      [GitHub_Workflow_Status] [Codecov]
+               [GitHub_Workflow_Status_(with_branch)] [Codecov]
 ## what's up goosepaper is a utility that delivers a daily newspaper to your
-remarkable tablet. that's cute! you can include RSS feeds, Twitter feeds, news
+remarkable tablet. that's cute! you can include RSS feeds, Mastodon feeds, news
 articles, wikipedia articles-of-the-day, weather, and more. I read it when I
 wake up so that I can feel anxious without having to get my phone. ## survey **
 [New!]** In response to feedback, I'm collecting anonymous survey responses. Do
 you want a goosepaper delivered but without requiring any code? Please [let me
 know your thoughts!](https://forms.gle/t3PUp2TxDQnzzs8x9) ## get started with
 docker By far the easiest way to get started with Goosepaper is to use Docker.
 ### step 0: write your config file Write a config file to tell Goosepaper what
@@ -55,28 +55,30 @@
 you don't pass an output flag, one will be generated based upon the time of
 generation. You DO need to pass a config file for now. An example config file
 is included here: [example-config.json](example-config.json). --- Check out
 [this example PDF](https://github.com/j6k4m8/goosepaper/blob/master/docs/
 Example-Nov-1-2020.pdf), generated on Nov 1 2020. ## existing story providers (
 [want to write your own?](https://github.com/j6k4m8/goosepaper/blob/master/
 CONTRIBUTING.md)) - [Wikipedia Top News / Current Events](https://github.com/
-j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py) - [Tweets]
-(https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/
-twitter.py) - [Weather](https://github.com/j6k4m8/goosepaper/blob/master/
-goosepaper/storyprovider/weather.py). These stories appear in the "ear" of the
-front page, just like a regular ol' newspaper - [RSS Feeds](https://github.com/
-j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py) - [Reddit
-Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/
-storyprovider/reddit.py) # More Questions, Infrequently Asked ### yes but
-pardon me â i haven't a remarkable tablet Do you have another kind of tablet?
-You may generate a print-ready PDF which you can use on another kind of robot
-as well! Just remove the last line of `main.py`. ### very nice! may i have it
-in comic sans? yes! you may do anything that you find to be fun and welcoming :
-) Check out the `styles.Styles` enum in the goosepaper library. You will find
-there what you seek. ### do all dogs' names start with the letter "B"? I do not
-think so, but it is a good question! ### may i use this to browse twitter? yes
-you may! you can add a list of usernames to the feed generator and it will make
-a print-ready version of twitter. this is helpful for when you are on twitter
-on your laptop but wish you had Other Twitter as well, in print form. # You May
-Also Like... - [remailable](https://github.com/j6k4m8/remailable): Email PDF
-documents to your reMarkable tablet - [rmapy fork](https://github.com/j6k4m8/
-rmapy): My fork of rmapy, with added features and bugfixes
+j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py) -
+[Mastodon Toots](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/
+storyprovider/mastodon.py) - [Weather](https://github.com/j6k4m8/goosepaper/
+blob/master/goosepaper/storyprovider/weather.py). These stories appear in the
+"ear" of the front page, just like a regular ol' newspaper - [RSS Feeds](https:
+//github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py) -
+[Reddit Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/
+goosepaper/storyprovider/reddit.py) # More Questions, Infrequently Asked ###
+yes but pardon me â i haven't a remarkable tablet Do you have another kind of
+tablet? You may generate a print-ready PDF which you can use on another kind of
+robot as well! Just remove the last line of `main.py`. ### very nice! may i
+have it in comic sans? yes! you may do anything that you find to be fun and
+welcoming :) Check out the `styles.Styles` enum in the goosepaper library. You
+will find there what you seek. ### do all dogs' names start with the letter
+"B"? I do not think so, but it is a good question! ### may i use this to browse
+twitter? ~~yes you may! you can add a list of usernames to the feed generator
+and it will make a print-ready version of twitter. this is helpful for when you
+are on twitter on your laptop but wish you had Other Twitter as well, in print
+form.~~ no! twitter has changed and now no one can play nicely with them.
+sorry! it is sad! # You May Also Like... - [remailable](https://github.com/
+j6k4m8/remailable): Email PDF documents to your reMarkable tablet - [rmapy
+fork](https://github.com/j6k4m8/rmapy): My fork of rmapy, with added features
+and bugfixes
```

### Comparing `goosepaper-0.6.0/README.md` & `goosepaper-0.7.0/goosepaper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: goosepaper
+Version: 0.7.0
+Summary: Generate and deliver a daily newspaper PDF
+Download-URL: https://github.com/j6k4m8/goosepaper/tarball/0.7.0
+Author: Jordan Matelsky
+Author-email: opensource@matelsky.com
+License: Apache 2.0
+Keywords: remarkable,tablet,pdf,news
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align=center><img align=center src='https://raw.githubusercontent.com/j6k4m8/goosepaper/master/docs/goose.svg' width=600 /></p>
 <h6 align=center>a daily newsfeed delivered to your remarkable tablet</h6>
 
 <p align=center>
   <a href="https://github.com/j6k4m8/goosepaper/" alt="GitHub repo size"><img src="https://img.shields.io/github/repo-size/j6k4m8/goosepaper?style=for-the-badge" /></a>
   <a href="https://github.com/j6k4m8/goosepaper" alt="GitHub last commit"><img src="https://img.shields.io/github/last-commit/j6k4m8/goosepaper?style=for-the-badge" /></a>
   <a href="https://jordan.matelsky.com" alt="This repo is pretty dope."><img src="https://img.shields.io/badge/pretty%20dope-%F0%9F%91%8C-blue?style=for-the-badge" /></a>
@@ -11,23 +28,23 @@
   <a href="https://pypi.org/project/goosepaper/"><img alt="PyPI" src="https://img.shields.io/pypi/v/goosepaper?style=for-the-badge"></a>
 </p>
 <p align=center>
   <a href="https://hub.docker.com/repository/docker/j6k4m8/goosepaper"><img alt="Docker Hub Automated Build" src="https://img.shields.io/badge/DockerHub_image-automated-green?style=for-the-badge"></a>
   <a href="https://github.com/j6k4m8/goosepaper/pkgs/container/goosepaper"><img alt="GitHub Container Registry Automated build" src="https://img.shields.io/badge/GHCR.io_image-automated-green?style=for-the-badge"></a>
  </p>
  <p align=center>
-  <a href="https://github.com/j6k4m8/goosepaper/actions?query=workflow%3A%22Python+Tests%22"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/j6k4m8/goosepaper/Python%20Tests?label=GitHub%20Actions&style=for-the-badge"></a>
+  <a href="https://github.com/j6k4m8/goosepaper/actions?query=workflow%3A%22Python+Tests%22"><img alt="GitHub Workflow Status (with branch)" src="https://img.shields.io/github/actions/workflow/status/j6k4m8/goosepaper/python-package.yml?branch=master&style=for-the-badge"></a>
   <a href="https://codecov.io/gh/j6k4m8/goosepaper"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/j6k4m8/goosepaper?logo=codecov&style=for-the-badge"></a>
 </p>
 
 ## what's up
 
 goosepaper is a utility that delivers a daily newspaper to your remarkable tablet. that's cute!
 
-you can include RSS feeds, Twitter feeds, news articles, wikipedia articles-of-the-day, weather, and more. I read it when I wake up so that I can feel anxious without having to get my phone.
+you can include RSS feeds, Mastodon feeds, news articles, wikipedia articles-of-the-day, weather, and more. I read it when I wake up so that I can feel anxious without having to get my phone.
 
 ## survey
 
 **[New!]** In response to feedback, I'm collecting anonymous survey responses. Do you want a goosepaper delivered but without requiring any code? Please [let me know your thoughts!](https://forms.gle/t3PUp2TxDQnzzs8x9)
 
 ## get started with docker
 
@@ -108,15 +125,15 @@
 ---
 
 Check out [this example PDF](https://github.com/j6k4m8/goosepaper/blob/master/docs/Example-Nov-1-2020.pdf), generated on Nov 1 2020.
 
 ## existing story providers ([want to write your own?](https://github.com/j6k4m8/goosepaper/blob/master/CONTRIBUTING.md))
 
 -   [Wikipedia Top News / Current Events](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py)
--   [Tweets](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/twitter.py)
+-   [Mastodon Toots](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/mastodon.py)
 -   [Weather](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/weather.py). These stories appear in the "ear" of the front page, just like a regular ol' newspaper
 -   [RSS Feeds](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py)
 -   [Reddit Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/reddit.py)
 
 # More Questions, Infrequently Asked
 
 ### yes but pardon me — i haven't a remarkable tablet
@@ -131,13 +148,15 @@
 
 ### do all dogs' names start with the letter "B"?
 
 I do not think so, but it is a good question!
 
 ### may i use this to browse twitter?
 
-yes you may! you can add a list of usernames to the feed generator and it will make a print-ready version of twitter. this is helpful for when you are on twitter on your laptop but wish you had Other Twitter as well, in print form.
+~~yes you may! you can add a list of usernames to the feed generator and it will make a print-ready version of twitter. this is helpful for when you are on twitter on your laptop but wish you had Other Twitter as well, in print form.~~
+
+no! twitter has changed and now no one can play nicely with them. sorry! it is sad!
 
 # You May Also Like...
 
 -   [remailable](https://github.com/j6k4m8/remailable): Email PDF documents to your reMarkable tablet
 -   [rmapy fork](https://github.com/j6k4m8/rmapy): My fork of rmapy, with added features and bugfixes
```

#### html2text {}

```diff
@@ -1,19 +1,28 @@
+Metadata-Version: 2.1 Name: goosepaper Version: 0.7.0 Summary: Generate and
+deliver a daily newspaper PDF Download-URL: https://github.com/j6k4m8/
+goosepaper/tarball/0.7.0 Author: Jordan Matelsky Author-email:
+opensource@matelsky.com License: Apache 2.0 Keywords:
+remarkable,tablet,pdf,news Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+License-File: LICENSE
   [https://raw.githubusercontent.com/j6k4m8/goosepaper/master/docs/goose.svg]
            * a daily newsfeed delivered to your remarkable tablet *
 [https://img.shields.io/github/repo-size/j6k4m8/goosepaper?style=for-the-badge]
   [https://img.shields.io/github/last-commit/j6k4m8/goosepaper?style=for-the-
 badge] [https://img.shields.io/badge/pretty%20dope-%F0%9F%91%8C-blue?style=for-
                                   the-badge]
 [https://img.shields.io/github/license/j6k4m8/goosepaper?style=for-the-badge]
                                     [PyPI]
    [Docker_Hub_Automated_Build] [GitHub_Container_Registry_Automated_build]
-                      [GitHub_Workflow_Status] [Codecov]
+               [GitHub_Workflow_Status_(with_branch)] [Codecov]
 ## what's up goosepaper is a utility that delivers a daily newspaper to your
-remarkable tablet. that's cute! you can include RSS feeds, Twitter feeds, news
+remarkable tablet. that's cute! you can include RSS feeds, Mastodon feeds, news
 articles, wikipedia articles-of-the-day, weather, and more. I read it when I
 wake up so that I can feel anxious without having to get my phone. ## survey **
 [New!]** In response to feedback, I'm collecting anonymous survey responses. Do
 you want a goosepaper delivered but without requiring any code? Please [let me
 know your thoughts!](https://forms.gle/t3PUp2TxDQnzzs8x9) ## get started with
 docker By far the easiest way to get started with Goosepaper is to use Docker.
 ### step 0: write your config file Write a config file to tell Goosepaper what
@@ -46,28 +55,30 @@
 you don't pass an output flag, one will be generated based upon the time of
 generation. You DO need to pass a config file for now. An example config file
 is included here: [example-config.json](example-config.json). --- Check out
 [this example PDF](https://github.com/j6k4m8/goosepaper/blob/master/docs/
 Example-Nov-1-2020.pdf), generated on Nov 1 2020. ## existing story providers (
 [want to write your own?](https://github.com/j6k4m8/goosepaper/blob/master/
 CONTRIBUTING.md)) - [Wikipedia Top News / Current Events](https://github.com/
-j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py) - [Tweets]
-(https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/
-twitter.py) - [Weather](https://github.com/j6k4m8/goosepaper/blob/master/
-goosepaper/storyprovider/weather.py). These stories appear in the "ear" of the
-front page, just like a regular ol' newspaper - [RSS Feeds](https://github.com/
-j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py) - [Reddit
-Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/
-storyprovider/reddit.py) # More Questions, Infrequently Asked ### yes but
-pardon me â i haven't a remarkable tablet Do you have another kind of tablet?
-You may generate a print-ready PDF which you can use on another kind of robot
-as well! Just remove the last line of `main.py`. ### very nice! may i have it
-in comic sans? yes! you may do anything that you find to be fun and welcoming :
-) Check out the `styles.Styles` enum in the goosepaper library. You will find
-there what you seek. ### do all dogs' names start with the letter "B"? I do not
-think so, but it is a good question! ### may i use this to browse twitter? yes
-you may! you can add a list of usernames to the feed generator and it will make
-a print-ready version of twitter. this is helpful for when you are on twitter
-on your laptop but wish you had Other Twitter as well, in print form. # You May
-Also Like... - [remailable](https://github.com/j6k4m8/remailable): Email PDF
-documents to your reMarkable tablet - [rmapy fork](https://github.com/j6k4m8/
-rmapy): My fork of rmapy, with added features and bugfixes
+j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py) -
+[Mastodon Toots](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/
+storyprovider/mastodon.py) - [Weather](https://github.com/j6k4m8/goosepaper/
+blob/master/goosepaper/storyprovider/weather.py). These stories appear in the
+"ear" of the front page, just like a regular ol' newspaper - [RSS Feeds](https:
+//github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py) -
+[Reddit Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/
+goosepaper/storyprovider/reddit.py) # More Questions, Infrequently Asked ###
+yes but pardon me â i haven't a remarkable tablet Do you have another kind of
+tablet? You may generate a print-ready PDF which you can use on another kind of
+robot as well! Just remove the last line of `main.py`. ### very nice! may i
+have it in comic sans? yes! you may do anything that you find to be fun and
+welcoming :) Check out the `styles.Styles` enum in the goosepaper library. You
+will find there what you seek. ### do all dogs' names start with the letter
+"B"? I do not think so, but it is a good question! ### may i use this to browse
+twitter? ~~yes you may! you can add a list of usernames to the feed generator
+and it will make a print-ready version of twitter. this is helpful for when you
+are on twitter on your laptop but wish you had Other Twitter as well, in print
+form.~~ no! twitter has changed and now no one can play nicely with them.
+sorry! it is sad! # You May Also Like... - [remailable](https://github.com/
+j6k4m8/remailable): Email PDF documents to your reMarkable tablet - [rmapy
+fork](https://github.com/j6k4m8/rmapy): My fork of rmapy, with added features
+and bugfixes
```

### Comparing `goosepaper-0.6.0/goosepaper/__main__.py` & `goosepaper-0.7.0/goosepaper/__main__.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/auth.py` & `goosepaper-0.7.0/goosepaper/auth.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/goosepaper.py` & `goosepaper-0.7.0/goosepaper/goosepaper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
+import pathlib
 from typing import List, Optional, Type, Union
 import datetime
 import io
 import tempfile
 from uuid import uuid4
 
 from goosepaper.story import Story
 
-from .styles import Style, AutumnStyle, FifthAvenueStyle, AcademyStyle
+from .styles import Style
 from .util import PlacementPreference
 from .storyprovider.storyprovider import StoryProvider
 
 
 def _get_style(style):
     if isinstance(style, str):
-        style_obj = {
-            "FifthAvenue": FifthAvenueStyle,
-            "Autumn": AutumnStyle,
-            "Academy": AcademyStyle,
-        }.get(style, FifthAvenueStyle)()
+        style_obj = Style(style)
     else:
         try:
             style_obj = style()
         except Exception as e:
             raise ValueError(f"Invalid style {style}") from e
     return style_obj
 
@@ -144,15 +141,15 @@
             </body>
             </html>
         """
 
     def to_pdf(
         self,
         filename: Union[str, io.BytesIO],
-        style: Union[str, Type[Style]] = FifthAvenueStyle,
+        style: Union[str] = "",
         font_size: int = 14,
     ) -> Optional[str]:
         """
         Renders the current Goosepaper to a PDF file on disk.
 
         Arguments:
             filename: The filename to save the PDF to. If this is an io.BytesIO
@@ -163,24 +160,32 @@
 
         Returns:
             str: The filename of the PDF file. If `filename` is an IO object,
                 then this will return None.
 
         """
         from weasyprint import HTML, CSS
+        from weasyprint.text.fonts import FontConfiguration
 
+        font_config = FontConfiguration()
         style_obj = _get_style(style)
         html = self.to_html()
         h = HTML(string=html)
-        c = CSS(string=style_obj.get_css(font_size))
+        base_url = str(pathlib.Path.cwd())
+        c = CSS(
+            string=style_obj.get_css(font_size),
+            font_config=font_config,
+            base_url=base_url,
+        )
         # Check if the file is a filepath (str):
         if isinstance(filename, str):
             h.write_pdf(
                 filename,
                 stylesheets=[c, *style_obj.get_stylesheets()],
+                font_config=font_config,
             )
             return filename
         elif isinstance(filename, io.BytesIO):
             # Create a tempfile to save the PDF to:
             tf = tempfile.NamedTemporaryFile(suffix=".pdf")
             h.write_pdf(
                 tf,
@@ -191,15 +196,15 @@
             return None
         else:
             raise ValueError(f"Invalid filename {filename}")
 
     def to_epub(
         self,
         filename: Union[str, io.BytesIO],
-        style: Union[str, Type[Style]] = FifthAvenueStyle,
+        style: Union[str, Type[Style]] = "",
         font_size: int = 14,
     ) -> Optional[str]:
         """
         Render the current Goosepaper to an epub file on disk.
 
         Arguments:
             filename: The filename to save the epub to. If `filename` is an
```

### Comparing `goosepaper-0.6.0/goosepaper/multiparser.py` & `goosepaper-0.7.0/goosepaper/multiparser.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/story.py` & `goosepaper-0.7.0/goosepaper/story.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/storyprovider/reddit.py` & `goosepaper-0.7.0/goosepaper/storyprovider/reddit.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/storyprovider/rss.py` & `goosepaper-0.7.0/goosepaper/storyprovider/rss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import requests
 import feedparser
+import urllib.parse
 from typing import List
 from readability import Document
 
 from .storyprovider import StoryProvider
 from ..story import Story
 
 
@@ -32,20 +33,21 @@
         stories = []
         for entry in feed.entries:
             date = datetime.datetime(*entry.updated_parsed[:6])
             if self._since is not None and date < self._since:
                 continue
 
             req = requests.get(entry["link"])
-            source = entry["link"].split(".")[1]
+            # Source is the URL root:
+            source = urllib.parse.urlparse(entry["link"]).netloc
             if not req.ok:
                 # Just return the headline content:
                 story = Story(
                     entry["title"],
-                    body_text=entry["description"] + " ⋮",
+                    body_html=entry["summary"],
                     byline=source,
                     date=date,
                 )
             else:
                 doc = Document(req.content)
                 story = Story(
                     doc.title(),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goosepaper-0.6.0/goosepaper/storyprovider/storyprovider.py` & `goosepaper-0.7.0/goosepaper/storyprovider/storyprovider.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/storyprovider/weather.py` & `goosepaper-0.7.0/goosepaper/storyprovider/weather.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,16 @@
     def get_stories(self, limit: int = 1, **kwargs) -> List[Story]:
         res = requests.get(self._build_url()).json()
         daily = res["daily"]
         todays_high = daily["temperature_2m_max"][0]
         todays_low = daily["temperature_2m_min"][0]
         # todays_precip = daily["precipitation_sum"][0]
         weathercode_string = self._weather_code_to_string(daily["weathercode"][0])
-        headline = f"{todays_high:.1f}ºF/{todays_low:.1f}ºF"
+        unit = "F" if self.F else "C"
+        headline = f"{todays_high:.1f}º{unit}/{todays_low:.1f}º{unit}"
         return [
             Story(
                 headline=headline,
                 body_text=f"{weathercode_string}",
                 placement_preference=PlacementPreference.EAR,
             )
         ]
```

### Comparing `goosepaper-0.6.0/goosepaper/storyprovider/wikipedia.py` & `goosepaper-0.7.0/goosepaper/storyprovider/wikipedia.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/test_goosepaper.py` & `goosepaper-0.7.0/goosepaper/test_goosepaper.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/test_utils.py` & `goosepaper-0.7.0/goosepaper/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,20 +17,38 @@
 def test_clean_text():
     assert clean_text("fooâ€TMbar") == "foo'bar"
 
 
 def test_construct_story_providers_from_config_dict():
     assert construct_story_providers_from_config_dict({}) == []
     stories = construct_story_providers_from_config_dict(
-        {"stories": [{"provider": "twitter", "config": {"usernames": "j6m8"}}]}
+        {
+            "stories": [
+                {
+                    "provider": "mastodon",
+                    "config": {
+                        "server": "https://neuromatch.social",
+                        "username": "j6m8",
+                        "limit": 1,
+                    },
+                }
+            ]
+        }
     )
     assert len(stories) == 1
 
     stories = construct_story_providers_from_config_dict(
         {
             "stories": [
-                {"provider": "twitter", "config": {"usernames": ["j6m8"]}},
+                {
+                    "provider": "mastodon",
+                    "config": {
+                        "server": "https://neuromatch.social",
+                        "username": "j6m8",
+                        "limit": 1,
+                    },
+                },
                 {"provider": "reddit", "config": {"subreddit": "worldnews"}},
             ]
         }
     )
     assert len(stories) == 2
```

### Comparing `goosepaper-0.6.0/goosepaper/upload.py` & `goosepaper-0.7.0/goosepaper/upload.py`

 * *Files identical despite different names*

### Comparing `goosepaper-0.6.0/goosepaper/util.py` & `goosepaper-0.7.0/goosepaper/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,28 +53,27 @@
         raise ValueError(
             "Honk Honk! Syntax Error in config file {0}".format(filepath)
         ) from err
     return config_dict
 
 
 def construct_story_providers_from_config_dict(config: dict):
-
     from goosepaper.storyprovider.rss import RSSFeedStoryProvider
-    from goosepaper.storyprovider.twitter import MultiTwitterStoryProvider
     from goosepaper.storyprovider.reddit import RedditHeadlineStoryProvider
+    from goosepaper.storyprovider.mastodon import MastodonStoryProvider
     from goosepaper.storyprovider.storyprovider import CustomTextStoryProvider
     from goosepaper.storyprovider.weather import OpenMeteoWeatherStoryProvider
     from goosepaper.storyprovider.wikipedia import WikipediaCurrentEventsStoryProvider
 
     StoryProviderConfigNames = {
         "lorem": CustomTextStoryProvider,
         "text": CustomTextStoryProvider,
-        "twitter": MultiTwitterStoryProvider,
         "reddit": RedditHeadlineStoryProvider,
         "weather": OpenMeteoWeatherStoryProvider,
+        "mastodon": MastodonStoryProvider,
         "openmeteo_weather": OpenMeteoWeatherStoryProvider,
         "wikipedia_current_events": WikipediaCurrentEventsStoryProvider,
         "rss": RSSFeedStoryProvider,
     }
 
     if "stories" not in config:
         return []
```

### Comparing `goosepaper-0.6.0/goosepaper.egg-info/PKG-INFO` & `goosepaper-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: goosepaper
-Version: 0.6.0
-Summary: Generate and deliver a daily newspaper PDF
-Home-page: UNKNOWN
-Author: Jordan Matelsky
-Author-email: opensource@matelsky.com
-License: Apache 2.0
-Download-URL: https://github.com/j6k4m8/goosepaper/tarball/0.6.0
-Keywords: remarkable,tablet,pdf,news
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align=center><img align=center src='https://raw.githubusercontent.com/j6k4m8/goosepaper/master/docs/goose.svg' width=600 /></p>
 <h6 align=center>a daily newsfeed delivered to your remarkable tablet</h6>
 
 <p align=center>
   <a href="https://github.com/j6k4m8/goosepaper/" alt="GitHub repo size"><img src="https://img.shields.io/github/repo-size/j6k4m8/goosepaper?style=for-the-badge" /></a>
   <a href="https://github.com/j6k4m8/goosepaper" alt="GitHub last commit"><img src="https://img.shields.io/github/last-commit/j6k4m8/goosepaper?style=for-the-badge" /></a>
   <a href="https://jordan.matelsky.com" alt="This repo is pretty dope."><img src="https://img.shields.io/badge/pretty%20dope-%F0%9F%91%8C-blue?style=for-the-badge" /></a>
@@ -30,23 +11,23 @@
   <a href="https://pypi.org/project/goosepaper/"><img alt="PyPI" src="https://img.shields.io/pypi/v/goosepaper?style=for-the-badge"></a>
 </p>
 <p align=center>
   <a href="https://hub.docker.com/repository/docker/j6k4m8/goosepaper"><img alt="Docker Hub Automated Build" src="https://img.shields.io/badge/DockerHub_image-automated-green?style=for-the-badge"></a>
   <a href="https://github.com/j6k4m8/goosepaper/pkgs/container/goosepaper"><img alt="GitHub Container Registry Automated build" src="https://img.shields.io/badge/GHCR.io_image-automated-green?style=for-the-badge"></a>
  </p>
  <p align=center>
-  <a href="https://github.com/j6k4m8/goosepaper/actions?query=workflow%3A%22Python+Tests%22"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/j6k4m8/goosepaper/Python%20Tests?label=GitHub%20Actions&style=for-the-badge"></a>
+  <a href="https://github.com/j6k4m8/goosepaper/actions?query=workflow%3A%22Python+Tests%22"><img alt="GitHub Workflow Status (with branch)" src="https://img.shields.io/github/actions/workflow/status/j6k4m8/goosepaper/python-package.yml?branch=master&style=for-the-badge"></a>
   <a href="https://codecov.io/gh/j6k4m8/goosepaper"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/j6k4m8/goosepaper?logo=codecov&style=for-the-badge"></a>
 </p>
 
 ## what's up
 
 goosepaper is a utility that delivers a daily newspaper to your remarkable tablet. that's cute!
 
-you can include RSS feeds, Twitter feeds, news articles, wikipedia articles-of-the-day, weather, and more. I read it when I wake up so that I can feel anxious without having to get my phone.
+you can include RSS feeds, Mastodon feeds, news articles, wikipedia articles-of-the-day, weather, and more. I read it when I wake up so that I can feel anxious without having to get my phone.
 
 ## survey
 
 **[New!]** In response to feedback, I'm collecting anonymous survey responses. Do you want a goosepaper delivered but without requiring any code? Please [let me know your thoughts!](https://forms.gle/t3PUp2TxDQnzzs8x9)
 
 ## get started with docker
 
@@ -127,15 +108,15 @@
 ---
 
 Check out [this example PDF](https://github.com/j6k4m8/goosepaper/blob/master/docs/Example-Nov-1-2020.pdf), generated on Nov 1 2020.
 
 ## existing story providers ([want to write your own?](https://github.com/j6k4m8/goosepaper/blob/master/CONTRIBUTING.md))
 
 -   [Wikipedia Top News / Current Events](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py)
--   [Tweets](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/twitter.py)
+-   [Mastodon Toots](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/mastodon.py)
 -   [Weather](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/weather.py). These stories appear in the "ear" of the front page, just like a regular ol' newspaper
 -   [RSS Feeds](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py)
 -   [Reddit Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/reddit.py)
 
 # More Questions, Infrequently Asked
 
 ### yes but pardon me — i haven't a remarkable tablet
@@ -150,15 +131,15 @@
 
 ### do all dogs' names start with the letter "B"?
 
 I do not think so, but it is a good question!
 
 ### may i use this to browse twitter?
 
-yes you may! you can add a list of usernames to the feed generator and it will make a print-ready version of twitter. this is helpful for when you are on twitter on your laptop but wish you had Other Twitter as well, in print form.
+~~yes you may! you can add a list of usernames to the feed generator and it will make a print-ready version of twitter. this is helpful for when you are on twitter on your laptop but wish you had Other Twitter as well, in print form.~~
+
+no! twitter has changed and now no one can play nicely with them. sorry! it is sad!
 
 # You May Also Like...
 
 -   [remailable](https://github.com/j6k4m8/remailable): Email PDF documents to your reMarkable tablet
 -   [rmapy fork](https://github.com/j6k4m8/rmapy): My fork of rmapy, with added features and bugfixes
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,19 @@
-Metadata-Version: 2.1 Name: goosepaper Version: 0.6.0 Summary: Generate and
-deliver a daily newspaper PDF Home-page: UNKNOWN Author: Jordan Matelsky
-Author-email: opensource@matelsky.com License: Apache 2.0 Download-URL: https:/
-/github.com/j6k4m8/goosepaper/tarball/0.6.0 Keywords:
-remarkable,tablet,pdf,news Platform: UNKNOWN Classifier: Development Status ::
-4 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
-text/markdown License-File: LICENSE
   [https://raw.githubusercontent.com/j6k4m8/goosepaper/master/docs/goose.svg]
            * a daily newsfeed delivered to your remarkable tablet *
 [https://img.shields.io/github/repo-size/j6k4m8/goosepaper?style=for-the-badge]
   [https://img.shields.io/github/last-commit/j6k4m8/goosepaper?style=for-the-
 badge] [https://img.shields.io/badge/pretty%20dope-%F0%9F%91%8C-blue?style=for-
                                   the-badge]
 [https://img.shields.io/github/license/j6k4m8/goosepaper?style=for-the-badge]
                                     [PyPI]
    [Docker_Hub_Automated_Build] [GitHub_Container_Registry_Automated_build]
-                      [GitHub_Workflow_Status] [Codecov]
+               [GitHub_Workflow_Status_(with_branch)] [Codecov]
 ## what's up goosepaper is a utility that delivers a daily newspaper to your
-remarkable tablet. that's cute! you can include RSS feeds, Twitter feeds, news
+remarkable tablet. that's cute! you can include RSS feeds, Mastodon feeds, news
 articles, wikipedia articles-of-the-day, weather, and more. I read it when I
 wake up so that I can feel anxious without having to get my phone. ## survey **
 [New!]** In response to feedback, I'm collecting anonymous survey responses. Do
 you want a goosepaper delivered but without requiring any code? Please [let me
 know your thoughts!](https://forms.gle/t3PUp2TxDQnzzs8x9) ## get started with
 docker By far the easiest way to get started with Goosepaper is to use Docker.
 ### step 0: write your config file Write a config file to tell Goosepaper what
@@ -55,28 +46,30 @@
 you don't pass an output flag, one will be generated based upon the time of
 generation. You DO need to pass a config file for now. An example config file
 is included here: [example-config.json](example-config.json). --- Check out
 [this example PDF](https://github.com/j6k4m8/goosepaper/blob/master/docs/
 Example-Nov-1-2020.pdf), generated on Nov 1 2020. ## existing story providers (
 [want to write your own?](https://github.com/j6k4m8/goosepaper/blob/master/
 CONTRIBUTING.md)) - [Wikipedia Top News / Current Events](https://github.com/
-j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py) - [Tweets]
-(https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/
-twitter.py) - [Weather](https://github.com/j6k4m8/goosepaper/blob/master/
-goosepaper/storyprovider/weather.py). These stories appear in the "ear" of the
-front page, just like a regular ol' newspaper - [RSS Feeds](https://github.com/
-j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py) - [Reddit
-Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/
-storyprovider/reddit.py) # More Questions, Infrequently Asked ### yes but
-pardon me â i haven't a remarkable tablet Do you have another kind of tablet?
-You may generate a print-ready PDF which you can use on another kind of robot
-as well! Just remove the last line of `main.py`. ### very nice! may i have it
-in comic sans? yes! you may do anything that you find to be fun and welcoming :
-) Check out the `styles.Styles` enum in the goosepaper library. You will find
-there what you seek. ### do all dogs' names start with the letter "B"? I do not
-think so, but it is a good question! ### may i use this to browse twitter? yes
-you may! you can add a list of usernames to the feed generator and it will make
-a print-ready version of twitter. this is helpful for when you are on twitter
-on your laptop but wish you had Other Twitter as well, in print form. # You May
-Also Like... - [remailable](https://github.com/j6k4m8/remailable): Email PDF
-documents to your reMarkable tablet - [rmapy fork](https://github.com/j6k4m8/
-rmapy): My fork of rmapy, with added features and bugfixes
+j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/wikipedia.py) -
+[Mastodon Toots](https://github.com/j6k4m8/goosepaper/blob/master/goosepaper/
+storyprovider/mastodon.py) - [Weather](https://github.com/j6k4m8/goosepaper/
+blob/master/goosepaper/storyprovider/weather.py). These stories appear in the
+"ear" of the front page, just like a regular ol' newspaper - [RSS Feeds](https:
+//github.com/j6k4m8/goosepaper/blob/master/goosepaper/storyprovider/rss.py) -
+[Reddit Subreddits](https://github.com/j6k4m8/goosepaper/blob/master/
+goosepaper/storyprovider/reddit.py) # More Questions, Infrequently Asked ###
+yes but pardon me â i haven't a remarkable tablet Do you have another kind of
+tablet? You may generate a print-ready PDF which you can use on another kind of
+robot as well! Just remove the last line of `main.py`. ### very nice! may i
+have it in comic sans? yes! you may do anything that you find to be fun and
+welcoming :) Check out the `styles.Styles` enum in the goosepaper library. You
+will find there what you seek. ### do all dogs' names start with the letter
+"B"? I do not think so, but it is a good question! ### may i use this to browse
+twitter? ~~yes you may! you can add a list of usernames to the feed generator
+and it will make a print-ready version of twitter. this is helpful for when you
+are on twitter on your laptop but wish you had Other Twitter as well, in print
+form.~~ no! twitter has changed and now no one can play nicely with them.
+sorry! it is sad! # You May Also Like... - [remailable](https://github.com/
+j6k4m8/remailable): Email PDF documents to your reMarkable tablet - [rmapy
+fork](https://github.com/j6k4m8/rmapy): My fork of rmapy, with added features
+and bugfixes
```

### Comparing `goosepaper-0.6.0/goosepaper.egg-info/SOURCES.txt` & `goosepaper-0.7.0/goosepaper.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 goosepaper/__init__.py
 goosepaper/__main__.py
 goosepaper/auth.py
 goosepaper/goosepaper.py
 goosepaper/multiparser.py
@@ -15,13 +16,19 @@
 goosepaper.egg-info/PKG-INFO
 goosepaper.egg-info/SOURCES.txt
 goosepaper.egg-info/dependency_links.txt
 goosepaper.egg-info/entry_points.txt
 goosepaper.egg-info/requires.txt
 goosepaper.egg-info/top_level.txt
 goosepaper/storyprovider/__init__.py
+goosepaper/storyprovider/mastodon.py
 goosepaper/storyprovider/reddit.py
 goosepaper/storyprovider/rss.py
 goosepaper/storyprovider/storyprovider.py
-goosepaper/storyprovider/twitter.py
+goosepaper/storyprovider/test_mastodon.py
 goosepaper/storyprovider/weather.py
-goosepaper/storyprovider/wikipedia.py
+goosepaper/storyprovider/wikipedia.py
+styles/Academy/stylesheet.css
+styles/Autumn/stylesheet.css
+styles/Autumn/stylesheets.txt
+styles/FifthAvenue/stylesheet.css
+styles/FifthAvenue/stylesheets.txt
```

### Comparing `goosepaper-0.6.0/setup.py` & `goosepaper-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from os import path
 from codecs import open as copen
 from setuptools import setup, find_packages
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with copen(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
```

