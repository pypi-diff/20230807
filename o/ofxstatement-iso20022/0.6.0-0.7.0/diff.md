# Comparing `tmp/ofxstatement-iso20022-0.6.0.tar.gz` & `tmp/ofxstatement-iso20022-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ofxstatement-iso20022-0.6.0.tar", last modified: Sun Feb  7 18:15:09 2021, max compression
+gzip compressed data, was "ofxstatement-iso20022-0.7.0.tar", last modified: Mon Aug  7 13:42:07 2023, max compression
```

## Comparing `ofxstatement-iso20022-0.6.0.tar` & `ofxstatement-iso20022-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-02-07 18:15:09.112095 ofxstatement-iso20022-0.6.0/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       19 2021-02-07 18:15:08.000000 ofxstatement-iso20022-0.6.0/MANIFEST.in
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1586 2021-02-07 18:15:09.112095 ofxstatement-iso20022-0.6.0/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      725 2021-02-07 18:15:08.000000 ofxstatement-iso20022-0.6.0/README.rst
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       72 2021-02-07 18:15:09.112095 ofxstatement-iso20022-0.6.0/setup.cfg
--rwxrwxr-x   0 andrey    (1000) andrey    (1000)     1320 2021-02-07 18:15:08.000000 ofxstatement-iso20022-0.6.0/setup.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-02-07 18:15:09.112095 ofxstatement-iso20022-0.6.0/src/
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-02-07 18:15:09.112095 ofxstatement-iso20022-0.6.0/src/ofxstatement/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2021-02-07 18:15:08.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement/__init__.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-02-07 18:15:09.112095 ofxstatement-iso20022-0.6.0/src/ofxstatement/plugins/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2021-02-07 18:15:08.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement/plugins/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     9029 2021-02-07 18:15:08.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement/plugins/iso20022.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2021-02-07 18:15:09.112095 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1586 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      542 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/SOURCES.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/dependency_links.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       72 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/entry_points.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       34 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/namespace_packages.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       28 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/requires.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       13 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/top_level.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2021-02-07 18:15:09.000000 ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/zip-safe
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       19 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/MANIFEST.in
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1531 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      845 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/README.rst
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       72 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/setup.cfg
+-rwxrwxr-x   0 andrey    (1000) andrey    (1000)     1320 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/setup.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/src/
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/src/ofxstatement/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement/__init__.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/src/ofxstatement/plugins/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       56 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement/plugins/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    10123 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement/plugins/iso20022.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1531 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      565 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       71 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/entry_points.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       34 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/namespace_packages.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       28 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/requires.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       13 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/top_level.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/zip-safe
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-08-07 13:42:07.166326 ofxstatement-iso20022-0.7.0/tests/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     6053 2023-08-07 13:42:07.000000 ofxstatement-iso20022-0.7.0/tests/test_iso20022.py
```

### Comparing `ofxstatement-iso20022-0.6.0/PKG-INFO` & `ofxstatement-iso20022-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: ofxstatement-iso20022
-Version: 0.6.0
+Version: 0.7.0
 Summary: ISO-20022 plugin for ofxstatement
 Home-page: https://github.com/kedder/ofxstatement-iso20022
 Author: Andrey Lebedev
 Author-email: andrey@lebedev.lt
 License: GPLv3
-Description: ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        ISO-20022 plugin for ofxstatement
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. image:: https://travis-ci.org/kedder/ofxstatement-iso20022.svg?branch=master
-            :target: https://travis-ci.org/kedder/ofxstatement-iso20022
-        
-        Plugin to read ISO-20022 formatted statements.
-        
-        Plugin supports the following configuration options:
-        
-        * ``currency``: Account currency. In case currency is not specified in ISO20022 
-          statement, you can specify it with this setting. Only statement lines with account 
-          currency will be included in OFX files.
-        
-        Currently implementation is very trivial and naive. If it doesn't work for
-        you, feel free to improve it or file a bug on github with sample (anonymized)
-        state file.
-        
 Keywords: ofx,banking,statement,iso-20022
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Provides-Extra: test
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+ISO-20022 plugin for ofxstatement
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. image:: https://travis-ci.org/kedder/ofxstatement-iso20022.svg?branch=master
+    :target: https://travis-ci.org/kedder/ofxstatement-iso20022
+
+Plugin to read ISO-20022 formatted statements.
+
+Plugin supports the following configuration options:
+
+* ``currency``: Account currency. In case currency is not specified in ISO20022 
+  statement, you can specify it with this setting. Only statement lines with account 
+  currency will be included in OFX files.
+* ``iban``: Account IBAN. In case the IBAN is not specified in the ISO20022 statement, you need to specify this option.
+
+Currently implementation is very trivial and naive. If it doesn't work for
+you, feel free to improve it or file a bug on github with sample (anonymized)
+state file.
```

### Comparing `ofxstatement-iso20022-0.6.0/README.rst` & `ofxstatement-iso20022-0.7.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 Plugin to read ISO-20022 formatted statements.
 
 Plugin supports the following configuration options:
 
 * ``currency``: Account currency. In case currency is not specified in ISO20022 
   statement, you can specify it with this setting. Only statement lines with account 
   currency will be included in OFX files.
+* ``iban``: Account IBAN. In case the IBAN is not specified in the ISO20022 statement, you need to specify this option.
 
 Currently implementation is very trivial and naive. If it doesn't work for
 you, feel free to improve it or file a bug on github with sample (anonymized)
 state file.
```

### Comparing `ofxstatement-iso20022-0.6.0/setup.py` & `ofxstatement-iso20022-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python3
 """Setup
 """
 from setuptools import find_packages
 from distutils.core import setup
 
-version = "0.6.0"
+version = "0.7.0"
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="ofxstatement-iso20022",
     version=version,
```

### Comparing `ofxstatement-iso20022-0.6.0/src/ofxstatement/plugins/iso20022.py` & `ofxstatement-iso20022-0.7.0/src/ofxstatement/plugins/iso20022.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ofxstatement import exceptions
 from ofxstatement.parser import AbstractStatementParser
 from ofxstatement.plugin import Plugin
 from ofxstatement.statement import Statement, StatementLine
 
 # ISO20022_NAMESPACE_ROOT = "urn:iso:std:iso:20022"
-CAMT053_NAMESPACE_ROOT = "urn:iso:std:iso:20022:tech:xsd:camt.052"
+CAMT052_NAMESPACE_ROOT = "urn:iso:std:iso:20022:tech:xsd:camt.052"
 CAMT053_NAMESPACE_ROOT = "urn:iso:std:iso:20022:tech:xsd:camt.053"
 
 
 CD_CREDIT = "CRDT"
 CD_DEBIT = "DBIT"
 
 
@@ -25,30 +25,35 @@
 
 
 class Iso20022Plugin(Plugin):
     """ISO-20022 plugin"""
 
     def get_parser(self, filename: str) -> "Iso20022Parser":
         default_ccy = self.settings.get("currency")
-        parser = Iso20022Parser(filename, currency=default_ccy)
+        default_iban = self.settings.get("iban")
+        parser = Iso20022Parser(filename, currency=default_ccy, iban=default_iban)
         return parser
 
 
 class Iso20022Parser(AbstractStatementParser):
     version: CamtVersion
     xmlns: Dict[str, str]
 
-    def __init__(self, filename: str, currency: str = None):
+    def __init__(
+        self, filename: str, currency: Optional[str] = None, iban: Optional[str] = None
+    ):
         self.filename = filename
         self.currency = currency
+        self.iban = iban
 
     def parse(self) -> Statement:
         """Main entry point for parsers"""
         self.statement = Statement()
         self.statement.currency = self.currency
+        self.statement.account_id = self.iban
         tree = ET.parse(self.filename)
 
         # Find out XML namespace and make sure we can parse it
         ns = self._get_namespace(tree.getroot())
         self.version = self._recognize_version(ns)
         self.xmlns = {"s": ns}
 
@@ -80,30 +85,48 @@
 
     def _parse_statement_properties(self, tree: ET.ElementTree) -> None:
         stmt = self._get_statement_el(tree)
 
         bnk = stmt.find("./s:Acct/s:Svcr/s:FinInstnId/s:BIC", self.xmlns)
         if bnk is None:
             bnk = stmt.find("./s:Acct/s:Svcr/s:FinInstnId/s:Nm", self.xmlns)
-        iban = stmt.find("./s:Acct/s:Id/s:IBAN", self.xmlns)
-        assert iban is not None
         ccy = stmt.find("./s:Acct/s:Ccy", self.xmlns)
         bals = stmt.findall("./s:Bal", self.xmlns)
+        ibanfind = stmt.find(
+            "./s:Acct/s:Id/s:IBAN",
+            self.xmlns,
+        )
+        if ibanfind is None:
+            ibanfind = stmt.find(
+                "./s:Ntry/s:NtryDtls/s:TxDtls/s:RltdPties/s:CdtrAcct/s:Id/s:IBAN",
+                self.xmlns,
+            )
+        # assert iban is not None
 
         acctCurrency = ccy.text if ccy is not None else None
         if acctCurrency:
             self.statement.currency = acctCurrency
         else:
             if self.statement.currency is None:
                 raise exceptions.ParseError(
                     0,
                     "No account currency provided in statement. Please "
                     "specify one in configuration file (e.g. currency=EUR)",
                 )
 
+        acctIban = ibanfind.text if ibanfind is not None else None
+        if acctIban:
+            self.statement.account_id = acctIban
+        else:
+            if self.statement.account_id is None:
+                raise exceptions.ParseError(
+                    0,
+                    "No iban found in the statement. Please specify one in the configuration file (e.g. iban=CH...)",
+                )
+
         bal_amts = {}
         bal_dates = {}
         for bal in bals:
             cd = bal.find("./s:Tp/s:CdOrPrtry/s:Cd", self.xmlns)
             amt = bal.find("./s:Amt", self.xmlns)
             dt = bal.find("./s:Dt", self.xmlns)
             assert cd is not None
@@ -120,15 +143,21 @@
             raise exceptions.ParseError(
                 0,
                 "No statement balance found for currency '%s'. Check "
                 "currency of statement file." % self.statement.currency,
             )
 
         self.statement.bank_id = bnk.text if bnk is not None else None
-        self.statement.account_id = iban.text
+
+        # This statement is required to avoid overwriting account_id with None
+        # when no IBAN can be found in the XML.
+        # Instead the configured value for IBAN will be used.
+        self.statement.account_id = (
+            acctIban if acctIban is not None else self.statement.account_id
+        )
 
         # From ISO 20022 Account Statement Guide:
         #
         # The following balance types are mandatory in the Bank-To-Customer
         # statement:
         #
         # OPBD – Book balance of the account at the beginning of the account
```

### Comparing `ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/PKG-INFO` & `ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: ofxstatement-iso20022
-Version: 0.6.0
+Version: 0.7.0
 Summary: ISO-20022 plugin for ofxstatement
 Home-page: https://github.com/kedder/ofxstatement-iso20022
 Author: Andrey Lebedev
 Author-email: andrey@lebedev.lt
 License: GPLv3
-Description: ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        ISO-20022 plugin for ofxstatement
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. image:: https://travis-ci.org/kedder/ofxstatement-iso20022.svg?branch=master
-            :target: https://travis-ci.org/kedder/ofxstatement-iso20022
-        
-        Plugin to read ISO-20022 formatted statements.
-        
-        Plugin supports the following configuration options:
-        
-        * ``currency``: Account currency. In case currency is not specified in ISO20022 
-          statement, you can specify it with this setting. Only statement lines with account 
-          currency will be included in OFX files.
-        
-        Currently implementation is very trivial and naive. If it doesn't work for
-        you, feel free to improve it or file a bug on github with sample (anonymized)
-        state file.
-        
 Keywords: ofx,banking,statement,iso-20022
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Provides-Extra: test
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+ISO-20022 plugin for ofxstatement
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. image:: https://travis-ci.org/kedder/ofxstatement-iso20022.svg?branch=master
+    :target: https://travis-ci.org/kedder/ofxstatement-iso20022
+
+Plugin to read ISO-20022 formatted statements.
+
+Plugin supports the following configuration options:
+
+* ``currency``: Account currency. In case currency is not specified in ISO20022 
+  statement, you can specify it with this setting. Only statement lines with account 
+  currency will be included in OFX files.
+* ``iban``: Account IBAN. In case the IBAN is not specified in the ISO20022 statement, you need to specify this option.
+
+Currently implementation is very trivial and naive. If it doesn't work for
+you, feel free to improve it or file a bug on github with sample (anonymized)
+state file.
```

### Comparing `ofxstatement-iso20022-0.6.0/src/ofxstatement_iso20022.egg-info/SOURCES.txt` & `ofxstatement-iso20022-0.7.0/src/ofxstatement_iso20022.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 src/ofxstatement_iso20022.egg-info/PKG-INFO
 src/ofxstatement_iso20022.egg-info/SOURCES.txt
 src/ofxstatement_iso20022.egg-info/dependency_links.txt
 src/ofxstatement_iso20022.egg-info/entry_points.txt
 src/ofxstatement_iso20022.egg-info/namespace_packages.txt
 src/ofxstatement_iso20022.egg-info/requires.txt
 src/ofxstatement_iso20022.egg-info/top_level.txt
-src/ofxstatement_iso20022.egg-info/zip-safe
+src/ofxstatement_iso20022.egg-info/zip-safe
+tests/test_iso20022.py
```

