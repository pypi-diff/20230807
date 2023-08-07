# Comparing `tmp/ofxstatement-0.8.0.tar.gz` & `tmp/ofxstatement-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofxstatement-0.8.0.tar", last modified: Mon Sep  6 05:57:57 2021, max compression
+gzip compressed data, was "ofxstatement-0.9.0.tar", last modified: Mon Aug  7 13:28:36 2023, max compression
```

## Comparing `ofxstatement-0.8.0.tar` & `ofxstatement-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2551 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/CHANGES.rst
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    35147 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/LICENSE.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      146 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/MANIFEST.in
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    16867 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    13511 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/README.rst
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      112 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/setup.cfg
--rwxrwxr-x   0 andrey    (1000) andrey    (1000)     1632 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/setup.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.535254 ofxstatement-0.8.0/src/
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/src/ofxstatement/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      862 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/configuration.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      580 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/exceptions.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    10510 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/ofx.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3451 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/parser.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1432 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/plugin.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/src/ofxstatement/plugins/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       75 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/plugins/README.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/plugins/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/py.typed
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    12232 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/statement.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/src/ofxstatement/tests/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/__init__.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/src/ofxstatement/tests/samples/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       29 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/samples/config.ini
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1089 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/test_configuration.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     4783 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/test_ofx.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     6619 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/test_ofx_invest.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      982 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/test_parser.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1100 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/test_plugin.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1601 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/test_statement.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     6508 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tests/test_tool.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     6166 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/tool.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      275 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement/ui.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-09-06 05:57:57.539255 ofxstatement-0.8.0/src/ofxstatement.egg-info/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    16867 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1092 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/SOURCES.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/dependency_links.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/entry_points.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       34 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/namespace_packages.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       62 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/requires.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       13 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/top_level.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2021-09-06 05:57:57.000000 ofxstatement-0.8.0/src/ofxstatement.egg-info/zip-safe
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2762 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/CHANGES.rst
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    35147 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/LICENSE.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      146 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/MANIFEST.in
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    17967 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    14420 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/README.rst
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      112 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/setup.cfg
+-rwxrwxr-x   0 andrey    (1000) andrey    (1000)     1632 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/setup.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.985330 ofxstatement-0.9.0/src/
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/src/ofxstatement/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      872 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/configuration.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      580 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/exceptions.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    10510 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/ofx.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3451 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/parser.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1432 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/plugin.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/src/ofxstatement/plugins/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       75 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/plugins/README.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/plugins/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/py.typed
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    12413 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/statement.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/src/ofxstatement/tests/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/__init__.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/src/ofxstatement/tests/samples/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       29 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/samples/config.ini
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1089 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/test_configuration.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     4782 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/test_ofx.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     6618 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/test_ofx_invest.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      982 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/test_parser.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1100 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/test_plugin.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1601 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/test_statement.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     6528 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tests/test_tool.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     6577 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/tool.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      275 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement/ui.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:28:36.989330 ofxstatement-0.9.0/src/ofxstatement.egg-info/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    17967 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1092 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       55 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/entry_points.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       34 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/namespace_packages.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       62 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/requires.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       13 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/top_level.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-08-07 13:28:36.000000 ofxstatement-0.9.0/src/ofxstatement.egg-info/zip-safe
```

### Comparing `ofxstatement-0.8.0/CHANGES.rst` & `ofxstatement-0.9.0/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 -------
 
+0.9.0 (2023-08-07)
+==================
+
+- New `-c` (`--config`) option for `convert` command, allows to specify the 
+  configuration file to use (#235).
+- Print the number of transactions in the output (#236).
+
+
 0.8.0 (2021-09-06)
 ==================
 
 - Support OFX CURRENCY and ORIGCURRENCY in statement lines. This allows plugins
   to add information about transaction currency to generated OFX statements.
 - Add `--pretty` flag to `convert` command to produce nicely intented OFX files.
```

### Comparing `ofxstatement-0.8.0/LICENSE.txt` & `ofxstatement-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/PKG-INFO` & `ofxstatement-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ofxstatement
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool to convert proprietary bank statement to OFX format, suitable for importing to GnuCash
 Home-page: https://github.com/kedder/ofxstatement
 Author: Andrey Lebedev
 Author-email: andrey@lebedev.lt
 License: GPLv3
 Keywords: ofx,banking,statement
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
@@ -19,14 +18,22 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Changes
 -------
 
+0.9.0 (2023-08-07)
+==================
+
+- New `-c` (`--config`) option for `convert` command, allows to specify the 
+  configuration file to use (#235).
+- Print the number of transactions in the output (#236).
+
+
 0.8.0 (2021-09-06)
 ==================
 
 - Support OFX CURRENCY and ORIGCURRENCY in statement lines. This allows plugins
   to add information about transaction currency to generated OFX statements.
 - Add `--pretty` flag to `convert` command to produce nicely intented OFX files.
 
@@ -111,16 +118,16 @@
   * ``refnum`` - translated to ``<REFNUM>`` in OFX.
   * ``trntype`` - translated to ``<TRNTYPE>`` in OFX.
 
 
 OFX Statement
 -------------
 
-.. image:: https://travis-ci.com/kedder/ofxstatement.svg?branch=master
-    :target: https://travis-ci.com/kedder/ofxstatement
+.. image:: https://github.com/kedder/ofxstatement/actions/workflows/test.yml/badge.svg?branch=master
+    :target: https://github.com/kedder/ofxstatement/actions/workflows/test.yml
 .. image:: https://coveralls.io/repos/kedder/ofxstatement/badge.png?branch=master
     :target: https://coveralls.io/r/kedder/ofxstatement?branch=master
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
@@ -225,14 +232,17 @@
                                   (``maxibps``) and banks using GPC
                                   format (e.g., FIO banka, module
                                   ``gpc``).
 
 `ofxstatement-airbankcz`_         Plugin for Air Bank a.s. (Czech Republic)
 `ofxstatement-raiffeisencz`_      Plugin for Raiffeisenbank a.s. (Czech Republic)
 `ofxstatement-unicreditcz`_       Plugin for UniCredit Bank Czech Republic and Slovakia
+`ofxstatement-equabankcz`_        Plugin for Equa Bank a.s. (Czech Republic)
+`ofxstatement-cz-komercni`_       Komerční banka (Czech Republic)
+`ofxstatement-mbankcz`_           mBank S.A. (Czech Republic)
 `ofxstatement-otp`_               Plugin for OTP Bank, operating in Hungary
 `ofxstatement-bubbas`_            Set of plugins, developed by @bubbas:
                                   ``dkb_cc`` and ``lbbamazon``.
 
 `banking.statements.osuuspankki`_ Finnish Osuuspankki bank
 `banking.statements.nordea`_      Nordea bank (at least Finnish branch of it)
 `ofxstatement-germany`_           Plugin for several german banks (1822direkt and Postbank at the moment)
@@ -249,45 +259,49 @@
 `ofxstatement-be-triodos`_        Belgian Triodos Bank CSV statements
 `ofxstatement-be-newb`_           Belgian cooperative bank newB
 `ofxstatement-betterment`_        Betterment (https://www.betterment.com/)
 `ofxstatement-simple`_            Simple (the bank, https://www.simple.com/) JSON financial statement format
 `ofxstatement-latvian`_           Latvian banks
 `ofxstatement-iso20022`_          Support for generic ISO-20022 format
 `ofxstatement-seb`_               SEB (Sweden), it parses Export.xlsx for private accounts
+`ofxstatement-ee-seb`_            SEB (Estonia), parses proprietary csv file
 `ofxstatement-paypal`_            PayPal, it parses ``*.csv`` for private accounts
 `ofxstatement-polish`_            Support for some Polish banks and financial institutions
 `ofxstatement-russian`_           Support for several Russian banks: Avangard, AlfaBank, Tinkoff, SberBank (both debit and csv), VTB.
 `ofxstatement-dab`_               DAB Bank (Germany)
 `ofxstatement-consors`_           Consorsbank (Germany)
 `ofxstatement-is-arionbanki`_     Arion bank in Iceland
 `ofxstatement-de-triodos`_        German Triodos Bank CSV statements (also works for GLS Bank)
 `ofxstatement-lansforsakringar`_  Länsförsäkringar (Sweden), it parses Kontoutdrag.xls for private accounts
 `ofxstatement-revolut`_           Revolut Mastercard
 `ofxstatement-transferwise`_      Transferwise CSV
+`ofxstatement-n26`_               N26 Bank
 `ofxstatement-sp-freiburg`_       Sparkasse Freiburg-Nördlicher Breisgau (Germany)
 `ofxstatement-al_bank`_           Arbejdernes Landsbank (Denmark)
 `ofxstatement-fineco`_            FinecoBank (Italy)
 `ofxstatement-intesasp`_          Intesa San Paolo (xlsx balance file)
 `ofxstatement-de-ing`_            Ing Diba Bank (Germany)
 `ofxstatement-us-first-republic`_ First Republic Bank (USA)
-`ofxstatement-cz-komercni`_       Komerční banka (Czech Republic)
 `ofxstatement-cd-tmb`_            Trust Merchant Bank (DRC)
 `ofxstatement-zm-stanbic`_        Stanbic Bank (Zambia)
 `ofxstatement-dutch`_             Dutch financial institutes like ICSCards and ING
 `ofxstatement-french`_            French financial institutes like BanquePopulaire
 `ofxstatement-mt940`_             All financial institutes providing Swift MT940 statements
 `ofxstatement-it-banks`_          Widiba and Webank italian banks
+`ofxstatement-chebanca`_          CheBanca! Italian bank (xlsx format)
 ================================= ============================================
 
 
 .. _ofxstatement-lithuanian: https://github.com/kedder/ofxstatement-lithuanian
 .. _ofxstatement-czech: https://gitlab.com/mcepl/ofxstatement-czech
 .. _ofxstatement-airbankcz: https://github.com/milankni/ofxstatement-airbankcz
 .. _ofxstatement-raiffeisencz: https://github.com/milankni/ofxstatement-raiffeisencz
 .. _ofxstatement-unicreditcz: https://github.com/milankni/ofxstatement-unicreditcz
+.. _ofxstatement-equabankcz: https://github.com/kosciCZ/ofxstatement-equabankcz
+.. _ofxstatement-mbankcz: https://github.com/SinyaWeo/ofxstatement-mbankcz
 .. _ofxstatement-otp: https://github.com/abesto/ofxstatement-otp
 .. _ofxstatement-bubbas: https://github.com/bubbas/ofxstatement-bubbas
 .. _banking.statements.osuuspankki: https://github.com/koodaamo/banking.statements.osuuspankki
 .. _banking.statements.nordea: https://github.com/koodaamo/banking.statements.nordea
 .. _ofxstatement-germany: https://github.com/MirkoDziadzka/ofxstatement-germany
 .. _ofxstatement-austrian: https://github.com/nblock/ofxstatement-austrian
 .. _ofxstatement-postfinance: https://pypi.python.org/pypi/ofxstatement-postfinance
@@ -299,41 +313,43 @@
 .. _ofxstatement-be-argenta: https://github.com/woutbr/ofxstatement-be-argenta
 .. _ofxstatement-be-crelan: https://gitlab.com/MagnificentMoustache/ofxstatement-be.crelan
 .. _ofxstatement-be-newb: https://github.com/SDaron/ofxstatement-be-newb
 .. _ofxstatement-betterment: https://github.com/cmayes/ofxstatement-betterment
 .. _ofxstatement-simple: https://github.com/cmayes/ofxstatement-simple
 .. _ofxstatement-latvian: https://github.com/gintsmurans/ofxstatement-latvian
 .. _ofxstatement-iso20022: https://github.com/kedder/ofxstatement-iso20022
-.. _ofxstatement-seb: https://github.com/themalkolm/ofxstatement-seb
+.. _ofxstatement-seb: https://github.com/gerasiov/ofxstatement-seb
 .. _ofxstatement-paypal: https://github.com/gerasiov/ofxstatement-paypal
 .. _ofxstatement-polish: https://github.com/yay6/ofxstatement-polish
 .. _ofxstatement-russian: https://github.com/gerasiov/ofxstatement-russian
 .. _ofxstatement-dab: https://github.com/JohannesKlug/ofxstatement-dab
 .. _ofxstatement-consors: https://github.com/JohannesKlug/ofxstatement-consors
 .. _ofxstatement-is-arionbanki: https://github.com/Dagur/ofxstatement-is-arionbanki
 .. _ofxstatement-be-triodos: https://github.com/renardeau/ofxstatement-be-triodos
 .. _ofxstatement-de-triodos: https://github.com/pianoslum/ofxstatement-de-triodos
 .. _ofxstatement-lansforsakringar: https://github.com/lbschenkel/ofxstatement-lansforsakringar
 .. _ofxstatement-revolut: https://github.com/mlaitinen/ofxstatement-revolut
 .. _ofxstatement-transferwise: https://github.com/kedder/ofxstatement-transferwise
+.. _ofxstatement-n26: https://github.com/3v1n0/ofxstatement-n26
 .. _ofxstatement-sp-freiburg: https://github.com/omarkohl/ofxstatement-sparkasse-freiburg
 .. _ofxstatement-al_bank: https://github.com/lbschenkel/ofxstatement-al_bank
 .. _ofxstatement-fineco: https://github.com/frankIT/ofxstatement-fineco
 .. _ofxstatement-intesasp: https://github.com/Jacotsu/ofxstatement-intesasp
 .. _ofxstatement-de-ing: https://github.com/fabolhak/ofxstatement-de-ing
 .. _ofxstatement-germany: https://github.com/MirkoDziadzka/ofxstatement-germany
 .. _ofxstatement-us-first-republic: https://github.com/medovina/ofxstatement-us-first-republic
 .. _ofxstatement-cz-komercni: https://github.com/medovina/ofxstatement-cz-komercni
 .. _ofxstatement-cd-tmb: https://github.com/BIZ4Africa/ofxstatement-cd-tmb
 .. _ofxstatement-zm-stanbic: https://github.com/BIZ4Africa/ofxstatement-zm-stanbic
 .. _ofxstatement-dutch: https://github.com/gpaulissen/ofxstatement-dutch
 .. _ofxstatement-french: https://github.com/gpaulissen/ofxstatement-french
 .. _ofxstatement-mt940: https://github.com/gpaulissen/ofxstatement-mt940
 .. _ofxstatement-it-banks: https://github.com/ecorini/ofxstatement-it-banks
-
+.. _ofxstatement-ee-seb: https://github.com/rsi2m/ofxstatement-ee-seb
+.. _ofxstatement-chebanca: https://github.com/3v1n0/ofxstatement-chebanca
 Advanced Configuration
 ======================
 
 While ofxstatement can be used without any configuration, some plugins may
 accept additional configuration parameters. These parameters can be specified
 in a configuration file. The configuration file can be edited using the ``edit-config``
 command that opens your favorite editor (defined by environment variable
@@ -368,19 +384,21 @@
 To convert the proprietary CSV file ``danske.csv`` into the OFX file ``danske.ofx``, run::
 
     $ ofxstatement -t danske:usd danske.csv danske.ofx
 
 Note that configuration parameters are plugin specific. See the plugin
 documentation for more info.
 
+To use a custom configuration file, pass the ``-c`` / ``--config`` option::
+
+    $ ofxstatement convert -t pluginname -c /path/to/myconfig.ini input.csv output.ofx
+
 Writing your own Plugin
 =======================
 
 If the plugin for your bank has not been developed yet (see `Known plugins`_
 section above) you can easily write your own, provided you have some knowledge
 about the Python programming language. There is an `ofxstatement-sample`_
 plugin project available that provides sample boilerplate and describes the
 plugin development process in detail.
 
 .. _ofxstatement-sample: https://github.com/kedder/ofxstatement-sample
-
-
```

### Comparing `ofxstatement-0.8.0/README.rst` & `ofxstatement-0.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 OFX Statement
 -------------
 
-.. image:: https://travis-ci.com/kedder/ofxstatement.svg?branch=master
-    :target: https://travis-ci.com/kedder/ofxstatement
+.. image:: https://github.com/kedder/ofxstatement/actions/workflows/test.yml/badge.svg?branch=master
+    :target: https://github.com/kedder/ofxstatement/actions/workflows/test.yml
 .. image:: https://coveralls.io/repos/kedder/ofxstatement/badge.png?branch=master
     :target: https://coveralls.io/r/kedder/ofxstatement?branch=master
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
@@ -111,14 +111,17 @@
                                   (``maxibps``) and banks using GPC
                                   format (e.g., FIO banka, module
                                   ``gpc``).
 
 `ofxstatement-airbankcz`_         Plugin for Air Bank a.s. (Czech Republic)
 `ofxstatement-raiffeisencz`_      Plugin for Raiffeisenbank a.s. (Czech Republic)
 `ofxstatement-unicreditcz`_       Plugin for UniCredit Bank Czech Republic and Slovakia
+`ofxstatement-equabankcz`_        Plugin for Equa Bank a.s. (Czech Republic)
+`ofxstatement-cz-komercni`_       Komerční banka (Czech Republic)
+`ofxstatement-mbankcz`_           mBank S.A. (Czech Republic)
 `ofxstatement-otp`_               Plugin for OTP Bank, operating in Hungary
 `ofxstatement-bubbas`_            Set of plugins, developed by @bubbas:
                                   ``dkb_cc`` and ``lbbamazon``.
 
 `banking.statements.osuuspankki`_ Finnish Osuuspankki bank
 `banking.statements.nordea`_      Nordea bank (at least Finnish branch of it)
 `ofxstatement-germany`_           Plugin for several german banks (1822direkt and Postbank at the moment)
@@ -135,45 +138,49 @@
 `ofxstatement-be-triodos`_        Belgian Triodos Bank CSV statements
 `ofxstatement-be-newb`_           Belgian cooperative bank newB
 `ofxstatement-betterment`_        Betterment (https://www.betterment.com/)
 `ofxstatement-simple`_            Simple (the bank, https://www.simple.com/) JSON financial statement format
 `ofxstatement-latvian`_           Latvian banks
 `ofxstatement-iso20022`_          Support for generic ISO-20022 format
 `ofxstatement-seb`_               SEB (Sweden), it parses Export.xlsx for private accounts
+`ofxstatement-ee-seb`_            SEB (Estonia), parses proprietary csv file
 `ofxstatement-paypal`_            PayPal, it parses ``*.csv`` for private accounts
 `ofxstatement-polish`_            Support for some Polish banks and financial institutions
 `ofxstatement-russian`_           Support for several Russian banks: Avangard, AlfaBank, Tinkoff, SberBank (both debit and csv), VTB.
 `ofxstatement-dab`_               DAB Bank (Germany)
 `ofxstatement-consors`_           Consorsbank (Germany)
 `ofxstatement-is-arionbanki`_     Arion bank in Iceland
 `ofxstatement-de-triodos`_        German Triodos Bank CSV statements (also works for GLS Bank)
 `ofxstatement-lansforsakringar`_  Länsförsäkringar (Sweden), it parses Kontoutdrag.xls for private accounts
 `ofxstatement-revolut`_           Revolut Mastercard
 `ofxstatement-transferwise`_      Transferwise CSV
+`ofxstatement-n26`_               N26 Bank
 `ofxstatement-sp-freiburg`_       Sparkasse Freiburg-Nördlicher Breisgau (Germany)
 `ofxstatement-al_bank`_           Arbejdernes Landsbank (Denmark)
 `ofxstatement-fineco`_            FinecoBank (Italy)
 `ofxstatement-intesasp`_          Intesa San Paolo (xlsx balance file)
 `ofxstatement-de-ing`_            Ing Diba Bank (Germany)
 `ofxstatement-us-first-republic`_ First Republic Bank (USA)
-`ofxstatement-cz-komercni`_       Komerční banka (Czech Republic)
 `ofxstatement-cd-tmb`_            Trust Merchant Bank (DRC)
 `ofxstatement-zm-stanbic`_        Stanbic Bank (Zambia)
 `ofxstatement-dutch`_             Dutch financial institutes like ICSCards and ING
 `ofxstatement-french`_            French financial institutes like BanquePopulaire
 `ofxstatement-mt940`_             All financial institutes providing Swift MT940 statements
 `ofxstatement-it-banks`_          Widiba and Webank italian banks
+`ofxstatement-chebanca`_          CheBanca! Italian bank (xlsx format)
 ================================= ============================================
 
 
 .. _ofxstatement-lithuanian: https://github.com/kedder/ofxstatement-lithuanian
 .. _ofxstatement-czech: https://gitlab.com/mcepl/ofxstatement-czech
 .. _ofxstatement-airbankcz: https://github.com/milankni/ofxstatement-airbankcz
 .. _ofxstatement-raiffeisencz: https://github.com/milankni/ofxstatement-raiffeisencz
 .. _ofxstatement-unicreditcz: https://github.com/milankni/ofxstatement-unicreditcz
+.. _ofxstatement-equabankcz: https://github.com/kosciCZ/ofxstatement-equabankcz
+.. _ofxstatement-mbankcz: https://github.com/SinyaWeo/ofxstatement-mbankcz
 .. _ofxstatement-otp: https://github.com/abesto/ofxstatement-otp
 .. _ofxstatement-bubbas: https://github.com/bubbas/ofxstatement-bubbas
 .. _banking.statements.osuuspankki: https://github.com/koodaamo/banking.statements.osuuspankki
 .. _banking.statements.nordea: https://github.com/koodaamo/banking.statements.nordea
 .. _ofxstatement-germany: https://github.com/MirkoDziadzka/ofxstatement-germany
 .. _ofxstatement-austrian: https://github.com/nblock/ofxstatement-austrian
 .. _ofxstatement-postfinance: https://pypi.python.org/pypi/ofxstatement-postfinance
@@ -185,41 +192,43 @@
 .. _ofxstatement-be-argenta: https://github.com/woutbr/ofxstatement-be-argenta
 .. _ofxstatement-be-crelan: https://gitlab.com/MagnificentMoustache/ofxstatement-be.crelan
 .. _ofxstatement-be-newb: https://github.com/SDaron/ofxstatement-be-newb
 .. _ofxstatement-betterment: https://github.com/cmayes/ofxstatement-betterment
 .. _ofxstatement-simple: https://github.com/cmayes/ofxstatement-simple
 .. _ofxstatement-latvian: https://github.com/gintsmurans/ofxstatement-latvian
 .. _ofxstatement-iso20022: https://github.com/kedder/ofxstatement-iso20022
-.. _ofxstatement-seb: https://github.com/themalkolm/ofxstatement-seb
+.. _ofxstatement-seb: https://github.com/gerasiov/ofxstatement-seb
 .. _ofxstatement-paypal: https://github.com/gerasiov/ofxstatement-paypal
 .. _ofxstatement-polish: https://github.com/yay6/ofxstatement-polish
 .. _ofxstatement-russian: https://github.com/gerasiov/ofxstatement-russian
 .. _ofxstatement-dab: https://github.com/JohannesKlug/ofxstatement-dab
 .. _ofxstatement-consors: https://github.com/JohannesKlug/ofxstatement-consors
 .. _ofxstatement-is-arionbanki: https://github.com/Dagur/ofxstatement-is-arionbanki
 .. _ofxstatement-be-triodos: https://github.com/renardeau/ofxstatement-be-triodos
 .. _ofxstatement-de-triodos: https://github.com/pianoslum/ofxstatement-de-triodos
 .. _ofxstatement-lansforsakringar: https://github.com/lbschenkel/ofxstatement-lansforsakringar
 .. _ofxstatement-revolut: https://github.com/mlaitinen/ofxstatement-revolut
 .. _ofxstatement-transferwise: https://github.com/kedder/ofxstatement-transferwise
+.. _ofxstatement-n26: https://github.com/3v1n0/ofxstatement-n26
 .. _ofxstatement-sp-freiburg: https://github.com/omarkohl/ofxstatement-sparkasse-freiburg
 .. _ofxstatement-al_bank: https://github.com/lbschenkel/ofxstatement-al_bank
 .. _ofxstatement-fineco: https://github.com/frankIT/ofxstatement-fineco
 .. _ofxstatement-intesasp: https://github.com/Jacotsu/ofxstatement-intesasp
 .. _ofxstatement-de-ing: https://github.com/fabolhak/ofxstatement-de-ing
 .. _ofxstatement-germany: https://github.com/MirkoDziadzka/ofxstatement-germany
 .. _ofxstatement-us-first-republic: https://github.com/medovina/ofxstatement-us-first-republic
 .. _ofxstatement-cz-komercni: https://github.com/medovina/ofxstatement-cz-komercni
 .. _ofxstatement-cd-tmb: https://github.com/BIZ4Africa/ofxstatement-cd-tmb
 .. _ofxstatement-zm-stanbic: https://github.com/BIZ4Africa/ofxstatement-zm-stanbic
 .. _ofxstatement-dutch: https://github.com/gpaulissen/ofxstatement-dutch
 .. _ofxstatement-french: https://github.com/gpaulissen/ofxstatement-french
 .. _ofxstatement-mt940: https://github.com/gpaulissen/ofxstatement-mt940
 .. _ofxstatement-it-banks: https://github.com/ecorini/ofxstatement-it-banks
-
+.. _ofxstatement-ee-seb: https://github.com/rsi2m/ofxstatement-ee-seb
+.. _ofxstatement-chebanca: https://github.com/3v1n0/ofxstatement-chebanca
 Advanced Configuration
 ======================
 
 While ofxstatement can be used without any configuration, some plugins may
 accept additional configuration parameters. These parameters can be specified
 in a configuration file. The configuration file can be edited using the ``edit-config``
 command that opens your favorite editor (defined by environment variable
@@ -254,14 +263,18 @@
 To convert the proprietary CSV file ``danske.csv`` into the OFX file ``danske.ofx``, run::
 
     $ ofxstatement -t danske:usd danske.csv danske.ofx
 
 Note that configuration parameters are plugin specific. See the plugin
 documentation for more info.
 
+To use a custom configuration file, pass the ``-c`` / ``--config`` option::
+
+    $ ofxstatement convert -t pluginname -c /path/to/myconfig.ini input.csv output.ofx
+
 Writing your own Plugin
 =======================
 
 If the plugin for your bank has not been developed yet (see `Known plugins`_
 section above) you can easily write your own, provided you have some knowledge
 about the Python programming language. There is an `ofxstatement-sample`_
 plugin project available that provides sample boilerplate and describes the
```

### Comparing `ofxstatement-0.8.0/setup.py` & `ofxstatement-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 from setuptools import find_packages
 from setuptools.command.test import test as TestCommand
 from distutils.core import setup
 import unittest
 import sys
 
-version = "0.8.0"
+version = "0.9.0"
 
 with open("CHANGES.rst") as chlogf, open("README.rst", encoding="utf-8") as rdmef:
     long_description = chlogf.read() + "\n\n" + rdmef.read()
 
 setup(
     name="ofxstatement",
     version=version,
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement/configuration.py` & `ofxstatement-0.9.0/src/ofxstatement/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def get_default_location() -> str:
     cdir = appdirs.user_config_dir(APP_NAME, APP_AUTHOR)
     return os.path.join(cdir, "config.ini")
 
 
-def read(location: str = None) -> Optional[MutableMapping]:
+def read(location: Optional[str] = None) -> Optional[MutableMapping]:
     if not location:
         location = get_default_location()
 
     if not os.path.exists(location):
         return None
 
     config = configparser.ConfigParser()
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement/exceptions.py` & `ofxstatement-0.9.0/src/ofxstatement/exceptions.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/ofx.py` & `ofxstatement-0.9.0/src/ofxstatement/ofx.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/parser.py` & `ofxstatement-0.9.0/src/ofxstatement/parser.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/plugin.py` & `ofxstatement-0.9.0/src/ofxstatement/plugin.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/statement.py` & `ofxstatement-0.9.0/src/ofxstatement/statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     start_date: Optional[datetime] = None
 
     end_balance: Optional[D] = None
     end_date: Optional[datetime] = None
 
     def __init__(
         self,
-        bank_id: str = None,
-        account_id: str = None,
-        currency: str = None,
+        bank_id: Optional[str] = None,
+        account_id: Optional[str] = None,
+        currency: Optional[str] = None,
         account_type: str = "CHECKING",
     ) -> None:
         self.lines = []
         self.invest_lines = []
         self.bank_id = bank_id
         self.account_id = account_id
         self.currency = currency
@@ -107,15 +107,15 @@
                 )
             )
             if not isclose(self.start_balance + total_amount, self.end_balance):
                 raise exceptions.ValidationError(msg, self)
 
 
 class StatementLine(Printable):
-    """Statement line data. """
+    """Statement line data."""
 
     id: Optional[str]
     # Date transaction was posted to account
     date: Optional[datetime]
     memo: Optional[str]
 
     # Amount of transaction
@@ -144,15 +144,19 @@
     # currency). Available since 0.7.2
     currency: Optional["Currency"] = None
 
     # Original amount and the original (foreign) currency. Available since 0.7.2
     orig_currency: Optional["Currency"] = None
 
     def __init__(
-        self, id: str = None, date: datetime = None, memo: str = None, amount: D = None
+        self,
+        id: Optional[str] = None,
+        date: Optional[datetime] = None,
+        memo: Optional[str] = None,
+        amount: Optional[D] = None,
     ) -> None:
         self.id = id
         self.date = date
         self.memo = memo
         self.amount = amount
 
         self.date_user = None
@@ -196,21 +200,21 @@
     """
 
     # ISO-4217 3-letter currency identifier
     symbol: str
     # Ratio of statement currency to `symbol` currency
     rate: Optional[D]
 
-    def __init__(self, symbol: str, rate: D = None) -> None:
+    def __init__(self, symbol: str, rate: Optional[D] = None) -> None:
         self.symbol = symbol
         self.rate = rate
 
 
 class InvestStatementLine(Printable):
-    """Invest statement line data. """
+    """Invest statement line data."""
 
     id: Optional[str]
     # Date transaction was posted to account
     date: Optional[datetime]
     memo: Optional[str]
 
     # ID or ticker of underlying security
@@ -224,21 +228,21 @@
     amount: Optional[D]
     fees: Optional[D] = None
     unit_price: Optional[D] = None  # required for buy/sell transactions
     units: Optional[D] = None  # required for buy/sell transactions
 
     def __init__(
         self,
-        id: str = None,
-        date: datetime = None,
-        memo: str = None,
-        trntype: str = None,
-        trntype_detailed: str = None,
-        security_id: str = None,
-        amount: D = None,
+        id: Optional[str] = None,
+        date: Optional[datetime] = None,
+        memo: Optional[str] = None,
+        trntype: Optional[str] = None,
+        trntype_detailed: Optional[str] = None,
+        security_id: Optional[str] = None,
+        amount: Optional[D] = None,
     ) -> None:
         self.id = id
         self.date = date
         self.memo = memo
         self.trntype = trntype
         self.trntype_detailed = trntype_detailed
         self.security_id = security_id
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tests/test_configuration.py` & `ofxstatement-0.9.0/src/ofxstatement/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tests/test_ofx.py` & `ofxstatement-0.9.0/src/ofxstatement/tests/test_ofx.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 def prettyPrint(xmlstr):
     dom = xml.dom.minidom.parseString(xmlstr)
     return dom.toprettyxml().replace("\t", "    ").replace("<!-- ", "<!--")
 
 
 class OfxWriterTest(TestCase):
     def test_ofxWriter(self) -> None:
-
         # Create sample statement:
         statement = Statement("BID", "ACCID", "LTL")
         statement.lines.append(
             StatementLine("1", datetime(2012, 2, 12), "Sample 1", Decimal("15.4"))
         )
         line = StatementLine("2", datetime(2012, 2, 12), "Sample 2", Decimal("25.0"))
         line.payee = ""
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tests/test_ofx_invest.py` & `ofxstatement-0.9.0/src/ofxstatement/tests/test_ofx_invest.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,14 @@
 def prettyPrint(xmlstr):
     dom = xml.dom.minidom.parseString(xmlstr)
     return dom.toprettyxml().replace("\t", "    ").replace("<!-- ", "<!--")
 
 
 class OfxInvestLinesWriterTest(TestCase):
     def test_ofxWriter(self) -> None:
-
         # Create sample statement:
         statement = Statement("BID", "ACCID", "LTL")
         statement.broker_id = "BROKERID"
         statement.end_date = datetime(2021, 5, 1)
 
         invest_line = InvestStatementLine(
             "3",
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tests/test_parser.py` & `ofxstatement-0.9.0/src/ofxstatement/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tests/test_plugin.py` & `ofxstatement-0.9.0/src/ofxstatement/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tests/test_statement.py` & `ofxstatement-0.9.0/src/ofxstatement/tests/test_statement.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tests/test_tool.py` & `ofxstatement-0.9.0/src/ofxstatement/tests/test_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         with configpatch, pluginpatch:
             ret = tool.convert(args)
 
         self.assertEqual(ret, 0)
         self.assertEqual(
             self.log.getvalue().splitlines(),
-            ["INFO: Conversion completed: %s" % inputfname],
+            ["INFO: Conversion completed: (0 lines) %s" % inputfname],
         )
 
     def test_convert_noconf(self) -> None:
         inputfname = os.path.join(self.tmpdir, "input")
         outputfname = os.path.join(self.tmpdir, "output")
         args = mock.Mock(type="test", input=inputfname, output=outputfname)
 
@@ -61,15 +61,15 @@
         with noconfigpatch, pluginpatch:
             ret = tool.convert(args)
 
         self.assertEqual(ret, 0)
 
         self.assertEqual(
             self.log.getvalue().splitlines(),
-            ["INFO: Conversion completed: %s" % inputfname],
+            ["INFO: Conversion completed: (0 lines) %s" % inputfname],
         )
 
     def test_convert_parseerror(self) -> None:
         inputfname = os.path.join(self.tmpdir, "input")
         outputfname = os.path.join(self.tmpdir, "output")
 
         class FailingParser(parser.StatementParser):
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement/tool.py` & `ofxstatement-0.9.0/src/ofxstatement/tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 import platform
 import sys
 import contextlib
 
 import pkg_resources
 
 from ofxstatement import ui, configuration, plugin, ofx, exceptions
+from typing import Optional, TextIO, Generator
 
 
 log = logging.getLogger(__name__)
 
 
 @contextlib.contextmanager
-def smart_open(filename: str = None, encoding: str = None):
+def smart_open(
+    filename: Optional[str] = None, encoding: Optional[str] = None
+) -> Generator[TextIO, None, None]:
     """See https://stackoverflow.com/questions/17602878/how-to-handle-both-with-open-and-sys-stdout-nicely"""  # noqa
+    fh: TextIO
+
     if filename and filename != "-":
         # encoding is required in cases when OS defaults to encoding which
         # doesn't support unicode characters, for example Windows defaults to
         # 'cp1252'
         fh = open(filename, "w", encoding=encoding)
     else:
         fh = sys.stdout
@@ -66,14 +71,21 @@
 
     subparsers = parser.add_subparsers(title="action")
 
     # convert
     parser_convert = subparsers.add_parser("convert", help="convert to OFX")
 
     parser_convert.add_argument(
+        "-c",
+        "--config",
+        metavar="myconfig.ini",
+        default=None,
+        help="custom config file to use",
+    )
+    parser_convert.add_argument(
         "-t",
         "--type",
         required=True,
         help=(
             "input file type. This is a section in "
             "the config file or plugin name if you "
             "have no config file."
@@ -136,15 +148,15 @@
         os.makedirs(configdir, mode=0o700)
     log.info("Running editor: %s %s" % (editor, configfname))
     subprocess.call(shlex.split(editor, posix=(os.name == "posix")) + [configfname])
 
 
 def convert(args: argparse.Namespace) -> int:
     appui = ui.UI()
-    config = configuration.read()
+    config = configuration.read(args.config)
 
     if config is None:
         # No configuration mode
         settings = {}
         pname = args.type
     else:
         # Configuration is loaded
@@ -185,15 +197,19 @@
         log.error("Statement validation error: %s" % (e.message))
         return 2  # Validation error
 
     with smart_open(args.output, settings.get("encoding", None)) as out:
         writer = ofx.OfxWriter(statement)
         out.write(writer.toxml(pretty=args.pretty))
 
-    log.info("Conversion completed: %s" % args.input)
+    n_lines = len(statement.lines)
+    log.info(
+        "Conversion completed: (%d line%s) %s"
+        % (n_lines, "s" if n_lines != 1 else "", args.input)
+    )
     return 0  # success
 
 
 def run(argv=None) -> int:
     parser = make_args_parser()
     args = parser.parse_args(argv)
     configure_logging(args)
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement.egg-info/PKG-INFO` & `ofxstatement-0.9.0/src/ofxstatement.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ofxstatement
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool to convert proprietary bank statement to OFX format, suitable for importing to GnuCash
 Home-page: https://github.com/kedder/ofxstatement
 Author: Andrey Lebedev
 Author-email: andrey@lebedev.lt
 License: GPLv3
 Keywords: ofx,banking,statement
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
@@ -19,14 +18,22 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Changes
 -------
 
+0.9.0 (2023-08-07)
+==================
+
+- New `-c` (`--config`) option for `convert` command, allows to specify the 
+  configuration file to use (#235).
+- Print the number of transactions in the output (#236).
+
+
 0.8.0 (2021-09-06)
 ==================
 
 - Support OFX CURRENCY and ORIGCURRENCY in statement lines. This allows plugins
   to add information about transaction currency to generated OFX statements.
 - Add `--pretty` flag to `convert` command to produce nicely intented OFX files.
 
@@ -111,16 +118,16 @@
   * ``refnum`` - translated to ``<REFNUM>`` in OFX.
   * ``trntype`` - translated to ``<TRNTYPE>`` in OFX.
 
 
 OFX Statement
 -------------
 
-.. image:: https://travis-ci.com/kedder/ofxstatement.svg?branch=master
-    :target: https://travis-ci.com/kedder/ofxstatement
+.. image:: https://github.com/kedder/ofxstatement/actions/workflows/test.yml/badge.svg?branch=master
+    :target: https://github.com/kedder/ofxstatement/actions/workflows/test.yml
 .. image:: https://coveralls.io/repos/kedder/ofxstatement/badge.png?branch=master
     :target: https://coveralls.io/r/kedder/ofxstatement?branch=master
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
@@ -225,14 +232,17 @@
                                   (``maxibps``) and banks using GPC
                                   format (e.g., FIO banka, module
                                   ``gpc``).
 
 `ofxstatement-airbankcz`_         Plugin for Air Bank a.s. (Czech Republic)
 `ofxstatement-raiffeisencz`_      Plugin for Raiffeisenbank a.s. (Czech Republic)
 `ofxstatement-unicreditcz`_       Plugin for UniCredit Bank Czech Republic and Slovakia
+`ofxstatement-equabankcz`_        Plugin for Equa Bank a.s. (Czech Republic)
+`ofxstatement-cz-komercni`_       Komerční banka (Czech Republic)
+`ofxstatement-mbankcz`_           mBank S.A. (Czech Republic)
 `ofxstatement-otp`_               Plugin for OTP Bank, operating in Hungary
 `ofxstatement-bubbas`_            Set of plugins, developed by @bubbas:
                                   ``dkb_cc`` and ``lbbamazon``.
 
 `banking.statements.osuuspankki`_ Finnish Osuuspankki bank
 `banking.statements.nordea`_      Nordea bank (at least Finnish branch of it)
 `ofxstatement-germany`_           Plugin for several german banks (1822direkt and Postbank at the moment)
@@ -249,45 +259,49 @@
 `ofxstatement-be-triodos`_        Belgian Triodos Bank CSV statements
 `ofxstatement-be-newb`_           Belgian cooperative bank newB
 `ofxstatement-betterment`_        Betterment (https://www.betterment.com/)
 `ofxstatement-simple`_            Simple (the bank, https://www.simple.com/) JSON financial statement format
 `ofxstatement-latvian`_           Latvian banks
 `ofxstatement-iso20022`_          Support for generic ISO-20022 format
 `ofxstatement-seb`_               SEB (Sweden), it parses Export.xlsx for private accounts
+`ofxstatement-ee-seb`_            SEB (Estonia), parses proprietary csv file
 `ofxstatement-paypal`_            PayPal, it parses ``*.csv`` for private accounts
 `ofxstatement-polish`_            Support for some Polish banks and financial institutions
 `ofxstatement-russian`_           Support for several Russian banks: Avangard, AlfaBank, Tinkoff, SberBank (both debit and csv), VTB.
 `ofxstatement-dab`_               DAB Bank (Germany)
 `ofxstatement-consors`_           Consorsbank (Germany)
 `ofxstatement-is-arionbanki`_     Arion bank in Iceland
 `ofxstatement-de-triodos`_        German Triodos Bank CSV statements (also works for GLS Bank)
 `ofxstatement-lansforsakringar`_  Länsförsäkringar (Sweden), it parses Kontoutdrag.xls for private accounts
 `ofxstatement-revolut`_           Revolut Mastercard
 `ofxstatement-transferwise`_      Transferwise CSV
+`ofxstatement-n26`_               N26 Bank
 `ofxstatement-sp-freiburg`_       Sparkasse Freiburg-Nördlicher Breisgau (Germany)
 `ofxstatement-al_bank`_           Arbejdernes Landsbank (Denmark)
 `ofxstatement-fineco`_            FinecoBank (Italy)
 `ofxstatement-intesasp`_          Intesa San Paolo (xlsx balance file)
 `ofxstatement-de-ing`_            Ing Diba Bank (Germany)
 `ofxstatement-us-first-republic`_ First Republic Bank (USA)
-`ofxstatement-cz-komercni`_       Komerční banka (Czech Republic)
 `ofxstatement-cd-tmb`_            Trust Merchant Bank (DRC)
 `ofxstatement-zm-stanbic`_        Stanbic Bank (Zambia)
 `ofxstatement-dutch`_             Dutch financial institutes like ICSCards and ING
 `ofxstatement-french`_            French financial institutes like BanquePopulaire
 `ofxstatement-mt940`_             All financial institutes providing Swift MT940 statements
 `ofxstatement-it-banks`_          Widiba and Webank italian banks
+`ofxstatement-chebanca`_          CheBanca! Italian bank (xlsx format)
 ================================= ============================================
 
 
 .. _ofxstatement-lithuanian: https://github.com/kedder/ofxstatement-lithuanian
 .. _ofxstatement-czech: https://gitlab.com/mcepl/ofxstatement-czech
 .. _ofxstatement-airbankcz: https://github.com/milankni/ofxstatement-airbankcz
 .. _ofxstatement-raiffeisencz: https://github.com/milankni/ofxstatement-raiffeisencz
 .. _ofxstatement-unicreditcz: https://github.com/milankni/ofxstatement-unicreditcz
+.. _ofxstatement-equabankcz: https://github.com/kosciCZ/ofxstatement-equabankcz
+.. _ofxstatement-mbankcz: https://github.com/SinyaWeo/ofxstatement-mbankcz
 .. _ofxstatement-otp: https://github.com/abesto/ofxstatement-otp
 .. _ofxstatement-bubbas: https://github.com/bubbas/ofxstatement-bubbas
 .. _banking.statements.osuuspankki: https://github.com/koodaamo/banking.statements.osuuspankki
 .. _banking.statements.nordea: https://github.com/koodaamo/banking.statements.nordea
 .. _ofxstatement-germany: https://github.com/MirkoDziadzka/ofxstatement-germany
 .. _ofxstatement-austrian: https://github.com/nblock/ofxstatement-austrian
 .. _ofxstatement-postfinance: https://pypi.python.org/pypi/ofxstatement-postfinance
@@ -299,41 +313,43 @@
 .. _ofxstatement-be-argenta: https://github.com/woutbr/ofxstatement-be-argenta
 .. _ofxstatement-be-crelan: https://gitlab.com/MagnificentMoustache/ofxstatement-be.crelan
 .. _ofxstatement-be-newb: https://github.com/SDaron/ofxstatement-be-newb
 .. _ofxstatement-betterment: https://github.com/cmayes/ofxstatement-betterment
 .. _ofxstatement-simple: https://github.com/cmayes/ofxstatement-simple
 .. _ofxstatement-latvian: https://github.com/gintsmurans/ofxstatement-latvian
 .. _ofxstatement-iso20022: https://github.com/kedder/ofxstatement-iso20022
-.. _ofxstatement-seb: https://github.com/themalkolm/ofxstatement-seb
+.. _ofxstatement-seb: https://github.com/gerasiov/ofxstatement-seb
 .. _ofxstatement-paypal: https://github.com/gerasiov/ofxstatement-paypal
 .. _ofxstatement-polish: https://github.com/yay6/ofxstatement-polish
 .. _ofxstatement-russian: https://github.com/gerasiov/ofxstatement-russian
 .. _ofxstatement-dab: https://github.com/JohannesKlug/ofxstatement-dab
 .. _ofxstatement-consors: https://github.com/JohannesKlug/ofxstatement-consors
 .. _ofxstatement-is-arionbanki: https://github.com/Dagur/ofxstatement-is-arionbanki
 .. _ofxstatement-be-triodos: https://github.com/renardeau/ofxstatement-be-triodos
 .. _ofxstatement-de-triodos: https://github.com/pianoslum/ofxstatement-de-triodos
 .. _ofxstatement-lansforsakringar: https://github.com/lbschenkel/ofxstatement-lansforsakringar
 .. _ofxstatement-revolut: https://github.com/mlaitinen/ofxstatement-revolut
 .. _ofxstatement-transferwise: https://github.com/kedder/ofxstatement-transferwise
+.. _ofxstatement-n26: https://github.com/3v1n0/ofxstatement-n26
 .. _ofxstatement-sp-freiburg: https://github.com/omarkohl/ofxstatement-sparkasse-freiburg
 .. _ofxstatement-al_bank: https://github.com/lbschenkel/ofxstatement-al_bank
 .. _ofxstatement-fineco: https://github.com/frankIT/ofxstatement-fineco
 .. _ofxstatement-intesasp: https://github.com/Jacotsu/ofxstatement-intesasp
 .. _ofxstatement-de-ing: https://github.com/fabolhak/ofxstatement-de-ing
 .. _ofxstatement-germany: https://github.com/MirkoDziadzka/ofxstatement-germany
 .. _ofxstatement-us-first-republic: https://github.com/medovina/ofxstatement-us-first-republic
 .. _ofxstatement-cz-komercni: https://github.com/medovina/ofxstatement-cz-komercni
 .. _ofxstatement-cd-tmb: https://github.com/BIZ4Africa/ofxstatement-cd-tmb
 .. _ofxstatement-zm-stanbic: https://github.com/BIZ4Africa/ofxstatement-zm-stanbic
 .. _ofxstatement-dutch: https://github.com/gpaulissen/ofxstatement-dutch
 .. _ofxstatement-french: https://github.com/gpaulissen/ofxstatement-french
 .. _ofxstatement-mt940: https://github.com/gpaulissen/ofxstatement-mt940
 .. _ofxstatement-it-banks: https://github.com/ecorini/ofxstatement-it-banks
-
+.. _ofxstatement-ee-seb: https://github.com/rsi2m/ofxstatement-ee-seb
+.. _ofxstatement-chebanca: https://github.com/3v1n0/ofxstatement-chebanca
 Advanced Configuration
 ======================
 
 While ofxstatement can be used without any configuration, some plugins may
 accept additional configuration parameters. These parameters can be specified
 in a configuration file. The configuration file can be edited using the ``edit-config``
 command that opens your favorite editor (defined by environment variable
@@ -368,19 +384,21 @@
 To convert the proprietary CSV file ``danske.csv`` into the OFX file ``danske.ofx``, run::
 
     $ ofxstatement -t danske:usd danske.csv danske.ofx
 
 Note that configuration parameters are plugin specific. See the plugin
 documentation for more info.
 
+To use a custom configuration file, pass the ``-c`` / ``--config`` option::
+
+    $ ofxstatement convert -t pluginname -c /path/to/myconfig.ini input.csv output.ofx
+
 Writing your own Plugin
 =======================
 
 If the plugin for your bank has not been developed yet (see `Known plugins`_
 section above) you can easily write your own, provided you have some knowledge
 about the Python programming language. There is an `ofxstatement-sample`_
 plugin project available that provides sample boilerplate and describes the
 plugin development process in detail.
 
 .. _ofxstatement-sample: https://github.com/kedder/ofxstatement-sample
-
-
```

### Comparing `ofxstatement-0.8.0/src/ofxstatement.egg-info/SOURCES.txt` & `ofxstatement-0.9.0/src/ofxstatement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

