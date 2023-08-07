# Comparing `tmp/invision-client-python-1.0.0.tar.gz` & `tmp/invision-client-python-1.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\invision-client-python-1.0.0.tar", last modified: Fri Jun 30 06:26:36 2023, max compression
+gzip compressed data, was "dist\invision-client-python-1.3.0b1.tar", last modified: Fri Jul 21 07:23:29 2023, max compression
```

## Comparing `invision-client-python-1.0.0.tar` & `invision-client-python-1.3.0b1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.797125 invision-client-python-1.0.0/
--rw-rw-rw-   0        0        0      453 2023-06-30 06:26:36.797125 invision-client-python-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4137 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.613161 invision-client-python-1.0.0/invision_client/
--rw-rw-rw-   0        0        0      789 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.630158 invision-client-python-1.0.0/invision_client/api/
--rw-rw-rw-   0        0        0      218 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/api/__init__.py
--rw-rw-rw-   0        0        0     6497 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/api/forums_api.py
--rw-rw-rw-   0        0        0     8552 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/api/members_api.py
--rw-rw-rw-   0        0        0    10824 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/api/topics_api.py
--rw-rw-rw-   0        0        0    39127 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/api_client.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.635161 invision-client-python-1.0.0/invision_client/apis/
--rw-rw-rw-   0        0        0      587 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/apis/__init__.py
--rw-rw-rw-   0        0        0    16285 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/configuration.py
--rw-rw-rw-   0        0        0     5113 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/exceptions.py
--rw-rw-rw-   0        0        0     1895 2023-06-27 10:05:59.000000 invision-client-python-1.0.0/invision_client/invision_api.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.700129 invision-client-python-1.0.0/invision_client/model/
--rw-rw-rw-   0        0        0      349 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/model/__init__.py
--rw-rw-rw-   0        0        0    12468 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/core_members_get200_response.py
--rw-rw-rw-   0        0        0    11603 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/field.py
--rw-rw-rw-   0        0        0    11780 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/fieldgroup.py
--rw-rw-rw-   0        0        0    12891 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/forum.py
--rw-rw-rw-   0        0        0    12464 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/forums_forums_get200_response.py
--rw-rw-rw-   0        0        0    11815 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/group.py
--rw-rw-rw-   0        0        0    17662 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/member.py
--rw-rw-rw-   0        0        0    12985 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/poll.py
--rw-rw-rw-   0        0        0    13085 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/post.py
--rw-rw-rw-   0        0        0    12202 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/post_reactions_inner.py
--rw-rw-rw-   0        0        0    11813 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/question.py
--rw-rw-rw-   0        0        0    11946 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/rank.py
--rw-rw-rw-   0        0        0    14972 2023-06-27 10:02:37.000000 invision-client-python-1.0.0/invision_client/model/topic.py
--rw-rw-rw-   0        0        0    82641 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/model_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.707126 invision-client-python-1.0.0/invision_client/models/
--rw-rw-rw-   0        0        0     1103 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/models/__init__.py
--rw-rw-rw-   0        0        0    14318 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/invision_client/rest.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.725125 invision-client-python-1.0.0/invision_client_python.egg-info/
--rw-rw-rw-   0        0        0      453 2023-06-30 06:26:36.000000 invision-client-python-1.0.0/invision_client_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1585 2023-06-30 06:26:36.000000 invision-client-python-1.0.0/invision_client_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 06:26:36.000000 invision-client-python-1.0.0/invision_client_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-30 06:26:36.000000 invision-client-python-1.0.0/invision_client_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-30 06:26:36.000000 invision-client-python-1.0.0/invision_client_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       76 2023-06-30 06:26:36.799127 invision-client-python-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1133 2023-06-27 10:02:38.000000 invision-client-python-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:26:36.793126 invision-client-python-1.0.0/test/
--rw-rw-rw-   0        0        0      960 2023-06-27 08:17:01.000000 invision-client-python-1.0.0/test/test_core_members_get200_response.py
--rw-rw-rw-   0        0        0     2184 2023-06-30 06:15:18.000000 invision-client-python-1.0.0/test/test_custom_api.py
--rw-rw-rw-   0        0        0      740 2023-06-27 08:17:01.000000 invision-client-python-1.0.0/test/test_field.py
--rw-rw-rw-   0        0        0      848 2023-06-27 08:17:01.000000 invision-client-python-1.0.0/test/test_fieldgroup.py
--rw-rw-rw-   0        0        0      740 2023-06-27 08:17:01.000000 invision-client-python-1.0.0/test/test_forum.py
--rw-rw-rw-   0        0        0      755 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_forums_api.py
--rw-rw-rw-   0        0        0      963 2023-06-27 08:17:01.000000 invision-client-python-1.0.0/test/test_forums_forums_get200_response.py
--rw-rw-rw-   0        0        0      740 2023-06-27 08:17:01.000000 invision-client-python-1.0.0/test/test_group.py
--rw-rw-rw-   0        0        0      982 2023-06-27 08:17:01.000000 invision-client-python-1.0.0/test/test_member.py
--rw-rw-rw-   0        0        0      759 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_members_api.py
--rw-rw-rw-   0        0        0      818 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_poll.py
--rw-rw-rw-   0        0        0      937 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_post.py
--rw-rw-rw-   0        0        0      833 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_post_reactions_inner.py
--rw-rw-rw-   0        0        0      761 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_question.py
--rw-rw-rw-   0        0        0      733 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_rank.py
--rw-rw-rw-   0        0        0      951 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_topic.py
--rw-rw-rw-   0        0        0      753 2023-06-27 08:17:02.000000 invision-client-python-1.0.0/test/test_topics_api.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:29.055587 invision-client-python-1.3.0b1/
+-rw-rw-rw-   0        0        0      455 2023-07-21 07:23:29.056586 invision-client-python-1.3.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:28.921587 invision-client-python-1.3.0b1/invision_client/
+-rw-rw-rw-   0        0        0      816 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:28.934587 invision-client-python-1.3.0b1/invision_client/api/
+-rw-rw-rw-   0        0        0      221 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/api/__init__.py
+-rw-rw-rw-   0        0        0     6679 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/api/forums_api.py
+-rw-rw-rw-   0        0        0     8783 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/api/members_api.py
+-rw-rw-rw-   0        0        0    11113 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/api/topics_api.py
+-rw-rw-rw-   0        0        0    40023 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:28.938587 invision-client-python-1.3.0b1/invision_client/apis/
+-rw-rw-rw-   0        0        0      606 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/apis/__init__.py
+-rw-rw-rw-   0        0        0    16731 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/configuration.py
+-rw-rw-rw-   0        0        0     5271 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/exceptions.py
+-rw-rw-rw-   0        0        0     1895 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/invision_api.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:28.985587 invision-client-python-1.3.0b1/invision_client/model/
+-rw-rw-rw-   0        0        0      354 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/__init__.py
+-rw-rw-rw-   0        0        0    12753 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/core_members_get200_response.py
+-rw-rw-rw-   0        0        0    11870 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/field.py
+-rw-rw-rw-   0        0        0    12053 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/fieldgroup.py
+-rw-rw-rw-   0        0        0    13182 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/forum.py
+-rw-rw-rw-   0        0        0    12749 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/forums_forums_get200_response.py
+-rw-rw-rw-   0        0        0    12086 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/group.py
+-rw-rw-rw-   0        0        0    18043 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/member.py
+-rw-rw-rw-   0        0        0    13282 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/poll.py
+-rw-rw-rw-   0        0        0    13384 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/post.py
+-rw-rw-rw-   0        0        0    12481 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/post_reactions_inner.py
+-rw-rw-rw-   0        0        0    12080 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/question.py
+-rw-rw-rw-   0        0        0    12221 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/rank.py
+-rw-rw-rw-   0        0        0    15313 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model/topic.py
+-rw-rw-rw-   0        0        0    84699 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/model_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:28.988587 invision-client-python-1.3.0b1/invision_client/models/
+-rw-rw-rw-   0        0        0     1127 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/models/__init__.py
+-rw-rw-rw-   0        0        0    14670 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/invision_client/rest.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:29.002587 invision-client-python-1.3.0b1/invision_client_python.egg-info/
+-rw-rw-rw-   0        0        0      455 2023-07-21 07:23:28.000000 invision-client-python-1.3.0b1/invision_client_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1585 2023-07-21 07:23:28.000000 invision-client-python-1.3.0b1/invision_client_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 07:23:28.000000 invision-client-python-1.3.0b1/invision_client_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-21 07:23:28.000000 invision-client-python-1.3.0b1/invision_client_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 07:23:28.000000 invision-client-python-1.3.0b1/invision_client_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       76 2023-07-21 07:23:29.058587 invision-client-python-1.3.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-07-21 07:22:48.000000 invision-client-python-1.3.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:23:29.053587 invision-client-python-1.3.0b1/test/
+-rw-rw-rw-   0        0        0      997 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_core_members_get200_response.py
+-rw-rw-rw-   0        0        0     2184 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_custom_api.py
+-rw-rw-rw-   0        0        0      775 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_field.py
+-rw-rw-rw-   0        0        0      885 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_fieldgroup.py
+-rw-rw-rw-   0        0        0      775 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_forum.py
+-rw-rw-rw-   0        0        0      790 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_forums_api.py
+-rw-rw-rw-   0        0        0     1000 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_forums_forums_get200_response.py
+-rw-rw-rw-   0        0        0      775 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_group.py
+-rw-rw-rw-   0        0        0     1023 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_member.py
+-rw-rw-rw-   0        0        0      794 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_members_api.py
+-rw-rw-rw-   0        0        0      855 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_poll.py
+-rw-rw-rw-   0        0        0      976 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_post.py
+-rw-rw-rw-   0        0        0      868 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_post_reactions_inner.py
+-rw-rw-rw-   0        0        0      796 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_question.py
+-rw-rw-rw-   0        0        0      768 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_rank.py
+-rw-rw-rw-   0        0        0      992 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_topic.py
+-rw-rw-rw-   0        0        0      788 2023-07-12 11:22:11.000000 invision-client-python-1.3.0b1/test/test_topics_api.py
```

### Comparing `invision-client-python-1.0.0/README.md` & `invision-client-python-1.3.0b1/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# invision-client-python
-No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
-
-This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
-
-- API version: 1.0.0
-- Package version: 1.0.0
-- Build package: org.openapitools.codegen.languages.PythonClientCodegen
-
-## Requirements.
-
-Python >=3.6
-
-## Installation & Usage
-### pip install
-
-If the python package is hosted on a repository, you can install directly using:
-
-```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
-```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-```python
-import invision_client
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
-```sh
-python setup.py install --user
-```
-(or `sudo python setup.py install` to install the package for all users)
-
-Then import the package:
-```python
-import invision_client
-```
-
-## Getting Started
-
-Please follow the [installation procedure](#installation--usage) and then run the following:
-
-```python
-
-import time
-import invision_client
-from pprint import pprint
-from invision_client.api import forums_api
-from invision_client.model.forums_forums_get200_response import ForumsForumsGet200Response
-# Defining the host is optional and defaults to https://tech.forums.silabs.net/api
-# See configuration.py for a list of all supported configuration parameters.
-configuration = invision_client.Configuration(
-    host = "https://tech.forums.silabs.net/api"
-)
-
-
-
-# Enter a context with an instance of the API client
-with invision_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = forums_api.ForumsApi(api_client)
-    clubs = 1 # int | Include club forums (optional) (default to 1)
-    page = 1 # int | Page number (optional)
-    per_page = 25 # int | Number of results per page (optional) (default to 25)
-
-    try:
-        # Get list of forums
-        api_response = api_instance.forums_forums_get(clubs=clubs, page=page, per_page=per_page)
-        pprint(api_response)
-    except invision_client.ApiException as e:
-        print("Exception when calling ForumsApi->forums_forums_get: %s\n" % e)
-```
-
-## Documentation for API Endpoints
-
-All URIs are relative to *https://tech.forums.silabs.net/api*
-
-Class | Method | HTTP request | Description
------------- | ------------- | ------------- | -------------
-*ForumsApi* | [**forums_forums_get**](docs/ForumsApi.md#forums_forums_get) | **GET** /forums/forums | Get list of forums
-*MembersApi* | [**core_members_get**](docs/MembersApi.md#core_members_get) | **GET** /core/members | Get list of members
-*TopicsApi* | [**forums_topics_post**](docs/TopicsApi.md#forums_topics_post) | **POST** /forums/topics | Create a topic
-
-
-## Documentation For Models
-
- - [CoreMembersGet200Response](docs/CoreMembersGet200Response.md)
- - [Field](docs/Field.md)
- - [Fieldgroup](docs/Fieldgroup.md)
- - [Forum](docs/Forum.md)
- - [ForumsForumsGet200Response](docs/ForumsForumsGet200Response.md)
- - [Group](docs/Group.md)
- - [Member](docs/Member.md)
- - [Poll](docs/Poll.md)
- - [Post](docs/Post.md)
- - [PostReactionsInner](docs/PostReactionsInner.md)
- - [Question](docs/Question.md)
- - [Rank](docs/Rank.md)
- - [Topic](docs/Topic.md)
-
-
-## Documentation For Authorization
-
- All endpoints do not require authorization.
-
-## Author
-
-
-
-
-## Notes for Large OpenAPI documents
-If the OpenAPI document is large, imports in invision_client.apis and invision_client.models may fail with a
-RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
-
-Solution 1:
-Use specific imports for apis and models like:
-- `from invision_client.api.default_api import DefaultApi`
-- `from invision_client.model.pet import Pet`
-
-Solution 2:
-Before importing the package, adjust the maximum recursion limit as shown below:
-```
-import sys
-sys.setrecursionlimit(1500)
-import invision_client
-from invision_client.apis import *
-from invision_client.models import *
-```
-
+# invision-client-python
+No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
+
+- API version: 1.0.0
+- Package version: 1.0.0
+- Build package: org.openapitools.codegen.languages.PythonClientCodegen
+
+## Requirements.
+
+Python >=3.6
+
+## Installation & Usage
+### pip install
+
+If the python package is hosted on a repository, you can install directly using:
+
+```sh
+pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+```
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
+
+Then import the package:
+```python
+import invision_client
+```
+
+### Setuptools
+
+Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
+
+```sh
+python setup.py install --user
+```
+(or `sudo python setup.py install` to install the package for all users)
+
+Then import the package:
+```python
+import invision_client
+```
+
+## Getting Started
+
+Please follow the [installation procedure](#installation--usage) and then run the following:
+
+```python
+
+import time
+import invision_client
+from pprint import pprint
+from invision_client.api import forums_api
+from invision_client.model.forums_forums_get200_response import ForumsForumsGet200Response
+# Defining the host is optional and defaults to https://tech.forums.silabs.net/api
+# See configuration.py for a list of all supported configuration parameters.
+configuration = invision_client.Configuration(
+    host = "https://tech.forums.silabs.net/api"
+)
+
+
+
+# Enter a context with an instance of the API client
+with invision_client.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = forums_api.ForumsApi(api_client)
+    clubs = 1 # int | Include club forums (optional) (default to 1)
+    page = 1 # int | Page number (optional)
+    per_page = 25 # int | Number of results per page (optional) (default to 25)
+
+    try:
+        # Get list of forums
+        api_response = api_instance.forums_forums_get(clubs=clubs, page=page, per_page=per_page)
+        pprint(api_response)
+    except invision_client.ApiException as e:
+        print("Exception when calling ForumsApi->forums_forums_get: %s\n" % e)
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *https://tech.forums.silabs.net/api*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*ForumsApi* | [**forums_forums_get**](docs/ForumsApi.md#forums_forums_get) | **GET** /forums/forums | Get list of forums
+*MembersApi* | [**core_members_get**](docs/MembersApi.md#core_members_get) | **GET** /core/members | Get list of members
+*TopicsApi* | [**forums_topics_post**](docs/TopicsApi.md#forums_topics_post) | **POST** /forums/topics | Create a topic
+
+
+## Documentation For Models
+
+ - [CoreMembersGet200Response](docs/CoreMembersGet200Response.md)
+ - [Field](docs/Field.md)
+ - [Fieldgroup](docs/Fieldgroup.md)
+ - [Forum](docs/Forum.md)
+ - [ForumsForumsGet200Response](docs/ForumsForumsGet200Response.md)
+ - [Group](docs/Group.md)
+ - [Member](docs/Member.md)
+ - [Poll](docs/Poll.md)
+ - [Post](docs/Post.md)
+ - [PostReactionsInner](docs/PostReactionsInner.md)
+ - [Question](docs/Question.md)
+ - [Rank](docs/Rank.md)
+ - [Topic](docs/Topic.md)
+
+
+## Documentation For Authorization
+
+ All endpoints do not require authorization.
+
+## Author
+
+
+
+
+## Notes for Large OpenAPI documents
+If the OpenAPI document is large, imports in invision_client.apis and invision_client.models may fail with a
+RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
+
+Solution 1:
+Use specific imports for apis and models like:
+- `from invision_client.api.default_api import DefaultApi`
+- `from invision_client.model.pet import Pet`
+
+Solution 2:
+Before importing the package, adjust the maximum recursion limit as shown below:
+```
+import sys
+sys.setrecursionlimit(1500)
+import invision_client
+from invision_client.apis import *
+from invision_client.models import *
+```
+
```

### Comparing `invision-client-python-1.0.0/invision_client/__init__.py` & `invision-client-python-1.3.0b1/invision_client/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# flake8: noqa
-
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-__version__ = "1.0.0"
-
-# import ApiClient
-from invision_client.api_client import ApiClient
-
-# import Configuration
-from invision_client.configuration import Configuration
-
-# import exceptions
-from invision_client.exceptions import OpenApiException
-from invision_client.exceptions import ApiAttributeError
-from invision_client.exceptions import ApiTypeError
-from invision_client.exceptions import ApiValueError
-from invision_client.exceptions import ApiKeyError
-from invision_client.exceptions import ApiException
+# flake8: noqa
+
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+__version__ = "1.0.0"
+
+# import ApiClient
+from invision_client.api_client import ApiClient
+
+# import Configuration
+from invision_client.configuration import Configuration
+
+# import exceptions
+from invision_client.exceptions import OpenApiException
+from invision_client.exceptions import ApiAttributeError
+from invision_client.exceptions import ApiTypeError
+from invision_client.exceptions import ApiValueError
+from invision_client.exceptions import ApiKeyError
+from invision_client.exceptions import ApiException
```

### Comparing `invision-client-python-1.0.0/invision_client/api/forums_api.py` & `invision-client-python-1.3.0b1/invision_client/api/forums_api.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.api_client import ApiClient, Endpoint as _Endpoint
-from invision_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
-)
-from invision_client.model.forums_forums_get200_response import ForumsForumsGet200Response
-
-
-class ForumsApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.forums_forums_get_endpoint = _Endpoint(
-            settings={
-                'response_type': (ForumsForumsGet200Response,),
-                'auth': [],
-                'endpoint_path': '/forums/forums',
-                'operation_id': 'forums_forums_get',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'clubs',
-                    'page',
-                    'per_page',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                    'clubs',
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                    ('clubs',): {
-
-                        "0": 0,
-                        "1": 1
-                    },
-                },
-                'openapi_types': {
-                    'clubs':
-                        (int,),
-                    'page':
-                        (int,),
-                    'per_page':
-                        (int,),
-                },
-                'attribute_map': {
-                    'clubs': 'clubs',
-                    'page': 'page',
-                    'per_page': 'perPage',
-                },
-                'location_map': {
-                    'clubs': 'query',
-                    'page': 'query',
-                    'per_page': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    '*/*'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-
-    def forums_forums_get(
-        self,
-        **kwargs
-    ):
-        """Get list of forums  # noqa: E501
-
-        Retrieves a list of forums  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.forums_forums_get(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            clubs (int): Include club forums. [optional] if omitted the server will use the default value of 1
-            page (int): Page number. [optional]
-            per_page (int): Number of results per page. [optional] if omitted the server will use the default value of 25
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            ForumsForumsGet200Response
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.forums_forums_get_endpoint.call_with_http_info(**kwargs)
-
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.api_client import ApiClient, Endpoint as _Endpoint
+from invision_client.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
+)
+from invision_client.model.forums_forums_get200_response import ForumsForumsGet200Response
+
+
+class ForumsApi(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None):
+        if api_client is None:
+            api_client = ApiClient()
+        self.api_client = api_client
+        self.forums_forums_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ForumsForumsGet200Response,),
+                'auth': [],
+                'endpoint_path': '/forums/forums',
+                'operation_id': 'forums_forums_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'clubs',
+                    'page',
+                    'per_page',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                    'clubs',
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                    ('clubs',): {
+
+                        "0": 0,
+                        "1": 1
+                    },
+                },
+                'openapi_types': {
+                    'clubs':
+                        (int,),
+                    'page':
+                        (int,),
+                    'per_page':
+                        (int,),
+                },
+                'attribute_map': {
+                    'clubs': 'clubs',
+                    'page': 'page',
+                    'per_page': 'perPage',
+                },
+                'location_map': {
+                    'clubs': 'query',
+                    'page': 'query',
+                    'per_page': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    '*/*'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+    def forums_forums_get(
+        self,
+        **kwargs
+    ):
+        """Get list of forums  # noqa: E501
+
+        Retrieves a list of forums  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.forums_forums_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            clubs (int): Include club forums. [optional] if omitted the server will use the default value of 1
+            page (int): Page number. [optional]
+            per_page (int): Number of results per page. [optional] if omitted the server will use the default value of 25
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ForumsForumsGet200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.forums_forums_get_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `invision-client-python-1.0.0/invision_client/api/members_api.py` & `invision-client-python-1.3.0b1/invision_client/api/members_api.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.api_client import ApiClient, Endpoint as _Endpoint
-from invision_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
-)
-from invision_client.model.core_members_get200_response import CoreMembersGet200Response
-
-
-class MembersApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.core_members_get_endpoint = _Endpoint(
-            settings={
-                'response_type': (CoreMembersGet200Response,),
-                'auth': [],
-                'endpoint_path': '/core/members',
-                'operation_id': 'core_members_get',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'ids',
-                    'sort_by',
-                    'sort_dir',
-                    'name',
-                    'email',
-                    'group',
-                    'activity_after',
-                    'activity_before',
-                    'page',
-                    'per_page',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                    'sort_by',
-                    'sort_dir',
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                    ('sort_by',): {
-
-                        "JOINED": "joined",
-                        "NAME": "name",
-                        "LAST_ACTIVITY": "last_activity"
-                    },
-                    ('sort_dir',): {
-
-                        "ASC": "asc",
-                        "DESC": "desc"
-                    },
-                },
-                'openapi_types': {
-                    'ids':
-                        (str,),
-                    'sort_by':
-                        (str,),
-                    'sort_dir':
-                        (str,),
-                    'name':
-                        (str,),
-                    'email':
-                        (str,),
-                    'group':
-                        (str,),
-                    'activity_after':
-                        (int,),
-                    'activity_before':
-                        (int,),
-                    'page':
-                        (int,),
-                    'per_page':
-                        (int,),
-                },
-                'attribute_map': {
-                    'ids': 'ids',
-                    'sort_by': 'sortBy',
-                    'sort_dir': 'sortDir',
-                    'name': 'name',
-                    'email': 'email',
-                    'group': 'group',
-                    'activity_after': 'activity_after',
-                    'activity_before': 'activity_before',
-                    'page': 'page',
-                    'per_page': 'perPage',
-                },
-                'location_map': {
-                    'ids': 'query',
-                    'sort_by': 'query',
-                    'sort_dir': 'query',
-                    'name': 'query',
-                    'email': 'query',
-                    'group': 'query',
-                    'activity_after': 'query',
-                    'activity_before': 'query',
-                    'page': 'query',
-                    'per_page': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    '*/*'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-
-    def core_members_get(
-        self,
-        **kwargs
-    ):
-        """Get list of members  # noqa: E501
-
-        Retrieves a list of members  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.core_members_get(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            ids (str): Comma-delimited list of member IDs. [optional]
-            sort_by (str): What to sort by. [optional]
-            sort_dir (str): Sort direction. [optional] if omitted the server will use the default value of "asc"
-            name (str): (Partial) user name to search for. [optional]
-            email (str): (Partial) Email address to search for. [optional]
-            group (str): Group ID or IDs to search for. [optional]
-            activity_after (int): Find members that have been active since unix timestamp. [optional]
-            activity_before (int): Find members that have been active before unix timestamp. [optional]
-            page (int): Page number. [optional]
-            per_page (int): Number of results per page. [optional] if omitted the server will use the default value of 25
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            CoreMembersGet200Response
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.core_members_get_endpoint.call_with_http_info(**kwargs)
-
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.api_client import ApiClient, Endpoint as _Endpoint
+from invision_client.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
+)
+from invision_client.model.core_members_get200_response import CoreMembersGet200Response
+
+
+class MembersApi(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None):
+        if api_client is None:
+            api_client = ApiClient()
+        self.api_client = api_client
+        self.core_members_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (CoreMembersGet200Response,),
+                'auth': [],
+                'endpoint_path': '/core/members',
+                'operation_id': 'core_members_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'ids',
+                    'sort_by',
+                    'sort_dir',
+                    'name',
+                    'email',
+                    'group',
+                    'activity_after',
+                    'activity_before',
+                    'page',
+                    'per_page',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                    'sort_by',
+                    'sort_dir',
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                    ('sort_by',): {
+
+                        "JOINED": "joined",
+                        "NAME": "name",
+                        "LAST_ACTIVITY": "last_activity"
+                    },
+                    ('sort_dir',): {
+
+                        "ASC": "asc",
+                        "DESC": "desc"
+                    },
+                },
+                'openapi_types': {
+                    'ids':
+                        (str,),
+                    'sort_by':
+                        (str,),
+                    'sort_dir':
+                        (str,),
+                    'name':
+                        (str,),
+                    'email':
+                        (str,),
+                    'group':
+                        (str,),
+                    'activity_after':
+                        (int,),
+                    'activity_before':
+                        (int,),
+                    'page':
+                        (int,),
+                    'per_page':
+                        (int,),
+                },
+                'attribute_map': {
+                    'ids': 'ids',
+                    'sort_by': 'sortBy',
+                    'sort_dir': 'sortDir',
+                    'name': 'name',
+                    'email': 'email',
+                    'group': 'group',
+                    'activity_after': 'activity_after',
+                    'activity_before': 'activity_before',
+                    'page': 'page',
+                    'per_page': 'perPage',
+                },
+                'location_map': {
+                    'ids': 'query',
+                    'sort_by': 'query',
+                    'sort_dir': 'query',
+                    'name': 'query',
+                    'email': 'query',
+                    'group': 'query',
+                    'activity_after': 'query',
+                    'activity_before': 'query',
+                    'page': 'query',
+                    'per_page': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    '*/*'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+    def core_members_get(
+        self,
+        **kwargs
+    ):
+        """Get list of members  # noqa: E501
+
+        Retrieves a list of members  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.core_members_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            ids (str): Comma-delimited list of member IDs. [optional]
+            sort_by (str): What to sort by. [optional]
+            sort_dir (str): Sort direction. [optional] if omitted the server will use the default value of "asc"
+            name (str): (Partial) user name to search for. [optional]
+            email (str): (Partial) Email address to search for. [optional]
+            group (str): Group ID or IDs to search for. [optional]
+            activity_after (int): Find members that have been active since unix timestamp. [optional]
+            activity_before (int): Find members that have been active before unix timestamp. [optional]
+            page (int): Page number. [optional]
+            per_page (int): Number of results per page. [optional] if omitted the server will use the default value of 25
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            CoreMembersGet200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.core_members_get_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `invision-client-python-1.0.0/invision_client/api/topics_api.py` & `invision-client-python-1.3.0b1/invision_client/api/topics_api.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.api_client import ApiClient, Endpoint as _Endpoint
-from invision_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
-)
-from invision_client.model.topic import Topic
-
-
-class TopicsApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.forums_topics_post_endpoint = _Endpoint(
-            settings={
-                'response_type': (Topic,),
-                'auth': [],
-                'endpoint_path': '/forums/topics',
-                'operation_id': 'forums_topics_post',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'forum',
-                    'title',
-                    'post',
-                    'author',
-                    'author_name',
-                    'prefix',
-                    'tags',
-                    'date',
-                    'ip_address',
-                    'locked',
-                    'open_time',
-                    'close_time',
-                    'hidden',
-                    'pinned',
-                    'featured',
-                    'poll_title',
-                    'poll_public',
-                    'poll_only',
-                    'poll_options',
-                ],
-                'required': [
-                    'forum',
-                    'title',
-                    'post',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'forum':
-                        (int,),
-                    'title':
-                        (str,),
-                    'post':
-                        (str,),
-                    'author':
-                        (int,),
-                    'author_name':
-                        (str,),
-                    'prefix':
-                        (str,),
-                    'tags':
-                        (str,),
-                    'date':
-                        (datetime,),
-                    'ip_address':
-                        (str,),
-                    'locked':
-                        (int,),
-                    'open_time':
-                        (datetime,),
-                    'close_time':
-                        (datetime,),
-                    'hidden':
-                        (int,),
-                    'pinned':
-                        (int,),
-                    'featured':
-                        (int,),
-                    'poll_title':
-                        (str,),
-                    'poll_public':
-                        (int,),
-                    'poll_only':
-                        (int,),
-                    'poll_options':
-                        ([bool, date, datetime, dict, float, int, list, str, none_type],),
-                },
-                'attribute_map': {
-                    'forum': 'forum',
-                    'title': 'title',
-                    'post': 'post',
-                    'author': 'author',
-                    'author_name': 'author_name',
-                    'prefix': 'prefix',
-                    'tags': 'tags',
-                    'date': 'date',
-                    'ip_address': 'ip_address',
-                    'locked': 'locked',
-                    'open_time': 'open_time',
-                    'close_time': 'close_time',
-                    'hidden': 'hidden',
-                    'pinned': 'pinned',
-                    'featured': 'featured',
-                    'poll_title': 'poll_title',
-                    'poll_public': 'poll_public',
-                    'poll_only': 'poll_only',
-                    'poll_options': 'poll_options',
-                },
-                'location_map': {
-                    'forum': 'form',
-                    'title': 'form',
-                    'post': 'form',
-                    'author': 'form',
-                    'author_name': 'form',
-                    'prefix': 'form',
-                    'tags': 'form',
-                    'date': 'form',
-                    'ip_address': 'form',
-                    'locked': 'form',
-                    'open_time': 'form',
-                    'close_time': 'form',
-                    'hidden': 'form',
-                    'pinned': 'form',
-                    'featured': 'form',
-                    'poll_title': 'form',
-                    'poll_public': 'form',
-                    'poll_only': 'form',
-                    'poll_options': 'form',
-                },
-                'collection_format_map': {
-                    'poll_options': 'csv',
-                }
-            },
-            headers_map={
-                'accept': [
-                    '*/*'
-                ],
-                'content_type': [
-                    'multipart/form-data'
-                ]
-            },
-            api_client=api_client
-        )
-
-    def forums_topics_post(
-        self,
-        forum,
-        title,
-        post,
-        **kwargs
-    ):
-        """Create a topic  # noqa: E501
-
-        Creates a new topic  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.forums_topics_post(forum, title, post, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            forum (int): The ID number of the forum the topic should be created in
-            title (str): The topic title
-            post (str): The post content as HTML
-
-        Keyword Args:
-            author (int): The ID number of the member creating the topic. [optional]
-            author_name (str): The guest name to be used if author is 0. [optional]
-            prefix (str): Prefix tag. [optional]
-            tags (str): Comma-separated list of tags. [optional]
-            date (datetime): The date/time that should be used for the topic/post post date. [optional]
-            ip_address (str): The IP address that should be stored for the topic/post. [optional]
-            locked (int): Indicates if the topic should be locked. [optional]
-            open_time (datetime): When the topic should be unlocked from. [optional]
-            close_time (datetime): When the topic should be locked from. [optional]
-            hidden (int): Indicates if the topic should be hidden. [optional]
-            pinned (int): Indicates if the topic should be pinned. [optional]
-            featured (int): Indicates if the topic should be featured. [optional]
-            poll_title (str): Poll title (to create a poll). [optional]
-            poll_public (int): Indicates if the poll is public. [optional]
-            poll_only (int): Indicates if this is a poll-only topic. [optional]
-            poll_options ([bool, date, datetime, dict, float, int, list, str, none_type]): Array of poll options. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            Topic
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['forum'] = \
-            forum
-        kwargs['title'] = \
-            title
-        kwargs['post'] = \
-            post
-        return self.forums_topics_post_endpoint.call_with_http_info(**kwargs)
-
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.api_client import ApiClient, Endpoint as _Endpoint
+from invision_client.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
+)
+from invision_client.model.topic import Topic
+
+
+class TopicsApi(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None):
+        if api_client is None:
+            api_client = ApiClient()
+        self.api_client = api_client
+        self.forums_topics_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (Topic,),
+                'auth': [],
+                'endpoint_path': '/forums/topics',
+                'operation_id': 'forums_topics_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'forum',
+                    'title',
+                    'post',
+                    'author',
+                    'author_name',
+                    'prefix',
+                    'tags',
+                    'date',
+                    'ip_address',
+                    'locked',
+                    'open_time',
+                    'close_time',
+                    'hidden',
+                    'pinned',
+                    'featured',
+                    'poll_title',
+                    'poll_public',
+                    'poll_only',
+                    'poll_options',
+                ],
+                'required': [
+                    'forum',
+                    'title',
+                    'post',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'forum':
+                        (int,),
+                    'title':
+                        (str,),
+                    'post':
+                        (str,),
+                    'author':
+                        (int,),
+                    'author_name':
+                        (str,),
+                    'prefix':
+                        (str,),
+                    'tags':
+                        (str,),
+                    'date':
+                        (datetime,),
+                    'ip_address':
+                        (str,),
+                    'locked':
+                        (int,),
+                    'open_time':
+                        (datetime,),
+                    'close_time':
+                        (datetime,),
+                    'hidden':
+                        (int,),
+                    'pinned':
+                        (int,),
+                    'featured':
+                        (int,),
+                    'poll_title':
+                        (str,),
+                    'poll_public':
+                        (int,),
+                    'poll_only':
+                        (int,),
+                    'poll_options':
+                        ([bool, date, datetime, dict, float, int, list, str, none_type],),
+                },
+                'attribute_map': {
+                    'forum': 'forum',
+                    'title': 'title',
+                    'post': 'post',
+                    'author': 'author',
+                    'author_name': 'author_name',
+                    'prefix': 'prefix',
+                    'tags': 'tags',
+                    'date': 'date',
+                    'ip_address': 'ip_address',
+                    'locked': 'locked',
+                    'open_time': 'open_time',
+                    'close_time': 'close_time',
+                    'hidden': 'hidden',
+                    'pinned': 'pinned',
+                    'featured': 'featured',
+                    'poll_title': 'poll_title',
+                    'poll_public': 'poll_public',
+                    'poll_only': 'poll_only',
+                    'poll_options': 'poll_options',
+                },
+                'location_map': {
+                    'forum': 'form',
+                    'title': 'form',
+                    'post': 'form',
+                    'author': 'form',
+                    'author_name': 'form',
+                    'prefix': 'form',
+                    'tags': 'form',
+                    'date': 'form',
+                    'ip_address': 'form',
+                    'locked': 'form',
+                    'open_time': 'form',
+                    'close_time': 'form',
+                    'hidden': 'form',
+                    'pinned': 'form',
+                    'featured': 'form',
+                    'poll_title': 'form',
+                    'poll_public': 'form',
+                    'poll_only': 'form',
+                    'poll_options': 'form',
+                },
+                'collection_format_map': {
+                    'poll_options': 'csv',
+                }
+            },
+            headers_map={
+                'accept': [
+                    '*/*'
+                ],
+                'content_type': [
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
+
+    def forums_topics_post(
+        self,
+        forum,
+        title,
+        post,
+        **kwargs
+    ):
+        """Create a topic  # noqa: E501
+
+        Creates a new topic  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.forums_topics_post(forum, title, post, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            forum (int): The ID number of the forum the topic should be created in
+            title (str): The topic title
+            post (str): The post content as HTML
+
+        Keyword Args:
+            author (int): The ID number of the member creating the topic. [optional]
+            author_name (str): The guest name to be used if author is 0. [optional]
+            prefix (str): Prefix tag. [optional]
+            tags (str): Comma-separated list of tags. [optional]
+            date (datetime): The date/time that should be used for the topic/post post date. [optional]
+            ip_address (str): The IP address that should be stored for the topic/post. [optional]
+            locked (int): Indicates if the topic should be locked. [optional]
+            open_time (datetime): When the topic should be unlocked from. [optional]
+            close_time (datetime): When the topic should be locked from. [optional]
+            hidden (int): Indicates if the topic should be hidden. [optional]
+            pinned (int): Indicates if the topic should be pinned. [optional]
+            featured (int): Indicates if the topic should be featured. [optional]
+            poll_title (str): Poll title (to create a poll). [optional]
+            poll_public (int): Indicates if the poll is public. [optional]
+            poll_only (int): Indicates if this is a poll-only topic. [optional]
+            poll_options ([bool, date, datetime, dict, float, int, list, str, none_type]): Array of poll options. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Topic
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['forum'] = \
+            forum
+        kwargs['title'] = \
+            title
+        kwargs['post'] = \
+            post
+        return self.forums_topics_post_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `invision-client-python-1.0.0/invision_client/apis/__init__.py` & `invision-client-python-1.3.0b1/invision_client/apis/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-
-# flake8: noqa
-
-# Import all APIs into this package.
-# If you have many APIs here with many many models used in each API this may
-# raise a `RecursionError`.
-# In order to avoid this, import only the API that you directly need like:
-#
-#   from invision_client.api.forums_api import ForumsApi
-#
-# or import this package, but before doing it, use:
-#
-#   import sys
-#   sys.setrecursionlimit(n)
-
-# Import APIs into API package:
-from invision_client.api.forums_api import ForumsApi
-from invision_client.api.members_api import MembersApi
-from invision_client.api.topics_api import TopicsApi
+
+# flake8: noqa
+
+# Import all APIs into this package.
+# If you have many APIs here with many many models used in each API this may
+# raise a `RecursionError`.
+# In order to avoid this, import only the API that you directly need like:
+#
+#   from invision_client.api.forums_api import ForumsApi
+#
+# or import this package, but before doing it, use:
+#
+#   import sys
+#   sys.setrecursionlimit(n)
+
+# Import APIs into API package:
+from invision_client.api.forums_api import ForumsApi
+from invision_client.api.members_api import MembersApi
+from invision_client.api.topics_api import TopicsApi
```

### Comparing `invision-client-python-1.0.0/invision_client/exceptions.py` & `invision-client-python-1.3.0b1/invision_client/exceptions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-class OpenApiException(Exception):
-    """The base exception class for all OpenAPIExceptions"""
-
-
-class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None,
-                 key_type=None):
-        """ Raises an exception for TypeErrors
-
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (list): a list of keys an indices to get to the
-                                 current_item
-                                 None if unset
-            valid_classes (tuple): the primitive classes that current item
-                                   should be an instance of
-                                   None if unset
-            key_type (bool): False if our value is a value in a dict
-                             True if it is a key in a dict
-                             False if our item is an item in a list
-                             None if unset
-        """
-        self.path_to_item = path_to_item
-        self.valid_classes = valid_classes
-        self.key_type = key_type
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiTypeError, self).__init__(full_msg)
-
-
-class ApiValueError(OpenApiException, ValueError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (list) the path to the exception in the
-                received_data dict. None if unset
-        """
-
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiValueError, self).__init__(full_msg)
-
-
-class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Raised when an attribute reference or assignment fails.
-
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (None/list) the path to the exception in the
-                received_data dict
-        """
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiAttributeError, self).__init__(full_msg)
-
-
-class ApiKeyError(OpenApiException, KeyError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (None/list) the path to the exception in the
-                received_data dict
-        """
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiKeyError, self).__init__(full_msg)
-
-
-class ApiException(OpenApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
-            self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
-
-    def __str__(self):
-        """Custom error messages for exception"""
-        error_message = "Status Code: {0}\n"\
-                        "Reason: {1}\n".format(self.status, self.reason)
-        if self.headers:
-            error_message += "HTTP response headers: {0}\n".format(
-                self.headers)
-
-        if self.body:
-            error_message += "HTTP response body: {0}\n".format(self.body)
-
-        return error_message
-
-
-class NotFoundException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
-
-
-class UnauthorizedException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
-
-
-class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
-
-
-class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
-
-
-def render_path(path_to_item):
-    """Returns a string representation of a path"""
-    result = ""
-    for pth in path_to_item:
-        if isinstance(pth, int):
-            result += "[{0}]".format(pth)
-        else:
-            result += "['{0}']".format(pth)
-    return result
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+class OpenApiException(Exception):
+    """The base exception class for all OpenAPIExceptions"""
+
+
+class ApiTypeError(OpenApiException, TypeError):
+    def __init__(self, msg, path_to_item=None, valid_classes=None,
+                 key_type=None):
+        """ Raises an exception for TypeErrors
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (list): a list of keys an indices to get to the
+                                 current_item
+                                 None if unset
+            valid_classes (tuple): the primitive classes that current item
+                                   should be an instance of
+                                   None if unset
+            key_type (bool): False if our value is a value in a dict
+                             True if it is a key in a dict
+                             False if our item is an item in a list
+                             None if unset
+        """
+        self.path_to_item = path_to_item
+        self.valid_classes = valid_classes
+        self.key_type = key_type
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiTypeError, self).__init__(full_msg)
+
+
+class ApiValueError(OpenApiException, ValueError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (list) the path to the exception in the
+                received_data dict. None if unset
+        """
+
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiValueError, self).__init__(full_msg)
+
+
+class ApiAttributeError(OpenApiException, AttributeError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Raised when an attribute reference or assignment fails.
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiAttributeError, self).__init__(full_msg)
+
+
+class ApiKeyError(OpenApiException, KeyError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiKeyError, self).__init__(full_msg)
+
+
+class ApiException(OpenApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
+        else:
+            self.status = status
+            self.reason = reason
+            self.body = None
+            self.headers = None
+
+    def __str__(self):
+        """Custom error messages for exception"""
+        error_message = "Status Code: {0}\n"\
+                        "Reason: {1}\n".format(self.status, self.reason)
+        if self.headers:
+            error_message += "HTTP response headers: {0}\n".format(
+                self.headers)
+
+        if self.body:
+            error_message += "HTTP response body: {0}\n".format(self.body)
+
+        return error_message
+
+
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
+
+def render_path(path_to_item):
+    """Returns a string representation of a path"""
+    result = ""
+    for pth in path_to_item:
+        if isinstance(pth, int):
+            result += "[{0}]".format(pth)
+        else:
+            result += "['{0}']".format(pth)
+    return result
```

### Comparing `invision-client-python-1.0.0/invision_client/invision_api.py` & `invision-client-python-1.3.0b1/invision_client/invision_api.py`

 * *Files identical despite different names*

### Comparing `invision-client-python-1.0.0/invision_client/model/core_members_get200_response.py` & `invision-client-python-1.3.0b1/invision_client/model/post.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,285 +1,299 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from invision_client.model.member import Member
-    globals()['Member'] = Member
-
-
-class CoreMembersGet200Response(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'page': (int,),  # noqa: E501
-            'per_page': (int,),  # noqa: E501
-            'total_results': (int,),  # noqa: E501
-            'total_pages': (int,),  # noqa: E501
-            'results': ([Member],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'page': 'page',  # noqa: E501
-        'per_page': 'perPage',  # noqa: E501
-        'total_results': 'totalResults',  # noqa: E501
-        'total_pages': 'totalPages',  # noqa: E501
-        'results': 'results',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CoreMembersGet200Response - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            page (int): [optional]  # noqa: E501
-            per_page (int): [optional]  # noqa: E501
-            total_results (int): [optional]  # noqa: E501
-            total_pages (int): [optional]  # noqa: E501
-            results ([Member]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """CoreMembersGet200Response - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            page (int): [optional]  # noqa: E501
-            per_page (int): [optional]  # noqa: E501
-            total_results (int): [optional]  # noqa: E501
-            total_pages (int): [optional]  # noqa: E501
-            results ([Member]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from invision_client.model.member import Member
+    from invision_client.model.post_reactions_inner import PostReactionsInner
+    globals()['Member'] = Member
+    globals()['PostReactionsInner'] = PostReactionsInner
+
+
+class Post(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'id': (int,),  # noqa: E501
+            'item_id': (int,),  # noqa: E501
+            'author': (Member,),  # noqa: E501
+            'date': (datetime,),  # noqa: E501
+            'content': (str,),  # noqa: E501
+            'hidden': (bool,),  # noqa: E501
+            'url': (str,),  # noqa: E501
+            'reactions': ([PostReactionsInner],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'item_id': 'item_id',  # noqa: E501
+        'author': 'author',  # noqa: E501
+        'date': 'date',  # noqa: E501
+        'content': 'content',  # noqa: E501
+        'hidden': 'hidden',  # noqa: E501
+        'url': 'url',  # noqa: E501
+        'reactions': 'reactions',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Post - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            item_id (int): [optional]  # noqa: E501
+            author (Member): [optional]  # noqa: E501
+            date (datetime): [optional]  # noqa: E501
+            content (str): [optional]  # noqa: E501
+            hidden (bool): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            reactions ([PostReactionsInner]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Post - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            item_id (int): [optional]  # noqa: E501
+            author (Member): [optional]  # noqa: E501
+            date (datetime): [optional]  # noqa: E501
+            content (str): [optional]  # noqa: E501
+            hidden (bool): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            reactions ([PostReactionsInner]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/field.py` & `invision-client-python-1.3.0b1/invision_client/model/forum.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,267 +1,291 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-
-class Field(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'name': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'name': 'name',  # noqa: E501
-        'value': 'value',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Field - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Field - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+
+class Forum(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'path': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'topics': (int,),  # noqa: E501
+            'url': (str,),  # noqa: E501
+            'parent_id': (int,),  # noqa: E501
+            'permissions': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'path': 'path',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'topics': 'topics',  # noqa: E501
+        'url': 'url',  # noqa: E501
+        'parent_id': 'parentId',  # noqa: E501
+        'permissions': 'permissions',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Forum - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            path (str): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            topics (int): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            parent_id (int): [optional]  # noqa: E501
+            permissions (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Forum - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            path (str): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            topics (int): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            parent_id (int): [optional]  # noqa: E501
+            permissions (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/fieldgroup.py` & `invision-client-python-1.3.0b1/invision_client/model/question.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,273 +1,267 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from invision_client.model.field import Field
-    globals()['Field'] = Field
-
-
-class Fieldgroup(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'name': (str,),  # noqa: E501
-            'fields': ([Field],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'name': 'name',  # noqa: E501
-        'fields': 'fields',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Fieldgroup - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            fields ([Field]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Fieldgroup - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            fields ([Field]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+
+class Question(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'question': (str,),  # noqa: E501
+            'options': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'question': 'question',  # noqa: E501
+        'options': 'options',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Question - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            question (str): [optional]  # noqa: E501
+            options (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Question - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            question (str): [optional]  # noqa: E501
+            options (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/forum.py` & `invision-client-python-1.3.0b1/invision_client/model/poll.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,291 +1,297 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-
-class Forum(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'path': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'topics': (int,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'parent_id': (int,),  # noqa: E501
-            'permissions': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'path': 'path',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'topics': 'topics',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'parent_id': 'parentId',  # noqa: E501
-        'permissions': 'permissions',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Forum - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            path (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            topics (int): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            parent_id (int): [optional]  # noqa: E501
-            permissions (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Forum - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            path (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            topics (int): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            parent_id (int): [optional]  # noqa: E501
-            permissions (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from invision_client.model.question import Question
+    globals()['Question'] = Question
+
+
+class Poll(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'id': (int,),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'start_date': (datetime,),  # noqa: E501
+            'closed': (bool,),  # noqa: E501
+            'closed_date': (datetime,),  # noqa: E501
+            'public': (bool,),  # noqa: E501
+            'votes': (int,),  # noqa: E501
+            'questions': ([Question],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'start_date': 'startDate',  # noqa: E501
+        'closed': 'closed',  # noqa: E501
+        'closed_date': 'closedDate',  # noqa: E501
+        'public': 'public',  # noqa: E501
+        'votes': 'votes',  # noqa: E501
+        'questions': 'questions',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Poll - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            start_date (datetime): [optional]  # noqa: E501
+            closed (bool): [optional]  # noqa: E501
+            closed_date (datetime): [optional]  # noqa: E501
+            public (bool): [optional]  # noqa: E501
+            votes (int): [optional]  # noqa: E501
+            questions ([Question]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Poll - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            start_date (datetime): [optional]  # noqa: E501
+            closed (bool): [optional]  # noqa: E501
+            closed_date (datetime): [optional]  # noqa: E501
+            public (bool): [optional]  # noqa: E501
+            votes (int): [optional]  # noqa: E501
+            questions ([Question]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/forums_forums_get200_response.py` & `invision-client-python-1.3.0b1/invision_client/model/core_members_get200_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,285 +1,285 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from invision_client.model.forum import Forum
-    globals()['Forum'] = Forum
-
-
-class ForumsForumsGet200Response(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'page': (int,),  # noqa: E501
-            'per_page': (int,),  # noqa: E501
-            'total_results': (int,),  # noqa: E501
-            'total_pages': (int,),  # noqa: E501
-            'results': ([Forum],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'page': 'page',  # noqa: E501
-        'per_page': 'perPage',  # noqa: E501
-        'total_results': 'totalResults',  # noqa: E501
-        'total_pages': 'totalPages',  # noqa: E501
-        'results': 'results',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ForumsForumsGet200Response - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            page (int): [optional]  # noqa: E501
-            per_page (int): [optional]  # noqa: E501
-            total_results (int): [optional]  # noqa: E501
-            total_pages (int): [optional]  # noqa: E501
-            results ([Forum]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """ForumsForumsGet200Response - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            page (int): [optional]  # noqa: E501
-            per_page (int): [optional]  # noqa: E501
-            total_results (int): [optional]  # noqa: E501
-            total_pages (int): [optional]  # noqa: E501
-            results ([Forum]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from invision_client.model.member import Member
+    globals()['Member'] = Member
+
+
+class CoreMembersGet200Response(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'page': (int,),  # noqa: E501
+            'per_page': (int,),  # noqa: E501
+            'total_results': (int,),  # noqa: E501
+            'total_pages': (int,),  # noqa: E501
+            'results': ([Member],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'page': 'page',  # noqa: E501
+        'per_page': 'perPage',  # noqa: E501
+        'total_results': 'totalResults',  # noqa: E501
+        'total_pages': 'totalPages',  # noqa: E501
+        'results': 'results',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """CoreMembersGet200Response - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            page (int): [optional]  # noqa: E501
+            per_page (int): [optional]  # noqa: E501
+            total_results (int): [optional]  # noqa: E501
+            total_pages (int): [optional]  # noqa: E501
+            results ([Member]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """CoreMembersGet200Response - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            page (int): [optional]  # noqa: E501
+            per_page (int): [optional]  # noqa: E501
+            total_results (int): [optional]  # noqa: E501
+            total_pages (int): [optional]  # noqa: E501
+            results ([Member]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/group.py` & `invision-client-python-1.3.0b1/invision_client/model/group.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,271 +1,271 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-
-class Group(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'formatted_name': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'formatted_name': 'formattedName',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Group - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            formatted_name (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Group - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            formatted_name (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+
+class Group(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'formatted_name': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'formatted_name': 'formattedName',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Group - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            formatted_name (str): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Group - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            formatted_name (str): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/member.py` & `invision-client-python-1.3.0b1/invision_client/model/member.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,381 +1,381 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from invision_client.model.fieldgroup import Fieldgroup
-    from invision_client.model.group import Group
-    from invision_client.model.rank import Rank
-    globals()['Fieldgroup'] = Fieldgroup
-    globals()['Group'] = Group
-    globals()['Rank'] = Rank
-
-
-class Member(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'title': (str,),  # noqa: E501
-            'timezone': (str,),  # noqa: E501
-            'formatted_name': (str,),  # noqa: E501
-            'primary_group': (Group,),  # noqa: E501
-            'secondary_groups': ([Group],),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'joined': (datetime,),  # noqa: E501
-            'registration_ip_address': (str,),  # noqa: E501
-            'warning_points': (int,),  # noqa: E501
-            'reputation_points': (int,),  # noqa: E501
-            'photo_url': (str,),  # noqa: E501
-            'photo_url_is_default': (bool,),  # noqa: E501
-            'cover_photo_url': (str,),  # noqa: E501
-            'profile_url': (str,),  # noqa: E501
-            'validating': (bool,),  # noqa: E501
-            'posts': (int,),  # noqa: E501
-            'last_activity': (datetime,),  # noqa: E501
-            'last_visit': (datetime,),  # noqa: E501
-            'last_post': (datetime,),  # noqa: E501
-            'profile_views': (int,),  # noqa: E501
-            'birthday': (str,),  # noqa: E501
-            'custom_fields': ([Fieldgroup],),  # noqa: E501
-            'rank': ([Rank],),  # noqa: E501
-            'achievements_points': (int,),  # noqa: E501
-            'allow_admin_emails': (bool,),  # noqa: E501
-            'completed': (bool,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'title': 'title',  # noqa: E501
-        'timezone': 'timezone',  # noqa: E501
-        'formatted_name': 'formattedName',  # noqa: E501
-        'primary_group': 'primaryGroup',  # noqa: E501
-        'secondary_groups': 'secondaryGroups',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'joined': 'joined',  # noqa: E501
-        'registration_ip_address': 'registrationIpAddress',  # noqa: E501
-        'warning_points': 'warningPoints',  # noqa: E501
-        'reputation_points': 'reputationPoints',  # noqa: E501
-        'photo_url': 'photoUrl',  # noqa: E501
-        'photo_url_is_default': 'photoUrlIsDefault',  # noqa: E501
-        'cover_photo_url': 'coverPhotoUrl',  # noqa: E501
-        'profile_url': 'profileUrl',  # noqa: E501
-        'validating': 'validating',  # noqa: E501
-        'posts': 'posts',  # noqa: E501
-        'last_activity': 'lastActivity',  # noqa: E501
-        'last_visit': 'lastVisit',  # noqa: E501
-        'last_post': 'lastPost',  # noqa: E501
-        'profile_views': 'profileViews',  # noqa: E501
-        'birthday': 'birthday',  # noqa: E501
-        'custom_fields': 'customFields',  # noqa: E501
-        'rank': 'rank',  # noqa: E501
-        'achievements_points': 'achievements_points',  # noqa: E501
-        'allow_admin_emails': 'allowAdminEmails',  # noqa: E501
-        'completed': 'completed',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Member - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            timezone (str): [optional]  # noqa: E501
-            formatted_name (str): [optional]  # noqa: E501
-            primary_group (Group): [optional]  # noqa: E501
-            secondary_groups ([Group]): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            joined (datetime): [optional]  # noqa: E501
-            registration_ip_address (str): [optional]  # noqa: E501
-            warning_points (int): [optional]  # noqa: E501
-            reputation_points (int): [optional]  # noqa: E501
-            photo_url (str): [optional]  # noqa: E501
-            photo_url_is_default (bool): [optional]  # noqa: E501
-            cover_photo_url (str): [optional]  # noqa: E501
-            profile_url (str): [optional]  # noqa: E501
-            validating (bool): [optional]  # noqa: E501
-            posts (int): [optional]  # noqa: E501
-            last_activity (datetime): [optional]  # noqa: E501
-            last_visit (datetime): [optional]  # noqa: E501
-            last_post (datetime): [optional]  # noqa: E501
-            profile_views (int): [optional]  # noqa: E501
-            birthday (str): [optional]  # noqa: E501
-            custom_fields ([Fieldgroup]): [optional]  # noqa: E501
-            rank ([Rank]): [optional]  # noqa: E501
-            achievements_points (int): [optional]  # noqa: E501
-            allow_admin_emails (bool): [optional]  # noqa: E501
-            completed (bool): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Member - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            timezone (str): [optional]  # noqa: E501
-            formatted_name (str): [optional]  # noqa: E501
-            primary_group (Group): [optional]  # noqa: E501
-            secondary_groups ([Group]): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            joined (datetime): [optional]  # noqa: E501
-            registration_ip_address (str): [optional]  # noqa: E501
-            warning_points (int): [optional]  # noqa: E501
-            reputation_points (int): [optional]  # noqa: E501
-            photo_url (str): [optional]  # noqa: E501
-            photo_url_is_default (bool): [optional]  # noqa: E501
-            cover_photo_url (str): [optional]  # noqa: E501
-            profile_url (str): [optional]  # noqa: E501
-            validating (bool): [optional]  # noqa: E501
-            posts (int): [optional]  # noqa: E501
-            last_activity (datetime): [optional]  # noqa: E501
-            last_visit (datetime): [optional]  # noqa: E501
-            last_post (datetime): [optional]  # noqa: E501
-            profile_views (int): [optional]  # noqa: E501
-            birthday (str): [optional]  # noqa: E501
-            custom_fields ([Fieldgroup]): [optional]  # noqa: E501
-            rank ([Rank]): [optional]  # noqa: E501
-            achievements_points (int): [optional]  # noqa: E501
-            allow_admin_emails (bool): [optional]  # noqa: E501
-            completed (bool): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from invision_client.model.fieldgroup import Fieldgroup
+    from invision_client.model.group import Group
+    from invision_client.model.rank import Rank
+    globals()['Fieldgroup'] = Fieldgroup
+    globals()['Group'] = Group
+    globals()['Rank'] = Rank
+
+
+class Member(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'timezone': (str,),  # noqa: E501
+            'formatted_name': (str,),  # noqa: E501
+            'primary_group': (Group,),  # noqa: E501
+            'secondary_groups': ([Group],),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'joined': (datetime,),  # noqa: E501
+            'registration_ip_address': (str,),  # noqa: E501
+            'warning_points': (int,),  # noqa: E501
+            'reputation_points': (int,),  # noqa: E501
+            'photo_url': (str,),  # noqa: E501
+            'photo_url_is_default': (bool,),  # noqa: E501
+            'cover_photo_url': (str,),  # noqa: E501
+            'profile_url': (str,),  # noqa: E501
+            'validating': (bool,),  # noqa: E501
+            'posts': (int,),  # noqa: E501
+            'last_activity': (datetime,),  # noqa: E501
+            'last_visit': (datetime,),  # noqa: E501
+            'last_post': (datetime,),  # noqa: E501
+            'profile_views': (int,),  # noqa: E501
+            'birthday': (str,),  # noqa: E501
+            'custom_fields': ([Fieldgroup],),  # noqa: E501
+            'rank': ([Rank],),  # noqa: E501
+            'achievements_points': (int,),  # noqa: E501
+            'allow_admin_emails': (bool,),  # noqa: E501
+            'completed': (bool,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'timezone': 'timezone',  # noqa: E501
+        'formatted_name': 'formattedName',  # noqa: E501
+        'primary_group': 'primaryGroup',  # noqa: E501
+        'secondary_groups': 'secondaryGroups',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'joined': 'joined',  # noqa: E501
+        'registration_ip_address': 'registrationIpAddress',  # noqa: E501
+        'warning_points': 'warningPoints',  # noqa: E501
+        'reputation_points': 'reputationPoints',  # noqa: E501
+        'photo_url': 'photoUrl',  # noqa: E501
+        'photo_url_is_default': 'photoUrlIsDefault',  # noqa: E501
+        'cover_photo_url': 'coverPhotoUrl',  # noqa: E501
+        'profile_url': 'profileUrl',  # noqa: E501
+        'validating': 'validating',  # noqa: E501
+        'posts': 'posts',  # noqa: E501
+        'last_activity': 'lastActivity',  # noqa: E501
+        'last_visit': 'lastVisit',  # noqa: E501
+        'last_post': 'lastPost',  # noqa: E501
+        'profile_views': 'profileViews',  # noqa: E501
+        'birthday': 'birthday',  # noqa: E501
+        'custom_fields': 'customFields',  # noqa: E501
+        'rank': 'rank',  # noqa: E501
+        'achievements_points': 'achievements_points',  # noqa: E501
+        'allow_admin_emails': 'allowAdminEmails',  # noqa: E501
+        'completed': 'completed',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Member - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            timezone (str): [optional]  # noqa: E501
+            formatted_name (str): [optional]  # noqa: E501
+            primary_group (Group): [optional]  # noqa: E501
+            secondary_groups ([Group]): [optional]  # noqa: E501
+            email (str): [optional]  # noqa: E501
+            joined (datetime): [optional]  # noqa: E501
+            registration_ip_address (str): [optional]  # noqa: E501
+            warning_points (int): [optional]  # noqa: E501
+            reputation_points (int): [optional]  # noqa: E501
+            photo_url (str): [optional]  # noqa: E501
+            photo_url_is_default (bool): [optional]  # noqa: E501
+            cover_photo_url (str): [optional]  # noqa: E501
+            profile_url (str): [optional]  # noqa: E501
+            validating (bool): [optional]  # noqa: E501
+            posts (int): [optional]  # noqa: E501
+            last_activity (datetime): [optional]  # noqa: E501
+            last_visit (datetime): [optional]  # noqa: E501
+            last_post (datetime): [optional]  # noqa: E501
+            profile_views (int): [optional]  # noqa: E501
+            birthday (str): [optional]  # noqa: E501
+            custom_fields ([Fieldgroup]): [optional]  # noqa: E501
+            rank ([Rank]): [optional]  # noqa: E501
+            achievements_points (int): [optional]  # noqa: E501
+            allow_admin_emails (bool): [optional]  # noqa: E501
+            completed (bool): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Member - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            timezone (str): [optional]  # noqa: E501
+            formatted_name (str): [optional]  # noqa: E501
+            primary_group (Group): [optional]  # noqa: E501
+            secondary_groups ([Group]): [optional]  # noqa: E501
+            email (str): [optional]  # noqa: E501
+            joined (datetime): [optional]  # noqa: E501
+            registration_ip_address (str): [optional]  # noqa: E501
+            warning_points (int): [optional]  # noqa: E501
+            reputation_points (int): [optional]  # noqa: E501
+            photo_url (str): [optional]  # noqa: E501
+            photo_url_is_default (bool): [optional]  # noqa: E501
+            cover_photo_url (str): [optional]  # noqa: E501
+            profile_url (str): [optional]  # noqa: E501
+            validating (bool): [optional]  # noqa: E501
+            posts (int): [optional]  # noqa: E501
+            last_activity (datetime): [optional]  # noqa: E501
+            last_visit (datetime): [optional]  # noqa: E501
+            last_post (datetime): [optional]  # noqa: E501
+            profile_views (int): [optional]  # noqa: E501
+            birthday (str): [optional]  # noqa: E501
+            custom_fields ([Fieldgroup]): [optional]  # noqa: E501
+            rank ([Rank]): [optional]  # noqa: E501
+            achievements_points (int): [optional]  # noqa: E501
+            allow_admin_emails (bool): [optional]  # noqa: E501
+            completed (bool): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/poll.py` & `invision-client-python-1.3.0b1/invision_client/model/post_reactions_inner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,297 +1,279 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from invision_client.model.question import Question
-    globals()['Question'] = Question
-
-
-class Poll(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'id': (int,),  # noqa: E501
-            'title': (str,),  # noqa: E501
-            'start_date': (datetime,),  # noqa: E501
-            'closed': (bool,),  # noqa: E501
-            'closed_date': (datetime,),  # noqa: E501
-            'public': (bool,),  # noqa: E501
-            'votes': (int,),  # noqa: E501
-            'questions': ([Question],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'title': 'title',  # noqa: E501
-        'start_date': 'startDate',  # noqa: E501
-        'closed': 'closed',  # noqa: E501
-        'closed_date': 'closedDate',  # noqa: E501
-        'public': 'public',  # noqa: E501
-        'votes': 'votes',  # noqa: E501
-        'questions': 'questions',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Poll - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            start_date (datetime): [optional]  # noqa: E501
-            closed (bool): [optional]  # noqa: E501
-            closed_date (datetime): [optional]  # noqa: E501
-            public (bool): [optional]  # noqa: E501
-            votes (int): [optional]  # noqa: E501
-            questions ([Question]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Poll - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            start_date (datetime): [optional]  # noqa: E501
-            closed (bool): [optional]  # noqa: E501
-            closed_date (datetime): [optional]  # noqa: E501
-            public (bool): [optional]  # noqa: E501
-            votes (int): [optional]  # noqa: E501
-            questions ([Question]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+
+class PostReactionsInner(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'member_id': ([str],),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
+            'icon': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'member_id': 'member_id',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'value': 'value',  # noqa: E501
+        'icon': 'icon',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """PostReactionsInner - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            member_id ([str]): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
+            icon (str): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """PostReactionsInner - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            member_id ([str]): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
+            icon (str): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/post.py` & `invision-client-python-1.3.0b1/invision_client/model/fieldgroup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,299 +1,273 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from invision_client.model.member import Member
-    from invision_client.model.post_reactions_inner import PostReactionsInner
-    globals()['Member'] = Member
-    globals()['PostReactionsInner'] = PostReactionsInner
-
-
-class Post(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'id': (int,),  # noqa: E501
-            'item_id': (int,),  # noqa: E501
-            'author': (Member,),  # noqa: E501
-            'date': (datetime,),  # noqa: E501
-            'content': (str,),  # noqa: E501
-            'hidden': (bool,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'reactions': ([PostReactionsInner],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'item_id': 'item_id',  # noqa: E501
-        'author': 'author',  # noqa: E501
-        'date': 'date',  # noqa: E501
-        'content': 'content',  # noqa: E501
-        'hidden': 'hidden',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'reactions': 'reactions',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Post - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            item_id (int): [optional]  # noqa: E501
-            author (Member): [optional]  # noqa: E501
-            date (datetime): [optional]  # noqa: E501
-            content (str): [optional]  # noqa: E501
-            hidden (bool): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            reactions ([PostReactionsInner]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Post - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            item_id (int): [optional]  # noqa: E501
-            author (Member): [optional]  # noqa: E501
-            date (datetime): [optional]  # noqa: E501
-            content (str): [optional]  # noqa: E501
-            hidden (bool): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            reactions ([PostReactionsInner]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from invision_client.model.field import Field
+    globals()['Field'] = Field
+
+
+class Fieldgroup(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'name': (str,),  # noqa: E501
+            'fields': ([Field],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'name': 'name',  # noqa: E501
+        'fields': 'fields',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Fieldgroup - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            name (str): [optional]  # noqa: E501
+            fields ([Field]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Fieldgroup - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            name (str): [optional]  # noqa: E501
+            fields ([Field]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/post_reactions_inner.py` & `invision-client-python-1.3.0b1/invision_client/model/field.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,279 +1,267 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-
-class PostReactionsInner(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'member_id': ([str],),  # noqa: E501
-            'title': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
-            'icon': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'member_id': 'member_id',  # noqa: E501
-        'title': 'title',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'value': 'value',  # noqa: E501
-        'icon': 'icon',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PostReactionsInner - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            member_id ([str]): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
-            icon (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """PostReactionsInner - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            member_id ([str]): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
-            icon (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+
+class Field(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'name': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'name': 'name',  # noqa: E501
+        'value': 'value',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Field - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            name (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Field - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            name (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/question.py` & `invision-client-python-1.3.0b1/invision_client/model/rank.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,267 +1,275 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-
-class Question(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'question': (str,),  # noqa: E501
-            'options': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'question': 'question',  # noqa: E501
-        'options': 'options',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Question - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            question (str): [optional]  # noqa: E501
-            options (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Question - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            question (str): [optional]  # noqa: E501
-            options (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+
+class Rank(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'url': (str,),  # noqa: E501
+            'points': (int,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'url': 'url',  # noqa: E501
+        'points': 'points',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Rank - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            points (int): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Rank - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            points (int): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/rank.py` & `invision-client-python-1.3.0b1/invision_client/model/forums_forums_get200_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,275 +1,285 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-
-class Rank(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'points': (int,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'points': 'points',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Rank - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            points (int): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Rank - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            points (int): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from invision_client.model.forum import Forum
+    globals()['Forum'] = Forum
+
+
+class ForumsForumsGet200Response(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'page': (int,),  # noqa: E501
+            'per_page': (int,),  # noqa: E501
+            'total_results': (int,),  # noqa: E501
+            'total_pages': (int,),  # noqa: E501
+            'results': ([Forum],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'page': 'page',  # noqa: E501
+        'per_page': 'perPage',  # noqa: E501
+        'total_results': 'totalResults',  # noqa: E501
+        'total_pages': 'totalPages',  # noqa: E501
+        'results': 'results',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ForumsForumsGet200Response - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            page (int): [optional]  # noqa: E501
+            per_page (int): [optional]  # noqa: E501
+            total_results (int): [optional]  # noqa: E501
+            total_pages (int): [optional]  # noqa: E501
+            results ([Forum]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ForumsForumsGet200Response - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            page (int): [optional]  # noqa: E501
+            per_page (int): [optional]  # noqa: E501
+            total_results (int): [optional]  # noqa: E501
+            total_pages (int): [optional]  # noqa: E501
+            results ([Forum]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model/topic.py` & `invision-client-python-1.3.0b1/invision_client/model/topic.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from invision_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from invision_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from invision_client.model.forum import Forum
-    from invision_client.model.poll import Poll
-    from invision_client.model.post import Post
-    globals()['Forum'] = Forum
-    globals()['Poll'] = Poll
-    globals()['Post'] = Post
-
-
-class Topic(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'id': (int,),  # noqa: E501
-            'title': (str,),  # noqa: E501
-            'forum': (Forum,),  # noqa: E501
-            'posts': (int,),  # noqa: E501
-            'views': (int,),  # noqa: E501
-            'prefix': (str,),  # noqa: E501
-            'tags': ([str],),  # noqa: E501
-            'first_post': (Post,),  # noqa: E501
-            'last_post': (Post,),  # noqa: E501
-            'best_answer': (Post,),  # noqa: E501
-            'locked': (bool,),  # noqa: E501
-            'hidden': (bool,),  # noqa: E501
-            'pinned': (bool,),  # noqa: E501
-            'featured': (bool,),  # noqa: E501
-            'archived': (bool,),  # noqa: E501
-            'poll': (Poll,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'rating': (float,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'title': 'title',  # noqa: E501
-        'forum': 'forum',  # noqa: E501
-        'posts': 'posts',  # noqa: E501
-        'views': 'views',  # noqa: E501
-        'prefix': 'prefix',  # noqa: E501
-        'tags': 'tags',  # noqa: E501
-        'first_post': 'firstPost',  # noqa: E501
-        'last_post': 'lastPost',  # noqa: E501
-        'best_answer': 'bestAnswer',  # noqa: E501
-        'locked': 'locked',  # noqa: E501
-        'hidden': 'hidden',  # noqa: E501
-        'pinned': 'pinned',  # noqa: E501
-        'featured': 'featured',  # noqa: E501
-        'archived': 'archived',  # noqa: E501
-        'poll': 'poll',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'rating': 'rating',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Topic - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            forum (Forum): [optional]  # noqa: E501
-            posts (int): [optional]  # noqa: E501
-            views (int): [optional]  # noqa: E501
-            prefix (str): [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
-            first_post (Post): [optional]  # noqa: E501
-            last_post (Post): [optional]  # noqa: E501
-            best_answer (Post): [optional]  # noqa: E501
-            locked (bool): [optional]  # noqa: E501
-            hidden (bool): [optional]  # noqa: E501
-            pinned (bool): [optional]  # noqa: E501
-            featured (bool): [optional]  # noqa: E501
-            archived (bool): [optional]  # noqa: E501
-            poll (Poll): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            rating (float): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Topic - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            forum (Forum): [optional]  # noqa: E501
-            posts (int): [optional]  # noqa: E501
-            views (int): [optional]  # noqa: E501
-            prefix (str): [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
-            first_post (Post): [optional]  # noqa: E501
-            last_post (Post): [optional]  # noqa: E501
-            best_answer (Post): [optional]  # noqa: E501
-            locked (bool): [optional]  # noqa: E501
-            hidden (bool): [optional]  # noqa: E501
-            pinned (bool): [optional]  # noqa: E501
-            featured (bool): [optional]  # noqa: E501
-            archived (bool): [optional]  # noqa: E501
-            poll (Poll): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            rating (float): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from invision_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from invision_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from invision_client.model.forum import Forum
+    from invision_client.model.poll import Poll
+    from invision_client.model.post import Post
+    globals()['Forum'] = Forum
+    globals()['Poll'] = Poll
+    globals()['Post'] = Post
+
+
+class Topic(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'id': (int,),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'forum': (Forum,),  # noqa: E501
+            'posts': (int,),  # noqa: E501
+            'views': (int,),  # noqa: E501
+            'prefix': (str,),  # noqa: E501
+            'tags': ([str],),  # noqa: E501
+            'first_post': (Post,),  # noqa: E501
+            'last_post': (Post,),  # noqa: E501
+            'best_answer': (Post,),  # noqa: E501
+            'locked': (bool,),  # noqa: E501
+            'hidden': (bool,),  # noqa: E501
+            'pinned': (bool,),  # noqa: E501
+            'featured': (bool,),  # noqa: E501
+            'archived': (bool,),  # noqa: E501
+            'poll': (Poll,),  # noqa: E501
+            'url': (str,),  # noqa: E501
+            'rating': (float,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'forum': 'forum',  # noqa: E501
+        'posts': 'posts',  # noqa: E501
+        'views': 'views',  # noqa: E501
+        'prefix': 'prefix',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
+        'first_post': 'firstPost',  # noqa: E501
+        'last_post': 'lastPost',  # noqa: E501
+        'best_answer': 'bestAnswer',  # noqa: E501
+        'locked': 'locked',  # noqa: E501
+        'hidden': 'hidden',  # noqa: E501
+        'pinned': 'pinned',  # noqa: E501
+        'featured': 'featured',  # noqa: E501
+        'archived': 'archived',  # noqa: E501
+        'poll': 'poll',  # noqa: E501
+        'url': 'url',  # noqa: E501
+        'rating': 'rating',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Topic - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            forum (Forum): [optional]  # noqa: E501
+            posts (int): [optional]  # noqa: E501
+            views (int): [optional]  # noqa: E501
+            prefix (str): [optional]  # noqa: E501
+            tags ([str]): [optional]  # noqa: E501
+            first_post (Post): [optional]  # noqa: E501
+            last_post (Post): [optional]  # noqa: E501
+            best_answer (Post): [optional]  # noqa: E501
+            locked (bool): [optional]  # noqa: E501
+            hidden (bool): [optional]  # noqa: E501
+            pinned (bool): [optional]  # noqa: E501
+            featured (bool): [optional]  # noqa: E501
+            archived (bool): [optional]  # noqa: E501
+            poll (Poll): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            rating (float): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Topic - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (int): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            forum (Forum): [optional]  # noqa: E501
+            posts (int): [optional]  # noqa: E501
+            views (int): [optional]  # noqa: E501
+            prefix (str): [optional]  # noqa: E501
+            tags ([str]): [optional]  # noqa: E501
+            first_post (Post): [optional]  # noqa: E501
+            last_post (Post): [optional]  # noqa: E501
+            best_answer (Post): [optional]  # noqa: E501
+            locked (bool): [optional]  # noqa: E501
+            hidden (bool): [optional]  # noqa: E501
+            pinned (bool): [optional]  # noqa: E501
+            featured (bool): [optional]  # noqa: E501
+            archived (bool): [optional]  # noqa: E501
+            poll (Poll): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            rating (float): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `invision-client-python-1.0.0/invision_client/model_utils.py` & `invision-client-python-1.3.0b1/invision_client/model_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,2058 +1,2058 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-from datetime import date, datetime  # noqa: F401
-from copy import deepcopy
-import inspect
-import io
-import os
-import pprint
-import re
-import tempfile
-import uuid
-
-from dateutil.parser import parse
-
-from invision_client.exceptions import (
-    ApiKeyError,
-    ApiAttributeError,
-    ApiTypeError,
-    ApiValueError,
-)
-
-none_type = type(None)
-file_type = io.IOBase
-
-
-def convert_js_args_to_python_args(fn):
-    from functools import wraps
-    @wraps(fn)
-    def wrapped_init(_self, *args, **kwargs):
-        """
-        An attribute named `self` received from the api will conflicts with the reserved `self`
-        parameter of a class method. During generation, `self` attributes are mapped
-        to `_self` in models. Here, we name `_self` instead of `self` to avoid conflicts.
-        """
-        spec_property_naming = kwargs.get('_spec_property_naming', False)
-        if spec_property_naming:
-            kwargs = change_keys_js_to_python(
-                kwargs, _self if isinstance(
-                    _self, type) else _self.__class__)
-        return fn(_self, *args, **kwargs)
-    return wrapped_init
-
-
-class cached_property(object):
-    # this caches the result of the function call for fn with no inputs
-    # use this as a decorator on function methods that you want converted
-    # into cached properties
-    result_key = '_results'
-
-    def __init__(self, fn):
-        self._fn = fn
-
-    def __get__(self, instance, cls=None):
-        if self.result_key in vars(self):
-            return vars(self)[self.result_key]
-        else:
-            result = self._fn()
-            setattr(self, self.result_key, result)
-            return result
-
-
-PRIMITIVE_TYPES = (list, float, int, bool, datetime, date, str, file_type)
-
-
-def allows_single_value_input(cls):
-    """
-    This function returns True if the input composed schema model or any
-    descendant model allows a value only input
-    This is true for cases where oneOf contains items like:
-    oneOf:
-      - float
-      - NumberWithValidation
-      - StringEnum
-      - ArrayModel
-      - null
-    TODO: lru_cache this
-    """
-    if (
-        issubclass(cls, ModelSimple) or
-        cls in PRIMITIVE_TYPES
-    ):
-        return True
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return False
-        return any(allows_single_value_input(c) for c in cls._composed_schemas['oneOf'])
-    return False
-
-
-def composed_model_input_classes(cls):
-    """
-    This function returns a list of the possible models that can be accepted as
-    inputs.
-    TODO: lru_cache this
-    """
-    if issubclass(cls, ModelSimple) or cls in PRIMITIVE_TYPES:
-        return [cls]
-    elif issubclass(cls, ModelNormal):
-        if cls.discriminator is None:
-            return [cls]
-        else:
-            return get_discriminated_classes(cls)
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return []
-        if cls.discriminator is None:
-            input_classes = []
-            for c in cls._composed_schemas['oneOf']:
-                input_classes.extend(composed_model_input_classes(c))
-            return input_classes
-        else:
-            return get_discriminated_classes(cls)
-    return []
-
-
-class OpenApiModel(object):
-    """The base class for all OpenAPIModels"""
-
-    def set_attribute(self, name, value):
-        # this is only used to set properties on self
-
-        path_to_item = []
-        if self._path_to_item:
-            path_to_item.extend(self._path_to_item)
-        path_to_item.append(name)
-
-        if name in self.openapi_types:
-            required_types_mixed = self.openapi_types[name]
-        elif self.additional_properties_type is None:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                path_to_item
-            )
-        elif self.additional_properties_type is not None:
-            required_types_mixed = self.additional_properties_type
-
-        if get_simple_class(name) != str:
-            error_msg = type_error_message(
-                var_name=name,
-                var_value=name,
-                valid_classes=(str,),
-                key_type=True
-            )
-            raise ApiTypeError(
-                error_msg,
-                path_to_item=path_to_item,
-                valid_classes=(str,),
-                key_type=True
-            )
-
-        if self._check_type:
-            value = validate_and_convert_types(
-                value, required_types_mixed, path_to_item, self._spec_property_naming,
-                self._check_type, configuration=self._configuration)
-        if (name,) in self.allowed_values:
-            check_allowed_values(
-                self.allowed_values,
-                (name,),
-                value
-            )
-        if (name,) in self.validations:
-            check_validations(
-                self.validations,
-                (name,),
-                value,
-                self._configuration
-            )
-        self.__dict__['_data_store'][name] = value
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        return not self == other
-
-    def __setattr__(self, attr, value):
-        """set the value of an attribute using dot notation: `instance.attr = val`"""
-        self[attr] = value
-
-    def __getattr__(self, attr):
-        """get the value of an attribute using dot notation: `instance.attr`"""
-        return self.__getitem__(attr)
-
-    def __copy__(self):
-        cls = self.__class__
-        if self.get("_spec_property_naming", False):
-            return cls._new_from_openapi_data(**self.__dict__)
-        else:
-            return cls.__new__(cls, **self.__dict__)
-
-    def __deepcopy__(self, memo):
-        cls = self.__class__
-
-        if self.get("_spec_property_naming", False):
-            new_inst = cls._new_from_openapi_data()
-        else:
-            new_inst = cls.__new__(cls, **self.__dict__)
-
-        for k, v in self.__dict__.items():
-            setattr(new_inst, k, deepcopy(v, memo))
-        return new_inst
-
-
-    def __new__(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
-            )
-
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-            cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = super(OpenApiModel, cls).__new__(cls)
-            self_inst.__init__(*args, **kwargs)
-
-        if kwargs.get("_spec_property_naming", False):
-            # when true, implies new is from deserialization
-            new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
-        else:
-            new_inst = new_cls.__new__(new_cls, *args, **kwargs)
-            new_inst.__init__(*args, **kwargs)
-
-        return new_inst
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _new_from_openapi_data(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
-            )
-
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-            cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = cls._from_openapi_data(*args, **kwargs)
-
-        new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
-        return new_inst
-
-
-class ModelSimple(OpenApiModel):
-    """the parent class of models whose type != object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
-
-        self.set_attribute(name, value)
-
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
-        )
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return str(self.value)
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
-
-        this_val = self._data_store['value']
-        that_val = other._data_store['value']
-        types = set()
-        types.add(this_val.__class__)
-        types.add(that_val.__class__)
-        vals_equal = this_val == that_val
-        return vals_equal
-
-
-class ModelNormal(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
-
-        self.set_attribute(name, value)
-
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
-        )
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
-
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
-            return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-class ModelComposed(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi and have oneOf/allOf/anyOf
-
-    When one sets a property we use var_name_to_model_instances to store the value in
-    the correct class instances + run any type checking + validation code.
-    When one gets a property we use var_name_to_model_instances to get the value
-    from the correct class instances.
-    This allows multiple composed schemas to contain the same property with additive
-    constraints on the value.
-
-    _composed_schemas (dict) stores the anyOf/allOf/oneOf classes
-    key (str): allOf/oneOf/anyOf
-    value (list): the classes in the XOf definition.
-        Note: none_type can be included when the openapi document version >= 3.1.0
-    _composed_instances (list): stores a list of instances of the composed schemas
-    defined in _composed_schemas. When properties are accessed in the self instance,
-    they are returned from the self._data_store or the data stores in the instances
-    in self._composed_schemas
-    _var_name_to_model_instances (dict): maps between a variable name on self and
-    the composed instances (self included) which contain that data
-    key (str): property name
-    value (list): list of class instances, self or instances in _composed_instances
-    which contain the value that the key is referring to.
-    """
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
-
-        """
-        Use cases:
-        1. additional_properties_type is None (additionalProperties == False in spec)
-            Check for property presence in self.openapi_types
-            if not present then throw an error
-            if present set in self, set attribute
-            always set on composed schemas
-        2.  additional_properties_type exists
-            set attribute on self
-            always set on composed schemas
-        """
-        if self.additional_properties_type is None:
-            """
-            For an attribute to exist on a composed schema it must:
-            - fulfill schema_requirements in the self composed schema not considering oneOf/anyOf/allOf schemas AND
-            - fulfill schema_requirements in each oneOf/anyOf/allOf schemas
-
-            schema_requirements:
-            For an attribute to exist on a schema it must:
-            - be present in properties at the schema OR
-            - have additionalProperties unset (defaults additionalProperties = any type) OR
-            - have additionalProperties set
-            """
-            if name not in self.openapi_types:
-                raise ApiAttributeError(
-                    "{0} has no attribute '{1}'".format(
-                        type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
-                )
-        # attribute must be set on self and composed instances
-        self.set_attribute(name, value)
-        for model_instance in self._composed_instances:
-            setattr(model_instance, name, value)
-        if name not in self._var_name_to_model_instances:
-            # we assigned an additional property
-            self.__dict__['_var_name_to_model_instances'][name] = self._composed_instances + [self]
-        return None
-
-    __unset_attribute_value__ = object()
-
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        # get the attribute from the correct instance
-        model_instances = self._var_name_to_model_instances.get(name)
-        values = []
-        # A composed model stores self and child (oneof/anyOf/allOf) models under
-        # self._var_name_to_model_instances.
-        # Any property must exist in self and all model instances
-        # The value stored in all model instances must be the same
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    v = model_instance._data_store[name]
-                    if v not in values:
-                        values.append(v)
-        len_values = len(values)
-        if len_values == 0:
-            return default
-        elif len_values == 1:
-            return values[0]
-        elif len_values > 1:
-            raise ApiValueError(
-                "Values stored for property {0} in {1} differ when looking "
-                "at self and self's composed instances. All values must be "
-                "the same".format(name, type(self).__name__),
-                [e for e in [self._path_to_item, name] if e]
-            )
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        value = self.get(name, self.__unset_attribute_value__)
-        if value is self.__unset_attribute_value__:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
-            )
-        return value
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        model_instances = self._var_name_to_model_instances.get(
-            name, self._additional_properties_model_instances)
-
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    return True
-
-        return False
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
-
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
-            return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-COERCION_INDEX_BY_TYPE = {
-    ModelComposed: 0,
-    ModelNormal: 1,
-    ModelSimple: 2,
-    none_type: 3,    # The type of 'None'.
-    list: 4,
-    dict: 5,
-    float: 6,
-    int: 7,
-    bool: 8,
-    datetime: 9,
-    date: 10,
-    str: 11,
-    file_type: 12,   # 'file_type' is an alias for the built-in 'file' or 'io.IOBase' type.
-}
-
-# these are used to limit what type conversions we try to do
-# when we have a valid type already and we want to try converting
-# to another type
-UPCONVERSION_TYPE_PAIRS = (
-    (str, datetime),
-    (str, date),
-    # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
-    (int, float),
-    (list, ModelComposed),
-    (dict, ModelComposed),
-    (str, ModelComposed),
-    (int, ModelComposed),
-    (float, ModelComposed),
-    (list, ModelComposed),
-    (list, ModelNormal),
-    (dict, ModelNormal),
-    (str, ModelSimple),
-    (int, ModelSimple),
-    (float, ModelSimple),
-    (list, ModelSimple),
-)
-
-COERCIBLE_TYPE_PAIRS = {
-    False: (  # client instantiation of a model with client data
-        # (dict, ModelComposed),
-        # (list, ModelComposed),
-        # (dict, ModelNormal),
-        # (list, ModelNormal),
-        # (str, ModelSimple),
-        # (int, ModelSimple),
-        # (float, ModelSimple),
-        # (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        # (str, datetime),
-        # (str, date),
-        # (int, str),
-        # (float, str),
-    ),
-    True: (  # server -> client data
-        (dict, ModelComposed),
-        (list, ModelComposed),
-        (dict, ModelNormal),
-        (list, ModelNormal),
-        (str, ModelSimple),
-        (int, ModelSimple),
-        (float, ModelSimple),
-        (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        (str, datetime),
-        (str, date),
-        # (int, str),
-        # (float, str),
-        (str, file_type)
-    ),
-}
-
-
-def get_simple_class(input_value):
-    """Returns an input_value's simple class that we will use for type checking
-    Python2:
-    float and int will return int, where int is the python3 int backport
-    str and unicode will return str, where str is the python3 str backport
-    Note: float and int ARE both instances of int backport
-    Note: str_py2 and unicode_py2 are NOT both instances of str backport
-
-    Args:
-        input_value (class/class_instance): the item for which we will return
-                                            the simple class
-    """
-    if isinstance(input_value, type):
-        # input_value is a class
-        return input_value
-    elif isinstance(input_value, tuple):
-        return tuple
-    elif isinstance(input_value, list):
-        return list
-    elif isinstance(input_value, dict):
-        return dict
-    elif isinstance(input_value, none_type):
-        return none_type
-    elif isinstance(input_value, file_type):
-        return file_type
-    elif isinstance(input_value, bool):
-        # this must be higher than the int check because
-        # isinstance(True, int) == True
-        return bool
-    elif isinstance(input_value, int):
-        return int
-    elif isinstance(input_value, datetime):
-        # this must be higher than the date check because
-        # isinstance(datetime_instance, date) == True
-        return datetime
-    elif isinstance(input_value, date):
-        return date
-    elif isinstance(input_value, str):
-        return str
-    return type(input_value)
-
-
-def check_allowed_values(allowed_values, input_variable_path, input_values):
-    """Raises an exception if the input_values are not allowed
-
-    Args:
-        allowed_values (dict): the allowed_values dict
-        input_variable_path (tuple): the path to the input variable
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking to see if they are in allowed_values
-    """
-    these_allowed_values = list(allowed_values[input_variable_path].values())
-    if (isinstance(input_values, list)
-            and not set(input_values).issubset(
-                set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values) - set(these_allowed_values))),
-        raise ApiValueError(
-            "Invalid values for `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
-        )
-    elif (isinstance(input_values, dict)
-            and not set(
-                input_values.keys()).issubset(set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values.keys()) - set(these_allowed_values)))
-        raise ApiValueError(
-            "Invalid keys in `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
-        )
-    elif (not isinstance(input_values, (list, dict))
-            and input_values not in these_allowed_values):
-        raise ApiValueError(
-            "Invalid value for `%s` (%s), must be one of %s" %
-            (
-                input_variable_path[0],
-                input_values,
-                these_allowed_values
-            )
-        )
-
-
-def is_json_validation_enabled(schema_keyword, configuration=None):
-    """Returns true if JSON schema validation is enabled for the specified
-    validation keyword. This can be used to skip JSON schema structural validation
-    as requested in the configuration.
-
-    Args:
-        schema_keyword (string): the name of a JSON schema validation keyword.
-        configuration (Configuration): the configuration class.
-    """
-
-    return (configuration is None or
-            not hasattr(configuration, '_disabled_client_side_validations') or
-            schema_keyword not in configuration._disabled_client_side_validations)
-
-
-def check_validations(
-        validations, input_variable_path, input_values,
-        configuration=None):
-    """Raises an exception if the input_values are invalid
-
-    Args:
-        validations (dict): the validation dictionary.
-        input_variable_path (tuple): the path to the input variable.
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking.
-        configuration (Configuration): the configuration class.
-    """
-
-    if input_values is None:
-        return
-
-    current_validations = validations[input_variable_path]
-    if (is_json_validation_enabled('multipleOf', configuration) and
-            'multiple_of' in current_validations and
-            isinstance(input_values, (int, float)) and
-            not (float(input_values) / current_validations['multiple_of']).is_integer()):
-        # Note 'multipleOf' will be as good as the floating point arithmetic.
-        raise ApiValueError(
-            "Invalid value for `%s`, value must be a multiple of "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['multiple_of']
-            )
-        )
-
-    if (is_json_validation_enabled('maxLength', configuration) and
-            'max_length' in current_validations and
-            len(input_values) > current_validations['max_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['max_length']
-            )
-        )
-
-    if (is_json_validation_enabled('minLength', configuration) and
-            'min_length' in current_validations and
-            len(input_values) < current_validations['min_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be greater than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['min_length']
-            )
-        )
-
-    if (is_json_validation_enabled('maxItems', configuration) and
-            'max_items' in current_validations and
-            len(input_values) > current_validations['max_items']):
-        raise ApiValueError(
-            "Invalid value for `%s`, number of items must be less than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['max_items']
-            )
-        )
-
-    if (is_json_validation_enabled('minItems', configuration) and
-            'min_items' in current_validations and
-            len(input_values) < current_validations['min_items']):
-        raise ValueError(
-            "Invalid value for `%s`, number of items must be greater than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['min_items']
-            )
-        )
-
-    items = ('exclusive_maximum', 'inclusive_maximum', 'exclusive_minimum',
-             'inclusive_minimum')
-    if (any(item in current_validations for item in items)):
-        if isinstance(input_values, list):
-            max_val = max(input_values)
-            min_val = min(input_values)
-        elif isinstance(input_values, dict):
-            max_val = max(input_values.values())
-            min_val = min(input_values.values())
-        else:
-            max_val = input_values
-            min_val = input_values
-
-    if (is_json_validation_enabled('exclusiveMaximum', configuration) and
-            'exclusive_maximum' in current_validations and
-            max_val >= current_validations['exclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than `%s`" % (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
-            )
-        )
-
-    if (is_json_validation_enabled('maximum', configuration) and
-            'inclusive_maximum' in current_validations and
-            max_val > current_validations['inclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_maximum']
-            )
-        )
-
-    if (is_json_validation_enabled('exclusiveMinimum', configuration) and
-            'exclusive_minimum' in current_validations and
-            min_val <= current_validations['exclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than `%s`" %
-            (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
-            )
-        )
-
-    if (is_json_validation_enabled('minimum', configuration) and
-            'inclusive_minimum' in current_validations and
-            min_val < current_validations['inclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than or equal "
-            "to `%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_minimum']
-            )
-        )
-    flags = current_validations.get('regex', {}).get('flags', 0)
-    if (is_json_validation_enabled('pattern', configuration) and
-            'regex' in current_validations and
-            not re.search(current_validations['regex']['pattern'],
-                          input_values, flags=flags)):
-        err_msg = r"Invalid value for `%s`, must match regular expression `%s`" % (
-            input_variable_path[0],
-            current_validations['regex']['pattern']
-        )
-        if flags != 0:
-            # Don't print the regex flags if the flags are not
-            # specified in the OAS document.
-            err_msg = r"%s with flags=`%s`" % (err_msg, flags)
-        raise ApiValueError(err_msg)
-
-
-def order_response_types(required_types):
-    """Returns the required types sorted in coercion order
-
-    Args:
-        required_types (list/tuple): collection of classes or instance of
-            list or dict with class information inside it.
-
-    Returns:
-        (list): coercion order sorted collection of classes or instance
-            of list or dict with class information inside it.
-    """
-
-    def index_getter(class_or_instance):
-        if isinstance(class_or_instance, list):
-            return COERCION_INDEX_BY_TYPE[list]
-        elif isinstance(class_or_instance, dict):
-            return COERCION_INDEX_BY_TYPE[dict]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelComposed)):
-            return COERCION_INDEX_BY_TYPE[ModelComposed]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelNormal)):
-            return COERCION_INDEX_BY_TYPE[ModelNormal]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelSimple)):
-            return COERCION_INDEX_BY_TYPE[ModelSimple]
-        elif class_or_instance in COERCION_INDEX_BY_TYPE:
-            return COERCION_INDEX_BY_TYPE[class_or_instance]
-        raise ApiValueError("Unsupported type: %s" % class_or_instance)
-
-    sorted_types = sorted(
-        required_types,
-        key=lambda class_or_instance: index_getter(class_or_instance)
-    )
-    return sorted_types
-
-
-def remove_uncoercible(required_types_classes, current_item, spec_property_naming,
-                       must_convert=True):
-    """Only keeps the type conversions that are possible
-
-    Args:
-        required_types_classes (tuple): tuple of classes that are required
-                          these should be ordered by COERCION_INDEX_BY_TYPE
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        current_item (any): the current item (input data) to be converted
-
-    Keyword Args:
-        must_convert (bool): if True the item to convert is of the wrong
-                          type and we want a big list of coercibles
-                          if False, we want a limited list of coercibles
-
-    Returns:
-        (list): the remaining coercible required types, classes only
-    """
-    current_type_simple = get_simple_class(current_item)
-
-    results_classes = []
-    for required_type_class in required_types_classes:
-        # convert our models to OpenApiModel
-        required_type_class_simplified = required_type_class
-        if isinstance(required_type_class_simplified, type):
-            if issubclass(required_type_class_simplified, ModelComposed):
-                required_type_class_simplified = ModelComposed
-            elif issubclass(required_type_class_simplified, ModelNormal):
-                required_type_class_simplified = ModelNormal
-            elif issubclass(required_type_class_simplified, ModelSimple):
-                required_type_class_simplified = ModelSimple
-
-        if required_type_class_simplified == current_type_simple:
-            # don't consider converting to one's own class
-            continue
-
-        class_pair = (current_type_simple, required_type_class_simplified)
-        if must_convert and class_pair in COERCIBLE_TYPE_PAIRS[spec_property_naming]:
-            results_classes.append(required_type_class)
-        elif class_pair in UPCONVERSION_TYPE_PAIRS:
-            results_classes.append(required_type_class)
-    return results_classes
-
-
-def get_discriminated_classes(cls):
-    """
-    Returns all the classes that a discriminator converts to
-    TODO: lru_cache this
-    """
-    possible_classes = []
-    key = list(cls.discriminator.keys())[0]
-    if is_type_nullable(cls):
-        possible_classes.append(cls)
-    for discr_cls in cls.discriminator[key].values():
-        if hasattr(discr_cls, 'discriminator') and discr_cls.discriminator is not None:
-            possible_classes.extend(get_discriminated_classes(discr_cls))
-        else:
-            possible_classes.append(discr_cls)
-    return possible_classes
-
-
-def get_possible_classes(cls, from_server_context):
-    # TODO: lru_cache this
-    possible_classes = [cls]
-    if from_server_context:
-        return possible_classes
-    if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-        possible_classes = []
-        possible_classes.extend(get_discriminated_classes(cls))
-    elif issubclass(cls, ModelComposed):
-        possible_classes.extend(composed_model_input_classes(cls))
-    return possible_classes
-
-
-def get_required_type_classes(required_types_mixed, spec_property_naming):
-    """Converts the tuple required_types into a tuple and a dict described
-    below
-
-    Args:
-        required_types_mixed (tuple/list): will contain either classes or
-            instance of list or dict
-        spec_property_naming (bool): if True these values came from the
-            server, and we use the data types in our endpoints.
-            If False, we are client side and we need to include
-            oneOf and discriminator classes inside the data types in our endpoints
-
-    Returns:
-        (valid_classes, dict_valid_class_to_child_types_mixed):
-            valid_classes (tuple): the valid classes that the current item
-                                   should be
-            dict_valid_class_to_child_types_mixed (dict):
-                valid_class (class): this is the key
-                child_types_mixed (list/dict/tuple): describes the valid child
-                    types
-    """
-    valid_classes = []
-    child_req_types_by_current_type = {}
-    for required_type in required_types_mixed:
-        if isinstance(required_type, list):
-            valid_classes.append(list)
-            child_req_types_by_current_type[list] = required_type
-        elif isinstance(required_type, tuple):
-            valid_classes.append(tuple)
-            child_req_types_by_current_type[tuple] = required_type
-        elif isinstance(required_type, dict):
-            valid_classes.append(dict)
-            child_req_types_by_current_type[dict] = required_type[str]
-        else:
-            valid_classes.extend(get_possible_classes(required_type, spec_property_naming))
-    return tuple(valid_classes), child_req_types_by_current_type
-
-
-def change_keys_js_to_python(input_dict, model_class):
-    """
-    Converts from javascript_key keys in the input_dict to python_keys in
-    the output dict using the mapping in model_class.
-    If the input_dict contains a key which does not declared in the model_class,
-    the key is added to the output dict as is. The assumption is the model_class
-    may have undeclared properties (additionalProperties attribute in the OAS
-    document).
-    """
-
-    if getattr(model_class, 'attribute_map', None) is None:
-        return input_dict
-    output_dict = {}
-    reversed_attr_map = {value: key for key, value in
-                         model_class.attribute_map.items()}
-    for javascript_key, value in input_dict.items():
-        python_key = reversed_attr_map.get(javascript_key)
-        if python_key is None:
-            # if the key is unknown, it is in error or it is an
-            # additionalProperties variable
-            python_key = javascript_key
-        output_dict[python_key] = value
-    return output_dict
-
-
-def get_type_error(var_value, path_to_item, valid_classes, key_type=False):
-    error_msg = type_error_message(
-        var_name=path_to_item[-1],
-        var_value=var_value,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-    return ApiTypeError(
-        error_msg,
-        path_to_item=path_to_item,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-
-
-def deserialize_primitive(data, klass, path_to_item):
-    """Deserializes string to primitive type.
-
-    :param data: str/int/float
-    :param klass: str/class the class to convert to
-
-    :return: int, float, str, bool, date, datetime
-    """
-    additional_message = ""
-    try:
-        if klass in {datetime, date}:
-            additional_message = (
-                "If you need your parameter to have a fallback "
-                "string value, please set its type as `type: {}` in your "
-                "spec. That allows the value to be any type. "
-            )
-            if klass == datetime:
-                if len(data) < 8:
-                    raise ValueError("This is not a datetime")
-                # The string should be in iso8601 datetime format.
-                parsed_datetime = parse(data)
-                date_only = (
-                    parsed_datetime.hour == 0 and
-                    parsed_datetime.minute == 0 and
-                    parsed_datetime.second == 0 and
-                    parsed_datetime.tzinfo is None and
-                    8 <= len(data) <= 10
-                )
-                if date_only:
-                    raise ValueError("This is a date, not a datetime")
-                return parsed_datetime
-            elif klass == date:
-                if len(data) < 8:
-                    raise ValueError("This is not a date")
-                return parse(data).date()
-        else:
-            converted_value = klass(data)
-            if isinstance(data, str) and klass == float:
-                if str(converted_value) != data:
-                    # '7' -> 7.0 -> '7.0' != '7'
-                    raise ValueError('This is not a float')
-            return converted_value
-    except (OverflowError, ValueError) as ex:
-        # parse can raise OverflowError
-        raise ApiValueError(
-            "{0}Failed to parse {1} as {2}".format(
-                additional_message, repr(data), klass.__name__
-            ),
-            path_to_item=path_to_item
-        ) from ex
-
-
-def get_discriminator_class(model_class,
-                            discr_name,
-                            discr_value, cls_visited):
-    """Returns the child class specified by the discriminator.
-
-    Args:
-        model_class (OpenApiModel): the model class.
-        discr_name (string): the name of the discriminator property.
-        discr_value (any): the discriminator value.
-        cls_visited (list): list of model classes that have been visited.
-            Used to determine the discriminator class without
-            visiting circular references indefinitely.
-
-    Returns:
-        used_model_class (class/None): the chosen child class that will be used
-            to deserialize the data, for example dog.Dog.
-            If a class is not found, None is returned.
-    """
-
-    if model_class in cls_visited:
-        # The class has already been visited and no suitable class was found.
-        return None
-    cls_visited.append(model_class)
-    used_model_class = None
-    if discr_name in model_class.discriminator:
-        class_name_to_discr_class = model_class.discriminator[discr_name]
-        used_model_class = class_name_to_discr_class.get(discr_value)
-    if used_model_class is None:
-        # We didn't find a discriminated class in class_name_to_discr_class.
-        # So look in the ancestor or descendant discriminators
-        # The discriminator mapping may exist in a descendant (anyOf, oneOf)
-        # or ancestor (allOf).
-        # Ancestor example: in the GrandparentAnimal -> ParentPet -> ChildCat
-        #   hierarchy, the discriminator mappings may be defined at any level
-        #   in the hierarchy.
-        # Descendant example:  mammal -> whale/zebra/Pig -> BasquePig/DanishPig
-        #   if we try to make BasquePig from mammal, we need to travel through
-        #   the oneOf descendant discriminators to find BasquePig
-        descendant_classes = model_class._composed_schemas.get('oneOf', ()) + \
-            model_class._composed_schemas.get('anyOf', ())
-        ancestor_classes = model_class._composed_schemas.get('allOf', ())
-        possible_classes = descendant_classes + ancestor_classes
-        for cls in possible_classes:
-            # Check if the schema has inherited discriminators.
-            if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-                used_model_class = get_discriminator_class(
-                    cls, discr_name, discr_value, cls_visited)
-                if used_model_class is not None:
-                    return used_model_class
-    return used_model_class
-
-
-def deserialize_model(model_data, model_class, path_to_item, check_type,
-                      configuration, spec_property_naming):
-    """Deserializes model_data to model instance.
-
-    Args:
-        model_data (int/str/float/bool/none_type/list/dict): data to instantiate the model
-        model_class (OpenApiModel): the model class
-        path_to_item (list): path to the model in the received data
-        check_type (bool): whether to check the data tupe for the values in
-            the model
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-
-    Returns:
-        model instance
-
-    Raise:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-
-    kw_args = dict(_check_type=check_type,
-                   _path_to_item=path_to_item,
-                   _configuration=configuration,
-                   _spec_property_naming=spec_property_naming)
-
-    if issubclass(model_class, ModelSimple):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
-    elif isinstance(model_data, list):
-        return model_class._new_from_openapi_data(*model_data, **kw_args)
-    if isinstance(model_data, dict):
-        kw_args.update(model_data)
-        return model_class._new_from_openapi_data(**kw_args)
-    elif isinstance(model_data, PRIMITIVE_TYPES):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
-
-
-def deserialize_file(response_data, configuration, content_disposition=None):
-    """Deserializes body to file
-
-    Saves response body into a file in a temporary folder,
-    using the filename from the `Content-Disposition` header if provided.
-
-    Args:
-        param response_data (str):  the file data to write
-        configuration (Configuration): the instance to use to convert files
-
-    Keyword Args:
-        content_disposition (str):  the value of the Content-Disposition
-            header
-
-    Returns:
-        (file_type): the deserialized file which is open
-            The user is responsible for closing and reading the file
-    """
-    fd, path = tempfile.mkstemp(dir=configuration.temp_folder_path)
-    os.close(fd)
-    os.remove(path)
-
-    if content_disposition:
-        filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
-                             content_disposition,
-                             flags=re.I)
-        if filename is not None:
-            filename = filename.group(1)
-        else:
-            filename = "default_" + str(uuid.uuid4())
-
-        path = os.path.join(os.path.dirname(path), filename)
-
-    with open(path, "wb") as f:
-        if isinstance(response_data, str):
-            # change str to bytes so we can write it
-            response_data = response_data.encode('utf-8')
-        f.write(response_data)
-
-    f = open(path, "rb")
-    return f
-
-
-def attempt_convert_item(input_value, valid_classes, path_to_item,
-                         configuration, spec_property_naming, key_type=False,
-                         must_convert=False, check_type=True):
-    """
-    Args:
-        input_value (any): the data to convert
-        valid_classes (any): the classes that are valid
-        path_to_item (list): the path to the item to convert
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        key_type (bool): if True we need to convert a key type (not supported)
-        must_convert (bool): if True we must convert
-        check_type (bool): if True we check the type or the returned data in
-            ModelComposed/ModelNormal/ModelSimple instances
-
-    Returns:
-        instance (any) the fixed item
-
-    Raises:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-    valid_classes_ordered = order_response_types(valid_classes)
-    valid_classes_coercible = remove_uncoercible(
-        valid_classes_ordered, input_value, spec_property_naming)
-    if not valid_classes_coercible or key_type:
-        # we do not handle keytype errors, json will take care
-        # of this for us
-        if configuration is None or not configuration.discard_unknown_keys:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=key_type)
-    for valid_class in valid_classes_coercible:
-        try:
-            if issubclass(valid_class, OpenApiModel):
-                return deserialize_model(input_value, valid_class,
-                                         path_to_item, check_type,
-                                         configuration, spec_property_naming)
-            elif valid_class == file_type:
-                return deserialize_file(input_value, configuration)
-            return deserialize_primitive(input_value, valid_class,
-                                         path_to_item)
-        except (ApiTypeError, ApiValueError, ApiKeyError) as conversion_exc:
-            if must_convert:
-                raise conversion_exc
-            # if we have conversion errors when must_convert == False
-            # we ignore the exception and move on to the next class
-            continue
-    # we were unable to convert, must_convert == False
-    return input_value
-
-
-def is_type_nullable(input_type):
-    """
-    Returns true if None is an allowed value for the specified input_type.
-
-    A type is nullable if at least one of the following conditions is true:
-    1. The OAS 'nullable' attribute has been specified,
-    1. The type is the 'null' type,
-    1. The type is a anyOf/oneOf composed schema, and a child schema is
-       the 'null' type.
-    Args:
-        input_type (type): the class of the input_value that we are
-            checking
-    Returns:
-        bool
-    """
-    if input_type is none_type:
-        return True
-    if issubclass(input_type, OpenApiModel) and input_type._nullable:
-        return True
-    if issubclass(input_type, ModelComposed):
-        # If oneOf/anyOf, check if the 'null' type is one of the allowed types.
-        for t in input_type._composed_schemas.get('oneOf', ()):
-            if is_type_nullable(t):
-                return True
-        for t in input_type._composed_schemas.get('anyOf', ()):
-            if is_type_nullable(t):
-                return True
-    return False
-
-
-def is_valid_type(input_class_simple, valid_classes):
-    """
-    Args:
-        input_class_simple (class): the class of the input_value that we are
-            checking
-        valid_classes (tuple): the valid classes that the current item
-            should be
-    Returns:
-        bool
-    """
-    if issubclass(input_class_simple, OpenApiModel) and \
-            valid_classes == (bool, date, datetime, dict, float, int, list, str, none_type,):
-        return True
-    valid_type = input_class_simple in valid_classes
-    if not valid_type and (
-            issubclass(input_class_simple, OpenApiModel) or
-            input_class_simple is none_type):
-        for valid_class in valid_classes:
-            if input_class_simple is none_type and is_type_nullable(valid_class):
-                # Schema is oneOf/anyOf and the 'null' type is one of the allowed types.
-                return True
-            if not (issubclass(valid_class, OpenApiModel) and valid_class.discriminator):
-                continue
-            discr_propertyname_py = list(valid_class.discriminator.keys())[0]
-            discriminator_classes = (
-                valid_class.discriminator[discr_propertyname_py].values()
-            )
-            valid_type = is_valid_type(input_class_simple, discriminator_classes)
-            if valid_type:
-                return True
-    return valid_type
-
-
-def validate_and_convert_types(input_value, required_types_mixed, path_to_item,
-                               spec_property_naming, _check_type, configuration=None):
-    """Raises a TypeError is there is a problem, otherwise returns value
-
-    Args:
-        input_value (any): the data to validate/convert
-        required_types_mixed (list/dict/tuple): A list of
-            valid classes, or a list tuples of valid classes, or a dict where
-            the value is a tuple of value classes
-        path_to_item: (list) the path to the data being validated
-            this stores a list of keys or indices to get to the data being
-            validated
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        _check_type: (boolean) if true, type will be checked and conversion
-            will be attempted.
-        configuration: (Configuration): the configuration class to use
-            when converting file_type items.
-            If passed, conversion will be attempted when possible
-            If not passed, no conversions will be attempted and
-            exceptions will be raised
-
-    Returns:
-        the correctly typed value
-
-    Raises:
-        ApiTypeError
-    """
-    results = get_required_type_classes(required_types_mixed, spec_property_naming)
-    valid_classes, child_req_types_by_current_type = results
-
-    input_class_simple = get_simple_class(input_value)
-    valid_type = is_valid_type(input_class_simple, valid_classes)
-    if not valid_type:
-        if (configuration
-                or (input_class_simple == dict
-                    and dict not in valid_classes)):
-            # if input_value is not valid_type try to convert it
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=True,
-                check_type=_check_type
-            )
-            return converted_instance
-        else:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=False)
-
-    # input_value's type is in valid_classes
-    if len(valid_classes) > 1 and configuration:
-        # there are valid classes which are not the current class
-        valid_classes_coercible = remove_uncoercible(
-            valid_classes, input_value, spec_property_naming, must_convert=False)
-        if valid_classes_coercible:
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes_coercible,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=False,
-                check_type=_check_type
-            )
-            return converted_instance
-
-    if child_req_types_by_current_type == {}:
-        # all types are of the required types and there are no more inner
-        # variables left to look at
-        return input_value
-    inner_required_types = child_req_types_by_current_type.get(
-        type(input_value)
-    )
-    if inner_required_types is None:
-        # for this type, there are not more inner variables left to look at
-        return input_value
-    if isinstance(input_value, list):
-        if input_value == []:
-            # allow an empty list
-            return input_value
-        for index, inner_value in enumerate(input_value):
-            inner_path = list(path_to_item)
-            inner_path.append(index)
-            input_value[index] = validate_and_convert_types(
-                inner_value,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    elif isinstance(input_value, dict):
-        if input_value == {}:
-            # allow an empty dict
-            return input_value
-        for inner_key, inner_val in input_value.items():
-            inner_path = list(path_to_item)
-            inner_path.append(inner_key)
-            if get_simple_class(inner_key) != str:
-                raise get_type_error(inner_key, inner_path, valid_classes,
-                                     key_type=True)
-            input_value[inner_key] = validate_and_convert_types(
-                inner_val,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    return input_value
-
-
-def model_to_dict(model_instance, serialize=True):
-    """Returns the model properties as a dict
-
-    Args:
-        model_instance (one of your model instances): the model instance that
-            will be converted to a dict.
-
-    Keyword Args:
-        serialize (bool): if True, the keys in the dict will be values from
-            attribute_map
-    """
-    result = {}
-
-    def extract_item(item): return (
-        item[0], model_to_dict(
-            item[1], serialize=serialize)) if hasattr(
-        item[1], '_data_store') else item
-
-    model_instances = [model_instance]
-    if model_instance._composed_schemas:
-        model_instances.extend(model_instance._composed_instances)
-    seen_json_attribute_names = set()
-    used_fallback_python_attribute_names = set()
-    py_to_json_map = {}
-    for model_instance in model_instances:
-        for attr, value in model_instance._data_store.items():
-            if serialize:
-                # we use get here because additional property key names do not
-                # exist in attribute_map
-                try:
-                    attr = model_instance.attribute_map[attr]
-                    py_to_json_map.update(model_instance.attribute_map)
-                    seen_json_attribute_names.add(attr)
-                except KeyError:
-                    used_fallback_python_attribute_names.add(attr)
-            if isinstance(value, list):
-                if not value:
-                    # empty list or None
-                    result[attr] = value
-                else:
-                    res = []
-                    for v in value:
-                        if isinstance(v, PRIMITIVE_TYPES) or v is None:
-                            res.append(v)
-                        elif isinstance(v, ModelSimple):
-                            res.append(v.value)
-                        elif isinstance(v, dict):
-                            res.append(dict(map(
-                                extract_item,
-                                v.items()
-                            )))
-                        else:
-                            res.append(model_to_dict(v, serialize=serialize))
-                    result[attr] = res
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    extract_item,
-                    value.items()
-                ))
-            elif isinstance(value, ModelSimple):
-                result[attr] = value.value
-            elif hasattr(value, '_data_store'):
-                result[attr] = model_to_dict(value, serialize=serialize)
-            else:
-                result[attr] = value
-    if serialize:
-        for python_key in used_fallback_python_attribute_names:
-            json_key = py_to_json_map.get(python_key)
-            if json_key is None:
-                continue
-            if python_key == json_key:
-                continue
-            json_key_assigned_no_need_for_python_key = json_key in seen_json_attribute_names
-            if json_key_assigned_no_need_for_python_key:
-                del result[python_key]
-
-    return result
-
-
-def type_error_message(var_value=None, var_name=None, valid_classes=None,
-                       key_type=None):
-    """
-    Keyword Args:
-        var_value (any): the variable which has the type_error
-        var_name (str): the name of the variable which has the typ error
-        valid_classes (tuple): the accepted classes for current_item's
-                                  value
-        key_type (bool): False if our value is a value in a dict
-                         True if it is a key in a dict
-                         False if our item is an item in a list
-    """
-    key_or_value = 'value'
-    if key_type:
-        key_or_value = 'key'
-    valid_classes_phrase = get_valid_classes_phrase(valid_classes)
-    msg = (
-        "Invalid type for variable '{0}'. Required {1} type {2} and "
-        "passed type was {3}".format(
-            var_name,
-            key_or_value,
-            valid_classes_phrase,
-            type(var_value).__name__,
-        )
-    )
-    return msg
-
-
-def get_valid_classes_phrase(input_classes):
-    """Returns a string phrase describing what types are allowed
-    """
-    all_classes = list(input_classes)
-    all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
-    all_class_names = [cls.__name__ for cls in all_classes]
-    if len(all_class_names) == 1:
-        return 'is {0}'.format(all_class_names[0])
-    return "is one of [{0}]".format(", ".join(all_class_names))
-
-
-def get_allof_instances(self, model_args, constant_args):
-    """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            used to make instances
-        constant_args (dict):
-            metadata arguments:
-            _check_type
-            _path_to_item
-            _spec_property_naming
-            _configuration
-            _visited_composed_classes
-
-    Returns
-        composed_instances (list)
-    """
-    composed_instances = []
-    for allof_class in self._composed_schemas['allOf']:
-
-        try:
-            if constant_args.get('_spec_property_naming'):
-                allof_instance = allof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                allof_instance = allof_class(**model_args, **constant_args)
-            composed_instances.append(allof_instance)
-        except Exception as ex:
-            raise ApiValueError(
-                "Invalid inputs given to generate an instance of '%s'. The "
-                "input data was invalid for the allOf schema '%s' in the composed "
-                "schema '%s'. Error=%s" % (
-                    allof_class.__name__,
-                    allof_class.__name__,
-                    self.__class__.__name__,
-                    str(ex)
-                )
-            ) from ex
-    return composed_instances
-
-
-def get_oneof_instance(cls, model_kwargs, constant_kwargs, model_arg=None):
-    """
-    Find the oneOf schema that matches the input data (e.g. payload).
-    If exactly one schema matches the input data, an instance of that schema
-    is returned.
-    If zero or more than one schema match the input data, an exception is raised.
-    In OAS 3.x, the payload MUST, by validation, match exactly one of the
-    schemas described by oneOf.
-
-    Args:
-        cls: the class we are handling
-        model_kwargs (dict): var_name to var_value
-            The input data, e.g. the payload that must match a oneOf schema
-            in the OpenAPI document.
-        constant_kwargs (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Kwargs:
-        model_arg: (int, float, bool, str, date, datetime, ModelSimple, None):
-            the value to assign to a primitive class or ModelSimple class
-            Notes:
-            - this is only passed in when oneOf includes types which are not object
-            - None is used to suppress handling of model_arg, nullable models are handled in __new__
-
-    Returns
-        oneof_instance (instance)
-    """
-    if len(cls._composed_schemas['oneOf']) == 0:
-        return None
-
-    oneof_instances = []
-    # Iterate over each oneOf schema and determine if the input data
-    # matches the oneOf schemas.
-    for oneof_class in cls._composed_schemas['oneOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if oneof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
-
-        single_value_input = allows_single_value_input(oneof_class)
-
-        try:
-            if not single_value_input:
-                if constant_kwargs.get('_spec_property_naming'):
-                    oneof_instance = oneof_class._from_openapi_data(
-                        **model_kwargs, **constant_kwargs)
-                else:
-                    oneof_instance = oneof_class(**model_kwargs, **constant_kwargs)
-            else:
-                if issubclass(oneof_class, ModelSimple):
-                    if constant_kwargs.get('_spec_property_naming'):
-                        oneof_instance = oneof_class._from_openapi_data(
-                            model_arg, **constant_kwargs)
-                    else:
-                        oneof_instance = oneof_class(model_arg, **constant_kwargs)
-                elif oneof_class in PRIMITIVE_TYPES:
-                    oneof_instance = validate_and_convert_types(
-                        model_arg,
-                        (oneof_class,),
-                        constant_kwargs['_path_to_item'],
-                        constant_kwargs['_spec_property_naming'],
-                        constant_kwargs['_check_type'],
-                        configuration=constant_kwargs['_configuration']
-                    )
-            oneof_instances.append(oneof_instance)
-        except Exception:
-            pass
-    if len(oneof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None "
-            "of the oneOf schemas matched the input data." %
-            cls.__name__
-        )
-    elif len(oneof_instances) > 1:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. Multiple "
-            "oneOf schemas matched the inputs, but a max of one is allowed." %
-            cls.__name__
-        )
-    return oneof_instances[0]
-
-
-def get_anyof_instances(self, model_args, constant_args):
-    """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            The input data, e.g. the payload that must match at least one
-            anyOf child schema in the OpenAPI document.
-        constant_args (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Returns
-        anyof_instances (list)
-    """
-    anyof_instances = []
-    if len(self._composed_schemas['anyOf']) == 0:
-        return anyof_instances
-
-    for anyof_class in self._composed_schemas['anyOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if anyof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
-
-        try:
-            if constant_args.get('_spec_property_naming'):
-                anyof_instance = anyof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                anyof_instance = anyof_class(**model_args, **constant_args)
-            anyof_instances.append(anyof_instance)
-        except Exception:
-            pass
-    if len(anyof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None of the "
-            "anyOf schemas matched the inputs." %
-            self.__class__.__name__
-        )
-    return anyof_instances
-
-
-def get_discarded_args(self, composed_instances, model_args):
-    """
-    Gathers the args that were discarded by configuration.discard_unknown_keys
-    """
-    model_arg_keys = model_args.keys()
-    discarded_args = set()
-    # arguments passed to self were already converted to python names
-    # before __init__ was called
-    for instance in composed_instances:
-        if instance.__class__ in self._composed_schemas['allOf']:
-            try:
-                keys = instance.to_dict().keys()
-                discarded_keys = model_args - keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-        else:
-            try:
-                all_keys = set(model_to_dict(instance, serialize=False).keys())
-                js_keys = model_to_dict(instance, serialize=True).keys()
-                all_keys.update(js_keys)
-                discarded_keys = model_arg_keys - all_keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-    return discarded_args
-
-
-def validate_get_composed_info(constant_args, model_args, self):
-    """
-    For composed schemas, generate schema instances for
-    all schemas in the oneOf/anyOf/allOf definition. If additional
-    properties are allowed, also assign those properties on
-    all matched schemas that contain additionalProperties.
-    Openapi schemas are python classes.
-
-    Exceptions are raised if:
-    - 0 or > 1 oneOf schema matches the model_args input data
-    - no anyOf schema matches the model_args input data
-    - any of the allOf schemas do not match the model_args input data
-
-    Args:
-        constant_args (dict): these are the args that every model requires
-        model_args (dict): these are the required and optional spec args that
-            were passed in to make this model
-        self (class): the class that we are instantiating
-            This class contains self._composed_schemas
-
-    Returns:
-        composed_info (list): length three
-            composed_instances (list): the composed instances which are not
-                self
-            var_name_to_model_instances (dict): a dict going from var_name
-                to the model_instance which holds that var_name
-                the model_instance may be self or an instance of one of the
-                classes in self.composed_instances()
-            additional_properties_model_instances (list): a list of the
-                model instances which have the property
-                additional_properties_type. This list can include self
-    """
-    # create composed_instances
-    composed_instances = []
-    allof_instances = get_allof_instances(self, model_args, constant_args)
-    composed_instances.extend(allof_instances)
-    oneof_instance = get_oneof_instance(self.__class__, model_args, constant_args)
-    if oneof_instance is not None:
-        composed_instances.append(oneof_instance)
-    anyof_instances = get_anyof_instances(self, model_args, constant_args)
-    composed_instances.extend(anyof_instances)
-    """
-    set additional_properties_model_instances
-    additional properties must be evaluated at the schema level
-    so self's additional properties are most important
-    If self is a composed schema with:
-    - no properties defined in self
-    - additionalProperties: False
-    Then for object payloads every property is an additional property
-    and they are not allowed, so only empty dict is allowed
-
-    Properties must be set on all matching schemas
-    so when a property is assigned toa composed instance, it must be set on all
-    composed instances regardless of additionalProperties presence
-    keeping it to prevent breaking changes in v5.0.1
-    TODO remove cls._additional_properties_model_instances in 6.0.0
-    """
-    additional_properties_model_instances = []
-    if self.additional_properties_type is not None:
-        additional_properties_model_instances = [self]
-
-    """
-    no need to set properties on self in here, they will be set in __init__
-    By here all composed schema oneOf/anyOf/allOf instances have their properties set using
-    model_args
-    """
-    discarded_args = get_discarded_args(self, composed_instances, model_args)
-
-    # map variable names to composed_instances
-    var_name_to_model_instances = {}
-    for prop_name in model_args:
-        if prop_name not in discarded_args:
-            var_name_to_model_instances[prop_name] = [self] + list(
-                filter(
-                    lambda x: prop_name in x.openapi_types, composed_instances))
-
-    return [
-        composed_instances,
-        var_name_to_model_instances,
-        additional_properties_model_instances,
-        discarded_args
-    ]
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+from datetime import date, datetime  # noqa: F401
+from copy import deepcopy
+import inspect
+import io
+import os
+import pprint
+import re
+import tempfile
+import uuid
+
+from dateutil.parser import parse
+
+from invision_client.exceptions import (
+    ApiKeyError,
+    ApiAttributeError,
+    ApiTypeError,
+    ApiValueError,
+)
+
+none_type = type(None)
+file_type = io.IOBase
+
+
+def convert_js_args_to_python_args(fn):
+    from functools import wraps
+    @wraps(fn)
+    def wrapped_init(_self, *args, **kwargs):
+        """
+        An attribute named `self` received from the api will conflicts with the reserved `self`
+        parameter of a class method. During generation, `self` attributes are mapped
+        to `_self` in models. Here, we name `_self` instead of `self` to avoid conflicts.
+        """
+        spec_property_naming = kwargs.get('_spec_property_naming', False)
+        if spec_property_naming:
+            kwargs = change_keys_js_to_python(
+                kwargs, _self if isinstance(
+                    _self, type) else _self.__class__)
+        return fn(_self, *args, **kwargs)
+    return wrapped_init
+
+
+class cached_property(object):
+    # this caches the result of the function call for fn with no inputs
+    # use this as a decorator on function methods that you want converted
+    # into cached properties
+    result_key = '_results'
+
+    def __init__(self, fn):
+        self._fn = fn
+
+    def __get__(self, instance, cls=None):
+        if self.result_key in vars(self):
+            return vars(self)[self.result_key]
+        else:
+            result = self._fn()
+            setattr(self, self.result_key, result)
+            return result
+
+
+PRIMITIVE_TYPES = (list, float, int, bool, datetime, date, str, file_type)
+
+
+def allows_single_value_input(cls):
+    """
+    This function returns True if the input composed schema model or any
+    descendant model allows a value only input
+    This is true for cases where oneOf contains items like:
+    oneOf:
+      - float
+      - NumberWithValidation
+      - StringEnum
+      - ArrayModel
+      - null
+    TODO: lru_cache this
+    """
+    if (
+        issubclass(cls, ModelSimple) or
+        cls in PRIMITIVE_TYPES
+    ):
+        return True
+    elif issubclass(cls, ModelComposed):
+        if not cls._composed_schemas['oneOf']:
+            return False
+        return any(allows_single_value_input(c) for c in cls._composed_schemas['oneOf'])
+    return False
+
+
+def composed_model_input_classes(cls):
+    """
+    This function returns a list of the possible models that can be accepted as
+    inputs.
+    TODO: lru_cache this
+    """
+    if issubclass(cls, ModelSimple) or cls in PRIMITIVE_TYPES:
+        return [cls]
+    elif issubclass(cls, ModelNormal):
+        if cls.discriminator is None:
+            return [cls]
+        else:
+            return get_discriminated_classes(cls)
+    elif issubclass(cls, ModelComposed):
+        if not cls._composed_schemas['oneOf']:
+            return []
+        if cls.discriminator is None:
+            input_classes = []
+            for c in cls._composed_schemas['oneOf']:
+                input_classes.extend(composed_model_input_classes(c))
+            return input_classes
+        else:
+            return get_discriminated_classes(cls)
+    return []
+
+
+class OpenApiModel(object):
+    """The base class for all OpenAPIModels"""
+
+    def set_attribute(self, name, value):
+        # this is only used to set properties on self
+
+        path_to_item = []
+        if self._path_to_item:
+            path_to_item.extend(self._path_to_item)
+        path_to_item.append(name)
+
+        if name in self.openapi_types:
+            required_types_mixed = self.openapi_types[name]
+        elif self.additional_properties_type is None:
+            raise ApiAttributeError(
+                "{0} has no attribute '{1}'".format(
+                    type(self).__name__, name),
+                path_to_item
+            )
+        elif self.additional_properties_type is not None:
+            required_types_mixed = self.additional_properties_type
+
+        if get_simple_class(name) != str:
+            error_msg = type_error_message(
+                var_name=name,
+                var_value=name,
+                valid_classes=(str,),
+                key_type=True
+            )
+            raise ApiTypeError(
+                error_msg,
+                path_to_item=path_to_item,
+                valid_classes=(str,),
+                key_type=True
+            )
+
+        if self._check_type:
+            value = validate_and_convert_types(
+                value, required_types_mixed, path_to_item, self._spec_property_naming,
+                self._check_type, configuration=self._configuration)
+        if (name,) in self.allowed_values:
+            check_allowed_values(
+                self.allowed_values,
+                (name,),
+                value
+            )
+        if (name,) in self.validations:
+            check_validations(
+                self.validations,
+                (name,),
+                value,
+                self._configuration
+            )
+        self.__dict__['_data_store'][name] = value
+
+    def __repr__(self):
+        """For `print` and `pprint`"""
+        return self.to_str()
+
+    def __ne__(self, other):
+        """Returns true if both objects are not equal"""
+        return not self == other
+
+    def __setattr__(self, attr, value):
+        """set the value of an attribute using dot notation: `instance.attr = val`"""
+        self[attr] = value
+
+    def __getattr__(self, attr):
+        """get the value of an attribute using dot notation: `instance.attr`"""
+        return self.__getitem__(attr)
+
+    def __copy__(self):
+        cls = self.__class__
+        if self.get("_spec_property_naming", False):
+            return cls._new_from_openapi_data(**self.__dict__)
+        else:
+            return cls.__new__(cls, **self.__dict__)
+
+    def __deepcopy__(self, memo):
+        cls = self.__class__
+
+        if self.get("_spec_property_naming", False):
+            new_inst = cls._new_from_openapi_data()
+        else:
+            new_inst = cls.__new__(cls, **self.__dict__)
+
+        for k, v in self.__dict__.items():
+            setattr(new_inst, k, deepcopy(v, memo))
+        return new_inst
+
+
+    def __new__(cls, *args, **kwargs):
+        # this function uses the discriminator to
+        # pick a new schema/class to instantiate because a discriminator
+        # propertyName value was passed in
+
+        if len(args) == 1:
+            arg = args[0]
+            if arg is None and is_type_nullable(cls):
+                # The input data is the 'null' value and the type is nullable.
+                return None
+
+            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
+                model_kwargs = {}
+                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
+                return oneof_instance
+
+        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
+        if (
+            cls.discriminator is None or
+            cls in visited_composed_classes
+        ):
+            # Use case 1: this openapi schema (cls) does not have a discriminator
+            # Use case 2: we have already visited this class before and are sure that we
+            # want to instantiate it this time. We have visited this class deserializing
+            # a payload with a discriminator. During that process we traveled through
+            # this class but did not make an instance of it. Now we are making an
+            # instance of a composed class which contains cls in it, so this time make an instance of cls.
+            #
+            # Here's an example of use case 2: If Animal has a discriminator
+            # petType and we pass in "Dog", and the class Dog
+            # allOf includes Animal, we move through Animal
+            # once using the discriminator, and pick Dog.
+            # Then in the composed schema dog Dog, we will make an instance of the
+            # Animal class (because Dal has allOf: Animal) but this time we won't travel
+            # through Animal's discriminator because we passed in
+            # _visited_composed_classes = (Animal,)
+
+            return super(OpenApiModel, cls).__new__(cls)
+
+        # Get the name and value of the discriminator property.
+        # The discriminator name is obtained from the discriminator meta-data
+        # and the discriminator value is obtained from the input data.
+        discr_propertyname_py = list(cls.discriminator.keys())[0]
+        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
+        if discr_propertyname_js in kwargs:
+            discr_value = kwargs[discr_propertyname_js]
+        elif discr_propertyname_py in kwargs:
+            discr_value = kwargs[discr_propertyname_py]
+        else:
+            # The input data does not contain the discriminator property.
+            path_to_item = kwargs.get('_path_to_item', ())
+            raise ApiValueError(
+                "Cannot deserialize input data due to missing discriminator. "
+                "The discriminator property '%s' is missing at path: %s" %
+                (discr_propertyname_js, path_to_item)
+            )
+
+        # Implementation note: the last argument to get_discriminator_class
+        # is a list of visited classes. get_discriminator_class may recursively
+        # call itself and update the list of visited classes, and the initial
+        # value must be an empty list. Hence not using 'visited_composed_classes'
+        new_cls = get_discriminator_class(
+            cls, discr_propertyname_py, discr_value, [])
+        if new_cls is None:
+            path_to_item = kwargs.get('_path_to_item', ())
+            disc_prop_value = kwargs.get(
+                discr_propertyname_js, kwargs.get(discr_propertyname_py))
+            raise ApiValueError(
+                "Cannot deserialize input data due to invalid discriminator "
+                "value. The OpenAPI document has no mapping for discriminator "
+                "property '%s'='%s' at path: %s" %
+                (discr_propertyname_js, disc_prop_value, path_to_item)
+            )
+
+        if new_cls in visited_composed_classes:
+            # if we are making an instance of a composed schema Descendent
+            # which allOf includes Ancestor, then Ancestor contains
+            # a discriminator that includes Descendent.
+            # So if we make an instance of Descendent, we have to make an
+            # instance of Ancestor to hold the allOf properties.
+            # This code detects that use case and makes the instance of Ancestor
+            # For example:
+            # When making an instance of Dog, _visited_composed_classes = (Dog,)
+            # then we make an instance of Animal to include in dog._composed_instances
+            # so when we are here, cls is Animal
+            # cls.discriminator != None
+            # cls not in _visited_composed_classes
+            # new_cls = Dog
+            # but we know we know that we already have Dog
+            # because it is in visited_composed_classes
+            # so make Animal here
+            return super(OpenApiModel, cls).__new__(cls)
+
+        # Build a list containing all oneOf and anyOf descendants.
+        oneof_anyof_classes = None
+        if cls._composed_schemas is not None:
+            oneof_anyof_classes = (
+                cls._composed_schemas.get('oneOf', ()) +
+                cls._composed_schemas.get('anyOf', ()))
+        oneof_anyof_child = new_cls in oneof_anyof_classes
+        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
+
+        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
+            # Validate that we can make self because when we make the
+            # new_cls it will not include the allOf validations in self
+            self_inst = super(OpenApiModel, cls).__new__(cls)
+            self_inst.__init__(*args, **kwargs)
+
+        if kwargs.get("_spec_property_naming", False):
+            # when true, implies new is from deserialization
+            new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
+        else:
+            new_inst = new_cls.__new__(new_cls, *args, **kwargs)
+            new_inst.__init__(*args, **kwargs)
+
+        return new_inst
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _new_from_openapi_data(cls, *args, **kwargs):
+        # this function uses the discriminator to
+        # pick a new schema/class to instantiate because a discriminator
+        # propertyName value was passed in
+
+        if len(args) == 1:
+            arg = args[0]
+            if arg is None and is_type_nullable(cls):
+                # The input data is the 'null' value and the type is nullable.
+                return None
+
+            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
+                model_kwargs = {}
+                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
+                return oneof_instance
+
+        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
+        if (
+            cls.discriminator is None or
+            cls in visited_composed_classes
+        ):
+            # Use case 1: this openapi schema (cls) does not have a discriminator
+            # Use case 2: we have already visited this class before and are sure that we
+            # want to instantiate it this time. We have visited this class deserializing
+            # a payload with a discriminator. During that process we traveled through
+            # this class but did not make an instance of it. Now we are making an
+            # instance of a composed class which contains cls in it, so this time make an instance of cls.
+            #
+            # Here's an example of use case 2: If Animal has a discriminator
+            # petType and we pass in "Dog", and the class Dog
+            # allOf includes Animal, we move through Animal
+            # once using the discriminator, and pick Dog.
+            # Then in the composed schema dog Dog, we will make an instance of the
+            # Animal class (because Dal has allOf: Animal) but this time we won't travel
+            # through Animal's discriminator because we passed in
+            # _visited_composed_classes = (Animal,)
+
+            return cls._from_openapi_data(*args, **kwargs)
+
+        # Get the name and value of the discriminator property.
+        # The discriminator name is obtained from the discriminator meta-data
+        # and the discriminator value is obtained from the input data.
+        discr_propertyname_py = list(cls.discriminator.keys())[0]
+        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
+        if discr_propertyname_js in kwargs:
+            discr_value = kwargs[discr_propertyname_js]
+        elif discr_propertyname_py in kwargs:
+            discr_value = kwargs[discr_propertyname_py]
+        else:
+            # The input data does not contain the discriminator property.
+            path_to_item = kwargs.get('_path_to_item', ())
+            raise ApiValueError(
+                "Cannot deserialize input data due to missing discriminator. "
+                "The discriminator property '%s' is missing at path: %s" %
+                (discr_propertyname_js, path_to_item)
+            )
+
+        # Implementation note: the last argument to get_discriminator_class
+        # is a list of visited classes. get_discriminator_class may recursively
+        # call itself and update the list of visited classes, and the initial
+        # value must be an empty list. Hence not using 'visited_composed_classes'
+        new_cls = get_discriminator_class(
+            cls, discr_propertyname_py, discr_value, [])
+        if new_cls is None:
+            path_to_item = kwargs.get('_path_to_item', ())
+            disc_prop_value = kwargs.get(
+                discr_propertyname_js, kwargs.get(discr_propertyname_py))
+            raise ApiValueError(
+                "Cannot deserialize input data due to invalid discriminator "
+                "value. The OpenAPI document has no mapping for discriminator "
+                "property '%s'='%s' at path: %s" %
+                (discr_propertyname_js, disc_prop_value, path_to_item)
+            )
+
+        if new_cls in visited_composed_classes:
+            # if we are making an instance of a composed schema Descendent
+            # which allOf includes Ancestor, then Ancestor contains
+            # a discriminator that includes Descendent.
+            # So if we make an instance of Descendent, we have to make an
+            # instance of Ancestor to hold the allOf properties.
+            # This code detects that use case and makes the instance of Ancestor
+            # For example:
+            # When making an instance of Dog, _visited_composed_classes = (Dog,)
+            # then we make an instance of Animal to include in dog._composed_instances
+            # so when we are here, cls is Animal
+            # cls.discriminator != None
+            # cls not in _visited_composed_classes
+            # new_cls = Dog
+            # but we know we know that we already have Dog
+            # because it is in visited_composed_classes
+            # so make Animal here
+            return cls._from_openapi_data(*args, **kwargs)
+
+        # Build a list containing all oneOf and anyOf descendants.
+        oneof_anyof_classes = None
+        if cls._composed_schemas is not None:
+            oneof_anyof_classes = (
+                cls._composed_schemas.get('oneOf', ()) +
+                cls._composed_schemas.get('anyOf', ()))
+        oneof_anyof_child = new_cls in oneof_anyof_classes
+        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
+
+        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
+            # Validate that we can make self because when we make the
+            # new_cls it will not include the allOf validations in self
+            self_inst = cls._from_openapi_data(*args, **kwargs)
+
+        new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
+        return new_inst
+
+
+class ModelSimple(OpenApiModel):
+    """the parent class of models whose type != object in their
+    swagger/openapi"""
+
+    def __setitem__(self, name, value):
+        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
+        if name in self.required_properties:
+            self.__dict__[name] = value
+            return
+
+        self.set_attribute(name, value)
+
+    def get(self, name, default=None):
+        """returns the value of an attribute or some default value if the attribute was not set"""
+        if name in self.required_properties:
+            return self.__dict__[name]
+
+        return self.__dict__['_data_store'].get(name, default)
+
+    def __getitem__(self, name):
+        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
+        if name in self:
+            return self.get(name)
+
+        raise ApiAttributeError(
+            "{0} has no attribute '{1}'".format(
+                type(self).__name__, name),
+            [e for e in [self._path_to_item, name] if e]
+        )
+
+    def __contains__(self, name):
+        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
+        if name in self.required_properties:
+            return name in self.__dict__
+
+        return name in self.__dict__['_data_store']
+
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return str(self.value)
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, self.__class__):
+            return False
+
+        this_val = self._data_store['value']
+        that_val = other._data_store['value']
+        types = set()
+        types.add(this_val.__class__)
+        types.add(that_val.__class__)
+        vals_equal = this_val == that_val
+        return vals_equal
+
+
+class ModelNormal(OpenApiModel):
+    """the parent class of models whose type == object in their
+    swagger/openapi"""
+
+    def __setitem__(self, name, value):
+        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
+        if name in self.required_properties:
+            self.__dict__[name] = value
+            return
+
+        self.set_attribute(name, value)
+
+    def get(self, name, default=None):
+        """returns the value of an attribute or some default value if the attribute was not set"""
+        if name in self.required_properties:
+            return self.__dict__[name]
+
+        return self.__dict__['_data_store'].get(name, default)
+
+    def __getitem__(self, name):
+        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
+        if name in self:
+            return self.get(name)
+
+        raise ApiAttributeError(
+            "{0} has no attribute '{1}'".format(
+                type(self).__name__, name),
+            [e for e in [self._path_to_item, name] if e]
+        )
+
+    def __contains__(self, name):
+        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
+        if name in self.required_properties:
+            return name in self.__dict__
+
+        return name in self.__dict__['_data_store']
+
+    def to_dict(self):
+        """Returns the model properties as a dict"""
+        return model_to_dict(self, serialize=False)
+
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return pprint.pformat(self.to_dict())
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, self.__class__):
+            return False
+
+        if not set(self._data_store.keys()) == set(other._data_store.keys()):
+            return False
+        for _var_name, this_val in self._data_store.items():
+            that_val = other._data_store[_var_name]
+            types = set()
+            types.add(this_val.__class__)
+            types.add(that_val.__class__)
+            vals_equal = this_val == that_val
+            if not vals_equal:
+                return False
+        return True
+
+
+class ModelComposed(OpenApiModel):
+    """the parent class of models whose type == object in their
+    swagger/openapi and have oneOf/allOf/anyOf
+
+    When one sets a property we use var_name_to_model_instances to store the value in
+    the correct class instances + run any type checking + validation code.
+    When one gets a property we use var_name_to_model_instances to get the value
+    from the correct class instances.
+    This allows multiple composed schemas to contain the same property with additive
+    constraints on the value.
+
+    _composed_schemas (dict) stores the anyOf/allOf/oneOf classes
+    key (str): allOf/oneOf/anyOf
+    value (list): the classes in the XOf definition.
+        Note: none_type can be included when the openapi document version >= 3.1.0
+    _composed_instances (list): stores a list of instances of the composed schemas
+    defined in _composed_schemas. When properties are accessed in the self instance,
+    they are returned from the self._data_store or the data stores in the instances
+    in self._composed_schemas
+    _var_name_to_model_instances (dict): maps between a variable name on self and
+    the composed instances (self included) which contain that data
+    key (str): property name
+    value (list): list of class instances, self or instances in _composed_instances
+    which contain the value that the key is referring to.
+    """
+
+    def __setitem__(self, name, value):
+        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
+        if name in self.required_properties:
+            self.__dict__[name] = value
+            return
+
+        """
+        Use cases:
+        1. additional_properties_type is None (additionalProperties == False in spec)
+            Check for property presence in self.openapi_types
+            if not present then throw an error
+            if present set in self, set attribute
+            always set on composed schemas
+        2.  additional_properties_type exists
+            set attribute on self
+            always set on composed schemas
+        """
+        if self.additional_properties_type is None:
+            """
+            For an attribute to exist on a composed schema it must:
+            - fulfill schema_requirements in the self composed schema not considering oneOf/anyOf/allOf schemas AND
+            - fulfill schema_requirements in each oneOf/anyOf/allOf schemas
+
+            schema_requirements:
+            For an attribute to exist on a schema it must:
+            - be present in properties at the schema OR
+            - have additionalProperties unset (defaults additionalProperties = any type) OR
+            - have additionalProperties set
+            """
+            if name not in self.openapi_types:
+                raise ApiAttributeError(
+                    "{0} has no attribute '{1}'".format(
+                        type(self).__name__, name),
+                    [e for e in [self._path_to_item, name] if e]
+                )
+        # attribute must be set on self and composed instances
+        self.set_attribute(name, value)
+        for model_instance in self._composed_instances:
+            setattr(model_instance, name, value)
+        if name not in self._var_name_to_model_instances:
+            # we assigned an additional property
+            self.__dict__['_var_name_to_model_instances'][name] = self._composed_instances + [self]
+        return None
+
+    __unset_attribute_value__ = object()
+
+    def get(self, name, default=None):
+        """returns the value of an attribute or some default value if the attribute was not set"""
+        if name in self.required_properties:
+            return self.__dict__[name]
+
+        # get the attribute from the correct instance
+        model_instances = self._var_name_to_model_instances.get(name)
+        values = []
+        # A composed model stores self and child (oneof/anyOf/allOf) models under
+        # self._var_name_to_model_instances.
+        # Any property must exist in self and all model instances
+        # The value stored in all model instances must be the same
+        if model_instances:
+            for model_instance in model_instances:
+                if name in model_instance._data_store:
+                    v = model_instance._data_store[name]
+                    if v not in values:
+                        values.append(v)
+        len_values = len(values)
+        if len_values == 0:
+            return default
+        elif len_values == 1:
+            return values[0]
+        elif len_values > 1:
+            raise ApiValueError(
+                "Values stored for property {0} in {1} differ when looking "
+                "at self and self's composed instances. All values must be "
+                "the same".format(name, type(self).__name__),
+                [e for e in [self._path_to_item, name] if e]
+            )
+
+    def __getitem__(self, name):
+        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
+        value = self.get(name, self.__unset_attribute_value__)
+        if value is self.__unset_attribute_value__:
+            raise ApiAttributeError(
+                "{0} has no attribute '{1}'".format(
+                    type(self).__name__, name),
+                    [e for e in [self._path_to_item, name] if e]
+            )
+        return value
+
+    def __contains__(self, name):
+        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
+
+        if name in self.required_properties:
+            return name in self.__dict__
+
+        model_instances = self._var_name_to_model_instances.get(
+            name, self._additional_properties_model_instances)
+
+        if model_instances:
+            for model_instance in model_instances:
+                if name in model_instance._data_store:
+                    return True
+
+        return False
+
+    def to_dict(self):
+        """Returns the model properties as a dict"""
+        return model_to_dict(self, serialize=False)
+
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return pprint.pformat(self.to_dict())
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, self.__class__):
+            return False
+
+        if not set(self._data_store.keys()) == set(other._data_store.keys()):
+            return False
+        for _var_name, this_val in self._data_store.items():
+            that_val = other._data_store[_var_name]
+            types = set()
+            types.add(this_val.__class__)
+            types.add(that_val.__class__)
+            vals_equal = this_val == that_val
+            if not vals_equal:
+                return False
+        return True
+
+
+COERCION_INDEX_BY_TYPE = {
+    ModelComposed: 0,
+    ModelNormal: 1,
+    ModelSimple: 2,
+    none_type: 3,    # The type of 'None'.
+    list: 4,
+    dict: 5,
+    float: 6,
+    int: 7,
+    bool: 8,
+    datetime: 9,
+    date: 10,
+    str: 11,
+    file_type: 12,   # 'file_type' is an alias for the built-in 'file' or 'io.IOBase' type.
+}
+
+# these are used to limit what type conversions we try to do
+# when we have a valid type already and we want to try converting
+# to another type
+UPCONVERSION_TYPE_PAIRS = (
+    (str, datetime),
+    (str, date),
+    # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
+    (int, float),
+    (list, ModelComposed),
+    (dict, ModelComposed),
+    (str, ModelComposed),
+    (int, ModelComposed),
+    (float, ModelComposed),
+    (list, ModelComposed),
+    (list, ModelNormal),
+    (dict, ModelNormal),
+    (str, ModelSimple),
+    (int, ModelSimple),
+    (float, ModelSimple),
+    (list, ModelSimple),
+)
+
+COERCIBLE_TYPE_PAIRS = {
+    False: (  # client instantiation of a model with client data
+        # (dict, ModelComposed),
+        # (list, ModelComposed),
+        # (dict, ModelNormal),
+        # (list, ModelNormal),
+        # (str, ModelSimple),
+        # (int, ModelSimple),
+        # (float, ModelSimple),
+        # (list, ModelSimple),
+        # (str, int),
+        # (str, float),
+        # (str, datetime),
+        # (str, date),
+        # (int, str),
+        # (float, str),
+    ),
+    True: (  # server -> client data
+        (dict, ModelComposed),
+        (list, ModelComposed),
+        (dict, ModelNormal),
+        (list, ModelNormal),
+        (str, ModelSimple),
+        (int, ModelSimple),
+        (float, ModelSimple),
+        (list, ModelSimple),
+        # (str, int),
+        # (str, float),
+        (str, datetime),
+        (str, date),
+        # (int, str),
+        # (float, str),
+        (str, file_type)
+    ),
+}
+
+
+def get_simple_class(input_value):
+    """Returns an input_value's simple class that we will use for type checking
+    Python2:
+    float and int will return int, where int is the python3 int backport
+    str and unicode will return str, where str is the python3 str backport
+    Note: float and int ARE both instances of int backport
+    Note: str_py2 and unicode_py2 are NOT both instances of str backport
+
+    Args:
+        input_value (class/class_instance): the item for which we will return
+                                            the simple class
+    """
+    if isinstance(input_value, type):
+        # input_value is a class
+        return input_value
+    elif isinstance(input_value, tuple):
+        return tuple
+    elif isinstance(input_value, list):
+        return list
+    elif isinstance(input_value, dict):
+        return dict
+    elif isinstance(input_value, none_type):
+        return none_type
+    elif isinstance(input_value, file_type):
+        return file_type
+    elif isinstance(input_value, bool):
+        # this must be higher than the int check because
+        # isinstance(True, int) == True
+        return bool
+    elif isinstance(input_value, int):
+        return int
+    elif isinstance(input_value, datetime):
+        # this must be higher than the date check because
+        # isinstance(datetime_instance, date) == True
+        return datetime
+    elif isinstance(input_value, date):
+        return date
+    elif isinstance(input_value, str):
+        return str
+    return type(input_value)
+
+
+def check_allowed_values(allowed_values, input_variable_path, input_values):
+    """Raises an exception if the input_values are not allowed
+
+    Args:
+        allowed_values (dict): the allowed_values dict
+        input_variable_path (tuple): the path to the input variable
+        input_values (list/str/int/float/date/datetime): the values that we
+            are checking to see if they are in allowed_values
+    """
+    these_allowed_values = list(allowed_values[input_variable_path].values())
+    if (isinstance(input_values, list)
+            and not set(input_values).issubset(
+                set(these_allowed_values))):
+        invalid_values = ", ".join(
+            map(str, set(input_values) - set(these_allowed_values))),
+        raise ApiValueError(
+            "Invalid values for `%s` [%s], must be a subset of [%s]" %
+            (
+                input_variable_path[0],
+                invalid_values,
+                ", ".join(map(str, these_allowed_values))
+            )
+        )
+    elif (isinstance(input_values, dict)
+            and not set(
+                input_values.keys()).issubset(set(these_allowed_values))):
+        invalid_values = ", ".join(
+            map(str, set(input_values.keys()) - set(these_allowed_values)))
+        raise ApiValueError(
+            "Invalid keys in `%s` [%s], must be a subset of [%s]" %
+            (
+                input_variable_path[0],
+                invalid_values,
+                ", ".join(map(str, these_allowed_values))
+            )
+        )
+    elif (not isinstance(input_values, (list, dict))
+            and input_values not in these_allowed_values):
+        raise ApiValueError(
+            "Invalid value for `%s` (%s), must be one of %s" %
+            (
+                input_variable_path[0],
+                input_values,
+                these_allowed_values
+            )
+        )
+
+
+def is_json_validation_enabled(schema_keyword, configuration=None):
+    """Returns true if JSON schema validation is enabled for the specified
+    validation keyword. This can be used to skip JSON schema structural validation
+    as requested in the configuration.
+
+    Args:
+        schema_keyword (string): the name of a JSON schema validation keyword.
+        configuration (Configuration): the configuration class.
+    """
+
+    return (configuration is None or
+            not hasattr(configuration, '_disabled_client_side_validations') or
+            schema_keyword not in configuration._disabled_client_side_validations)
+
+
+def check_validations(
+        validations, input_variable_path, input_values,
+        configuration=None):
+    """Raises an exception if the input_values are invalid
+
+    Args:
+        validations (dict): the validation dictionary.
+        input_variable_path (tuple): the path to the input variable.
+        input_values (list/str/int/float/date/datetime): the values that we
+            are checking.
+        configuration (Configuration): the configuration class.
+    """
+
+    if input_values is None:
+        return
+
+    current_validations = validations[input_variable_path]
+    if (is_json_validation_enabled('multipleOf', configuration) and
+            'multiple_of' in current_validations and
+            isinstance(input_values, (int, float)) and
+            not (float(input_values) / current_validations['multiple_of']).is_integer()):
+        # Note 'multipleOf' will be as good as the floating point arithmetic.
+        raise ApiValueError(
+            "Invalid value for `%s`, value must be a multiple of "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['multiple_of']
+            )
+        )
+
+    if (is_json_validation_enabled('maxLength', configuration) and
+            'max_length' in current_validations and
+            len(input_values) > current_validations['max_length']):
+        raise ApiValueError(
+            "Invalid value for `%s`, length must be less than or equal to "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['max_length']
+            )
+        )
+
+    if (is_json_validation_enabled('minLength', configuration) and
+            'min_length' in current_validations and
+            len(input_values) < current_validations['min_length']):
+        raise ApiValueError(
+            "Invalid value for `%s`, length must be greater than or equal to "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['min_length']
+            )
+        )
+
+    if (is_json_validation_enabled('maxItems', configuration) and
+            'max_items' in current_validations and
+            len(input_values) > current_validations['max_items']):
+        raise ApiValueError(
+            "Invalid value for `%s`, number of items must be less than or "
+            "equal to `%s`" % (
+                input_variable_path[0],
+                current_validations['max_items']
+            )
+        )
+
+    if (is_json_validation_enabled('minItems', configuration) and
+            'min_items' in current_validations and
+            len(input_values) < current_validations['min_items']):
+        raise ValueError(
+            "Invalid value for `%s`, number of items must be greater than or "
+            "equal to `%s`" % (
+                input_variable_path[0],
+                current_validations['min_items']
+            )
+        )
+
+    items = ('exclusive_maximum', 'inclusive_maximum', 'exclusive_minimum',
+             'inclusive_minimum')
+    if (any(item in current_validations for item in items)):
+        if isinstance(input_values, list):
+            max_val = max(input_values)
+            min_val = min(input_values)
+        elif isinstance(input_values, dict):
+            max_val = max(input_values.values())
+            min_val = min(input_values.values())
+        else:
+            max_val = input_values
+            min_val = input_values
+
+    if (is_json_validation_enabled('exclusiveMaximum', configuration) and
+            'exclusive_maximum' in current_validations and
+            max_val >= current_validations['exclusive_maximum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value less than `%s`" % (
+                input_variable_path[0],
+                current_validations['exclusive_maximum']
+            )
+        )
+
+    if (is_json_validation_enabled('maximum', configuration) and
+            'inclusive_maximum' in current_validations and
+            max_val > current_validations['inclusive_maximum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value less than or equal to "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['inclusive_maximum']
+            )
+        )
+
+    if (is_json_validation_enabled('exclusiveMinimum', configuration) and
+            'exclusive_minimum' in current_validations and
+            min_val <= current_validations['exclusive_minimum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value greater than `%s`" %
+            (
+                input_variable_path[0],
+                current_validations['exclusive_maximum']
+            )
+        )
+
+    if (is_json_validation_enabled('minimum', configuration) and
+            'inclusive_minimum' in current_validations and
+            min_val < current_validations['inclusive_minimum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value greater than or equal "
+            "to `%s`" % (
+                input_variable_path[0],
+                current_validations['inclusive_minimum']
+            )
+        )
+    flags = current_validations.get('regex', {}).get('flags', 0)
+    if (is_json_validation_enabled('pattern', configuration) and
+            'regex' in current_validations and
+            not re.search(current_validations['regex']['pattern'],
+                          input_values, flags=flags)):
+        err_msg = r"Invalid value for `%s`, must match regular expression `%s`" % (
+            input_variable_path[0],
+            current_validations['regex']['pattern']
+        )
+        if flags != 0:
+            # Don't print the regex flags if the flags are not
+            # specified in the OAS document.
+            err_msg = r"%s with flags=`%s`" % (err_msg, flags)
+        raise ApiValueError(err_msg)
+
+
+def order_response_types(required_types):
+    """Returns the required types sorted in coercion order
+
+    Args:
+        required_types (list/tuple): collection of classes or instance of
+            list or dict with class information inside it.
+
+    Returns:
+        (list): coercion order sorted collection of classes or instance
+            of list or dict with class information inside it.
+    """
+
+    def index_getter(class_or_instance):
+        if isinstance(class_or_instance, list):
+            return COERCION_INDEX_BY_TYPE[list]
+        elif isinstance(class_or_instance, dict):
+            return COERCION_INDEX_BY_TYPE[dict]
+        elif (inspect.isclass(class_or_instance)
+                and issubclass(class_or_instance, ModelComposed)):
+            return COERCION_INDEX_BY_TYPE[ModelComposed]
+        elif (inspect.isclass(class_or_instance)
+                and issubclass(class_or_instance, ModelNormal)):
+            return COERCION_INDEX_BY_TYPE[ModelNormal]
+        elif (inspect.isclass(class_or_instance)
+                and issubclass(class_or_instance, ModelSimple)):
+            return COERCION_INDEX_BY_TYPE[ModelSimple]
+        elif class_or_instance in COERCION_INDEX_BY_TYPE:
+            return COERCION_INDEX_BY_TYPE[class_or_instance]
+        raise ApiValueError("Unsupported type: %s" % class_or_instance)
+
+    sorted_types = sorted(
+        required_types,
+        key=lambda class_or_instance: index_getter(class_or_instance)
+    )
+    return sorted_types
+
+
+def remove_uncoercible(required_types_classes, current_item, spec_property_naming,
+                       must_convert=True):
+    """Only keeps the type conversions that are possible
+
+    Args:
+        required_types_classes (tuple): tuple of classes that are required
+                          these should be ordered by COERCION_INDEX_BY_TYPE
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+        current_item (any): the current item (input data) to be converted
+
+    Keyword Args:
+        must_convert (bool): if True the item to convert is of the wrong
+                          type and we want a big list of coercibles
+                          if False, we want a limited list of coercibles
+
+    Returns:
+        (list): the remaining coercible required types, classes only
+    """
+    current_type_simple = get_simple_class(current_item)
+
+    results_classes = []
+    for required_type_class in required_types_classes:
+        # convert our models to OpenApiModel
+        required_type_class_simplified = required_type_class
+        if isinstance(required_type_class_simplified, type):
+            if issubclass(required_type_class_simplified, ModelComposed):
+                required_type_class_simplified = ModelComposed
+            elif issubclass(required_type_class_simplified, ModelNormal):
+                required_type_class_simplified = ModelNormal
+            elif issubclass(required_type_class_simplified, ModelSimple):
+                required_type_class_simplified = ModelSimple
+
+        if required_type_class_simplified == current_type_simple:
+            # don't consider converting to one's own class
+            continue
+
+        class_pair = (current_type_simple, required_type_class_simplified)
+        if must_convert and class_pair in COERCIBLE_TYPE_PAIRS[spec_property_naming]:
+            results_classes.append(required_type_class)
+        elif class_pair in UPCONVERSION_TYPE_PAIRS:
+            results_classes.append(required_type_class)
+    return results_classes
+
+
+def get_discriminated_classes(cls):
+    """
+    Returns all the classes that a discriminator converts to
+    TODO: lru_cache this
+    """
+    possible_classes = []
+    key = list(cls.discriminator.keys())[0]
+    if is_type_nullable(cls):
+        possible_classes.append(cls)
+    for discr_cls in cls.discriminator[key].values():
+        if hasattr(discr_cls, 'discriminator') and discr_cls.discriminator is not None:
+            possible_classes.extend(get_discriminated_classes(discr_cls))
+        else:
+            possible_classes.append(discr_cls)
+    return possible_classes
+
+
+def get_possible_classes(cls, from_server_context):
+    # TODO: lru_cache this
+    possible_classes = [cls]
+    if from_server_context:
+        return possible_classes
+    if hasattr(cls, 'discriminator') and cls.discriminator is not None:
+        possible_classes = []
+        possible_classes.extend(get_discriminated_classes(cls))
+    elif issubclass(cls, ModelComposed):
+        possible_classes.extend(composed_model_input_classes(cls))
+    return possible_classes
+
+
+def get_required_type_classes(required_types_mixed, spec_property_naming):
+    """Converts the tuple required_types into a tuple and a dict described
+    below
+
+    Args:
+        required_types_mixed (tuple/list): will contain either classes or
+            instance of list or dict
+        spec_property_naming (bool): if True these values came from the
+            server, and we use the data types in our endpoints.
+            If False, we are client side and we need to include
+            oneOf and discriminator classes inside the data types in our endpoints
+
+    Returns:
+        (valid_classes, dict_valid_class_to_child_types_mixed):
+            valid_classes (tuple): the valid classes that the current item
+                                   should be
+            dict_valid_class_to_child_types_mixed (dict):
+                valid_class (class): this is the key
+                child_types_mixed (list/dict/tuple): describes the valid child
+                    types
+    """
+    valid_classes = []
+    child_req_types_by_current_type = {}
+    for required_type in required_types_mixed:
+        if isinstance(required_type, list):
+            valid_classes.append(list)
+            child_req_types_by_current_type[list] = required_type
+        elif isinstance(required_type, tuple):
+            valid_classes.append(tuple)
+            child_req_types_by_current_type[tuple] = required_type
+        elif isinstance(required_type, dict):
+            valid_classes.append(dict)
+            child_req_types_by_current_type[dict] = required_type[str]
+        else:
+            valid_classes.extend(get_possible_classes(required_type, spec_property_naming))
+    return tuple(valid_classes), child_req_types_by_current_type
+
+
+def change_keys_js_to_python(input_dict, model_class):
+    """
+    Converts from javascript_key keys in the input_dict to python_keys in
+    the output dict using the mapping in model_class.
+    If the input_dict contains a key which does not declared in the model_class,
+    the key is added to the output dict as is. The assumption is the model_class
+    may have undeclared properties (additionalProperties attribute in the OAS
+    document).
+    """
+
+    if getattr(model_class, 'attribute_map', None) is None:
+        return input_dict
+    output_dict = {}
+    reversed_attr_map = {value: key for key, value in
+                         model_class.attribute_map.items()}
+    for javascript_key, value in input_dict.items():
+        python_key = reversed_attr_map.get(javascript_key)
+        if python_key is None:
+            # if the key is unknown, it is in error or it is an
+            # additionalProperties variable
+            python_key = javascript_key
+        output_dict[python_key] = value
+    return output_dict
+
+
+def get_type_error(var_value, path_to_item, valid_classes, key_type=False):
+    error_msg = type_error_message(
+        var_name=path_to_item[-1],
+        var_value=var_value,
+        valid_classes=valid_classes,
+        key_type=key_type
+    )
+    return ApiTypeError(
+        error_msg,
+        path_to_item=path_to_item,
+        valid_classes=valid_classes,
+        key_type=key_type
+    )
+
+
+def deserialize_primitive(data, klass, path_to_item):
+    """Deserializes string to primitive type.
+
+    :param data: str/int/float
+    :param klass: str/class the class to convert to
+
+    :return: int, float, str, bool, date, datetime
+    """
+    additional_message = ""
+    try:
+        if klass in {datetime, date}:
+            additional_message = (
+                "If you need your parameter to have a fallback "
+                "string value, please set its type as `type: {}` in your "
+                "spec. That allows the value to be any type. "
+            )
+            if klass == datetime:
+                if len(data) < 8:
+                    raise ValueError("This is not a datetime")
+                # The string should be in iso8601 datetime format.
+                parsed_datetime = parse(data)
+                date_only = (
+                    parsed_datetime.hour == 0 and
+                    parsed_datetime.minute == 0 and
+                    parsed_datetime.second == 0 and
+                    parsed_datetime.tzinfo is None and
+                    8 <= len(data) <= 10
+                )
+                if date_only:
+                    raise ValueError("This is a date, not a datetime")
+                return parsed_datetime
+            elif klass == date:
+                if len(data) < 8:
+                    raise ValueError("This is not a date")
+                return parse(data).date()
+        else:
+            converted_value = klass(data)
+            if isinstance(data, str) and klass == float:
+                if str(converted_value) != data:
+                    # '7' -> 7.0 -> '7.0' != '7'
+                    raise ValueError('This is not a float')
+            return converted_value
+    except (OverflowError, ValueError) as ex:
+        # parse can raise OverflowError
+        raise ApiValueError(
+            "{0}Failed to parse {1} as {2}".format(
+                additional_message, repr(data), klass.__name__
+            ),
+            path_to_item=path_to_item
+        ) from ex
+
+
+def get_discriminator_class(model_class,
+                            discr_name,
+                            discr_value, cls_visited):
+    """Returns the child class specified by the discriminator.
+
+    Args:
+        model_class (OpenApiModel): the model class.
+        discr_name (string): the name of the discriminator property.
+        discr_value (any): the discriminator value.
+        cls_visited (list): list of model classes that have been visited.
+            Used to determine the discriminator class without
+            visiting circular references indefinitely.
+
+    Returns:
+        used_model_class (class/None): the chosen child class that will be used
+            to deserialize the data, for example dog.Dog.
+            If a class is not found, None is returned.
+    """
+
+    if model_class in cls_visited:
+        # The class has already been visited and no suitable class was found.
+        return None
+    cls_visited.append(model_class)
+    used_model_class = None
+    if discr_name in model_class.discriminator:
+        class_name_to_discr_class = model_class.discriminator[discr_name]
+        used_model_class = class_name_to_discr_class.get(discr_value)
+    if used_model_class is None:
+        # We didn't find a discriminated class in class_name_to_discr_class.
+        # So look in the ancestor or descendant discriminators
+        # The discriminator mapping may exist in a descendant (anyOf, oneOf)
+        # or ancestor (allOf).
+        # Ancestor example: in the GrandparentAnimal -> ParentPet -> ChildCat
+        #   hierarchy, the discriminator mappings may be defined at any level
+        #   in the hierarchy.
+        # Descendant example:  mammal -> whale/zebra/Pig -> BasquePig/DanishPig
+        #   if we try to make BasquePig from mammal, we need to travel through
+        #   the oneOf descendant discriminators to find BasquePig
+        descendant_classes = model_class._composed_schemas.get('oneOf', ()) + \
+            model_class._composed_schemas.get('anyOf', ())
+        ancestor_classes = model_class._composed_schemas.get('allOf', ())
+        possible_classes = descendant_classes + ancestor_classes
+        for cls in possible_classes:
+            # Check if the schema has inherited discriminators.
+            if hasattr(cls, 'discriminator') and cls.discriminator is not None:
+                used_model_class = get_discriminator_class(
+                    cls, discr_name, discr_value, cls_visited)
+                if used_model_class is not None:
+                    return used_model_class
+    return used_model_class
+
+
+def deserialize_model(model_data, model_class, path_to_item, check_type,
+                      configuration, spec_property_naming):
+    """Deserializes model_data to model instance.
+
+    Args:
+        model_data (int/str/float/bool/none_type/list/dict): data to instantiate the model
+        model_class (OpenApiModel): the model class
+        path_to_item (list): path to the model in the received data
+        check_type (bool): whether to check the data tupe for the values in
+            the model
+        configuration (Configuration): the instance to use to convert files
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+
+    Returns:
+        model instance
+
+    Raise:
+        ApiTypeError
+        ApiValueError
+        ApiKeyError
+    """
+
+    kw_args = dict(_check_type=check_type,
+                   _path_to_item=path_to_item,
+                   _configuration=configuration,
+                   _spec_property_naming=spec_property_naming)
+
+    if issubclass(model_class, ModelSimple):
+        return model_class._new_from_openapi_data(model_data, **kw_args)
+    elif isinstance(model_data, list):
+        return model_class._new_from_openapi_data(*model_data, **kw_args)
+    if isinstance(model_data, dict):
+        kw_args.update(model_data)
+        return model_class._new_from_openapi_data(**kw_args)
+    elif isinstance(model_data, PRIMITIVE_TYPES):
+        return model_class._new_from_openapi_data(model_data, **kw_args)
+
+
+def deserialize_file(response_data, configuration, content_disposition=None):
+    """Deserializes body to file
+
+    Saves response body into a file in a temporary folder,
+    using the filename from the `Content-Disposition` header if provided.
+
+    Args:
+        param response_data (str):  the file data to write
+        configuration (Configuration): the instance to use to convert files
+
+    Keyword Args:
+        content_disposition (str):  the value of the Content-Disposition
+            header
+
+    Returns:
+        (file_type): the deserialized file which is open
+            The user is responsible for closing and reading the file
+    """
+    fd, path = tempfile.mkstemp(dir=configuration.temp_folder_path)
+    os.close(fd)
+    os.remove(path)
+
+    if content_disposition:
+        filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
+                             content_disposition,
+                             flags=re.I)
+        if filename is not None:
+            filename = filename.group(1)
+        else:
+            filename = "default_" + str(uuid.uuid4())
+
+        path = os.path.join(os.path.dirname(path), filename)
+
+    with open(path, "wb") as f:
+        if isinstance(response_data, str):
+            # change str to bytes so we can write it
+            response_data = response_data.encode('utf-8')
+        f.write(response_data)
+
+    f = open(path, "rb")
+    return f
+
+
+def attempt_convert_item(input_value, valid_classes, path_to_item,
+                         configuration, spec_property_naming, key_type=False,
+                         must_convert=False, check_type=True):
+    """
+    Args:
+        input_value (any): the data to convert
+        valid_classes (any): the classes that are valid
+        path_to_item (list): the path to the item to convert
+        configuration (Configuration): the instance to use to convert files
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+        key_type (bool): if True we need to convert a key type (not supported)
+        must_convert (bool): if True we must convert
+        check_type (bool): if True we check the type or the returned data in
+            ModelComposed/ModelNormal/ModelSimple instances
+
+    Returns:
+        instance (any) the fixed item
+
+    Raises:
+        ApiTypeError
+        ApiValueError
+        ApiKeyError
+    """
+    valid_classes_ordered = order_response_types(valid_classes)
+    valid_classes_coercible = remove_uncoercible(
+        valid_classes_ordered, input_value, spec_property_naming)
+    if not valid_classes_coercible or key_type:
+        # we do not handle keytype errors, json will take care
+        # of this for us
+        if configuration is None or not configuration.discard_unknown_keys:
+            raise get_type_error(input_value, path_to_item, valid_classes,
+                                 key_type=key_type)
+    for valid_class in valid_classes_coercible:
+        try:
+            if issubclass(valid_class, OpenApiModel):
+                return deserialize_model(input_value, valid_class,
+                                         path_to_item, check_type,
+                                         configuration, spec_property_naming)
+            elif valid_class == file_type:
+                return deserialize_file(input_value, configuration)
+            return deserialize_primitive(input_value, valid_class,
+                                         path_to_item)
+        except (ApiTypeError, ApiValueError, ApiKeyError) as conversion_exc:
+            if must_convert:
+                raise conversion_exc
+            # if we have conversion errors when must_convert == False
+            # we ignore the exception and move on to the next class
+            continue
+    # we were unable to convert, must_convert == False
+    return input_value
+
+
+def is_type_nullable(input_type):
+    """
+    Returns true if None is an allowed value for the specified input_type.
+
+    A type is nullable if at least one of the following conditions is true:
+    1. The OAS 'nullable' attribute has been specified,
+    1. The type is the 'null' type,
+    1. The type is a anyOf/oneOf composed schema, and a child schema is
+       the 'null' type.
+    Args:
+        input_type (type): the class of the input_value that we are
+            checking
+    Returns:
+        bool
+    """
+    if input_type is none_type:
+        return True
+    if issubclass(input_type, OpenApiModel) and input_type._nullable:
+        return True
+    if issubclass(input_type, ModelComposed):
+        # If oneOf/anyOf, check if the 'null' type is one of the allowed types.
+        for t in input_type._composed_schemas.get('oneOf', ()):
+            if is_type_nullable(t):
+                return True
+        for t in input_type._composed_schemas.get('anyOf', ()):
+            if is_type_nullable(t):
+                return True
+    return False
+
+
+def is_valid_type(input_class_simple, valid_classes):
+    """
+    Args:
+        input_class_simple (class): the class of the input_value that we are
+            checking
+        valid_classes (tuple): the valid classes that the current item
+            should be
+    Returns:
+        bool
+    """
+    if issubclass(input_class_simple, OpenApiModel) and \
+            valid_classes == (bool, date, datetime, dict, float, int, list, str, none_type,):
+        return True
+    valid_type = input_class_simple in valid_classes
+    if not valid_type and (
+            issubclass(input_class_simple, OpenApiModel) or
+            input_class_simple is none_type):
+        for valid_class in valid_classes:
+            if input_class_simple is none_type and is_type_nullable(valid_class):
+                # Schema is oneOf/anyOf and the 'null' type is one of the allowed types.
+                return True
+            if not (issubclass(valid_class, OpenApiModel) and valid_class.discriminator):
+                continue
+            discr_propertyname_py = list(valid_class.discriminator.keys())[0]
+            discriminator_classes = (
+                valid_class.discriminator[discr_propertyname_py].values()
+            )
+            valid_type = is_valid_type(input_class_simple, discriminator_classes)
+            if valid_type:
+                return True
+    return valid_type
+
+
+def validate_and_convert_types(input_value, required_types_mixed, path_to_item,
+                               spec_property_naming, _check_type, configuration=None):
+    """Raises a TypeError is there is a problem, otherwise returns value
+
+    Args:
+        input_value (any): the data to validate/convert
+        required_types_mixed (list/dict/tuple): A list of
+            valid classes, or a list tuples of valid classes, or a dict where
+            the value is a tuple of value classes
+        path_to_item: (list) the path to the data being validated
+            this stores a list of keys or indices to get to the data being
+            validated
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+        _check_type: (boolean) if true, type will be checked and conversion
+            will be attempted.
+        configuration: (Configuration): the configuration class to use
+            when converting file_type items.
+            If passed, conversion will be attempted when possible
+            If not passed, no conversions will be attempted and
+            exceptions will be raised
+
+    Returns:
+        the correctly typed value
+
+    Raises:
+        ApiTypeError
+    """
+    results = get_required_type_classes(required_types_mixed, spec_property_naming)
+    valid_classes, child_req_types_by_current_type = results
+
+    input_class_simple = get_simple_class(input_value)
+    valid_type = is_valid_type(input_class_simple, valid_classes)
+    if not valid_type:
+        if (configuration
+                or (input_class_simple == dict
+                    and dict not in valid_classes)):
+            # if input_value is not valid_type try to convert it
+            converted_instance = attempt_convert_item(
+                input_value,
+                valid_classes,
+                path_to_item,
+                configuration,
+                spec_property_naming,
+                key_type=False,
+                must_convert=True,
+                check_type=_check_type
+            )
+            return converted_instance
+        else:
+            raise get_type_error(input_value, path_to_item, valid_classes,
+                                 key_type=False)
+
+    # input_value's type is in valid_classes
+    if len(valid_classes) > 1 and configuration:
+        # there are valid classes which are not the current class
+        valid_classes_coercible = remove_uncoercible(
+            valid_classes, input_value, spec_property_naming, must_convert=False)
+        if valid_classes_coercible:
+            converted_instance = attempt_convert_item(
+                input_value,
+                valid_classes_coercible,
+                path_to_item,
+                configuration,
+                spec_property_naming,
+                key_type=False,
+                must_convert=False,
+                check_type=_check_type
+            )
+            return converted_instance
+
+    if child_req_types_by_current_type == {}:
+        # all types are of the required types and there are no more inner
+        # variables left to look at
+        return input_value
+    inner_required_types = child_req_types_by_current_type.get(
+        type(input_value)
+    )
+    if inner_required_types is None:
+        # for this type, there are not more inner variables left to look at
+        return input_value
+    if isinstance(input_value, list):
+        if input_value == []:
+            # allow an empty list
+            return input_value
+        for index, inner_value in enumerate(input_value):
+            inner_path = list(path_to_item)
+            inner_path.append(index)
+            input_value[index] = validate_and_convert_types(
+                inner_value,
+                inner_required_types,
+                inner_path,
+                spec_property_naming,
+                _check_type,
+                configuration=configuration
+            )
+    elif isinstance(input_value, dict):
+        if input_value == {}:
+            # allow an empty dict
+            return input_value
+        for inner_key, inner_val in input_value.items():
+            inner_path = list(path_to_item)
+            inner_path.append(inner_key)
+            if get_simple_class(inner_key) != str:
+                raise get_type_error(inner_key, inner_path, valid_classes,
+                                     key_type=True)
+            input_value[inner_key] = validate_and_convert_types(
+                inner_val,
+                inner_required_types,
+                inner_path,
+                spec_property_naming,
+                _check_type,
+                configuration=configuration
+            )
+    return input_value
+
+
+def model_to_dict(model_instance, serialize=True):
+    """Returns the model properties as a dict
+
+    Args:
+        model_instance (one of your model instances): the model instance that
+            will be converted to a dict.
+
+    Keyword Args:
+        serialize (bool): if True, the keys in the dict will be values from
+            attribute_map
+    """
+    result = {}
+
+    def extract_item(item): return (
+        item[0], model_to_dict(
+            item[1], serialize=serialize)) if hasattr(
+        item[1], '_data_store') else item
+
+    model_instances = [model_instance]
+    if model_instance._composed_schemas:
+        model_instances.extend(model_instance._composed_instances)
+    seen_json_attribute_names = set()
+    used_fallback_python_attribute_names = set()
+    py_to_json_map = {}
+    for model_instance in model_instances:
+        for attr, value in model_instance._data_store.items():
+            if serialize:
+                # we use get here because additional property key names do not
+                # exist in attribute_map
+                try:
+                    attr = model_instance.attribute_map[attr]
+                    py_to_json_map.update(model_instance.attribute_map)
+                    seen_json_attribute_names.add(attr)
+                except KeyError:
+                    used_fallback_python_attribute_names.add(attr)
+            if isinstance(value, list):
+                if not value:
+                    # empty list or None
+                    result[attr] = value
+                else:
+                    res = []
+                    for v in value:
+                        if isinstance(v, PRIMITIVE_TYPES) or v is None:
+                            res.append(v)
+                        elif isinstance(v, ModelSimple):
+                            res.append(v.value)
+                        elif isinstance(v, dict):
+                            res.append(dict(map(
+                                extract_item,
+                                v.items()
+                            )))
+                        else:
+                            res.append(model_to_dict(v, serialize=serialize))
+                    result[attr] = res
+            elif isinstance(value, dict):
+                result[attr] = dict(map(
+                    extract_item,
+                    value.items()
+                ))
+            elif isinstance(value, ModelSimple):
+                result[attr] = value.value
+            elif hasattr(value, '_data_store'):
+                result[attr] = model_to_dict(value, serialize=serialize)
+            else:
+                result[attr] = value
+    if serialize:
+        for python_key in used_fallback_python_attribute_names:
+            json_key = py_to_json_map.get(python_key)
+            if json_key is None:
+                continue
+            if python_key == json_key:
+                continue
+            json_key_assigned_no_need_for_python_key = json_key in seen_json_attribute_names
+            if json_key_assigned_no_need_for_python_key:
+                del result[python_key]
+
+    return result
+
+
+def type_error_message(var_value=None, var_name=None, valid_classes=None,
+                       key_type=None):
+    """
+    Keyword Args:
+        var_value (any): the variable which has the type_error
+        var_name (str): the name of the variable which has the typ error
+        valid_classes (tuple): the accepted classes for current_item's
+                                  value
+        key_type (bool): False if our value is a value in a dict
+                         True if it is a key in a dict
+                         False if our item is an item in a list
+    """
+    key_or_value = 'value'
+    if key_type:
+        key_or_value = 'key'
+    valid_classes_phrase = get_valid_classes_phrase(valid_classes)
+    msg = (
+        "Invalid type for variable '{0}'. Required {1} type {2} and "
+        "passed type was {3}".format(
+            var_name,
+            key_or_value,
+            valid_classes_phrase,
+            type(var_value).__name__,
+        )
+    )
+    return msg
+
+
+def get_valid_classes_phrase(input_classes):
+    """Returns a string phrase describing what types are allowed
+    """
+    all_classes = list(input_classes)
+    all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
+    all_class_names = [cls.__name__ for cls in all_classes]
+    if len(all_class_names) == 1:
+        return 'is {0}'.format(all_class_names[0])
+    return "is one of [{0}]".format(", ".join(all_class_names))
+
+
+def get_allof_instances(self, model_args, constant_args):
+    """
+    Args:
+        self: the class we are handling
+        model_args (dict): var_name to var_value
+            used to make instances
+        constant_args (dict):
+            metadata arguments:
+            _check_type
+            _path_to_item
+            _spec_property_naming
+            _configuration
+            _visited_composed_classes
+
+    Returns
+        composed_instances (list)
+    """
+    composed_instances = []
+    for allof_class in self._composed_schemas['allOf']:
+
+        try:
+            if constant_args.get('_spec_property_naming'):
+                allof_instance = allof_class._from_openapi_data(**model_args, **constant_args)
+            else:
+                allof_instance = allof_class(**model_args, **constant_args)
+            composed_instances.append(allof_instance)
+        except Exception as ex:
+            raise ApiValueError(
+                "Invalid inputs given to generate an instance of '%s'. The "
+                "input data was invalid for the allOf schema '%s' in the composed "
+                "schema '%s'. Error=%s" % (
+                    allof_class.__name__,
+                    allof_class.__name__,
+                    self.__class__.__name__,
+                    str(ex)
+                )
+            ) from ex
+    return composed_instances
+
+
+def get_oneof_instance(cls, model_kwargs, constant_kwargs, model_arg=None):
+    """
+    Find the oneOf schema that matches the input data (e.g. payload).
+    If exactly one schema matches the input data, an instance of that schema
+    is returned.
+    If zero or more than one schema match the input data, an exception is raised.
+    In OAS 3.x, the payload MUST, by validation, match exactly one of the
+    schemas described by oneOf.
+
+    Args:
+        cls: the class we are handling
+        model_kwargs (dict): var_name to var_value
+            The input data, e.g. the payload that must match a oneOf schema
+            in the OpenAPI document.
+        constant_kwargs (dict): var_name to var_value
+            args that every model requires, including configuration, server
+            and path to item.
+
+    Kwargs:
+        model_arg: (int, float, bool, str, date, datetime, ModelSimple, None):
+            the value to assign to a primitive class or ModelSimple class
+            Notes:
+            - this is only passed in when oneOf includes types which are not object
+            - None is used to suppress handling of model_arg, nullable models are handled in __new__
+
+    Returns
+        oneof_instance (instance)
+    """
+    if len(cls._composed_schemas['oneOf']) == 0:
+        return None
+
+    oneof_instances = []
+    # Iterate over each oneOf schema and determine if the input data
+    # matches the oneOf schemas.
+    for oneof_class in cls._composed_schemas['oneOf']:
+        # The composed oneOf schema allows the 'null' type and the input data
+        # is the null value. This is a OAS >= 3.1 feature.
+        if oneof_class is none_type:
+            # skip none_types because we are deserializing dict data.
+            # none_type deserialization is handled in the __new__ method
+            continue
+
+        single_value_input = allows_single_value_input(oneof_class)
+
+        try:
+            if not single_value_input:
+                if constant_kwargs.get('_spec_property_naming'):
+                    oneof_instance = oneof_class._from_openapi_data(
+                        **model_kwargs, **constant_kwargs)
+                else:
+                    oneof_instance = oneof_class(**model_kwargs, **constant_kwargs)
+            else:
+                if issubclass(oneof_class, ModelSimple):
+                    if constant_kwargs.get('_spec_property_naming'):
+                        oneof_instance = oneof_class._from_openapi_data(
+                            model_arg, **constant_kwargs)
+                    else:
+                        oneof_instance = oneof_class(model_arg, **constant_kwargs)
+                elif oneof_class in PRIMITIVE_TYPES:
+                    oneof_instance = validate_and_convert_types(
+                        model_arg,
+                        (oneof_class,),
+                        constant_kwargs['_path_to_item'],
+                        constant_kwargs['_spec_property_naming'],
+                        constant_kwargs['_check_type'],
+                        configuration=constant_kwargs['_configuration']
+                    )
+            oneof_instances.append(oneof_instance)
+        except Exception:
+            pass
+    if len(oneof_instances) == 0:
+        raise ApiValueError(
+            "Invalid inputs given to generate an instance of %s. None "
+            "of the oneOf schemas matched the input data." %
+            cls.__name__
+        )
+    elif len(oneof_instances) > 1:
+        raise ApiValueError(
+            "Invalid inputs given to generate an instance of %s. Multiple "
+            "oneOf schemas matched the inputs, but a max of one is allowed." %
+            cls.__name__
+        )
+    return oneof_instances[0]
+
+
+def get_anyof_instances(self, model_args, constant_args):
+    """
+    Args:
+        self: the class we are handling
+        model_args (dict): var_name to var_value
+            The input data, e.g. the payload that must match at least one
+            anyOf child schema in the OpenAPI document.
+        constant_args (dict): var_name to var_value
+            args that every model requires, including configuration, server
+            and path to item.
+
+    Returns
+        anyof_instances (list)
+    """
+    anyof_instances = []
+    if len(self._composed_schemas['anyOf']) == 0:
+        return anyof_instances
+
+    for anyof_class in self._composed_schemas['anyOf']:
+        # The composed oneOf schema allows the 'null' type and the input data
+        # is the null value. This is a OAS >= 3.1 feature.
+        if anyof_class is none_type:
+            # skip none_types because we are deserializing dict data.
+            # none_type deserialization is handled in the __new__ method
+            continue
+
+        try:
+            if constant_args.get('_spec_property_naming'):
+                anyof_instance = anyof_class._from_openapi_data(**model_args, **constant_args)
+            else:
+                anyof_instance = anyof_class(**model_args, **constant_args)
+            anyof_instances.append(anyof_instance)
+        except Exception:
+            pass
+    if len(anyof_instances) == 0:
+        raise ApiValueError(
+            "Invalid inputs given to generate an instance of %s. None of the "
+            "anyOf schemas matched the inputs." %
+            self.__class__.__name__
+        )
+    return anyof_instances
+
+
+def get_discarded_args(self, composed_instances, model_args):
+    """
+    Gathers the args that were discarded by configuration.discard_unknown_keys
+    """
+    model_arg_keys = model_args.keys()
+    discarded_args = set()
+    # arguments passed to self were already converted to python names
+    # before __init__ was called
+    for instance in composed_instances:
+        if instance.__class__ in self._composed_schemas['allOf']:
+            try:
+                keys = instance.to_dict().keys()
+                discarded_keys = model_args - keys
+                discarded_args.update(discarded_keys)
+            except Exception:
+                # allOf integer schema will throw exception
+                pass
+        else:
+            try:
+                all_keys = set(model_to_dict(instance, serialize=False).keys())
+                js_keys = model_to_dict(instance, serialize=True).keys()
+                all_keys.update(js_keys)
+                discarded_keys = model_arg_keys - all_keys
+                discarded_args.update(discarded_keys)
+            except Exception:
+                # allOf integer schema will throw exception
+                pass
+    return discarded_args
+
+
+def validate_get_composed_info(constant_args, model_args, self):
+    """
+    For composed schemas, generate schema instances for
+    all schemas in the oneOf/anyOf/allOf definition. If additional
+    properties are allowed, also assign those properties on
+    all matched schemas that contain additionalProperties.
+    Openapi schemas are python classes.
+
+    Exceptions are raised if:
+    - 0 or > 1 oneOf schema matches the model_args input data
+    - no anyOf schema matches the model_args input data
+    - any of the allOf schemas do not match the model_args input data
+
+    Args:
+        constant_args (dict): these are the args that every model requires
+        model_args (dict): these are the required and optional spec args that
+            were passed in to make this model
+        self (class): the class that we are instantiating
+            This class contains self._composed_schemas
+
+    Returns:
+        composed_info (list): length three
+            composed_instances (list): the composed instances which are not
+                self
+            var_name_to_model_instances (dict): a dict going from var_name
+                to the model_instance which holds that var_name
+                the model_instance may be self or an instance of one of the
+                classes in self.composed_instances()
+            additional_properties_model_instances (list): a list of the
+                model instances which have the property
+                additional_properties_type. This list can include self
+    """
+    # create composed_instances
+    composed_instances = []
+    allof_instances = get_allof_instances(self, model_args, constant_args)
+    composed_instances.extend(allof_instances)
+    oneof_instance = get_oneof_instance(self.__class__, model_args, constant_args)
+    if oneof_instance is not None:
+        composed_instances.append(oneof_instance)
+    anyof_instances = get_anyof_instances(self, model_args, constant_args)
+    composed_instances.extend(anyof_instances)
+    """
+    set additional_properties_model_instances
+    additional properties must be evaluated at the schema level
+    so self's additional properties are most important
+    If self is a composed schema with:
+    - no properties defined in self
+    - additionalProperties: False
+    Then for object payloads every property is an additional property
+    and they are not allowed, so only empty dict is allowed
+
+    Properties must be set on all matching schemas
+    so when a property is assigned toa composed instance, it must be set on all
+    composed instances regardless of additionalProperties presence
+    keeping it to prevent breaking changes in v5.0.1
+    TODO remove cls._additional_properties_model_instances in 6.0.0
+    """
+    additional_properties_model_instances = []
+    if self.additional_properties_type is not None:
+        additional_properties_model_instances = [self]
+
+    """
+    no need to set properties on self in here, they will be set in __init__
+    By here all composed schema oneOf/anyOf/allOf instances have their properties set using
+    model_args
+    """
+    discarded_args = get_discarded_args(self, composed_instances, model_args)
+
+    # map variable names to composed_instances
+    var_name_to_model_instances = {}
+    for prop_name in model_args:
+        if prop_name not in discarded_args:
+            var_name_to_model_instances[prop_name] = [self] + list(
+                filter(
+                    lambda x: prop_name in x.openapi_types, composed_instances))
+
+    return [
+        composed_instances,
+        var_name_to_model_instances,
+        additional_properties_model_instances,
+        discarded_args
+    ]
```

### Comparing `invision-client-python-1.0.0/invision_client/models/__init__.py` & `invision-client-python-1.3.0b1/invision_client/models/__init__.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# flake8: noqa
-
-# import all models into this package
-# if you have many models here with many references from one model to another this may
-# raise a RecursionError
-# to avoid this, import only the models that you directly need like:
-# from from invision_client.model.pet import Pet
-# or import this package, but before doing it, use:
-# import sys
-# sys.setrecursionlimit(n)
-
-from invision_client.model.core_members_get200_response import CoreMembersGet200Response
-from invision_client.model.field import Field
-from invision_client.model.fieldgroup import Fieldgroup
-from invision_client.model.forum import Forum
-from invision_client.model.forums_forums_get200_response import ForumsForumsGet200Response
-from invision_client.model.group import Group
-from invision_client.model.member import Member
-from invision_client.model.poll import Poll
-from invision_client.model.post import Post
-from invision_client.model.post_reactions_inner import PostReactionsInner
-from invision_client.model.question import Question
-from invision_client.model.rank import Rank
-from invision_client.model.topic import Topic
+# flake8: noqa
+
+# import all models into this package
+# if you have many models here with many references from one model to another this may
+# raise a RecursionError
+# to avoid this, import only the models that you directly need like:
+# from from invision_client.model.pet import Pet
+# or import this package, but before doing it, use:
+# import sys
+# sys.setrecursionlimit(n)
+
+from invision_client.model.core_members_get200_response import CoreMembersGet200Response
+from invision_client.model.field import Field
+from invision_client.model.fieldgroup import Fieldgroup
+from invision_client.model.forum import Forum
+from invision_client.model.forums_forums_get200_response import ForumsForumsGet200Response
+from invision_client.model.group import Group
+from invision_client.model.member import Member
+from invision_client.model.poll import Poll
+from invision_client.model.post import Post
+from invision_client.model.post_reactions_inner import PostReactionsInner
+from invision_client.model.question import Question
+from invision_client.model.rank import Rank
+from invision_client.model.topic import Topic
```

### Comparing `invision-client-python-1.0.0/invision_client/rest.py` & `invision-client-python-1.3.0b1/invision_client/rest.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,352 +1,352 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import io
-import json
-import logging
-import re
-import ssl
-from urllib.parse import urlencode
-from urllib.parse import urlparse
-from urllib.request import proxy_bypass_environment
-import urllib3
-import ipaddress
-
-from invision_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
-
-
-logger = logging.getLogger(__name__)
-
-
-class RESTResponse(io.IOBase):
-
-    def __init__(self, resp):
-        self.urllib3_response = resp
-        self.status = resp.status
-        self.reason = resp.reason
-        self.data = resp.data
-
-    def getheaders(self):
-        """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
-
-    def getheader(self, name, default=None):
-        """Returns a given response header."""
-        return self.urllib3_response.getheader(name, default)
-
-
-class RESTClientObject(object):
-
-    def __init__(self, configuration, pools_size=4, maxsize=None):
-        # urllib3.PoolManager will pass all kw parameters to connectionpool
-        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
-        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
-        # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
-        # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
-
-        # cert_reqs
-        if configuration.verify_ssl:
-            cert_reqs = ssl.CERT_REQUIRED
-        else:
-            cert_reqs = ssl.CERT_NONE
-
-        addition_pool_args = {}
-        if configuration.assert_hostname is not None:
-            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
-
-        if configuration.retries is not None:
-            addition_pool_args['retries'] = configuration.retries
-
-        if configuration.socket_options is not None:
-            addition_pool_args['socket_options'] = configuration.socket_options
-
-        if maxsize is None:
-            if configuration.connection_pool_maxsize is not None:
-                maxsize = configuration.connection_pool_maxsize
-            else:
-                maxsize = 4
-
-        # https pool manager
-        if configuration.proxy and not should_bypass_proxies(
-                configuration.host, no_proxy=configuration.no_proxy or ''):
-            self.pool_manager = urllib3.ProxyManager(
-                num_pools=pools_size,
-                maxsize=maxsize,
-                cert_reqs=cert_reqs,
-                ca_certs=configuration.ssl_ca_cert,
-                cert_file=configuration.cert_file,
-                key_file=configuration.key_file,
-                proxy_url=configuration.proxy,
-                proxy_headers=configuration.proxy_headers,
-                **addition_pool_args
-            )
-        else:
-            self.pool_manager = urllib3.PoolManager(
-                num_pools=pools_size,
-                maxsize=maxsize,
-                cert_reqs=cert_reqs,
-                ca_certs=configuration.ssl_ca_cert,
-                cert_file=configuration.cert_file,
-                key_file=configuration.key_file,
-                **addition_pool_args
-            )
-
-    def request(self, method, url, query_params=None, headers=None,
-                body=None, post_params=None, _preload_content=True,
-                _request_timeout=None):
-        """Perform requests.
-
-        :param method: http request method
-        :param url: http request url
-        :param query_params: query parameters in the url
-        :param headers: http request headers
-        :param body: request json body, for `application/json`
-        :param post_params: request post parameters,
-                            `application/x-www-form-urlencoded`
-                            and `multipart/form-data`
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        """
-        method = method.upper()
-        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
-                          'PATCH', 'OPTIONS']
-
-        if post_params and body:
-            raise ApiValueError(
-                "body parameter cannot be used with post_params parameter."
-            )
-
-        post_params = post_params or {}
-        headers = headers or {}
-
-        timeout = None
-        if _request_timeout:
-            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
-                timeout = urllib3.Timeout(total=_request_timeout)
-            elif (isinstance(_request_timeout, tuple) and
-                  len(_request_timeout) == 2):
-                timeout = urllib3.Timeout(
-                    connect=_request_timeout[0], read=_request_timeout[1])
-
-        try:
-            # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
-            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
-                if (method != 'DELETE') and ('Content-Type' not in headers):
-                    headers['Content-Type'] = 'application/json'
-                if query_params:
-                    url += '?' + urlencode(query_params)
-                if ('Content-Type' not in headers) or (re.search('json',
-                                                                 headers['Content-Type'], re.IGNORECASE)):
-                    request_body = None
-                    if body is not None:
-                        request_body = json.dumps(body)
-                    r = self.pool_manager.request(
-                        method, url,
-                        body=request_body,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
-                    r = self.pool_manager.request(
-                        method, url,
-                        fields=post_params,
-                        encode_multipart=False,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                elif headers['Content-Type'] == 'multipart/form-data':
-                    # must del headers['Content-Type'], or the correct
-                    # Content-Type which generated by urllib3 will be
-                    # overwritten.
-                    del headers['Content-Type']
-                    r = self.pool_manager.request(
-                        method, url,
-                        fields=post_params,
-                        encode_multipart=True,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                # Pass a `string` parameter directly in the body to support
-                # other content types than Json when `body` argument is
-                # provided in serialized form
-                elif isinstance(body, str) or isinstance(body, bytes):
-                    request_body = body
-                    r = self.pool_manager.request(
-                        method, url,
-                        body=request_body,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                else:
-                    # Cannot generate the request from given parameters
-                    msg = """Cannot prepare a request message for provided
-                             arguments. Please check that your arguments match
-                             declared content type."""
-                    raise ApiException(status=0, reason=msg)
-            # For `GET`, `HEAD`
-            else:
-                r = self.pool_manager.request(method, url,
-                                              fields=query_params,
-                                              preload_content=_preload_content,
-                                              timeout=timeout,
-                                              headers=headers)
-        except urllib3.exceptions.SSLError as e:
-            msg = "{0}\n{1}".format(type(e).__name__, str(e))
-            raise ApiException(status=0, reason=msg)
-
-        if _preload_content:
-            r = RESTResponse(r)
-
-            # log response body
-            logger.debug("response body: %s", r.data)
-
-        if not 200 <= r.status <= 299:
-            if r.status == 401:
-                raise UnauthorizedException(http_resp=r)
-
-            if r.status == 403:
-                raise ForbiddenException(http_resp=r)
-
-            if r.status == 404:
-                raise NotFoundException(http_resp=r)
-
-            if 500 <= r.status <= 599:
-                raise ServiceException(http_resp=r)
-
-            raise ApiException(http_resp=r)
-
-        return r
-
-    def GET(self, url, headers=None, query_params=None, _preload_content=True,
-            _request_timeout=None):
-        return self.request("GET", url,
-                            headers=headers,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            query_params=query_params)
-
-    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
-             _request_timeout=None):
-        return self.request("HEAD", url,
-                            headers=headers,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            query_params=query_params)
-
-    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
-                body=None, _preload_content=True, _request_timeout=None):
-        return self.request("OPTIONS", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def DELETE(self, url, headers=None, query_params=None, body=None,
-               _preload_content=True, _request_timeout=None):
-        return self.request("DELETE", url,
-                            headers=headers,
-                            query_params=query_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def POST(self, url, headers=None, query_params=None, post_params=None,
-             body=None, _preload_content=True, _request_timeout=None):
-        return self.request("POST", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def PUT(self, url, headers=None, query_params=None, post_params=None,
-            body=None, _preload_content=True, _request_timeout=None):
-        return self.request("PUT", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def PATCH(self, url, headers=None, query_params=None, post_params=None,
-              body=None, _preload_content=True, _request_timeout=None):
-        return self.request("PATCH", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-# end of class RESTClientObject
-
-
-def is_ipv4(target):
-    """ Test if IPv4 address or not
-    """
-    try:
-        chk = ipaddress.IPv4Address(target)
-        return True
-    except ipaddress.AddressValueError:
-        return False
-
-
-def in_ipv4net(target, net):
-    """ Test if target belongs to given IPv4 network
-    """
-    try:
-        nw = ipaddress.IPv4Network(net)
-        ip = ipaddress.IPv4Address(target)
-        if ip in nw:
-            return True
-        return False
-    except ipaddress.AddressValueError:
-        return False
-    except ipaddress.NetmaskValueError:
-        return False
-
-
-def should_bypass_proxies(url, no_proxy=None):
-    """ Yet another requests.should_bypass_proxies
-    Test if proxies should not be used for a particular url.
-    """
-
-    parsed = urlparse(url)
-
-    # special cases
-    if parsed.hostname in [None, '']:
-        return True
-
-    # special cases
-    if no_proxy in [None, '']:
-        return False
-    if no_proxy == '*':
-        return True
-
-    no_proxy = no_proxy.lower().replace(' ', '');
-    entries = (
-        host for host in no_proxy.split(',') if host
-    )
-
-    if is_ipv4(parsed.hostname):
-        for item in entries:
-            if in_ipv4net(parsed.hostname, item):
-                return True
-    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy})
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import io
+import json
+import logging
+import re
+import ssl
+from urllib.parse import urlencode
+from urllib.parse import urlparse
+from urllib.request import proxy_bypass_environment
+import urllib3
+import ipaddress
+
+from invision_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+
+
+logger = logging.getLogger(__name__)
+
+
+class RESTResponse(io.IOBase):
+
+    def __init__(self, resp):
+        self.urllib3_response = resp
+        self.status = resp.status
+        self.reason = resp.reason
+        self.data = resp.data
+
+    def getheaders(self):
+        """Returns a dictionary of the response headers."""
+        return self.urllib3_response.getheaders()
+
+    def getheader(self, name, default=None):
+        """Returns a given response header."""
+        return self.urllib3_response.getheader(name, default)
+
+
+class RESTClientObject(object):
+
+    def __init__(self, configuration, pools_size=4, maxsize=None):
+        # urllib3.PoolManager will pass all kw parameters to connectionpool
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
+        # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
+        # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
+
+        # cert_reqs
+        if configuration.verify_ssl:
+            cert_reqs = ssl.CERT_REQUIRED
+        else:
+            cert_reqs = ssl.CERT_NONE
+
+        addition_pool_args = {}
+        if configuration.assert_hostname is not None:
+            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
+
+        if configuration.retries is not None:
+            addition_pool_args['retries'] = configuration.retries
+
+        if configuration.socket_options is not None:
+            addition_pool_args['socket_options'] = configuration.socket_options
+
+        if maxsize is None:
+            if configuration.connection_pool_maxsize is not None:
+                maxsize = configuration.connection_pool_maxsize
+            else:
+                maxsize = 4
+
+        # https pool manager
+        if configuration.proxy and not should_bypass_proxies(
+                configuration.host, no_proxy=configuration.no_proxy or ''):
+            self.pool_manager = urllib3.ProxyManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=configuration.ssl_ca_cert,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                proxy_url=configuration.proxy,
+                proxy_headers=configuration.proxy_headers,
+                **addition_pool_args
+            )
+        else:
+            self.pool_manager = urllib3.PoolManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=configuration.ssl_ca_cert,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                **addition_pool_args
+            )
+
+    def request(self, method, url, query_params=None, headers=None,
+                body=None, post_params=None, _preload_content=True,
+                _request_timeout=None):
+        """Perform requests.
+
+        :param method: http request method
+        :param url: http request url
+        :param query_params: query parameters in the url
+        :param headers: http request headers
+        :param body: request json body, for `application/json`
+        :param post_params: request post parameters,
+                            `application/x-www-form-urlencoded`
+                            and `multipart/form-data`
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        """
+        method = method.upper()
+        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
+                          'PATCH', 'OPTIONS']
+
+        if post_params and body:
+            raise ApiValueError(
+                "body parameter cannot be used with post_params parameter."
+            )
+
+        post_params = post_params or {}
+        headers = headers or {}
+
+        timeout = None
+        if _request_timeout:
+            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
+                timeout = urllib3.Timeout(total=_request_timeout)
+            elif (isinstance(_request_timeout, tuple) and
+                  len(_request_timeout) == 2):
+                timeout = urllib3.Timeout(
+                    connect=_request_timeout[0], read=_request_timeout[1])
+
+        try:
+            # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
+            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
+                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
+                if (method != 'DELETE') and ('Content-Type' not in headers):
+                    headers['Content-Type'] = 'application/json'
+                if query_params:
+                    url += '?' + urlencode(query_params)
+                if ('Content-Type' not in headers) or (re.search('json',
+                                                                 headers['Content-Type'], re.IGNORECASE)):
+                    request_body = None
+                    if body is not None:
+                        request_body = json.dumps(body)
+                    r = self.pool_manager.request(
+                        method, url,
+                        body=request_body,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
+                    r = self.pool_manager.request(
+                        method, url,
+                        fields=post_params,
+                        encode_multipart=False,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                elif headers['Content-Type'] == 'multipart/form-data':
+                    # must del headers['Content-Type'], or the correct
+                    # Content-Type which generated by urllib3 will be
+                    # overwritten.
+                    del headers['Content-Type']
+                    r = self.pool_manager.request(
+                        method, url,
+                        fields=post_params,
+                        encode_multipart=True,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                # Pass a `string` parameter directly in the body to support
+                # other content types than Json when `body` argument is
+                # provided in serialized form
+                elif isinstance(body, str) or isinstance(body, bytes):
+                    request_body = body
+                    r = self.pool_manager.request(
+                        method, url,
+                        body=request_body,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                else:
+                    # Cannot generate the request from given parameters
+                    msg = """Cannot prepare a request message for provided
+                             arguments. Please check that your arguments match
+                             declared content type."""
+                    raise ApiException(status=0, reason=msg)
+            # For `GET`, `HEAD`
+            else:
+                r = self.pool_manager.request(method, url,
+                                              fields=query_params,
+                                              preload_content=_preload_content,
+                                              timeout=timeout,
+                                              headers=headers)
+        except urllib3.exceptions.SSLError as e:
+            msg = "{0}\n{1}".format(type(e).__name__, str(e))
+            raise ApiException(status=0, reason=msg)
+
+        if _preload_content:
+            r = RESTResponse(r)
+
+            # log response body
+            logger.debug("response body: %s", r.data)
+
+        if not 200 <= r.status <= 299:
+            if r.status == 401:
+                raise UnauthorizedException(http_resp=r)
+
+            if r.status == 403:
+                raise ForbiddenException(http_resp=r)
+
+            if r.status == 404:
+                raise NotFoundException(http_resp=r)
+
+            if 500 <= r.status <= 599:
+                raise ServiceException(http_resp=r)
+
+            raise ApiException(http_resp=r)
+
+        return r
+
+    def GET(self, url, headers=None, query_params=None, _preload_content=True,
+            _request_timeout=None):
+        return self.request("GET", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
+             _request_timeout=None):
+        return self.request("HEAD", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
+                body=None, _preload_content=True, _request_timeout=None):
+        return self.request("OPTIONS", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def DELETE(self, url, headers=None, query_params=None, body=None,
+               _preload_content=True, _request_timeout=None):
+        return self.request("DELETE", url,
+                            headers=headers,
+                            query_params=query_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def POST(self, url, headers=None, query_params=None, post_params=None,
+             body=None, _preload_content=True, _request_timeout=None):
+        return self.request("POST", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def PUT(self, url, headers=None, query_params=None, post_params=None,
+            body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PUT", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def PATCH(self, url, headers=None, query_params=None, post_params=None,
+              body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PATCH", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+# end of class RESTClientObject
+
+
+def is_ipv4(target):
+    """ Test if IPv4 address or not
+    """
+    try:
+        chk = ipaddress.IPv4Address(target)
+        return True
+    except ipaddress.AddressValueError:
+        return False
+
+
+def in_ipv4net(target, net):
+    """ Test if target belongs to given IPv4 network
+    """
+    try:
+        nw = ipaddress.IPv4Network(net)
+        ip = ipaddress.IPv4Address(target)
+        if ip in nw:
+            return True
+        return False
+    except ipaddress.AddressValueError:
+        return False
+    except ipaddress.NetmaskValueError:
+        return False
+
+
+def should_bypass_proxies(url, no_proxy=None):
+    """ Yet another requests.should_bypass_proxies
+    Test if proxies should not be used for a particular url.
+    """
+
+    parsed = urlparse(url)
+
+    # special cases
+    if parsed.hostname in [None, '']:
+        return True
+
+    # special cases
+    if no_proxy in [None, '']:
+        return False
+    if no_proxy == '*':
+        return True
+
+    no_proxy = no_proxy.lower().replace(' ', '');
+    entries = (
+        host for host in no_proxy.split(',') if host
+    )
+
+    if is_ipv4(parsed.hostname):
+        for item in entries:
+            if in_ipv4net(parsed.hostname, item):
+                return True
+    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy})
```

### Comparing `invision-client-python-1.0.0/invision_client_python.egg-info/SOURCES.txt` & `invision-client-python-1.3.0b1/invision_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invision-client-python-1.0.0/setup.py` & `invision-client-python-1.3.0b1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-    Invision Community API
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-from setuptools import setup, find_packages  # noqa: H301
-
-NAME = "invision-client-python"
-VERSION = "1.0.0"
-# To install the library, run the following
-#
-# python setup.py install
-#
-# prerequisite: setuptools
-# http://pypi.python.org/pypi/setuptools
-
-REQUIRES = [
-  "urllib3 >= 1.25.3",
-  "python-dateutil",
-]
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description="Invision Community API",
-    author="OpenAPI Generator community",
-    author_email="team@openapitools.org",
-    url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Invision Community API"],
-    python_requires=">=3.6",
-    install_requires=REQUIRES,
-    packages=find_packages(exclude=["test", "tests"]),
-    include_package_data=True,
-    long_description="""\
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-    """
-)
+"""
+    Invision Community API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+from setuptools import setup, find_packages  # noqa: H301
+
+NAME = "invision-client-python"
+VERSION = "1.3.0b1"
+# To install the library, run the following
+#
+# python setup.py install
+#
+# prerequisite: setuptools
+# http://pypi.python.org/pypi/setuptools
+
+REQUIRES = [
+  "urllib3 >= 1.25.3",
+  "python-dateutil",
+]
+
+setup(
+    name=NAME,
+    version=VERSION,
+    description="Invision Community API",
+    author="OpenAPI Generator community",
+    author_email="team@openapitools.org",
+    url="",
+    keywords=["OpenAPI", "OpenAPI-Generator", "Invision Community API"],
+    python_requires=">=3.6",
+    install_requires=REQUIRES,
+    packages=find_packages(exclude=["test", "tests"]),
+    include_package_data=True,
+    long_description="""\
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    """
+)
```

### Comparing `invision-client-python-1.0.0/test/test_core_members_get200_response.py` & `invision-client-python-1.3.0b1/test/test_field.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.member import Member
-globals()['Member'] = Member
-from invision_client.model.core_members_get200_response import CoreMembersGet200Response
-
-
-class TestCoreMembersGet200Response(unittest.TestCase):
-    """CoreMembersGet200Response unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testCoreMembersGet200Response(self):
-        """Test CoreMembersGet200Response"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CoreMembersGet200Response()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.field import Field
+
+
+class TestField(unittest.TestCase):
+    """Field unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testField(self):
+        """Test Field"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Field()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_custom_api.py` & `invision-client-python-1.3.0b1/test/test_custom_api.py`

 * *Files identical despite different names*

### Comparing `invision-client-python-1.0.0/test/test_field.py` & `invision-client-python-1.3.0b1/test/test_fieldgroup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.field import Field
-
-
-class TestField(unittest.TestCase):
-    """Field unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testField(self):
-        """Test Field"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Field()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.field import Field
+globals()['Field'] = Field
+from invision_client.model.fieldgroup import Fieldgroup
+
+
+class TestFieldgroup(unittest.TestCase):
+    """Fieldgroup unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testFieldgroup(self):
+        """Test Fieldgroup"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Fieldgroup()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_forum.py` & `invision-client-python-1.3.0b1/test/test_core_members_get200_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.forum import Forum
-
-
-class TestForum(unittest.TestCase):
-    """Forum unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testForum(self):
-        """Test Forum"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Forum()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.member import Member
+globals()['Member'] = Member
+from invision_client.model.core_members_get200_response import CoreMembersGet200Response
+
+
+class TestCoreMembersGet200Response(unittest.TestCase):
+    """CoreMembersGet200Response unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testCoreMembersGet200Response(self):
+        """Test CoreMembersGet200Response"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = CoreMembersGet200Response()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_forums_api.py` & `invision-client-python-1.3.0b1/test/test_poll.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import unittest
-
-import invision_client
-from invision_client.api.forums_api import ForumsApi  # noqa: E501
-
-
-class TestForumsApi(unittest.TestCase):
-    """ForumsApi unit test stubs"""
-
-    def setUp(self):
-        self.api = ForumsApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_forums_forums_get(self):
-        """Test case for forums_forums_get
-
-        Get list of forums  # noqa: E501
-        """
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.question import Question
+globals()['Question'] = Question
+from invision_client.model.poll import Poll
+
+
+class TestPoll(unittest.TestCase):
+    """Poll unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testPoll(self):
+        """Test Poll"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Poll()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_forums_forums_get200_response.py` & `invision-client-python-1.3.0b1/test/test_post_reactions_inner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.forum import Forum
-globals()['Forum'] = Forum
-from invision_client.model.forums_forums_get200_response import ForumsForumsGet200Response
-
-
-class TestForumsForumsGet200Response(unittest.TestCase):
-    """ForumsForumsGet200Response unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testForumsForumsGet200Response(self):
-        """Test ForumsForumsGet200Response"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ForumsForumsGet200Response()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.post_reactions_inner import PostReactionsInner
+
+
+class TestPostReactionsInner(unittest.TestCase):
+    """PostReactionsInner unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testPostReactionsInner(self):
+        """Test PostReactionsInner"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = PostReactionsInner()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_group.py` & `invision-client-python-1.3.0b1/test/test_post.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.group import Group
-
-
-class TestGroup(unittest.TestCase):
-    """Group unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testGroup(self):
-        """Test Group"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Group()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.member import Member
+from invision_client.model.post_reactions_inner import PostReactionsInner
+globals()['Member'] = Member
+globals()['PostReactionsInner'] = PostReactionsInner
+from invision_client.model.post import Post
+
+
+class TestPost(unittest.TestCase):
+    """Post unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testPost(self):
+        """Test Post"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Post()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_member.py` & `invision-client-python-1.3.0b1/test/test_member.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.fieldgroup import Fieldgroup
-from invision_client.model.group import Group
-from invision_client.model.rank import Rank
-globals()['Fieldgroup'] = Fieldgroup
-globals()['Group'] = Group
-globals()['Rank'] = Rank
-from invision_client.model.member import Member
-
-
-class TestMember(unittest.TestCase):
-    """Member unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testMember(self):
-        """Test Member"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Member()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.fieldgroup import Fieldgroup
+from invision_client.model.group import Group
+from invision_client.model.rank import Rank
+globals()['Fieldgroup'] = Fieldgroup
+globals()['Group'] = Group
+globals()['Rank'] = Rank
+from invision_client.model.member import Member
+
+
+class TestMember(unittest.TestCase):
+    """Member unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testMember(self):
+        """Test Member"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Member()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_poll.py` & `invision-client-python-1.3.0b1/test/test_rank.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.question import Question
-globals()['Question'] = Question
-from invision_client.model.poll import Poll
-
-
-class TestPoll(unittest.TestCase):
-    """Poll unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testPoll(self):
-        """Test Poll"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Poll()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import invision_client
+from invision_client.model.rank import Rank
+
+
+class TestRank(unittest.TestCase):
+    """Rank unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testRank(self):
+        """Test Rank"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Rank()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `invision-client-python-1.0.0/test/test_question.py` & `invision-client-python-1.3.0b1/test/test_topics_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    Invision Community API Schema
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import invision_client
-from invision_client.model.question import Question
-
-
-class TestQuestion(unittest.TestCase):
-    """Question unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testQuestion(self):
-        """Test Question"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Question()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    Invision Community API Schema
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import unittest
+
+import invision_client
+from invision_client.api.topics_api import TopicsApi  # noqa: E501
+
+
+class TestTopicsApi(unittest.TestCase):
+    """TopicsApi unit test stubs"""
+
+    def setUp(self):
+        self.api = TopicsApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_forums_topics_post(self):
+        """Test case for forums_topics_post
+
+        Create a topic  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

