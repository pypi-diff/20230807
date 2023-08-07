# Comparing `tmp/plone.volto-4.0.9.tar.gz` & `tmp/plone.volto-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.volto-4.0.9.tar", last modified: Thu Jun 22 19:24:03 2023, max compression
+gzip compressed data, was "plone.volto-4.1.0.tar", last modified: Mon Aug  7 19:08:34 2023, max compression
```

## Comparing `plone.volto-4.0.9.tar` & `plone.volto-4.1.0.tar`

### file list

```diff
@@ -1,167 +1,158 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.142418 plone.volto-4.0.9/
--rw-r--r--   0 maurits    (501) staff       (20)    13945 2023-06-22 19:24:02.000000 plone.volto-4.0.9/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      369 2023-06-22 19:24:02.000000 plone.volto-4.0.9/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)    26169 2023-06-22 19:24:03.142043 plone.volto-4.0.9/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    10929 2023-06-22 19:24:02.000000 plone.volto-4.0.9/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.109167 plone.volto-4.0.9/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-22 19:24:02.000000 plone.volto-4.0.9/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      657 2023-06-22 19:24:02.000000 plone.volto-4.0.9/docs/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)       74 2023-06-22 19:24:02.000000 plone.volto-4.0.9/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      881 2023-06-22 19:24:02.000000 plone.volto-4.0.9/pyproject.toml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.110174 plone.volto-4.0.9/requirements/
--rw-r--r--   0 maurits    (501) staff       (20)       12 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/dev.txt
--rw-r--r--   0 maurits    (501) staff       (20)       73 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/plone-5.2.txt
--rw-r--r--   0 maurits    (501) staff       (20)       69 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/plone-6.0.txt
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/prod.txt
--rw-r--r--   0 maurits    (501) staff       (20)      402 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-06-22 19:24:03.142554 plone.volto-4.0.9/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2227 2023-06-22 19:24:02.000000 plone.volto-4.0.9/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.102243 plone.volto-4.0.9/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.110418 plone.volto-4.0.9/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.117643 plone.volto-4.0.9/src/plone/volto/
--rw-r--r--   0 maurits    (501) staff       (20)      222 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.119151 plone.volto-4.0.9/src/plone/volto/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1168 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      534 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/headtitle.py
--rw-r--r--   0 maurits    (501) staff       (20)      345 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/navtitle.py
--rw-r--r--   0 maurits    (501) staff       (20)      727 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/preview.py
--rw-r--r--   0 maurits    (501) staff       (20)     2475 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/preview_link.py
--rw-r--r--   0 maurits    (501) staff       (20)     1614 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/blocksuuidfixer.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.121590 plone.volto-4.0.9/src/plone/volto/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2046 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/breadcrumbs.py
--rw-r--r--   0 maurits    (501) staff       (20)     1743 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3673 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5548 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)     6949 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.pt
--rw-r--r--   0 maurits    (501) staff       (20)    14011 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.py
--rw-r--r--   0 maurits    (501) staff       (20)     4499 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/navigation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.121965 plone.volto-4.0.9/src/plone/volto/browser/static/
--rw-r--r--   0 maurits    (501) staff       (20)      754 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/static/volto.svg
--rw-r--r--   0 maurits    (501) staff       (20)     1368 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/voltobackendwarning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3273 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      697 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/content.py
--rw-r--r--   0 maurits    (501) staff       (20)      974 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/controlpanel.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.123098 plone.volto-4.0.9/src/plone/volto/coresandbox/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      540 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    28820 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/example.py
--rw-r--r--   0 maurits    (501) staff       (20)      745 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.123761 plone.volto-4.0.9/src/plone/volto/cors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/cors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      462 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/cors/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.124975 plone.volto-4.0.9/src/plone/volto/default_homepage/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    34756 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/default.py
--rw-r--r--   0 maurits    (501) staff       (20)    28345 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/demo.py
--rw-r--r--   0 maurits    (501) staff       (20)     3019 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      516 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/dependencies.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1062 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1006 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1576 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/linkintegrity.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.125501 plone.volto-4.0.9/src/plone/volto/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.103599 plone.volto-4.0.9/src/plone/volto/locales/de/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.126108 plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     2258 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4528 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.103885 plone.volto-4.0.9/src/plone/volto/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.126623 plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      622 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     3830 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.104121 plone.volto-4.0.9/src/plone/volto/locales/es/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.127215 plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     2559 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4693 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.104357 plone.volto-4.0.9/src/plone/volto/locales/eu/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.127694 plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     2478 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4611 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.104593 plone.volto-4.0.9/src/plone/volto/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.128242 plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     1145 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4086 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
--rw-r--r--   0 maurits    (501) staff       (20)     3777 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/plone.volto.pot
--rwxr-xr-x   0 maurits    (501) staff       (20)      502 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/update.sh
--rw-r--r--   0 maurits    (501) staff       (20)      256 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/patches.py
--rw-r--r--   0 maurits    (501) staff       (20)      858 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/patches.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.106045 plone.volto-4.0.9/src/plone/volto/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.129223 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/
--rw-r--r--   0 maurits    (501) staff       (20)      206 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/diff_tool.xml
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      210 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/repositorytool.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.129553 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2466 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types/example.xml
--rw-r--r--   0 maurits    (501) staff       (20)      165 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.131171 plone.volto-4.0.9/src/plone/volto/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      639 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      156 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      196 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      612 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      181 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1791 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.132856 plone.volto-4.0.9/src/plone/volto/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)      286 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)      814 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)      501 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      604 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/LRF.xml
--rw-r--r--   0 maurits    (501) staff       (20)      464 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/News_Item.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.133520 plone.volto-4.0.9/src/plone/volto/profiles/demo/
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/demo/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      291 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/demo/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.133765 plone.volto-4.0.9/src/plone/volto/profiles/homepage/
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/homepage/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.134251 plone.volto-4.0.9/src/plone/volto/profiles/multilingual/
--rw-r--r--   0 maurits    (501) staff       (20)      209 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/multilingual/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      546 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/multilingual/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.134927 plone.volto-4.0.9/src/plone/volto/profiles/richtext/
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/richtext/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.135169 plone.volto-4.0.9/src/plone/volto/profiles/richtext/types/
--rw-r--r--   0 maurits    (501) staff       (20)      320 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/richtext/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/richtext/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.135416 plone.volto-4.0.9/src/plone/volto/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      114 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3591 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3436 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scaling.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.137688 plone.volto-4.0.9/src/plone/volto/scripts/
--rw-r--r--   0 maurits    (501) staff       (20)      752 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/add_image_field_metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)     1206 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/auditblocks.py
--rw-r--r--   0 maurits    (501) staff       (20)      202 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/clear-rebuild-catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)      773 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/listingaddsummary.py
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/migrate_richtext.py
--rwxr-xr-x   0 maurits    (501) staff       (20)      123 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/packdb.py
--rw-r--r--   0 maurits    (501) staff       (20)     1594 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/searchscalesinimageblocks.py
--rw-r--r--   0 maurits    (501) staff       (20)      932 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     9939 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      312 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     4513 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.140586 plone.volto-4.0.9/src/plone/volto/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_coresandbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     2442 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_linkintegrity.py
--rw-r--r--   0 maurits    (501) staff       (20)    11771 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_migrate_to_volto.py
--rw-r--r--   0 maurits    (501) staff       (20)     1823 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_preview_link_behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)     2126 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_scripts.py
--rw-r--r--   0 maurits    (501) staff       (20)     3102 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1709 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_summary_serialization.py
--rw-r--r--   0 maurits    (501) staff       (20)    11245 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_transforms.py
--rw-r--r--   0 maurits    (501) staff       (20)     6498 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     4805 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/transforms.py
--rw-r--r--   0 maurits    (501) staff       (20)     5327 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     2222 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/upgrades.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.141649 plone.volto-4.0.9/src/plone/volto/vocabularies/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/vocabularies/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      105 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/vocabularies/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4305 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/vocabularies/subject.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.112559 plone.volto-4.0.9/src/plone.volto.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    26169 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5012 2023-06-22 19:24:03.000000 plone.volto-4.0.9/src/plone.volto.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.109063 plone.volto-4.1.0/
+-rw-r--r--   0 davisagli   (501) staff       (20)    14566 2023-08-07 19:08:33.000000 plone.volto-4.1.0/CHANGES.rst
+-rw-r--r--   0 davisagli   (501) staff       (20)      369 2023-08-07 19:08:33.000000 plone.volto-4.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 davisagli   (501) staff       (20)    26790 2023-08-07 19:08:34.108908 plone.volto-4.1.0/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)    10929 2023-08-07 19:08:33.000000 plone.volto-4.1.0/README.rst
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.095941 plone.volto-4.1.0/docs/
+-rw-r--r--   0 davisagli   (501) staff       (20)    18092 2023-08-07 19:08:33.000000 plone.volto-4.1.0/docs/LICENSE.GPL
+-rw-r--r--   0 davisagli   (501) staff       (20)      657 2023-08-07 19:08:33.000000 plone.volto-4.1.0/docs/LICENSE.rst
+-rw-r--r--   0 davisagli   (501) staff       (20)       74 2023-08-07 19:08:33.000000 plone.volto-4.1.0/docs/index.rst
+-rw-r--r--   0 davisagli   (501) staff       (20)      881 2023-08-07 19:08:33.000000 plone.volto-4.1.0/pyproject.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)      402 2023-08-07 19:08:33.000000 plone.volto-4.1.0/requirements.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       38 2023-08-07 19:08:34.109097 plone.volto-4.1.0/setup.cfg
+-rw-r--r--   0 davisagli   (501) staff       (20)     2227 2023-08-07 19:08:33.000000 plone.volto-4.1.0/setup.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.092540 plone.volto-4.1.0/src/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.096058 plone.volto-4.1.0/src/plone/
+-rw-r--r--   0 davisagli   (501) staff       (20)       80 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.099169 plone.volto-4.1.0/src/plone/volto/
+-rw-r--r--   0 davisagli   (501) staff       (20)      222 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.099825 plone.volto-4.1.0/src/plone/volto/behaviors/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/behaviors/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1168 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/behaviors/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      534 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/behaviors/headtitle.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      345 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/behaviors/navtitle.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      727 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/behaviors/preview.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2475 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/behaviors/preview_link.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1614 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/blocksuuidfixer.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.100849 plone.volto-4.1.0/src/plone/volto/browser/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2046 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/breadcrumbs.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1743 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     3673 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/migrate_richtext.pt
+-rw-r--r--   0 davisagli   (501) staff       (20)     5548 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/migrate_richtext.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     6949 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/migrate_to_volto.pt
+-rw-r--r--   0 davisagli   (501) staff       (20)    14011 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/migrate_to_volto.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4499 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/navigation.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.100967 plone.volto-4.1.0/src/plone/volto/browser/static/
+-rw-r--r--   0 davisagli   (501) staff       (20)      754 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/static/volto.svg
+-rw-r--r--   0 davisagli   (501) staff       (20)     1368 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/browser/voltobackendwarning.pt
+-rw-r--r--   0 davisagli   (501) staff       (20)     2713 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      697 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/content.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      974 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/controlpanel.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.101423 plone.volto-4.1.0/src/plone/volto/coresandbox/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/coresandbox/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      540 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/coresandbox/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)    28820 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/coresandbox/example.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      745 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/coresandbox/vocabularies.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.101656 plone.volto-4.1.0/src/plone/volto/cors/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/cors/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      462 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/cors/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.102131 plone.volto-4.1.0/src/plone/volto/default_homepage/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/default_homepage/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)    34756 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/default_homepage/default.py
+-rw-r--r--   0 davisagli   (501) staff       (20)    28345 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/default_homepage/demo.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3019 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/default_homepage/lrf.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      516 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/dependencies.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     1424 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/indexers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1006 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/interfaces.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1576 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/linkintegrity.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.102357 plone.volto-4.1.0/src/plone/volto/locales/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.093185 plone.volto-4.1.0/src/plone/volto/locales/de/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.102468 plone.volto-4.1.0/src/plone/volto/locales/de/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     4905 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.093304 plone.volto-4.1.0/src/plone/volto/locales/en/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.102582 plone.volto-4.1.0/src/plone/volto/locales/en/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     4201 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.093426 plone.volto-4.1.0/src/plone/volto/locales/es/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.102696 plone.volto-4.1.0/src/plone/volto/locales/es/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     5074 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.093546 plone.volto-4.1.0/src/plone/volto/locales/eu/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.102810 plone.volto-4.1.0/src/plone/volto/locales/eu/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     4982 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.093674 plone.volto-4.1.0/src/plone/volto/locales/it/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.102929 plone.volto-4.1.0/src/plone/volto/locales/it/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     4457 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
+-rw-r--r--   0 davisagli   (501) staff       (20)     4148 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/locales/plone.volto.pot
+-rwxr-xr-x   0 davisagli   (501) staff       (20)      502 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/locales/update.sh
+-rw-r--r--   0 davisagli   (501) staff       (20)      256 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/overrides.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     2524 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/patches.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      858 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/patches.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.094397 plone.volto-4.1.0/src/plone/volto/profiles/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.103388 plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/
+-rw-r--r--   0 davisagli   (501) staff       (20)      206 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/diff_tool.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      141 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      210 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/repositorytool.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.103504 plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/types/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2466 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/types/example.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/types.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.104176 plone.volto-4.1.0/src/plone/volto/profiles/default/
+-rw-r--r--   0 davisagli   (501) staff       (20)      639 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/actions.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      156 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      314 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/catalog.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      612 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/controlpanel.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      181 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)     1791 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/registry.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.104861 plone.volto-4.1.0/src/plone/volto/profiles/default/types/
+-rw-r--r--   0 davisagli   (501) staff       (20)      286 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/types/Collection.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      814 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/types/Document.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      501 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/types/Event.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      278 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/types/Folder.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      604 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/types/LRF.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      464 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/default/types/News_Item.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.105078 plone.volto-4.1.0/src/plone/volto/profiles/demo/
+-rw-r--r--   0 davisagli   (501) staff       (20)      141 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/demo/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      291 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/demo/rolemap.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.105194 plone.volto-4.1.0/src/plone/volto/profiles/homepage/
+-rw-r--r--   0 davisagli   (501) staff       (20)      141 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/homepage/metadata.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.105425 plone.volto-4.1.0/src/plone/volto/profiles/multilingual/
+-rw-r--r--   0 davisagli   (501) staff       (20)      209 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/multilingual/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      546 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/multilingual/registry.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.105635 plone.volto-4.1.0/src/plone/volto/profiles/richtext/
+-rw-r--r--   0 davisagli   (501) staff       (20)      141 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/richtext/metadata.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.105760 plone.volto-4.1.0/src/plone/volto/profiles/richtext/types/
+-rw-r--r--   0 davisagli   (501) staff       (20)      320 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/richtext/types/Document.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      166 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/richtext/types.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.105893 plone.volto-4.1.0/src/plone/volto/profiles/uninstall/
+-rw-r--r--   0 davisagli   (501) staff       (20)      114 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)     3696 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/profiles.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     3436 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scaling.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.106896 plone.volto-4.1.0/src/plone/volto/scripts/
+-rw-r--r--   0 davisagli   (501) staff       (20)      752 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/add_image_field_metadata.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1206 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/auditblocks.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      202 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/clear-rebuild-catalog.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      773 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/listingaddsummary.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      724 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/migrate_richtext.py
+-rwxr-xr-x   0 davisagli   (501) staff       (20)      123 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/packdb.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1594 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/searchscalesinimageblocks.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      932 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/scripts/utils.py
+-rw-r--r--   0 davisagli   (501) staff       (20)    10185 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/setuphandlers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      312 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/summary.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4513 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/testing.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.108272 plone.volto-4.1.0/src/plone/volto/tests/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1172 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_coresandbox.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3112 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_indexers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2442 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_linkintegrity.py
+-rw-r--r--   0 davisagli   (501) staff       (20)    11771 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_migrate_to_volto.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1823 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_preview_link_behavior.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2126 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_scripts.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3102 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_setup.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1709 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_summary_serialization.py
+-rw-r--r--   0 davisagli   (501) staff       (20)    11245 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_transforms.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     6498 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/tests/test_upgrades.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4777 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/transforms.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     6086 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/upgrades.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2222 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/upgrades.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.108642 plone.volto-4.1.0/src/plone/volto/vocabularies/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/vocabularies/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      105 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/vocabularies/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     4305 2023-08-07 19:08:33.000000 plone.volto-4.1.0/src/plone/volto/vocabularies/subject.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2023-08-07 19:08:34.096980 plone.volto-4.1.0/src/plone.volto.egg-info/
+-rw-r--r--   0 davisagli   (501) staff       (20)    26790 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     4684 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/SOURCES.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/dependency_links.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       40 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/entry_points.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        6 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/namespace_packages.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/not-zip-safe
+-rw-r--r--   0 davisagli   (501) staff       (20)      249 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/requires.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        6 2023-08-07 19:08:34.000000 plone.volto-4.1.0/src/plone.volto.egg-info/top_level.txt
```

### Comparing `plone.volto-4.0.9/CHANGES.rst` & `plone.volto-4.1.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,42 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2023-08-07)
+------------------
+
+New features:
+
+
+- Add `block_types` index to zcatalog. By default it is only added for new Plone sites.
+  To add it to an existing site, run `plone.volto.upgrades.add_block_types_index` manually.
+  [margaridasp, davisagli] (#4778)
+
+
+Bug fixes:
+
+
+- Change the implementation for finding nested blocks to use an IBlockVisitor adapter. @davisagli (#127)
+- Fix missing translations for head_title field. @davisagli (#130)
+
+
+4.0.10 (2023-07-14)
+-------------------
+
+Bug fixes:
+
+
+- Use the plone.app.multilingual conditionally so as is not an explicit dependency
+  [@foxtrot-01] (#119)
+
+
 4.0.9 (2023-06-22)
 ------------------
 
 Bug fixes:
 
 
 - Let the migration-form @@migrate_to_volto transform richtext to slate-blocks by default.
```

### Comparing `plone.volto-4.0.9/PKG-INFO` & `plone.volto-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.volto
-Version: 4.0.9
+Version: 4.1.0
 Summary: Volto integration add-on for Plone
 Home-page: https://github.com/plone/plone.volto
 Author: Plone Foundation
 Author-email: tisto@plone.org
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -322,14 +322,42 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2023-08-07)
+------------------
+
+New features:
+
+
+- Add `block_types` index to zcatalog. By default it is only added for new Plone sites.
+  To add it to an existing site, run `plone.volto.upgrades.add_block_types_index` manually.
+  [margaridasp, davisagli] (#4778)
+
+
+Bug fixes:
+
+
+- Change the implementation for finding nested blocks to use an IBlockVisitor adapter. @davisagli (#127)
+- Fix missing translations for head_title field. @davisagli (#130)
+
+
+4.0.10 (2023-07-14)
+-------------------
+
+Bug fixes:
+
+
+- Use the plone.app.multilingual conditionally so as is not an explicit dependency
+  [@foxtrot-01] (#119)
+
+
 4.0.9 (2023-06-22)
 ------------------
 
 Bug fixes:
 
 
 - Let the migration-form @@migrate_to_volto transform richtext to slate-blocks by default.
```

### Comparing `plone.volto-4.0.9/README.rst` & `plone.volto-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/docs/LICENSE.GPL` & `plone.volto-4.1.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/docs/LICENSE.rst` & `plone.volto-4.1.0/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/pyproject.toml` & `plone.volto-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/setup.py` & `plone.volto-4.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         readfile("CONTRIBUTORS.rst"),
         readfile("CHANGES.rst"),
     ]
 )
 
 setup(
     name="plone.volto",
-    version="4.0.9",
+    version="4.1.0",
     description="Volto integration add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -55,15 +55,15 @@
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.7",
     install_requires=[
         "plone.api",
         "Products.GenericSetup",
         "setuptools",
-        "plone.restapi>=8.13.0",
+        "plone.restapi>=8.41.0",
         "plone.app.vocabularies>=4.3.0",
         "collective.monkeypatcher",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             "plone.testing",
```

### Comparing `plone.volto-4.0.9/src/plone/volto/behaviors/configure.zcml` & `plone.volto-4.1.0/src/plone/volto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/behaviors/headtitle.py` & `plone.volto-4.1.0/src/plone/volto/behaviors/headtitle.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/behaviors/preview.py` & `plone.volto-4.1.0/src/plone/volto/behaviors/preview.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/behaviors/preview_link.py` & `plone.volto-4.1.0/src/plone/volto/behaviors/preview_link.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/blocksuuidfixer.py` & `plone.volto-4.1.0/src/plone/volto/blocksuuidfixer.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/breadcrumbs.py` & `plone.volto-4.1.0/src/plone/volto/browser/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/configure.zcml` & `plone.volto-4.1.0/src/plone/volto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.pt` & `plone.volto-4.1.0/src/plone/volto/browser/migrate_richtext.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.py` & `plone.volto-4.1.0/src/plone/volto/browser/migrate_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.pt` & `plone.volto-4.1.0/src/plone/volto/browser/migrate_to_volto.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.py` & `plone.volto-4.1.0/src/plone/volto/browser/migrate_to_volto.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/navigation.py` & `plone.volto-4.1.0/src/plone/volto/browser/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/static/volto.svg` & `plone.volto-4.1.0/src/plone/volto/browser/static/volto.svg`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/browser/voltobackendwarning.pt` & `plone.volto-4.1.0/src/plone/volto/browser/voltobackendwarning.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/configure.zcml` & `plone.volto-4.1.0/src/plone/volto/configure.zcml`

 * *Files 13% similar despite different names*

```diff
@@ -49,54 +49,44 @@
       factory=".indexers.hasPreviewImage"
       name="hasPreviewImage"
       />
   <adapter
       factory=".indexers.image_field_indexer"
       name="image_field"
       />
+  <adapter
+      factory=".indexers.block_types_indexer"
+      name="block_types"
+      />
 
   <utility
       factory=".summary.JSONSummarySerializerMetadata"
       name="plone.volto.summary_serializer_metadata"
       />
 
-  <configure zcml:condition="have plonerestapi-7">
-    <subscriber
-        factory=".transforms.NestedResolveUIDDeserializer"
-        provides="plone.restapi.interfaces.IBlockFieldDeserializationTransformer"
-        />
-    <subscriber
-        factory=".transforms.NestedResolveUIDDeserializerRoot"
-        provides="plone.restapi.interfaces.IBlockFieldDeserializationTransformer"
-        />
-    <subscriber
-        factory=".transforms.NestedResolveUIDSerializer"
-        provides="plone.restapi.interfaces.IBlockFieldSerializationTransformer"
-        />
-    <subscriber
-        factory=".transforms.NestedResolveUIDSerializerRoot"
-        provides="plone.restapi.interfaces.IBlockFieldSerializationTransformer"
-        />
-    <subscriber
-        factory=".transforms.PreviewImageResolveUIDDeserializer"
-        provides="plone.restapi.interfaces.IBlockFieldDeserializationTransformer"
-        />
-    <subscriber
-        factory=".transforms.PreviewImageResolveUIDDeserializerRoot"
-        provides="plone.restapi.interfaces.IBlockFieldDeserializationTransformer"
-        />
-    <subscriber
-        factory=".transforms.PreviewImageResolveUIDSerializer"
-        provides="plone.restapi.interfaces.IBlockFieldSerializationTransformer"
-        />
-    <subscriber
-        factory=".transforms.PreviewImageResolveUIDSerializerRoot"
-        provides="plone.restapi.interfaces.IBlockFieldSerializationTransformer"
-        />
+  <subscriber
+      factory=".transforms.NestedBlocksVisitor"
+      provides="plone.restapi.interfaces.IBlockVisitor"
+      />
+  <subscriber
+      factory=".transforms.PreviewImageResolveUIDDeserializer"
+      provides="plone.restapi.interfaces.IBlockFieldDeserializationTransformer"
+      />
+  <subscriber
+      factory=".transforms.PreviewImageResolveUIDDeserializerRoot"
+      provides="plone.restapi.interfaces.IBlockFieldDeserializationTransformer"
+      />
+  <subscriber
+      factory=".transforms.PreviewImageResolveUIDSerializer"
+      provides="plone.restapi.interfaces.IBlockFieldSerializationTransformer"
+      />
+  <subscriber
+      factory=".transforms.PreviewImageResolveUIDSerializerRoot"
+      provides="plone.restapi.interfaces.IBlockFieldSerializationTransformer"
+      />
 
-    <subscriber
-        factory=".linkintegrity.NestedBlockLinkRetriever"
-        provides="plone.restapi.interfaces.IBlockFieldLinkIntegrityRetriever"
-        />
-  </configure>
+  <subscriber
+      factory=".linkintegrity.NestedBlockLinkRetriever"
+      provides="plone.restapi.interfaces.IBlockFieldLinkIntegrityRetriever"
+      />
 
 </configure>
```

### Comparing `plone.volto-4.0.9/src/plone/volto/content.py` & `plone.volto-4.1.0/src/plone/volto/content.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/controlpanel.py` & `plone.volto-4.1.0/src/plone/volto/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/coresandbox/configure.zcml` & `plone.volto-4.1.0/src/plone/volto/coresandbox/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/coresandbox/example.py` & `plone.volto-4.1.0/src/plone/volto/coresandbox/example.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/coresandbox/vocabularies.py` & `plone.volto-4.1.0/src/plone/volto/coresandbox/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/default_homepage/default.py` & `plone.volto-4.1.0/src/plone/volto/default_homepage/default.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/default_homepage/demo.py` & `plone.volto-4.1.0/src/plone/volto/default_homepage/demo.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/default_homepage/lrf.py` & `plone.volto-4.1.0/src/plone/volto/default_homepage/lrf.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/dependencies.zcml` & `plone.volto-4.1.0/src/plone/volto/dependencies.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/indexers.py` & `plone.volto-4.1.0/src/plone/volto/indexers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from Acquisition import aq_base
 from plone.dexterity.interfaces import IDexterityContent
 from plone.indexer.decorator import indexer
+from plone.restapi.blocks import visit_blocks
 from plone.volto.behaviors.preview import IPreview
 
 
 @indexer(IPreview)
 def hasPreviewImage(obj):
     """
     Indexer for knowing in a catalog search if a content with the IPreview behavior has
@@ -29,7 +30,18 @@
         getattr(base_obj, "preview_image_link", False)
         and not base_obj.preview_image_link.isBroken()
     ):
         image_field = "preview_image_link"
     elif getattr(base_obj, "image", False):
         image_field = "image"
     return image_field
+
+
+@indexer(IDexterityContent)
+def block_types_indexer(obj):
+    """Indexer for all block types included in a page."""
+    block_types = set()
+    for block in visit_blocks(obj, obj.blocks):
+        block_type = block.get("@type")
+        if block_type:
+            block_types.add(block_type)
+    return block_types
```

### Comparing `plone.volto-4.0.9/src/plone/volto/interfaces.py` & `plone.volto-4.1.0/src/plone/volto/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/linkintegrity.py` & `plone.volto-4.1.0/src/plone/volto/linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po` & `plone.volto-4.1.0/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,147 +1,160 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-08-11 23:31+0000\n"
+"POT-Creation-Date: 2023-08-07 18:19+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: de\n"
 "Language-Name: Deutsch\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone.volto\n"
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Adds Head title field"
 msgstr "Kopftitel Feld hinzufügen"
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Configures the Plone backend to work with Volto, the new default frontend for Plone 6."
 msgstr "Konfiguration des Plone Backends für Volto, dem neuen Standard-Frontend von Plone 6"
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Creates a default page for the site"
 msgstr "Erstellt eine Startseite für die Webseite"
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Creates a default page for the site using (legacy) draftJS blocks"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Creates a default page for the site using slate blocks"
 msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Head title field"
 msgstr "Kopftitel Feld"
 
-#: plone/volto/behaviors/headtitle.py:13
-msgid "Header title"
-msgstr "Kopftitel"
-
-#: plone/volto/behaviors/headtitle.py:15
-msgid "Header title should consist of year and number of the report"
-msgstr "Kopftitel sollte aus Jahr und Nummer des Berichts bestehen"
-
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 #: plone/volto/behaviors/navtitle.py:12
 msgid "Navigation title"
 msgstr "Navigationstitel"
 
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 msgid "Navigation title used in sections, menus and doormats"
 msgstr "Navigationstitel der in der Navigation, Brotkrumen und Auflistungen verwendet wird"
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Plone 6 Frontend (Default content on homepage with draftJS blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Plone 6 Frontend (Default content on homepage with slate blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Plone 6 Frontend (Default content on homepage)"
 msgstr "Plone 6 Frontend (Standard Inhalte)"
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Plone 6 Frontend (plone.volto)"
 msgstr "Plone 6 Frontend (plone.volto)"
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Plone 6 Frontend (plone.volto): uninstall"
 msgstr "Plone 6 Frontend (plone.volto): Deinstallation"
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview Image"
 msgstr "Vorschaubild"
 
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview Image Link"
+msgstr ""
+
 #: plone/volto/behaviors/preview.py:23
+#: plone/volto/behaviors/preview_link.py:43
 msgid "Preview image caption"
 msgstr "Legende zum Vorschaubild"
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview image for listings"
 msgstr "Vorschaubild für Auflistungen"
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview image for listings based on links"
+msgstr ""
+
+#: plone/volto/profiles.zcml:61
 msgid "Special requirements and setup for demo site"
 msgstr "Setup für Demo Website"
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "Special test fixture for coresandbox use cases"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "Special test fixture for multilingual use case"
 msgstr "Text Fixture für Mehrsprachigkeit"
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "Specific profile for re-adding the richtext behavior"
 msgstr "Profil um das Rich-Text Behavior erneut hinzuzufügen"
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Uninstalls the plone.volto add-on."
 msgstr "Deinstalliert die Erweiterung plone.volto"
 
 #. Default: "The languages in which the site should be translatable."
 #: plone/volto/coresandbox/example.py:811
 msgid "description_available_languages"
 msgstr ""
 
 #. Default: "Available languages"
 #: plone/volto/coresandbox/example.py:810
 msgid "heading_available_languages"
 msgstr ""
 
+#. Default: "The header title is shown above the title in teasers."
+#: plone/volto/behaviors/headtitle.py:15
+msgid "help_head_title"
+msgstr "Der Kopftitel wird in Teaser-Blöcken über dem Titel angezeigt."
+
 #. Default: "Insert an image that will be used in listing and teaser blocks."
 #: plone/volto/behaviors/preview.py:15
+#: plone/volto/behaviors/preview_link.py:25
 msgid "help_previewimage"
 msgstr "Bild einfügen welches in Auflistungen und Anreißer-Blöcken verwendet wird."
 
+#. Default: "Header title"
+#: plone/volto/behaviors/headtitle.py:13
+msgid "label_head_title"
+msgstr "Kopftitel"
+
 #. Default: "Preview image"
 #: plone/volto/behaviors/preview.py:14
+#: plone/volto/behaviors/preview_link.py:24
 msgid "label_previewimage"
 msgstr "Vorschaubild"
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "plone.volto coresandbox Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/profiles.zcml:61
 msgid "plone.volto demo special requirements"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "plone.volto multilingual Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "plone.volto p51 profile"
 msgstr ""
```

### Comparing `plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po` & `plone.volto-4.1.0/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,147 +1,160 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-08-11 23:31+0000\n"
+"POT-Creation-Date: 2023-08-07 18:19+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone.volto\n"
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Adds Head title field"
 msgstr ""
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Configures the Plone backend to work with Volto, the new default frontend for Plone 6."
 msgstr ""
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Creates a default page for the site"
 msgstr ""
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Creates a default page for the site using (legacy) draftJS blocks"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Creates a default page for the site using slate blocks"
 msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Head title field"
 msgstr ""
 
-#: plone/volto/behaviors/headtitle.py:13
-msgid "Header title"
-msgstr ""
-
-#: plone/volto/behaviors/headtitle.py:15
-msgid "Header title should consist of year and number of the report"
-msgstr ""
-
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 #: plone/volto/behaviors/navtitle.py:12
 msgid "Navigation title"
 msgstr "Navigation title"
 
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 msgid "Navigation title used in sections, menus and doormats"
 msgstr ""
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Plone 6 Frontend (Default content on homepage with draftJS blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Plone 6 Frontend (Default content on homepage with slate blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Plone 6 Frontend (Default content on homepage)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Plone 6 Frontend (plone.volto)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Plone 6 Frontend (plone.volto): uninstall"
 msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview Image"
 msgstr ""
 
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview Image Link"
+msgstr ""
+
 #: plone/volto/behaviors/preview.py:23
+#: plone/volto/behaviors/preview_link.py:43
 msgid "Preview image caption"
 msgstr "Preview image caption"
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview image for listings"
 msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview image for listings based on links"
+msgstr ""
+
+#: plone/volto/profiles.zcml:61
 msgid "Special requirements and setup for demo site"
 msgstr ""
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "Special test fixture for coresandbox use cases"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "Special test fixture for multilingual use case"
 msgstr ""
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "Specific profile for re-adding the richtext behavior"
 msgstr ""
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Uninstalls the plone.volto add-on."
 msgstr ""
 
 #. Default: "The languages in which the site should be translatable."
 #: plone/volto/coresandbox/example.py:811
 msgid "description_available_languages"
 msgstr ""
 
 #. Default: "Available languages"
 #: plone/volto/coresandbox/example.py:810
 msgid "heading_available_languages"
 msgstr ""
 
+#. Default: "The header title is shown above the title in teasers."
+#: plone/volto/behaviors/headtitle.py:15
+msgid "help_head_title"
+msgstr ""
+
 #. Default: "Insert an image that will be used in listing and teaser blocks."
 #: plone/volto/behaviors/preview.py:15
+#: plone/volto/behaviors/preview_link.py:25
 msgid "help_previewimage"
 msgstr ""
 
+#. Default: "Header title"
+#: plone/volto/behaviors/headtitle.py:13
+msgid "label_head_title"
+msgstr ""
+
 #. Default: "Preview image"
 #: plone/volto/behaviors/preview.py:14
+#: plone/volto/behaviors/preview_link.py:24
 msgid "label_previewimage"
 msgstr "Preview image"
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "plone.volto coresandbox Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/profiles.zcml:61
 msgid "plone.volto demo special requirements"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "plone.volto multilingual Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "plone.volto p51 profile"
 msgstr ""
```

### Comparing `plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po` & `plone.volto-4.1.0/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,149 +1,162 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Mikel Larreategi <mlarreategi@codesyntax.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
-"POT-Creation-Date: 2022-08-11 23:31+0000\n"
+"POT-Creation-Date: 2023-08-07 18:19+0000\n"
 "PO-Revision-Date: 2021-11-21 16:58+0100\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "Language-Code: es\n"
 "Language-Name: Spanish\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone.volto\n"
 "Language: es\n"
 "X-Generator: Poedit 2.3\n"
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Adds Head title field"
 msgstr "Añade el campo de título de cabecera"
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Configures the Plone backend to work with Volto, the new default frontend for Plone 6."
 msgstr "Configura Plone para funcionar con Volto, el nuevo frontal de Plone 6."
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Creates a default page for the site"
 msgstr "Crea la página por defecto del sitio"
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Creates a default page for the site using (legacy) draftJS blocks"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Creates a default page for the site using slate blocks"
 msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Head title field"
 msgstr "Campo de título de cabecera"
 
-#: plone/volto/behaviors/headtitle.py:13
-msgid "Header title"
-msgstr "Título de cabecera"
-
-#: plone/volto/behaviors/headtitle.py:15
-msgid "Header title should consist of year and number of the report"
-msgstr "El título de cabecera debería tener el año y número de informe"
-
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 #: plone/volto/behaviors/navtitle.py:12
 msgid "Navigation title"
 msgstr "Título de la navegación"
 
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 msgid "Navigation title used in sections, menus and doormats"
 msgstr "Título de la navegación utilizado en secciones, menús y acordeones"
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Plone 6 Frontend (Default content on homepage with draftJS blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Plone 6 Frontend (Default content on homepage with slate blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Plone 6 Frontend (Default content on homepage)"
 msgstr "Frontal Plone 6 (contenido por defecto en la portada)"
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Plone 6 Frontend (plone.volto)"
 msgstr "Frontal Plone 6 (plone.volto)"
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Plone 6 Frontend (plone.volto): uninstall"
 msgstr "Frontal Plone 6 (plone.volto): desinstalar"
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview Image"
 msgstr "Imagen"
 
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview Image Link"
+msgstr ""
+
 #: plone/volto/behaviors/preview.py:23
+#: plone/volto/behaviors/preview_link.py:43
 msgid "Preview image caption"
 msgstr "Preview image caption"
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview image for listings"
 msgstr "Imagen para listados"
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview image for listings based on links"
+msgstr ""
+
+#: plone/volto/profiles.zcml:61
 msgid "Special requirements and setup for demo site"
 msgstr "Configuración especial para instalar el sitio de demo"
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "Special test fixture for coresandbox use cases"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "Special test fixture for multilingual use case"
 msgstr "Perfil especial para configurar los tests de un sitio multilingüe"
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "Specific profile for re-adding the richtext behavior"
 msgstr "Perfil específico para añadir otra vez el comportamiento de texto"
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Uninstalls the plone.volto add-on."
 msgstr "Desinstalar plone.volto"
 
 #. Default: "The languages in which the site should be translatable."
 #: plone/volto/coresandbox/example.py:811
 msgid "description_available_languages"
 msgstr ""
 
 #. Default: "Available languages"
 #: plone/volto/coresandbox/example.py:810
 msgid "heading_available_languages"
 msgstr ""
 
+#. Default: "The header title is shown above the title in teasers."
+#: plone/volto/behaviors/headtitle.py:15
+msgid "help_head_title"
+msgstr "El título del cabecera se muestra encima del título en los bloques teaser."
+
 #. Default: "Insert an image that will be used in listing and teaser blocks."
 #: plone/volto/behaviors/preview.py:15
+#: plone/volto/behaviors/preview_link.py:25
 msgid "help_previewimage"
 msgstr "Introduzca la imagen que se utilizará en los listados y otros bloques"
 
+#. Default: "Header title"
+#: plone/volto/behaviors/headtitle.py:13
+msgid "label_head_title"
+msgstr "Título de cabecera"
+
 #. Default: "Preview image"
 #: plone/volto/behaviors/preview.py:14
+#: plone/volto/behaviors/preview_link.py:24
 msgid "label_previewimage"
 msgstr "Imagen"
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "plone.volto coresandbox Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/profiles.zcml:61
 msgid "plone.volto demo special requirements"
 msgstr "Requisitos especiales de la demo de plone.volto"
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "plone.volto multilingual Cypress tests fixtures"
 msgstr "Tests de plone.volto multilingüe"
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "plone.volto p51 profile"
 msgstr "Perfil plone.volto p51"
```

### Comparing `plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po` & `plone.volto-4.1.0/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,149 +1,160 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
-# Mikel Larreategi <mlarreategi@codesyntax.com>, 2021
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
-"POT-Creation-Date: 2022-08-11 23:31+0000\n"
-"PO-Revision-Date: 2021-11-21 16:50+0100\n"
-"Last-Translator: \n"
-"Language-Team: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
+"POT-Creation-Date: 2023-08-07 18:19+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"Language-Code: eu\n"
-"Language-Name: Basque\n"
+"Plural-Forms: nplurals=1; plural=0\n"
+"Language-Code: it\n"
+"Language-Name: Italian\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone.volto\n"
-"Language: eu\n"
-"X-Generator: Poedit 2.3\n"
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Adds Head title field"
-msgstr "Goiburuko izenburua gehitu"
+msgstr ""
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Configures the Plone backend to work with Volto, the new default frontend for Plone 6."
-msgstr "Plone Voltorekin funtzionatzeko konfiguratzen du, Plone 6rako Frontend berria."
+msgstr "Configura il backend di Plone per lavorare con Volto."
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Creates a default page for the site"
-msgstr "Atariaren defektuzko orri berria sortzen du"
+msgstr "Crea una pagina di default per questo sito"
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Creates a default page for the site using (legacy) draftJS blocks"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Creates a default page for the site using slate blocks"
 msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Head title field"
-msgstr "Goiburuko izenburuaren eremua"
-
-#: plone/volto/behaviors/headtitle.py:13
-msgid "Header title"
-msgstr "Goiburuko izenburua"
-
-#: plone/volto/behaviors/headtitle.py:15
-msgid "Header title should consist of year and number of the report"
-msgstr "Goiburukoan erabiliko den izenburua"
+msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 #: plone/volto/behaviors/navtitle.py:12
 msgid "Navigation title"
-msgstr "Nabigazioaren izenburua"
+msgstr "Navigation title"
 
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 msgid "Navigation title used in sections, menus and doormats"
-msgstr "Atal, menu eta akordeoietan erabiliko den nabigazioaren izenburua"
+msgstr ""
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Plone 6 Frontend (Default content on homepage with draftJS blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Plone 6 Frontend (Default content on homepage with slate blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Plone 6 Frontend (Default content on homepage)"
-msgstr "Plone 6 Frontenda (hasiera orria defektuzko edukiarekin)"
+msgstr ""
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Plone 6 Frontend (plone.volto)"
-msgstr "Plone 6 Frontenda (plone.volto)"
+msgstr ""
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Plone 6 Frontend (plone.volto): uninstall"
-msgstr "Plone 6 Frontenda (plone.volto): kendu"
+msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview Image"
-msgstr "Irudia"
+msgstr "Immagine di anteprima"
+
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview Image Link"
+msgstr ""
 
 #: plone/volto/behaviors/preview.py:23
+#: plone/volto/behaviors/preview_link.py:43
 msgid "Preview image caption"
-msgstr "Irudi-oina"
+msgstr "Didascalia dell'immagine di anteprima"
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview image for listings"
-msgstr "Zerrendetan erabiliko den irudia"
+msgstr "Immagine di anteprima da utilizzare nei blocchi listing."
+
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview image for listings based on links"
+msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/profiles.zcml:61
 msgid "Special requirements and setup for demo site"
-msgstr "Demo webgunea konfiguratzeko profil berezia"
+msgstr ""
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "Special test fixture for coresandbox use cases"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "Special test fixture for multilingual use case"
-msgstr "Webgune eleanitzetan erabiltzeko profila"
+msgstr ""
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "Specific profile for re-adding the richtext behavior"
-msgstr "Testu aberatseko portaera gehitzeko profila"
+msgstr ""
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Uninstalls the plone.volto add-on."
-msgstr "plone.volto kendu"
+msgstr ""
 
 #. Default: "The languages in which the site should be translatable."
 #: plone/volto/coresandbox/example.py:811
 msgid "description_available_languages"
 msgstr ""
 
 #. Default: "Available languages"
 #: plone/volto/coresandbox/example.py:810
 msgid "heading_available_languages"
 msgstr ""
 
+#. Default: "The header title is shown above the title in teasers."
+#: plone/volto/behaviors/headtitle.py:15
+msgid "help_head_title"
+msgstr ""
+
 #. Default: "Insert an image that will be used in listing and teaser blocks."
 #: plone/volto/behaviors/preview.py:15
+#: plone/volto/behaviors/preview_link.py:25
 msgid "help_previewimage"
-msgstr "Kargatu zerrendetan eta destakatuen blokeetan defektuz erabiliko den irudia"
+msgstr "Immagine che verrà utilizzata nei blocchi listing e teaser."
+
+#. Default: "Header title"
+#: plone/volto/behaviors/headtitle.py:13
+msgid "label_head_title"
+msgstr ""
 
 #. Default: "Preview image"
 #: plone/volto/behaviors/preview.py:14
+#: plone/volto/behaviors/preview_link.py:24
 msgid "label_previewimage"
-msgstr "Irudia"
+msgstr "Immagine di anteprima"
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "plone.volto coresandbox Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/profiles.zcml:61
 msgid "plone.volto demo special requirements"
-msgstr "plone.volto demoren konfigurazio berezia"
+msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "plone.volto multilingual Cypress tests fixtures"
-msgstr "plone.volto eleanitzaren Cypress testen konfigurazioa"
+msgstr ""
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "plone.volto p51 profile"
-msgstr "plone.volto p51 profila"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po` & `plone.volto-4.1.0/src/plone/volto/locales/plone.volto.pot`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,160 @@
-# --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
-# SOME DESCRIPTIVE TITLE.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
+#SOME DESCRIPTIVE TITLE.
+#FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-08-11 23:31+0000\n"
+"POT-Creation-Date: 2023-08-07 18:19+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
-"Language-Code: it\n"
-"Language-Name: Italian\n"
+"Language-Code: en\n"
+"Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone.volto\n"
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Adds Head title field"
 msgstr ""
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Configures the Plone backend to work with Volto, the new default frontend for Plone 6."
-msgstr "Configura il backend di Plone per lavorare con Volto."
+msgstr ""
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Creates a default page for the site"
-msgstr "Crea una pagina di default per questo sito"
+msgstr ""
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Creates a default page for the site using (legacy) draftJS blocks"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Creates a default page for the site using slate blocks"
 msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:31
+#: plone/volto/behaviors/configure.zcml:42
 msgid "Head title field"
 msgstr ""
 
-#: plone/volto/behaviors/headtitle.py:13
-msgid "Header title"
-msgstr ""
-
-#: plone/volto/behaviors/headtitle.py:15
-msgid "Header title should consist of year and number of the report"
-msgstr ""
-
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 #: plone/volto/behaviors/navtitle.py:12
 msgid "Navigation title"
-msgstr "Navigation title"
+msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:24
+#: plone/volto/behaviors/configure.zcml:35
 msgid "Navigation title used in sections, menus and doormats"
 msgstr ""
 
-#: plone/volto/profiles.zcml:42
+#: plone/volto/profiles.zcml:43
 msgid "Plone 6 Frontend (Default content on homepage with draftJS blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:51
+#: plone/volto/profiles.zcml:52
 msgid "Plone 6 Frontend (Default content on homepage with slate blocks)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:33
+#: plone/volto/profiles.zcml:34
 msgid "Plone 6 Frontend (Default content on homepage)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:15
+#: plone/volto/profiles.zcml:16
 msgid "Plone 6 Frontend (plone.volto)"
 msgstr ""
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Plone 6 Frontend (plone.volto): uninstall"
 msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview Image"
-msgstr "Immagine di anteprima"
+msgstr ""
+
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview Image Link"
+msgstr ""
 
 #: plone/volto/behaviors/preview.py:23
+#: plone/volto/behaviors/preview_link.py:43
 msgid "Preview image caption"
-msgstr "Didascalia dell'immagine di anteprima"
+msgstr ""
 
-#: plone/volto/behaviors/configure.zcml:17
+#: plone/volto/behaviors/configure.zcml:18
 msgid "Preview image for listings"
-msgstr "Immagine di anteprima da utilizzare nei blocchi listing."
+msgstr ""
+
+#: plone/volto/behaviors/configure.zcml:26
+msgid "Preview image for listings based on links"
+msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/profiles.zcml:61
 msgid "Special requirements and setup for demo site"
 msgstr ""
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "Special test fixture for coresandbox use cases"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "Special test fixture for multilingual use case"
 msgstr ""
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "Specific profile for re-adding the richtext behavior"
 msgstr ""
 
-#: plone/volto/profiles.zcml:24
+#: plone/volto/profiles.zcml:25
 msgid "Uninstalls the plone.volto add-on."
 msgstr ""
 
 #. Default: "The languages in which the site should be translatable."
 #: plone/volto/coresandbox/example.py:811
 msgid "description_available_languages"
 msgstr ""
 
 #. Default: "Available languages"
 #: plone/volto/coresandbox/example.py:810
 msgid "heading_available_languages"
 msgstr ""
 
+#. Default: "The header title is shown above the title in teasers."
+#: plone/volto/behaviors/headtitle.py:15
+msgid "help_head_title"
+msgstr ""
+
 #. Default: "Insert an image that will be used in listing and teaser blocks."
 #: plone/volto/behaviors/preview.py:15
+#: plone/volto/behaviors/preview_link.py:25
 msgid "help_previewimage"
-msgstr "Immagine che verrà utilizzata nei blocchi listing e teaser."
+msgstr ""
+
+#. Default: "Header title"
+#: plone/volto/behaviors/headtitle.py:13
+msgid "label_head_title"
+msgstr ""
 
 #. Default: "Preview image"
 #: plone/volto/behaviors/preview.py:14
+#: plone/volto/behaviors/preview_link.py:24
 msgid "label_previewimage"
-msgstr "Immagine di anteprima"
+msgstr ""
 
-#: plone/volto/profiles.zcml:70
+#: plone/volto/profiles.zcml:71
 msgid "plone.volto coresandbox Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:60
+#: plone/volto/profiles.zcml:61
 msgid "plone.volto demo special requirements"
 msgstr ""
 
-#: plone/volto/profiles.zcml:80
+#: plone/volto/profiles.zcml:82
 msgid "plone.volto multilingual Cypress tests fixtures"
 msgstr ""
 
-#: plone/volto/profiles.zcml:88
+#: plone/volto/profiles.zcml:90
 msgid "plone.volto p51 profile"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `plone.volto-4.0.9/src/plone/volto/patches.py` & `plone.volto-4.1.0/src/plone/volto/patches.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/patches.zcml` & `plone.volto-4.1.0/src/plone/volto/patches.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types/example.xml` & `plone.volto-4.1.0/src/plone/volto/profiles/coresandbox/types/example.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles/default/actions.xml` & `plone.volto-4.1.0/src/plone/volto/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles/default/controlpanel.xml` & `plone.volto-4.1.0/src/plone/volto/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles/default/registry.xml` & `plone.volto-4.1.0/src/plone/volto/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles/default/types/Document.xml` & `plone.volto-4.1.0/src/plone/volto/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles/default/types/LRF.xml` & `plone.volto-4.1.0/src/plone/volto/profiles/default/types/LRF.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles/multilingual/registry.xml` & `plone.volto-4.1.0/src/plone/volto/profiles/multilingual/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/profiles.zcml` & `plone.volto-4.1.0/src/plone/volto/profiles.zcml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
     i18n_domain="plone.volto"
     >
 
   <genericsetup:registerProfile
       name="default"
       title="Plone 6 Frontend (plone.volto)"
       description="Configures the Plone backend to work with Volto, the new default frontend for Plone 6."
@@ -73,14 +74,15 @@
   <genericsetup:registerProfile
       name="multilingual"
       title="plone.volto multilingual Cypress tests fixtures"
       description="Special test fixture for multilingual use case"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       directory="profiles/multilingual"
       post_handler=".setuphandlers.post_install_multilingual"
+      zcml:condition="installed plone.app.multilingual"
       />
 
   <genericsetup:registerProfile
       name="richtext"
       title="plone.volto p51 profile"
       description="Specific profile for re-adding the richtext behavior"
       provides="Products.GenericSetup.interfaces.EXTENSION"
```

### Comparing `plone.volto-4.0.9/src/plone/volto/scaling.py` & `plone.volto-4.1.0/src/plone/volto/scaling.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/scripts/add_image_field_metadata.py` & `plone.volto-4.1.0/src/plone/volto/scripts/add_image_field_metadata.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/scripts/auditblocks.py` & `plone.volto-4.1.0/src/plone/volto/scripts/auditblocks.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/scripts/listingaddsummary.py` & `plone.volto-4.1.0/src/plone/volto/scripts/listingaddsummary.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/scripts/migrate_richtext.py` & `plone.volto-4.1.0/src/plone/volto/scripts/migrate_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/scripts/searchscalesinimageblocks.py` & `plone.volto-4.1.0/src/plone/volto/scripts/searchscalesinimageblocks.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/scripts/utils.py` & `plone.volto-4.1.0/src/plone/volto/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/setuphandlers.py` & `plone.volto-4.1.0/src/plone/volto/setuphandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # -*- coding: utf-8 -*-
 from importlib import import_module
 from plone import api
-from plone.app.multilingual.browser.setup import SetupMultilingualSite
-from plone.app.multilingual.setuphandlers import enable_translatable_behavior
 from plone.dexterity.interfaces import IDexterityFTI
 from plone.volto.default_homepage.default import default_home
 from plone.volto.default_homepage.demo import demo_home_page
 from plone.volto.default_homepage.lrf import default_lrf_home
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.interfaces import INonInstallable
 from Products.CMFPlone.utils import get_installer
 from zope.component import queryUtility
 from zope.interface import implementer
 
 import json
 import logging
+import pkg_resources
 import transaction
 
 
+try:
+    pkg_resources.get_distribution("plone.app.multilingual")
+    from plone.app.multilingual.browser.setup import SetupMultilingualSite
+    from plone.app.multilingual.setuphandlers import enable_translatable_behavior
+
+    HAS_MULTILINGUAL = True
+except pkg_resources.DistributionNotFound:
+    HAS_MULTILINGUAL = False
+
 PLONE_6 = getattr(import_module("Products.CMFPlone.factory"), "PLONE60MARKER", False)
 
 logger = logging.getLogger("plone.volto")
 
 NO_RICHTEXT_BEHAVIOR_CONTENT_TYPES = [
     "Plone Site",
     "Document",
@@ -64,20 +72,21 @@
 def post_install_multilingual(context):
     """Post install script for multilingual fixture"""
     enable_pam(context)
     create_default_homepage(context)
 
 
 def enable_pam(portal):
-    # Ensure that portal is portal
-    portal = api.portal.get()
-    # Setup the plone.app.multilingual data
-    sms = SetupMultilingualSite(portal)
-    sms.setupSite(portal)
-    enable_translatable_behavior(portal)
+    if HAS_MULTILINGUAL:
+        # Ensure that portal is portal
+        portal = api.portal.get()
+        # Setup the plone.app.multilingual data
+        sms = SetupMultilingualSite(portal)
+        sms.setupSite(portal)
+        enable_translatable_behavior(portal)
 
 
 def ensure_pam_consistency(portal):
     """Makes sure that all the content in a language branch has language"""
 
     # Ensure that all the objects below an LFR is of the intended language
     pc = getToolByName(portal, "portal_catalog")
```

### Comparing `plone.volto-4.0.9/src/plone/volto/testing.py` & `plone.volto-4.1.0/src/plone/volto/testing.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_coresandbox.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_coresandbox.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_linkintegrity.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_migrate_to_volto.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_migrate_to_volto.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_preview_link_behavior.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_preview_link_behavior.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_scripts.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_setup.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_summary_serialization.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_summary_serialization.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_transforms.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/tests/test_upgrades.py` & `plone.volto-4.1.0/src/plone/volto/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/transforms.py` & `plone.volto-4.1.0/src/plone/volto/transforms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,43 @@
 from plone.restapi.behaviors import IBlocks
 from plone.restapi.deserializer.blocks import ResolveUIDDeserializerBase
 from plone.restapi.interfaces import IBlockFieldDeserializationTransformer
 from plone.restapi.interfaces import IBlockFieldSerializationTransformer
+from plone.restapi.interfaces import IBlockVisitor
 from plone.restapi.serializer.blocks import ResolveUIDSerializerBase
 from Products.CMFPlone.interfaces import IPloneSiteRoot
 from zope.component import adapter
 from zope.component import subscribers
 from zope.interface import implementer
+from zope.interface import Interface
 from zope.publisher.interfaces.browser import IBrowserRequest
 
 
+@implementer(IBlockVisitor)
+@adapter(Interface, IBrowserRequest)
+class NestedBlocksVisitor:
+    """Visit nested blocks in columns, hrefList, or slides."""
+
+    def __init__(self, context, request):
+        pass
+
+    def __call__(self, block_value):
+        for nested_name in ("columns", "hrefList", "slides"):
+            nested_blocks = block_value.get(nested_name, [])
+            if not isinstance(nested_blocks, list):
+                continue
+            yield from nested_blocks
+
+
 class NestedResolveUIDDeserializerBase(object):
     """The "url" smart block field for nested blocks
 
+    [Deprecated -- replaced by NestedBlocksVisitor above,
+    but the base class is still here in case someone extended it.]
+
     This is a generic handler. In all blocks, it converts any "url"
     field from using resolveuid to an "absolute" URL
     """
 
     order = 1
     block_type = None
 
@@ -47,27 +68,20 @@
             if not isinstance(nested_blocks, list):
                 continue
             for nested_block in nested_blocks:
                 self._transform(nested_block)
         return block
 
 
-@adapter(IBlocks, IBrowserRequest)
-@implementer(IBlockFieldDeserializationTransformer)
-class NestedResolveUIDDeserializer(NestedResolveUIDDeserializerBase):
-    """Deserializer for content-types that implements IBlocks behavior"""
-
-
-@adapter(IPloneSiteRoot, IBrowserRequest)
-@implementer(IBlockFieldDeserializationTransformer)
-class NestedResolveUIDDeserializerRoot(NestedResolveUIDDeserializerBase):
-    """Deserializer for site root"""
-
-
 class NestedResolveUIDSerializerBase(object):
+    """
+    [Deprecated -- replaced by NestedBlocksVisitor above,
+    but the base class is still here in case someone extended it.]
+    """
+
     order = 1
     block_type = None
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
@@ -96,26 +110,14 @@
             for nested_block in nested_blocks:
                 self._transform(nested_block)
         return block
 
 
 @adapter(IBlocks, IBrowserRequest)
 @implementer(IBlockFieldDeserializationTransformer)
-class NestedResolveUIDSerializer(NestedResolveUIDSerializerBase):
-    """Deserializer for content-types that implements IBlocks behavior"""
-
-
-@adapter(IPloneSiteRoot, IBrowserRequest)
-@implementer(IBlockFieldDeserializationTransformer)
-class NestedResolveUIDSerializerRoot(NestedResolveUIDSerializerBase):
-    """Deserializer for site root"""
-
-
-@adapter(IBlocks, IBrowserRequest)
-@implementer(IBlockFieldDeserializationTransformer)
 class PreviewImageResolveUIDDeserializer(ResolveUIDDeserializerBase):
     """Deserializer for resolveuid in preview_image field"""
 
     fields = ["preview_image"]
 
 
 @adapter(IPloneSiteRoot, IBrowserRequest)
```

### Comparing `plone.volto-4.0.9/src/plone/volto/upgrades.py` & `plone.volto-4.1.0/src/plone/volto/upgrades.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 from plone.registry.interfaces import IRegistry
 from plone.registry.record import Record
 from plone.restapi.behaviors import IBlocks
 from plone.volto import content
 from plone.volto import logger
 from plone.volto.setuphandlers import NO_RICHTEXT_BEHAVIOR_CONTENT_TYPES
 from plone.volto.setuphandlers import remove_behavior
+from Products.CMFCore.utils import getToolByName
 from zope.component import getUtility
 
+import transaction
+
 
 MIGRATION = {
     "Document": content.FolderishDocument,
     "Event": content.FolderishEvent,
     "News Item": content.FolderishNewsItem,
 }
 
@@ -119,7 +122,24 @@
 
 def add_control_panel_classic_icon(context):
     registry = getUtility(IRegistry)
     registry.records["plone.icon.volto-settings"] = Record(
         field.TextLine(title="Plone Icon Volto Control Panel"),
     )
     registry["plone.icon.volto-settings"] = "++plone++plone.volto/volto.svg"
+
+
+def add_block_types_index(context):
+    catalog = getToolByName(context, "portal_catalog")
+    indexes = catalog.indexes()
+    if "block_types" not in indexes:
+        catalog.addIndex("block_types", "KeywordIndex")
+        logger.info("Added block_types index.")
+    brains = catalog(object_provides="plone.restapi.behaviors.IBlocks")
+    total = len(brains)
+    for index, brain in enumerate(brains):
+        obj = brain.getObject()
+        obj.reindexObject(idxs=["block_types"], update_metadata=0)
+        logger.info("Reindexing object %s.", brain.getPath())
+        if index % 250 == 0:
+            logger.info(f"Reindexed {index}/{total} objects")
+            transaction.commit()
```

### Comparing `plone.volto-4.0.9/src/plone/volto/upgrades.zcml` & `plone.volto-4.1.0/src/plone/volto/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone/volto/vocabularies/subject.py` & `plone.volto-4.1.0/src/plone/volto/vocabularies/subject.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.9/src/plone.volto.egg-info/PKG-INFO` & `plone.volto-4.1.0/src/plone.volto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.volto
-Version: 4.0.9
+Version: 4.1.0
 Summary: Volto integration add-on for Plone
 Home-page: https://github.com/plone/plone.volto
 Author: Plone Foundation
 Author-email: tisto@plone.org
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -322,14 +322,42 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2023-08-07)
+------------------
+
+New features:
+
+
+- Add `block_types` index to zcatalog. By default it is only added for new Plone sites.
+  To add it to an existing site, run `plone.volto.upgrades.add_block_types_index` manually.
+  [margaridasp, davisagli] (#4778)
+
+
+Bug fixes:
+
+
+- Change the implementation for finding nested blocks to use an IBlockVisitor adapter. @davisagli (#127)
+- Fix missing translations for head_title field. @davisagli (#130)
+
+
+4.0.10 (2023-07-14)
+-------------------
+
+Bug fixes:
+
+
+- Use the plone.app.multilingual conditionally so as is not an explicit dependency
+  [@foxtrot-01] (#119)
+
+
 4.0.9 (2023-06-22)
 ------------------
 
 Bug fixes:
 
 
 - Let the migration-form @@migrate_to_volto transform richtext to slate-blocks by default.
```

### Comparing `plone.volto-4.0.9/src/plone.volto.egg-info/SOURCES.txt` & `plone.volto-4.1.0/src/plone.volto.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 README.rst
 pyproject.toml
 requirements.txt
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.rst
 docs/index.rst
-requirements/dev.txt
-requirements/plone-5.2.txt
-requirements/plone-6.0.txt
-requirements/prod.txt
 src/plone/__init__.py
 src/plone.volto.egg-info/PKG-INFO
 src/plone.volto.egg-info/SOURCES.txt
 src/plone.volto.egg-info/dependency_links.txt
 src/plone.volto.egg-info/entry_points.txt
 src/plone.volto.egg-info/namespace_packages.txt
 src/plone.volto.egg-info/not-zip-safe
@@ -64,23 +60,18 @@
 src/plone/volto/cors/configure.zcml
 src/plone/volto/default_homepage/__init__.py
 src/plone/volto/default_homepage/default.py
 src/plone/volto/default_homepage/demo.py
 src/plone/volto/default_homepage/lrf.py
 src/plone/volto/locales/plone.volto.pot
 src/plone/volto/locales/update.sh
-src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
-src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
-src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
-src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
-src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
 src/plone/volto/profiles/coresandbox/diff_tool.xml
 src/plone/volto/profiles/coresandbox/metadata.xml
 src/plone/volto/profiles/coresandbox/repositorytool.xml
 src/plone/volto/profiles/coresandbox/types.xml
 src/plone/volto/profiles/coresandbox/types/example.xml
 src/plone/volto/profiles/default/actions.xml
@@ -110,14 +101,15 @@
 src/plone/volto/scripts/listingaddsummary.py
 src/plone/volto/scripts/migrate_richtext.py
 src/plone/volto/scripts/packdb.py
 src/plone/volto/scripts/searchscalesinimageblocks.py
 src/plone/volto/scripts/utils.py
 src/plone/volto/tests/__init__.py
 src/plone/volto/tests/test_coresandbox.py
+src/plone/volto/tests/test_indexers.py
 src/plone/volto/tests/test_linkintegrity.py
 src/plone/volto/tests/test_migrate_to_volto.py
 src/plone/volto/tests/test_preview_link_behavior.py
 src/plone/volto/tests/test_scripts.py
 src/plone/volto/tests/test_setup.py
 src/plone/volto/tests/test_summary_serialization.py
 src/plone/volto/tests/test_transforms.py
```

