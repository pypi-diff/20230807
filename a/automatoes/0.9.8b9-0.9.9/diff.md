# Comparing `tmp/automatoes-0.9.8b9.tar.gz` & `tmp/automatoes-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatoes-0.9.8b9.tar", last modified: Fri Oct 14 16:33:11 2022, max compression
+gzip compressed data, was "automatoes-0.9.9.tar", last modified: Thu Dec 29 04:19:42 2022, max compression
```

## Comparing `automatoes-0.9.8b9.tar` & `automatoes-0.9.9.tar`

### file list

```diff
@@ -1,41 +1,55 @@
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-10-14 16:33:11.236301 automatoes-0.9.8b9/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2534 2020-11-23 16:49:03.000000 automatoes-0.9.8b9/CHANGELOG.md
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    11405 2021-11-23 08:10:32.000000 automatoes-0.9.8b9/LICENSE
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      199 2022-10-11 18:00:40.000000 automatoes-0.9.8b9/MANIFEST.in
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    12245 2022-10-14 16:33:11.236301 automatoes-0.9.8b9/PKG-INFO
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    11276 2022-03-12 06:32:03.000000 automatoes-0.9.8b9/README.md
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-10-14 16:33:11.234301 automatoes-0.9.8b9/automatoes/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1091 2022-10-14 16:31:34.000000 automatoes-0.9.8b9/automatoes/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    19018 2022-10-11 04:00:00.000000 automatoes-0.9.8b9/automatoes/acme.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    10163 2020-11-23 16:50:47.000000 automatoes-0.9.8b9/automatoes/authorize.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-10-14 16:33:11.235301 automatoes-0.9.8b9/automatoes/cli/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    10291 2022-10-14 15:47:31.000000 automatoes-0.9.8b9/automatoes/cli/__init__.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-10-14 16:33:11.236301 automatoes-0.9.8b9/automatoes/cli/commands/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2022-03-22 03:36:55.000000 automatoes-0.9.8b9/automatoes/cli/commands/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1025 2022-03-24 03:33:11.000000 automatoes-0.9.8b9/automatoes/cli/commands/account.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1493 2022-03-24 04:52:39.000000 automatoes-0.9.8b9/automatoes/cli/commands/help.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1009 2022-03-24 03:33:11.000000 automatoes-0.9.8b9/automatoes/cli/commands/order.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-10-14 16:33:11.236301 automatoes-0.9.8b9/automatoes/conf/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      196 2022-03-24 03:33:29.000000 automatoes-0.9.8b9/automatoes/conf/automatoes.yml
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     7102 2022-01-23 18:23:34.000000 automatoes-0.9.8b9/automatoes/crypto.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1319 2020-11-23 16:49:03.000000 automatoes-0.9.8b9/automatoes/errors.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4806 2022-10-14 16:28:37.000000 automatoes-0.9.8b9/automatoes/helpers.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2313 2022-10-10 20:50:31.000000 automatoes-0.9.8b9/automatoes/info.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     9399 2020-11-23 16:49:03.000000 automatoes-0.9.8b9/automatoes/issue.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3335 2022-03-22 04:22:33.000000 automatoes-0.9.8b9/automatoes/messages.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4425 2022-03-24 03:35:54.000000 automatoes-0.9.8b9/automatoes/model.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3908 2022-01-18 05:15:43.000000 automatoes-0.9.8b9/automatoes/protocol.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3528 2022-10-13 03:34:32.000000 automatoes-0.9.8b9/automatoes/register.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1869 2020-11-23 16:49:03.000000 automatoes-0.9.8b9/automatoes/revoke.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1758 2020-11-23 16:49:03.000000 automatoes-0.9.8b9/automatoes/upgrade.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-10-14 16:33:11.235301 automatoes-0.9.8b9/automatoes.egg-info/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    12245 2022-10-14 16:33:11.000000 automatoes-0.9.8b9/automatoes.egg-info/PKG-INFO
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      775 2022-10-14 16:33:11.000000 automatoes-0.9.8b9/automatoes.egg-info/SOURCES.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2022-10-14 16:33:11.000000 automatoes-0.9.8b9/automatoes.egg-info/dependency_links.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      101 2022-10-14 16:33:11.000000 automatoes-0.9.8b9/automatoes.egg-info/entry_points.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       44 2022-10-14 16:33:11.000000 automatoes-0.9.8b9/automatoes.egg-info/requires.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       11 2022-10-14 16:33:11.000000 automatoes-0.9.8b9/automatoes.egg-info/top_level.txt
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-10-14 16:33:11.236301 automatoes-0.9.8b9/requirements/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       44 2022-10-14 15:48:09.000000 automatoes-0.9.8b9/requirements/basic.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       38 2022-10-14 16:33:11.236301 automatoes-0.9.8b9/setup.cfg
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3123 2022-10-11 17:49:49.000000 automatoes-0.9.8b9/setup.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.513669 automatoes-0.9.9/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6035 2022-11-04 03:24:13.000000 automatoes-0.9.9/CHANGELOG.md
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    11417 2022-11-04 03:18:08.000000 automatoes-0.9.9/LICENSE
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      199 2022-10-11 18:00:40.000000 automatoes-0.9.9/MANIFEST.in
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    12430 2022-12-29 04:19:42.512669 automatoes-0.9.9/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    11411 2022-11-04 04:18:42.000000 automatoes-0.9.9/README.md
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.510669 automatoes-0.9.9/automatoes/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1085 2022-12-29 04:14:39.000000 automatoes-0.9.9/automatoes/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    19018 2022-10-11 04:00:00.000000 automatoes-0.9.9/automatoes/acme.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    10163 2020-11-23 16:50:47.000000 automatoes-0.9.9/automatoes/authorize.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.511669 automatoes-0.9.9/automatoes/bin/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-28 19:27:48.000000 automatoes-0.9.9/automatoes/bin/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      733 2022-12-29 04:04:18.000000 automatoes-0.9.9/automatoes/bin/automatoes-cli.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      772 2020-11-23 16:49:03.000000 automatoes-0.9.9/automatoes/bin/manuale-cli.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.511669 automatoes-0.9.9/automatoes/cli/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     9313 2022-12-29 04:05:10.000000 automatoes-0.9.9/automatoes/cli/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2705 2022-12-28 20:10:52.000000 automatoes-0.9.9/automatoes/cli/automatoes.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.511669 automatoes-0.9.9/automatoes/cli/commands/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2022-03-22 03:36:55.000000 automatoes-0.9.9/automatoes/cli/commands/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1338 2022-12-29 04:04:22.000000 automatoes-0.9.9/automatoes/cli/commands/account.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1444 2022-12-29 04:04:32.000000 automatoes-0.9.9/automatoes/cli/commands/help.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      960 2022-12-29 04:04:40.000000 automatoes-0.9.9/automatoes/cli/commands/order.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2022-11-04 23:29:01.000000 automatoes-0.9.9/automatoes/cli/manuale.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.512669 automatoes-0.9.9/automatoes/conf/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      196 2022-03-24 03:33:29.000000 automatoes-0.9.9/automatoes/conf/automatoes.yml
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      193 2022-12-29 04:05:43.000000 automatoes-0.9.9/automatoes/conf/manuale.yml
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     7102 2022-11-04 03:45:22.000000 automatoes-0.9.9/automatoes/crypto.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1319 2020-11-23 16:49:03.000000 automatoes-0.9.9/automatoes/errors.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2705 2022-10-15 02:03:14.000000 automatoes-0.9.9/automatoes/helpers.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2313 2022-10-10 20:50:31.000000 automatoes-0.9.9/automatoes/info.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     9399 2020-11-23 16:49:03.000000 automatoes-0.9.9/automatoes/issue.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3335 2022-03-22 04:22:33.000000 automatoes-0.9.9/automatoes/messages.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4425 2022-03-24 03:35:54.000000 automatoes-0.9.9/automatoes/model.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3908 2022-01-18 05:15:43.000000 automatoes-0.9.9/automatoes/protocol.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3630 2022-10-15 03:40:03.000000 automatoes-0.9.9/automatoes/register.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1869 2020-11-23 16:49:03.000000 automatoes-0.9.9/automatoes/revoke.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1758 2020-11-23 16:49:03.000000 automatoes-0.9.9/automatoes/upgrade.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.510669 automatoes-0.9.9/automatoes.egg-info/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    12430 2022-12-29 04:19:42.000000 automatoes-0.9.9/automatoes.egg-info/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1062 2022-12-29 04:19:42.000000 automatoes-0.9.9/automatoes.egg-info/SOURCES.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2022-12-29 04:19:42.000000 automatoes-0.9.9/automatoes.egg-info/dependency_links.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      101 2022-12-29 04:19:42.000000 automatoes-0.9.9/automatoes.egg-info/entry_points.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       44 2022-12-29 04:19:42.000000 automatoes-0.9.9/automatoes.egg-info/requires.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       17 2022-12-29 04:19:42.000000 automatoes-0.9.9/automatoes.egg-info/top_level.txt
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.512669 automatoes-0.9.9/requirements/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       44 2022-11-04 03:57:40.000000 automatoes-0.9.9/requirements/basic.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       38 2022-12-29 04:19:42.513669 automatoes-0.9.9/setup.cfg
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3174 2022-11-04 03:16:42.000000 automatoes-0.9.9/setup.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.512669 automatoes-0.9.9/tests/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      816 2022-11-04 21:30:56.000000 automatoes-0.9.9/tests/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1692 2022-11-04 21:46:50.000000 automatoes-0.9.9/tests/crypto_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2022-12-29 04:19:42.512669 automatoes-0.9.9/tests/features/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-11-23 16:49:03.000000 automatoes-0.9.9/tests/features/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2105 2022-01-18 04:44:31.000000 automatoes-0.9.9/tests/features/environment.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1004 2022-11-04 21:48:45.000000 automatoes-0.9.9/tests/runtests.py
```

### Comparing `automatoes-0.9.8b9/LICENSE` & `automatoes-0.9.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2019-2021 Flavio Garcia
+   Copyright 2019-2022 Flávio Gonçalves Garcia
    Copyright 2016-2017 Veeti Paananen under MIT License
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `automatoes-0.9.8b9/PKG-INFO` & `automatoes-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: automatoes
-Version: 0.9.8b9
+Version: 0.9.9
 Summary: Let's Encrypt/ACME V2 client replacement for Manuale. Manual or automated your choice.
 Home-page: https://github.com/candango/automatoes
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 License: Apache License V2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Candango Automat-o-es
 
 [![PyPI](https://img.shields.io/pypi/v/automatoes.svg)](https://pypi.org/project/automatoes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/automatoes.svg)](https://pypi.org/project/automatoes/#files)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Fautomatoes%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/automatoes/goto)
-[![Join the chat at https://gitter.im/candango/automatoes](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/candango/automatoes)
+[![Requirements Status](https://requires.io/github/candango/automatoes/requirements.svg?branch=develop)](https://requires.io/github/candango/automatoes/requirements/?branch=develop)
 
 
 Automatoes is a [Let's Encrypt](https://letsencrypt.org)/[ACME](https://github.com/ietf-wg-acme/acme/)
 client for advanced users and developers. It is intended to be used by anyone
 because we don't care if you're a robot, a processes or a person.
 
 We will keep the `manuale` command to provide manual workflow designed by the
@@ -65,15 +66,15 @@
 * Awful, undiscoverable name.
 
 * And finally, if the `openssl` binary is your spirit animal after all, you can
 still bring your own keys and/or CSR's. Everybody wins.
 
 ## Installation
 
-Python 3.5 or above is required.
+Python 3.6 or above is required.
 
 ### Using your package manager
 
 * TO DO
 
 * Package maintainers wanted: your package here?
 
@@ -203,29 +204,29 @@
 > 1. /acme/authz/challenge1 and /acme/authz/challenge2 are called and stored at
 > working_directory/orders/<sha256sum(domain.com other.domain.com)>
 > 1. the file name for challenges will be <domain>_challenge.json
 > 1. you fulfill all challenges either by dns or http, dns is default.
 > Just saying... you know the drill right? Same as before.
 > 1. manuale the Let's Encrypt! message and you can issue the certificate
 
-* If any challenge fails we delete the order file as the order will be set as
-invalid in the server. Invalid orders are considered fulfilled and not pending,
+* If any challenge fails we delete the order file because it will be invalid
+in the server side. Invalid orders are considered fulfilled and not pending,
 we can discard them.
-* If you hit Ctrl+c, the order will start from the server state as we can
-continue to process from the local file stored. Even challenges will be
-maintained, in a case when one challenge is validated and 2 are pending, if
-a Ctrl+c was hit, were recognize that in the next attempt.
-* If you call issue and there is an existent invalid order file than we delete
-the order and a new one is created.
+* If you hit Ctrl+c, the order will start from the state found in the local
+file stored. Even challenges will be maintained, in a case when one challenge
+is validated and 2 are pending, if Ctrl+c was hit, we'll recognize them in a 
+next attempt.
+* If you call the authorize command and there is an existent invalid order,
+this one will be deleted, and a new order will be created.
 
 > `manuale issue domain.com other.domain.com`
 
 > 1. /acme/order/<order_id>/finalize is called with the pem generated
 > or the one provided by you
-> 1. /acme/cert/<cert_id> is called and we place keys like we use to do before
+> 1. /acme/cert/<cert_id> is called, and we place keys like we use to do before
 > 1. we're done!
 
 * If you try to issue certificates for a domain sequence and an oder is pending
 or invalid, automatoes will ask you to run authorize before.
 
 After authorizing a domain sequence you need run issue with the same domain
 sequence because:
@@ -244,73 +245,78 @@
 >
 >   *  **If the CSR and order identifiers differ** <--- TALKING ABOUT THIS
 >
 >   *  If the account is not authorized for the identifiers indicated in the CSR
 >
 >   *  If the CSR requests extensions that the CA is not willing to include
 
-Trying to keeping thing as [KISS](https://www.acronymfinder.com/KISS.html) as
-possible we can complicate things later. Now we need ACME V2.
+Trying to keep thing as [KISS](https://www.acronymfinder.com/KISS.html) as
+possible, we can complicate things later. Now we need ACME V2.
 
 To create a certificate for a domain sequence authorized by a previous order
 just:
 
- 1. call authorize again. Chances are that no challenge will be needed but it
+ 1. call authorize again. Chances are that no challenge will be needed, but it
  depends on the ACME V2 server implementation.
  1. fulfill challenge(s) if needed
  1. call issue with same domain sequence authorize
  1. we're done!
 
-In another words, a domain sequence defines the order identifier locally.
+In other words, a domain sequence defines how the order identifier is created
+locally.
 
 The sha256sum command from coreutils can be used if you have a bash script
 to monitor `manuale` execution:
 
 ```
 > echo "domain.com other.domain.com" | sha256sum
 83ccaf9441b1abea98837e2f4c2fc18122c0e9ee4e39dd1995387f4d5d495b69  -
 
 > echo "other.domain.com domain.com" | sha256sum
 d0bd2c4957537572ffb7150a7dc89e61f44f9ab603b75be481118e37ec5a6163  -
 ```
 
-Storing meta files at working_directory/orders directory will let you
+Storing meta files at working_directory/orders directory will let us
 automate things better. Don't delete those files let Automatoes handle them for
 you.
 
 Here are more some features we can explore with this local file structure in
 the future:
 
  - control and advise about limits, as Acme V2 enforce limits for opened orders
  per account
  - list orders and status (for pending orders)
  - create partial authorizations (that will be on automatoes command not in
  manuale)
  - SDK?
  - Can you imagine more? Create a feature request for us.
 
-Also the manuale command can be called with a verbose parameter(-v) right now
+Also, the manuale command can be called with a verbose parameter(-v) right now
 providing more output.
 
 ## See also
 
 * [Best practices for server configuration](https://wiki.mozilla.org/Security/Server_Side_TLS)
 * [Configuration generator for common servers](https://mozilla.github.io/server-side-tls/ssl-config-generator/)
 * [Test your server](https://www.ssllabs.com/ssltest/)
 * [Other clients](https://community.letsencrypt.org/t/list-of-client-implementations/2103)
 
 ## Support
 
-For direct support [join gitter chat at https://gitter.im/candango/automatoes](https://gitter.im/candango/automatoes).
+For direct support create a
+[new discussion](https://github.com/candango/automatoes/discussions/new?category=help)
+or a
+[new ticket](https://github.com/candango/automatoes/issues/new)
+we'll love to see how to help you.
 
 Automatoes is one of
 [Candango Open Source Group](http://www.candango.org/projects/)
 initiatives. Available under the
 [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
 
-This web site and all documentation is licensed under
+This website and all documentation are licensed under
 [Creative Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
 
 Copyright © 2019-2022 Flávio Gonçalves Garcia
 Copyright © 2016-2017 Veeti Paananen under MIT License
```

### Comparing `automatoes-0.9.8b9/README.md` & `automatoes-0.9.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Candango Automat-o-es
 
 [![PyPI](https://img.shields.io/pypi/v/automatoes.svg)](https://pypi.org/project/automatoes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/automatoes.svg)](https://pypi.org/project/automatoes/#files)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Fautomatoes%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/automatoes/goto)
-[![Join the chat at https://gitter.im/candango/automatoes](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/candango/automatoes)
+[![Requirements Status](https://requires.io/github/candango/automatoes/requirements.svg?branch=develop)](https://requires.io/github/candango/automatoes/requirements/?branch=develop)
 
 
 Automatoes is a [Let's Encrypt](https://letsencrypt.org)/[ACME](https://github.com/ietf-wg-acme/acme/)
 client for advanced users and developers. It is intended to be used by anyone
 because we don't care if you're a robot, a processes or a person.
 
 We will keep the `manuale` command to provide manual workflow designed by the
@@ -41,15 +41,15 @@
 * Awful, undiscoverable name.
 
 * And finally, if the `openssl` binary is your spirit animal after all, you can
 still bring your own keys and/or CSR's. Everybody wins.
 
 ## Installation
 
-Python 3.5 or above is required.
+Python 3.6 or above is required.
 
 ### Using your package manager
 
 * TO DO
 
 * Package maintainers wanted: your package here?
 
@@ -179,29 +179,29 @@
 > 1. /acme/authz/challenge1 and /acme/authz/challenge2 are called and stored at
 > working_directory/orders/<sha256sum(domain.com other.domain.com)>
 > 1. the file name for challenges will be <domain>_challenge.json
 > 1. you fulfill all challenges either by dns or http, dns is default.
 > Just saying... you know the drill right? Same as before.
 > 1. manuale the Let's Encrypt! message and you can issue the certificate
 
-* If any challenge fails we delete the order file as the order will be set as
-invalid in the server. Invalid orders are considered fulfilled and not pending,
+* If any challenge fails we delete the order file because it will be invalid
+in the server side. Invalid orders are considered fulfilled and not pending,
 we can discard them.
-* If you hit Ctrl+c, the order will start from the server state as we can
-continue to process from the local file stored. Even challenges will be
-maintained, in a case when one challenge is validated and 2 are pending, if
-a Ctrl+c was hit, were recognize that in the next attempt.
-* If you call issue and there is an existent invalid order file than we delete
-the order and a new one is created.
+* If you hit Ctrl+c, the order will start from the state found in the local
+file stored. Even challenges will be maintained, in a case when one challenge
+is validated and 2 are pending, if Ctrl+c was hit, we'll recognize them in a 
+next attempt.
+* If you call the authorize command and there is an existent invalid order,
+this one will be deleted, and a new order will be created.
 
 > `manuale issue domain.com other.domain.com`
 
 > 1. /acme/order/<order_id>/finalize is called with the pem generated
 > or the one provided by you
-> 1. /acme/cert/<cert_id> is called and we place keys like we use to do before
+> 1. /acme/cert/<cert_id> is called, and we place keys like we use to do before
 > 1. we're done!
 
 * If you try to issue certificates for a domain sequence and an oder is pending
 or invalid, automatoes will ask you to run authorize before.
 
 After authorizing a domain sequence you need run issue with the same domain
 sequence because:
@@ -220,71 +220,76 @@
 >
 >   *  **If the CSR and order identifiers differ** <--- TALKING ABOUT THIS
 >
 >   *  If the account is not authorized for the identifiers indicated in the CSR
 >
 >   *  If the CSR requests extensions that the CA is not willing to include
 
-Trying to keeping thing as [KISS](https://www.acronymfinder.com/KISS.html) as
-possible we can complicate things later. Now we need ACME V2.
+Trying to keep thing as [KISS](https://www.acronymfinder.com/KISS.html) as
+possible, we can complicate things later. Now we need ACME V2.
 
 To create a certificate for a domain sequence authorized by a previous order
 just:
 
- 1. call authorize again. Chances are that no challenge will be needed but it
+ 1. call authorize again. Chances are that no challenge will be needed, but it
  depends on the ACME V2 server implementation.
  1. fulfill challenge(s) if needed
  1. call issue with same domain sequence authorize
  1. we're done!
 
-In another words, a domain sequence defines the order identifier locally.
+In other words, a domain sequence defines how the order identifier is created
+locally.
 
 The sha256sum command from coreutils can be used if you have a bash script
 to monitor `manuale` execution:
 
 ```
 > echo "domain.com other.domain.com" | sha256sum
 83ccaf9441b1abea98837e2f4c2fc18122c0e9ee4e39dd1995387f4d5d495b69  -
 
 > echo "other.domain.com domain.com" | sha256sum
 d0bd2c4957537572ffb7150a7dc89e61f44f9ab603b75be481118e37ec5a6163  -
 ```
 
-Storing meta files at working_directory/orders directory will let you
+Storing meta files at working_directory/orders directory will let us
 automate things better. Don't delete those files let Automatoes handle them for
 you.
 
 Here are more some features we can explore with this local file structure in
 the future:
 
  - control and advise about limits, as Acme V2 enforce limits for opened orders
  per account
  - list orders and status (for pending orders)
  - create partial authorizations (that will be on automatoes command not in
  manuale)
  - SDK?
  - Can you imagine more? Create a feature request for us.
 
-Also the manuale command can be called with a verbose parameter(-v) right now
+Also, the manuale command can be called with a verbose parameter(-v) right now
 providing more output.
 
 ## See also
 
 * [Best practices for server configuration](https://wiki.mozilla.org/Security/Server_Side_TLS)
 * [Configuration generator for common servers](https://mozilla.github.io/server-side-tls/ssl-config-generator/)
 * [Test your server](https://www.ssllabs.com/ssltest/)
 * [Other clients](https://community.letsencrypt.org/t/list-of-client-implementations/2103)
 
 ## Support
 
-For direct support [join gitter chat at https://gitter.im/candango/automatoes](https://gitter.im/candango/automatoes).
+For direct support create a
+[new discussion](https://github.com/candango/automatoes/discussions/new?category=help)
+or a
+[new ticket](https://github.com/candango/automatoes/issues/new)
+we'll love to see how to help you.
 
 Automatoes is one of
 [Candango Open Source Group](http://www.candango.org/projects/)
 initiatives. Available under the
 [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
 
-This web site and all documentation is licensed under
+This website and all documentation are licensed under
 [Creative Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
 
 Copyright © 2019-2022 Flávio Gonçalves Garcia
 Copyright © 2016-2017 Veeti Paananen under MIT License
```

### Comparing `automatoes-0.9.8b9/automatoes/__init__.py` & `automatoes-0.9.9/automatoes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __author__ = "Flavio Garcia <piraz@candango.org>"
-__version__ = (0, 9, 8, "b9")
+__version__ = (0, 9, 9)
 __licence__ = "Apache License V2.0"
 
 
 def get_version():
     if isinstance(__version__[-1], str):
         return '.'.join(map(str, __version__[:-1])) + __version__[-1]
     return ".".join(map(str, __version__))
```

### Comparing `automatoes-0.9.8b9/automatoes/acme.py` & `automatoes-0.9.9/automatoes/acme.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/authorize.py` & `automatoes-0.9.9/automatoes/authorize.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/cli/__init__.py` & `automatoes-0.9.9/automatoes/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2019-2022 Flávio Gonçalves Garcia
+# Copyright 2019-2023 Flávio Gonçalves Garcia
 # Copyright 2016-2017 Veeti Paananen under MIT License
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -25,21 +25,18 @@
 from ..model import Account
 from ..register import register
 from ..revoke import revoke
 from ..upgrade import upgrade
 from ..errors import AutomatoesError
 
 import argparse
-from cartola import config, sysexits
-import click
+from cartola import sysexits
 import logging
 import os
 import sys
-import taskio
-from taskio.core import TaskioCliContext
 
 
 logger = logging.getLogger(__name__)
 
 # Defaults
 LETS_ENCRYPT_PRODUCTION = "https://acme-v02.api.letsencrypt.org/"
 DEFAULT_ACCOUNT_PATH = 'account.json'
@@ -47,50 +44,25 @@
 
 AUTOMATOES_ROOT = os.path.abspath(
     os.path.join(os.path.dirname(__file__), "..", ".."))
 AUTOMATOES_CONFIG_PATH = os.path.join(AUTOMATOES_ROOT, "automatoes", "conf")
 AUTOMATOES_CONFIG_FILE = os.path.join(AUTOMATOES_CONFIG_PATH, "automatoes.yml")
 
 
-class AutomatoesCliContext(TaskioCliContext):
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.AUTOMATOES_ROOT = AUTOMATOES_ROOT
-        self.AUTOMATOES_CONFIG_PATH = AUTOMATOES_CONFIG_PATH
-        self.AUTOMATOES_CONFIG_FILE = AUTOMATOES_CONFIG_FILE
-        self.account = None
-        self.server = None
-        self.verbose = False
-        self.root = None
-
-
-pass_context = click.make_pass_decorator(AutomatoesCliContext,
-                                         ensure=True)
-
-
-@taskio.root(taskio_conf=config.load_yaml_file(AUTOMATOES_CONFIG_FILE))
-@click.option("-a", "--account", help=messages.OPTION_ACCOUNT_HELP,
-              default=DEFAULT_ACCOUNT_PATH, show_default=True)
-@click.option("-s", "--server", help=messages.OPTION_SERVER_HELP,
-              default=LETS_ENCRYPT_PRODUCTION, show_default=True)
-@pass_context
-def automatoes_cli(ctx: AutomatoesCliContext, account, server):
-    print(ctx)
-    ctx.account = account
-    ctx.server = server
-
-
 # Command handlers
 def _register(args):
+    verbose = False
+    if args.verbose > 0:
+        verbose = True
     register(
         server=args.server,
         account_path=args.account,
         email=args.email,
-        key_file=args.key_file
+        key_file=args.key_file,
+        verbose=verbose
     )
 
 
 def _authorize(args):
     paths = get_paths(args.account)
     account = load_account(args.account)
     verbose = False
```

### Comparing `automatoes-0.9.8b9/automatoes/cli/commands/account.py` & `automatoes-0.9.9/automatoes/cli/commands/order.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2019-2022 Flávio Gonçalves Garcia
-# Copyright 2016-2017 Veeti Paananen under MIT License
+# Copyright 2019-2023 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ...cli import pass_context
+from ..automatoes import pass_context
 import taskio
 
 
-@taskio.group(name="account", short_help="Group with commands related to "
-                                         "account managment")
+@taskio.group(name="order", short_help="Group with commands related to order "
+                                       "managment")
 @pass_context
-def account(ctx):
+def order(ctx):
     pass
 
 
-@account.command(name="list", short_help="List accounts")
+@order.command(name="list", short_help="List orders")
 @pass_context
-def account_list(ctx):
-    print("List accounts")
+def order_list(ctx):
+    print("List orders")
```

### Comparing `automatoes-0.9.8b9/automatoes/cli/commands/help.py` & `automatoes-0.9.9/automatoes/cli/commands/help.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2019-2022 Flávio Gonçalves Garcia
-# Copyright 2016-2017 Veeti Paananen under MIT License
+# Copyright 2019-2023 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ...cli import AutomatoesCliContext, pass_context
+from ..automatoes import AutomatoesCliContext, pass_context
 import click
 
 
 @click.command(short_help="Show the list of commands")
 @pass_context
 def commands(ctx: AutomatoesCliContext):
     rv = []
```

### Comparing `automatoes-0.9.8b9/automatoes/cli/commands/order.py` & `automatoes-0.9.9/automatoes/bin/automatoes-cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,22 @@
+#!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2019-2022 Flávio Gonçalves Garcia
-# Copyright 2016-2017 Veeti Paananen under MIT License
+# Copyright 2019-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ...cli import pass_context
-import taskio
+from automatoes.cli.automatoes import automatoes_cli
 
 
-@taskio.group(name="order", short_help="Group with commands related to order "
-                                       "managment")
-@pass_context
-def order(ctx):
-    pass
-
-
-@order.command(name="list", short_help="List orders")
-@pass_context
-def order_list(ctx):
-    print("List orders")
+if __name__ == "__main__":
+    automatoes_cli()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `automatoes-0.9.8b9/automatoes/crypto.py` & `automatoes-0.9.9/automatoes/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,13 +228,13 @@
     """
     Exports a X.509 certificate for the ACME protocol (JOSE Base64 DER).
     """
     return jose_b64(cert.public_bytes(Encoding.DER))
 
 
 def strip_certificates(data):
-    p = re.compile("-----BEGIN CERTIFICATE-----\n(?s).+?"
+    p = re.compile("(?s)-----BEGIN CERTIFICATE-----\n.+?"
                    "-----END CERTIFICATE-----\n")
     stripped_data = []
     for cert in p.findall(data.decode()):
         stripped_data.append(cert.encode())
     return stripped_data
```

### Comparing `automatoes-0.9.8b9/automatoes/errors.py` & `automatoes-0.9.9/automatoes/errors.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/info.py` & `automatoes-0.9.9/automatoes/info.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/issue.py` & `automatoes-0.9.9/automatoes/issue.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/messages.py` & `automatoes-0.9.9/automatoes/messages.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/model.py` & `automatoes-0.9.9/automatoes/model.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/protocol.py` & `automatoes-0.9.9/automatoes/protocol.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/register.py` & `automatoes-0.9.9/automatoes/register.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2019-2020 Flavio Garcia
+# Copyright 2019-2022 Flávio Gonçálves Garcia
 # Copyright 2016-2017 Veeti Paananen under MIT License
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -28,27 +28,28 @@
 )
 from .helpers import confirm
 from .model import Account
 
 import os
 
 
-def register(server, account_path, email, key_file):
+def register(server, account_path, email, key_file, verbose=False):
     print("Candango Automatoes {}. Manuale replacement.\n\n".format(
         get_version()))
     # Don't overwrite silently
     if os.path.exists(account_path):
         if not confirm("The account file {} already exists. Continuing will"
                        " overwrite it with the new key."
-                       " Continue?".format(account_path), default=False):
+                       " Continue?".format(account_path), default=False,
+                       verbose=verbose):
             raise AutomatoesError("Aborting.")
 
     # Confirm e-mail
     if not confirm("You're about to register a new account with e-mail "
-                   "{} as contact. Continue?".format(email)):
+                   "{} as contact. Continue?".format(email), verbose=verbose):
         raise AutomatoesError("Aborting.")
 
     # Load key or generate
     if key_file:
         try:
             with open(key_file, 'rb') as f:
                 account = Account(key=load_private_key(f.read()))
@@ -70,15 +71,15 @@
         if terms is None:
             print("  There is no terms being enforced in this server. "
                   "Resuming execution...")
             terms_agreed = True
         else:
             print("  This server requires you to agree to these terms:")
             print("    {}".format(terms))
-            if confirm("Agreed?"):
+            if confirm("Agreed?", verbose=verbose):
                 terms_agreed = True
             else:
                 print("Your account will still be created, but it won't be "
                       "usable before agreeing to terms.")
         acmev2.register(email, terms_agreed)
         print("  Account {} created.".format(account.uri))
     except IOError as e:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `automatoes-0.9.8b9/automatoes/revoke.py` & `automatoes-0.9.9/automatoes/revoke.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes/upgrade.py` & `automatoes-0.9.9/automatoes/upgrade.py`

 * *Files identical despite different names*

### Comparing `automatoes-0.9.8b9/automatoes.egg-info/PKG-INFO` & `automatoes-0.9.9/automatoes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: automatoes
-Version: 0.9.8b9
+Version: 0.9.9
 Summary: Let's Encrypt/ACME V2 client replacement for Manuale. Manual or automated your choice.
 Home-page: https://github.com/candango/automatoes
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 License: Apache License V2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Candango Automat-o-es
 
 [![PyPI](https://img.shields.io/pypi/v/automatoes.svg)](https://pypi.org/project/automatoes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/automatoes.svg)](https://pypi.org/project/automatoes/#files)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Fautomatoes%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/automatoes/goto)
-[![Join the chat at https://gitter.im/candango/automatoes](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/candango/automatoes)
+[![Requirements Status](https://requires.io/github/candango/automatoes/requirements.svg?branch=develop)](https://requires.io/github/candango/automatoes/requirements/?branch=develop)
 
 
 Automatoes is a [Let's Encrypt](https://letsencrypt.org)/[ACME](https://github.com/ietf-wg-acme/acme/)
 client for advanced users and developers. It is intended to be used by anyone
 because we don't care if you're a robot, a processes or a person.
 
 We will keep the `manuale` command to provide manual workflow designed by the
@@ -65,15 +66,15 @@
 * Awful, undiscoverable name.
 
 * And finally, if the `openssl` binary is your spirit animal after all, you can
 still bring your own keys and/or CSR's. Everybody wins.
 
 ## Installation
 
-Python 3.5 or above is required.
+Python 3.6 or above is required.
 
 ### Using your package manager
 
 * TO DO
 
 * Package maintainers wanted: your package here?
 
@@ -203,29 +204,29 @@
 > 1. /acme/authz/challenge1 and /acme/authz/challenge2 are called and stored at
 > working_directory/orders/<sha256sum(domain.com other.domain.com)>
 > 1. the file name for challenges will be <domain>_challenge.json
 > 1. you fulfill all challenges either by dns or http, dns is default.
 > Just saying... you know the drill right? Same as before.
 > 1. manuale the Let's Encrypt! message and you can issue the certificate
 
-* If any challenge fails we delete the order file as the order will be set as
-invalid in the server. Invalid orders are considered fulfilled and not pending,
+* If any challenge fails we delete the order file because it will be invalid
+in the server side. Invalid orders are considered fulfilled and not pending,
 we can discard them.
-* If you hit Ctrl+c, the order will start from the server state as we can
-continue to process from the local file stored. Even challenges will be
-maintained, in a case when one challenge is validated and 2 are pending, if
-a Ctrl+c was hit, were recognize that in the next attempt.
-* If you call issue and there is an existent invalid order file than we delete
-the order and a new one is created.
+* If you hit Ctrl+c, the order will start from the state found in the local
+file stored. Even challenges will be maintained, in a case when one challenge
+is validated and 2 are pending, if Ctrl+c was hit, we'll recognize them in a 
+next attempt.
+* If you call the authorize command and there is an existent invalid order,
+this one will be deleted, and a new order will be created.
 
 > `manuale issue domain.com other.domain.com`
 
 > 1. /acme/order/<order_id>/finalize is called with the pem generated
 > or the one provided by you
-> 1. /acme/cert/<cert_id> is called and we place keys like we use to do before
+> 1. /acme/cert/<cert_id> is called, and we place keys like we use to do before
 > 1. we're done!
 
 * If you try to issue certificates for a domain sequence and an oder is pending
 or invalid, automatoes will ask you to run authorize before.
 
 After authorizing a domain sequence you need run issue with the same domain
 sequence because:
@@ -244,73 +245,78 @@
 >
 >   *  **If the CSR and order identifiers differ** <--- TALKING ABOUT THIS
 >
 >   *  If the account is not authorized for the identifiers indicated in the CSR
 >
 >   *  If the CSR requests extensions that the CA is not willing to include
 
-Trying to keeping thing as [KISS](https://www.acronymfinder.com/KISS.html) as
-possible we can complicate things later. Now we need ACME V2.
+Trying to keep thing as [KISS](https://www.acronymfinder.com/KISS.html) as
+possible, we can complicate things later. Now we need ACME V2.
 
 To create a certificate for a domain sequence authorized by a previous order
 just:
 
- 1. call authorize again. Chances are that no challenge will be needed but it
+ 1. call authorize again. Chances are that no challenge will be needed, but it
  depends on the ACME V2 server implementation.
  1. fulfill challenge(s) if needed
  1. call issue with same domain sequence authorize
  1. we're done!
 
-In another words, a domain sequence defines the order identifier locally.
+In other words, a domain sequence defines how the order identifier is created
+locally.
 
 The sha256sum command from coreutils can be used if you have a bash script
 to monitor `manuale` execution:
 
 ```
 > echo "domain.com other.domain.com" | sha256sum
 83ccaf9441b1abea98837e2f4c2fc18122c0e9ee4e39dd1995387f4d5d495b69  -
 
 > echo "other.domain.com domain.com" | sha256sum
 d0bd2c4957537572ffb7150a7dc89e61f44f9ab603b75be481118e37ec5a6163  -
 ```
 
-Storing meta files at working_directory/orders directory will let you
+Storing meta files at working_directory/orders directory will let us
 automate things better. Don't delete those files let Automatoes handle them for
 you.
 
 Here are more some features we can explore with this local file structure in
 the future:
 
  - control and advise about limits, as Acme V2 enforce limits for opened orders
  per account
  - list orders and status (for pending orders)
  - create partial authorizations (that will be on automatoes command not in
  manuale)
  - SDK?
  - Can you imagine more? Create a feature request for us.
 
-Also the manuale command can be called with a verbose parameter(-v) right now
+Also, the manuale command can be called with a verbose parameter(-v) right now
 providing more output.
 
 ## See also
 
 * [Best practices for server configuration](https://wiki.mozilla.org/Security/Server_Side_TLS)
 * [Configuration generator for common servers](https://mozilla.github.io/server-side-tls/ssl-config-generator/)
 * [Test your server](https://www.ssllabs.com/ssltest/)
 * [Other clients](https://community.letsencrypt.org/t/list-of-client-implementations/2103)
 
 ## Support
 
-For direct support [join gitter chat at https://gitter.im/candango/automatoes](https://gitter.im/candango/automatoes).
+For direct support create a
+[new discussion](https://github.com/candango/automatoes/discussions/new?category=help)
+or a
+[new ticket](https://github.com/candango/automatoes/issues/new)
+we'll love to see how to help you.
 
 Automatoes is one of
 [Candango Open Source Group](http://www.candango.org/projects/)
 initiatives. Available under the
 [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
 
-This web site and all documentation is licensed under
+This website and all documentation are licensed under
 [Creative Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
 
 Copyright © 2019-2022 Flávio Gonçalves Garcia
 Copyright © 2016-2017 Veeti Paananen under MIT License
```

### Comparing `automatoes-0.9.8b9/automatoes.egg-info/SOURCES.txt` & `automatoes-0.9.9/automatoes.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,25 @@
 automatoes/upgrade.py
 automatoes.egg-info/PKG-INFO
 automatoes.egg-info/SOURCES.txt
 automatoes.egg-info/dependency_links.txt
 automatoes.egg-info/entry_points.txt
 automatoes.egg-info/requires.txt
 automatoes.egg-info/top_level.txt
+automatoes/bin/__init__.py
+automatoes/bin/automatoes-cli.py
+automatoes/bin/manuale-cli.py
 automatoes/cli/__init__.py
+automatoes/cli/automatoes.py
+automatoes/cli/manuale.py
 automatoes/cli/commands/__init__.py
 automatoes/cli/commands/account.py
 automatoes/cli/commands/help.py
 automatoes/cli/commands/order.py
 automatoes/conf/automatoes.yml
-requirements/basic.txt
+automatoes/conf/manuale.yml
+requirements/basic.txt
+tests/__init__.py
+tests/crypto_test.py
+tests/runtests.py
+tests/features/__init__.py
+tests/features/environment.py
```

### Comparing `automatoes-0.9.8b9/setup.py` & `automatoes-0.9.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,18 +63,19 @@
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     packages=find_packages(),
     package_dir={'automatoes': "automatoes"},
     include_package_data=True,
     install_requires=resolve_requires("requirements/basic.txt"),
     entry_points={
```

