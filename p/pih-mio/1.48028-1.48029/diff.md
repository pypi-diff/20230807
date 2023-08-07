# Comparing `tmp/pih-mio-1.48028.tar.gz` & `tmp/pih-mio-1.48029.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48028.tar", last modified: Sat Aug  5 14:22:39 2023, max compression
+gzip compressed data, was "pih-mio-1.48029.tar", last modified: Sun Aug  6 08:12:01 2023, max compression
```

## Comparing `pih-mio-1.48028.tar` & `pih-mio-1.48029.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 14:22:39.136757 pih-mio-1.48028/
-drwxrwxrwx   0        0        0        0 2023-08-05 14:22:39.183637 pih-mio-1.48028/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48028/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      161 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   168461 2023-08-05 14:21:36.000000 pih-mio-1.48028/MobileHelperService/api.py
--rw-rw-rw-   0        0        0      721 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/service.py
--rw-rw-rw-   0        0        0     9592 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      989 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-05 14:22:39.683623 pih-mio-1.48028/PKG-INFO
--rw-rw-rw-   0        0        0     1658 2023-08-05 09:44:51.000000 pih-mio-1.48028/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 14:22:39.652377 pih-mio-1.48028/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 14:22:39.699461 pih-mio-1.48028/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 08:12:01.026921 pih-mio-1.48029/
+drwxrwxrwx   0        0        0        0 2023-08-06 08:12:01.589400 pih-mio-1.48029/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48029/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-08-05 09:47:04.000000 pih-mio-1.48029/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   168407 2023-08-06 08:10:45.000000 pih-mio-1.48029/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0      721 2023-08-05 09:47:04.000000 pih-mio-1.48029/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0     9592 2023-08-05 09:47:04.000000 pih-mio-1.48029/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      989 2023-08-05 09:47:04.000000 pih-mio-1.48029/MobileHelperService/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-06 08:12:02.027103 pih-mio-1.48029/PKG-INFO
+-rw-rw-rw-   0        0        0     1658 2023-08-05 09:44:51.000000 pih-mio-1.48029/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 08:12:01.980017 pih-mio-1.48029/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-06 08:12:00.000000 pih-mio-1.48029/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-08-06 08:12:00.000000 pih-mio-1.48029/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 08:12:00.000000 pih-mio-1.48029/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-08-06 08:12:00.000000 pih-mio-1.48029/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-06 08:12:00.000000 pih-mio-1.48029/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-06 08:12:00.000000 pih-mio-1.48029/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 08:12:02.042553 pih-mio-1.48029/setup.cfg
```

### Comparing `pih-mio-1.48028/MobileHelperService/api.py` & `pih-mio-1.48029/MobileHelperService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from MobileHelperContent.content import MEDIA_CONTENT
 import requests
 from io import BytesIO
 
 class MIO:
 
     NAME: str = "mio"       
-    VERSION: str = "1.48028"  
+    VERSION: str = "1.48029"  
 
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
         return self.args[0]
 
@@ -1309,19 +1309,18 @@
         section_list = section_list or CheckableSections.all()
         self.console_apps_api.resources_and_indications_check(section_list, False, self.is_forced, all)
 
     def register_ct_indications_handler(self) -> None:
         self.console_apps_api.register_ct_indications()
 
     def create_polibase_db_backup_handler(self) -> None:
-        from PolibaseDBService.api import PolibaseDBApi
-        dump_name: str = PolibaseDBApi.get_default_name()
+        name: str = A.D.now_to_string(A.CT_P.DATABASE_DATETIME_FORMAT)
         answer: bool = self.input.yes_no(
-            f"Изменить имя файла дампа базы данных", False, b("Отправьте имя"), f"Использовать имя: {b(dump_name)} - отправьте {A.CT.VISUAL.NUMBER_SYMBOLS[0]}")
-        if A.A_P.DB.backup(self.input.answer if answer else dump_name):
+            f"Изменить имя файла дампа базы данных", False, b("Отправьте имя"), f"Использовать имя: {b(name)} - отправьте {A.CT.VISUAL.NUMBER_SYMBOLS[0]}")
+        if A.A_P.DB.backup(self.input.answer if answer else name):
             self.write_line(i(f"{self.user_given_name}, ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе {b('Backup Console')}"))
 
     def robocopy_job_run_handler(self) -> None:
         forced: bool = self.is_forced
         source_job_name: str | None = self.first_arg()
         if not A.D_C.empty(source_job_name):
             source_job_name = source_job_name.lower()
```

### Comparing `pih-mio-1.48028/MobileHelperService/service.py` & `pih-mio-1.48029/MobileHelperService/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48028/MobileHelperService/service_api.py` & `pih-mio-1.48029/MobileHelperService/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48028/MobileHelperService/tools.py` & `pih-mio-1.48029/MobileHelperService/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48028/pih-mio_setup.py` & `pih-mio-1.48029/pih-mio_setup.py`

 * *Files identical despite different names*

