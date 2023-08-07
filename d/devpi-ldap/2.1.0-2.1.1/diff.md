# Comparing `tmp/devpi-ldap-2.1.0.tar.gz` & `tmp/devpi-ldap-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/devpi-ldap-2.1.0.tar", last modified: Sat Dec  4 11:49:48 2021, max compression
+gzip compressed data, was "/private/var/folders/59/l4m0cwnj1yldp5prd49z_1dr0000gn/T/devpi-arpp2z9p/devpi-ldap/dist/tmpgayte72r/devpi-ldap-2.1.1.tar", last modified: Mon Aug  7 09:43:34 2023, max compression
```

## Comparing `devpi-ldap-2.1.0.tar` & `devpi-ldap-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/
--rw-r--r--   0 fschulze   (501) staff       (20)     1891 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/CHANGELOG.rst
--rw-r--r--   0 fschulze   (501) staff       (20)       49 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)    10268 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     5594 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/README.rst
--rw-r--r--   0 fschulze   (501) staff       (20)       73 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/devpi-ldap.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap/
--rw-r--r--   0 fschulze   (501) staff       (20)       22 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/devpi_ldap/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13263 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/devpi_ldap/main.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)    10268 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)      410 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       98 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/not-zip-safe
--rw-r--r--   0 fschulze   (501) staff       (20)       38 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       22 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/devpi_ldap.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      115 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/setup.cfg
--rw-r--r--   0 fschulze   (501) staff       (20)     1703 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-12-04 11:49:48.000000 devpi-ldap-2.1.0/tests/
--rw-r--r--   0 fschulze   (501) staff       (20)      457 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/tests/conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)    16054 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/tests/test_ldap.py
--rw-r--r--   0 fschulze   (501) staff       (20)      532 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/tox.ini
--rw-rw-r--   0 fschulze   (501) staff       (20)     3364 2021-12-04 11:49:47.000000 devpi-ldap-2.1.0/windows-vm.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/
+-rw-r--r--   0 fschulze   (501) staff       (20)     2045 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/CHANGELOG.rst
+-rw-r--r--   0 fschulze   (501) staff       (20)       49 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)    10576 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     5594 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/README.rst
+-rw-r--r--   0 fschulze   (501) staff       (20)       73 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/devpi-ldap.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap/
+-rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/devpi_ldap/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    13136 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/devpi_ldap/main.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)    10576 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      410 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       98 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)       38 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/devpi_ldap.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      115 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/setup.cfg
+-rw-r--r--   0 fschulze   (501) staff       (20)     1709 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-07 09:43:34.000000 devpi-ldap-2.1.1/tests/
+-rw-r--r--   0 fschulze   (501) staff       (20)      457 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/tests/conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    17243 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/tests/test_ldap.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      567 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/tox.ini
+-rw-rw-r--   0 fschulze   (501) staff       (20)     3364 2023-08-07 09:43:33.000000 devpi-ldap-2.1.1/windows-vm.rst
```

### Comparing `devpi-ldap-2.1.0/CHANGELOG.rst` & `devpi-ldap-2.1.1/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.1.1 - 2023-08-07
+------------------
+
+- Use ``escape_filter_chars`` before calling LDAP ``search`` method.
+  [mr-scrawley (Micha Schmierer), fschulze]
+
+
 2.1.0 - 2021-12-04
 ------------------
 
 - Fix issue #50: new server_pool setting.
 
 
 2.0.0 - 2021-05-16
```

### Comparing `devpi-ldap-2.1.0/PKG-INFO` & `devpi-ldap-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: devpi-ldap
-Version: 2.1.0
+Version: 2.1.1
 Summary: devpi-ldap: LDAP authentication for devpi-server
 Home-page: https://github.com/devpi/devpi-ldap
 Maintainer: Florian Schulze
-Maintainer-email: florian.schulze@gmx.net
+Maintainer-email: mail@pyfidelity.com
 License: MIT
 Description: devpi-ldap: LDAP authentication for devpi-server
         ================================================
         
         .. image:: https://img.shields.io/pypi/v/devpi-ldap.svg?style=flat
             :target: https://pypi.python.org/pypi/devpi-ldap/
             :alt: Latest Version
@@ -161,14 +161,21 @@
                 filter: (&(objectClass=group)(member={userdn}))
                 attribute_name: CN
         
         
         Changelog
         =========
         
+        2.1.1 - 2023-08-07
+        ------------------
+        
+        - Use ``escape_filter_chars`` before calling LDAP ``search`` method.
+          [mr-scrawley (Micha Schmierer), fschulze]
+        
+        
         2.1.0 - 2021-12-04
         ------------------
         
         - Fix issue #50: new server_pool setting.
         
         
         2.0.0 - 2021-05-16
@@ -264,8 +271,10 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
```

### Comparing `devpi-ldap-2.1.0/README.rst` & `devpi-ldap-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-ldap-2.1.0/devpi_ldap/main.py` & `devpi-ldap-2.1.1/devpi_ldap/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from devpi_common.metadata import Version
 from devpi_server import __version__ as server_version
 from devpi_server.log import threadlog
 from devpi_server.auth import AuthException
+from ldap3.utils.conv import escape_filter_chars
 from pluggy import HookimplMarker
 import argparse
 import getpass
 import ldap3
 import os
 import socket
 import sys
@@ -15,26 +16,14 @@
 
 ldap = None
 notset = object()
 server_hookimpl = HookimplMarker("devpiserver")
 DEFAULT_TIMEOUT = 10
 
 
-def escape(s):
-    repl = (
-        ('*', '\\\\2A'),
-        ('(', '\\\\28'),
-        (')', '\\\\29'),
-        ('\\', '\\\\5C'),
-        ('\0', '\\\\00'))
-    for c, r in repl:
-        s = s.replace(c, r)
-    return s
-
-
 def fatal(msg):
     threadlog.error(msg)
     sys.exit(1)
 
 
 class LDAP(dict):
     ldap3 = ldap3  # for dependency injection
@@ -175,15 +164,16 @@
         return conn
 
     def _search(self, conn, config, **kw):
         config = dict(config)
         conn = self._build_search_conn(conn, config)
         if not conn:
             return []
-        search_filter = config['filter'].format(**kw)
+        escaped_kw = {k: escape_filter_chars(v) for k, v in kw.items()}
+        search_filter = config['filter'].format(**escaped_kw)
         search_scope = self._search_scope(config)
         attribute_name = config['attribute_name']
         found = conn.search(
             config['base'], search_filter,
             search_scope=search_scope, attributes=[attribute_name])
         if found:
             if any(attribute_name in x.get('attributes', {}) for x in conn.response):
@@ -251,15 +241,14 @@
         """
         if 'server_pool' in self:
             threadlog.debug("Validating user '%s' against LDAP at %s." % (username, [
                 server['url'] for server in self['server_pool']
             ]))
         else:
             threadlog.debug("Validating user '%s' against LDAP at %s." % (username, self['url']))
-        username = escape(username)
         userdn = self._userdn(username)
         if not userdn:
             return dict(status="unknown")
         if not password.strip():
             return self._rejection()
         conn = self.connection(self.server_pool(), userdn=userdn, password=password)
         if not self._open_and_bind(conn):
```

### Comparing `devpi-ldap-2.1.0/devpi_ldap.egg-info/PKG-INFO` & `devpi-ldap-2.1.1/devpi_ldap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: devpi-ldap
-Version: 2.1.0
+Version: 2.1.1
 Summary: devpi-ldap: LDAP authentication for devpi-server
 Home-page: https://github.com/devpi/devpi-ldap
 Maintainer: Florian Schulze
-Maintainer-email: florian.schulze@gmx.net
+Maintainer-email: mail@pyfidelity.com
 License: MIT
 Description: devpi-ldap: LDAP authentication for devpi-server
         ================================================
         
         .. image:: https://img.shields.io/pypi/v/devpi-ldap.svg?style=flat
             :target: https://pypi.python.org/pypi/devpi-ldap/
             :alt: Latest Version
@@ -161,14 +161,21 @@
                 filter: (&(objectClass=group)(member={userdn}))
                 attribute_name: CN
         
         
         Changelog
         =========
         
+        2.1.1 - 2023-08-07
+        ------------------
+        
+        - Use ``escape_filter_chars`` before calling LDAP ``search`` method.
+          [mr-scrawley (Micha Schmierer), fschulze]
+        
+        
         2.1.0 - 2021-12-04
         ------------------
         
         - Fix issue #50: new server_pool setting.
         
         
         2.0.0 - 2021-05-16
@@ -264,8 +271,10 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
```

### Comparing `devpi-ldap-2.1.0/setup.py` & `devpi-ldap-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,32 +25,32 @@
 setup(
     name="devpi-ldap",
     description="devpi-ldap: LDAP authentication for devpi-server",
     long_description=README + "\n\n" + CHANGELOG,
     url="https://github.com/devpi/devpi-ldap",
     version=get_version("devpi_ldap"),
     maintainer="Florian Schulze",
-    maintainer_email="florian.schulze@gmx.net",
+    maintainer_email="mail@pyfidelity.com",
     license="MIT",
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python"] + [
             "Programming Language :: Python :: %s" % x
-            for x in "3 3.6 3.7 3.8 3.9".split()],
+            for x in "3 3.6 3.7 3.8 3.9 3.10 3.11".split()],
     entry_points={
         'console_scripts': [
             "devpi-ldap = devpi_ldap.main:main"],
         'devpi_server': [
             "devpi-ldap = devpi_ldap.main"]},
     install_requires=[
         'PyYAML',
         'devpi-server>=5',
-        'ldap3>=0.9.8.6'],
+        'ldap3>=0.9.9.3'],
     include_package_data=True,
     python_requires='>=3.6',
     zip_safe=False,
     packages=['devpi_ldap'],
     py_modules=['devpi-ldap'],
 )
```

### Comparing `devpi-ldap-2.1.0/tests/test_ldap.py` & `devpi-ldap-2.1.1/tests/test_ldap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import print_function, unicode_literals
+from ldap3.utils.conv import escape_filter_chars
 import ldap3
 import sys
 import pytest
 import yaml
 
 
 def test_importable():
@@ -202,15 +203,15 @@
 
     def open(self):
         pass
 
     def bind(self):
         if self.user is None:
             return True
-        user = self.server_pool.servers[0].users.get(self.user)
+        user = self.server_pool.servers[0].users.get(escape_filter_chars(self.user))
         if user is None:
             self.result = "Bind failed, user not found"
             return False
         if self.password == '' or user['pw'] == self.password:
             return True
         self.result = "Bind failed, invalid credentials"
         return False
@@ -232,15 +233,16 @@
         search_filter = search_filter.split(":")
         if search_filter[0] == 'user':
             user = self.server_pool.servers[0].users.get(search_filter[1])
             if user is not None:
                 self.response = [dict(attributes=dict(
                     (k, [user.get(k, fixDn(user, k))]) for k in attributes if fixDn(user, k) is not dnplaceholder))]
                 if dnplaceholder.triggered:
-                    self.response[0][dnplaceholder.triggered] = search_filter[1]
+                    self.response[0][dnplaceholder.triggered] = user.get(
+                        dnplaceholder.triggered, search_filter[1])
                 return True
         elif search_filter[0] == 'group':
             user = self.server_pool.servers[0].users.get(search_filter[1])
             if user is not None and 'groups' in user:
                 self.response = [
                     dict(attributes=dict(
                         (k, [g[k]]) for k in attributes))
@@ -371,14 +373,24 @@
     main([user_search_config.strpath, 'user'])
     out, err = capsys.readouterr()
     assert out.splitlines() == [
         'Result: {"status": "ok"}',
         "Authentication successful, the user is member of the following groups: "]
 
 
+def test_main_user_with_parentheses(MockServer, capsys, getpass, main, user_search_config):
+    MockServer.users['user \\28foo\\29'] = dict(pw="password", dn="user (foo)")
+    getpass.return_value = "password"
+    main([user_search_config.strpath, 'user (foo)'])
+    out, err = capsys.readouterr()
+    assert out.splitlines() == [
+        'Result: {"status": "ok"}',
+        "Authentication successful, the user is member of the following groups: "]
+
+
 def test_main_user_with_search_userdn(MockServer, capsys, getpass, main, userdn_search_config):
     MockServer.users['search'] = dict(pw="foo", dn="search")
     MockServer.users['user'] = dict(pw="password", dn="user")
     getpass.return_value = "password"
     main([userdn_search_config.strpath, 'user'])
     out, err = capsys.readouterr()
     assert out.splitlines() == [
@@ -423,14 +435,25 @@
     main([group_userdn_search_config.strpath, 'user'])
     out, err = capsys.readouterr()
     assert out.splitlines() == [
         'Result: {"groups": ["users"], "status": "ok"}',
         "Authentication successful, the user is member of the following groups: users"]
 
 
+def test_main_user_parentheses_with_search_userdn_with_group(MockServer, capsys, getpass, main, group_userdn_search_config):
+    MockServer.users['search'] = dict(pw="foo", dn="search")
+    MockServer.users['user \\28foo\\29'] = dict(pw="password", dn="user (foo)", groups=[dict(cn='users')])
+    getpass.return_value = "password"
+    main([group_userdn_search_config.strpath, 'user (foo)'])
+    out, err = capsys.readouterr()
+    assert out.splitlines() == [
+        'Result: {"groups": ["users"], "status": "ok"}',
+        "Authentication successful, the user is member of the following groups: users"]
+
+
 def test_reject_as_unknown(LDAP, reject_as_unknown_config):
     ldap = LDAP(reject_as_unknown_config.strpath)
     assert ldap._rejection() == dict(status="reject")
 
 
 def test_reject_as_unknown_empty(LDAP, reject_as_unknown_config):
     ldap = LDAP(reject_as_unknown_config.strpath)
```

### Comparing `devpi-ldap-2.1.0/tox.ini` & `devpi-ldap-2.1.1/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tox]
-envlist = {py36}{,-ldap0,-ldap1}{,-devpi5},py39{,-devpi5}
+envlist = {py36}{,-ldap0,-ldap1}{,-devpi5},py39{,-devpi5},py311
 
 
 [gh-actions]
 python =
     3.6: py36
     3.9: py39
+    3.11: py311
 
 
 [testenv]
 commands = py.test --cov {envsitepackagesdir}/devpi_ldap {posargs:tests}
 deps =
+    flake8<5
     webtest
     mock
     pytest
     pytest-cov
     pytest-flake8
     ldap0: ldap3<1dev
     ldap1: ldap3<2dev
```

### Comparing `devpi-ldap-2.1.0/windows-vm.rst` & `devpi-ldap-2.1.1/windows-vm.rst`

 * *Files identical despite different names*

