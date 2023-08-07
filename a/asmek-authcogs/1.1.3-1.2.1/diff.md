# Comparing `tmp/asmek_authcogs-1.1.3.tar.gz` & `tmp/asmek_authcogs-1.2.1.tar.gz`

## Comparing `asmek_authcogs-1.1.3.tar` & `asmek_authcogs-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/app_settings.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/apps.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/auth_hooks.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/Images/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/Images/eve-o-4.png
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/Images/smt_bomb_icon-1.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/__init__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/about.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/auth.py
--rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/links.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/recruit.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/siege.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/0001_initial.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/0002_alter_link_name.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/0003_alter_general_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/LICENSE
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/app_settings.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/apps.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/auth_hooks.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/Images/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/Images/eve-o-4.png
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/Images/smt_bomb_icon-1.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/cogs/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/cogs/about.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/cogs/auth.py
+-rw-r--r--   0        0        0    10715 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/cogs/hr.py
+-rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/cogs/links.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/cogs/siege.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/migrations/0001_initial.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/migrations/0002_alter_link_name.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/migrations/0003_alter_general_options.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/migrations/0004_authcogs_delete_general.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/asmek_authcogs/migrations/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 asmek_authcogs-1.2.1/PKG-INFO
```

### Comparing `asmek_authcogs-1.1.3/CHANGELOG.md` & `asmek_authcogs-1.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/.github/workflows/publish.yml` & `asmek_authcogs-1.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/models.py` & `asmek_authcogs-1.2.1/asmek_authcogs/models.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/Images/eve-o-4.png` & `asmek_authcogs-1.2.1/asmek_authcogs/Images/eve-o-4.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/Images/smt_bomb_icon-1.png` & `asmek_authcogs-1.2.1/asmek_authcogs/Images/smt_bomb_icon-1.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/cogs/about.py` & `asmek_authcogs-1.2.1/asmek_authcogs/cogs/about.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/cogs/auth.py` & `asmek_authcogs-1.2.1/asmek_authcogs/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/cogs/links.py` & `asmek_authcogs-1.2.1/asmek_authcogs/cogs/links.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/cogs/siege.py` & `asmek_authcogs-1.2.1/asmek_authcogs/cogs/siege.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/asmek_authcogs/migrations/0001_initial.py` & `asmek_authcogs-1.2.1/asmek_authcogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/.gitignore` & `asmek_authcogs-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/LICENSE` & `asmek_authcogs-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/README.md` & `asmek_authcogs-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/pyproject.toml` & `asmek_authcogs-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.3/PKG-INFO` & `asmek_authcogs-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmek-authcogs
-Version: 1.1.3
+Version: 1.2.1
 Summary: ASMEK customized cogs for aa-discordbot
 Project-URL: Documentation, https://github.com/AstrumMechanica/asmek-authcogs#readme
 Project-URL: Issues, https://github.com/AstrumMechanica/asmek-authcogs/issues
 Project-URL: Source, https://github.com/AstrumMechanica/asmek-authcogs
 Author-email: AstrumMechanica <astrummechanica@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
```

