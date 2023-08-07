# Comparing `tmp/red-postgres-0.1.3.tar.gz` & `tmp/red-postgres-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red-postgres-0.1.3.tar", last modified: Fri Jul 28 20:00:54 2023, max compression
+gzip compressed data, was "red-postgres-0.1.5.tar", last modified: Mon Aug  7 02:41:04 2023, max compression
```

## Comparing `red-postgres-0.1.3.tar` & `red-postgres-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 20:00:54.707491 red-postgres-0.1.3/
--rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6287 2023-07-28 20:00:54.707491 red-postgres-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5750 2023-06-02 15:00:17.000000 red-postgres-0.1.3/README.md
--rw-rw-rw-   0        0        0     1583 2023-07-28 20:00:29.000000 red-postgres-0.1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-28 20:00:54.686491 red-postgres-0.1.3/red_postgres/
--rw-rw-rw-   0        0        0      235 2023-07-28 19:59:22.000000 red-postgres-0.1.3/red_postgres/__init__.py
--rw-rw-rw-   0        0        0     5303 2023-07-17 00:55:17.000000 red-postgres-0.1.3/red_postgres/engine.py
-drwxrwxrwx   0        0        0        0 2023-07-28 20:00:54.705490 red-postgres-0.1.3/red_postgres.egg-info/
--rw-rw-rw-   0        0        0     6287 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 20:00:54.708490 red-postgres-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 02:41:04.895687 red-postgres-0.1.5/
+-rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6510 2023-08-07 02:41:04.895687 red-postgres-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5973 2023-08-07 00:50:02.000000 red-postgres-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1583 2023-08-07 02:40:06.000000 red-postgres-0.1.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-07 02:41:04.875688 red-postgres-0.1.5/red_postgres/
+-rw-rw-rw-   0        0        0      266 2023-08-07 02:40:17.000000 red-postgres-0.1.5/red_postgres/__init__.py
+-rw-rw-rw-   0        0        0     7388 2023-08-07 02:40:17.000000 red-postgres-0.1.5/red_postgres/engine.py
+-rw-rw-rw-   0        0        0       60 2023-08-07 01:53:16.000000 red-postgres-0.1.5/red_postgres/errors.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:41:04.893687 red-postgres-0.1.5/red_postgres.egg-info/
+-rw-rw-rw-   0        0        0     6510 2023-08-07 02:41:04.000000 red-postgres-0.1.5/red_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-08-07 02:41:04.000000 red-postgres-0.1.5/red_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:41:04.000000 red-postgres-0.1.5/red_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-07 02:41:04.000000 red-postgres-0.1.5/red_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 02:41:04.895687 red-postgres-0.1.5/setup.cfg
```

### Comparing `red-postgres-0.1.3/LICENSE` & `red-postgres-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `red-postgres-0.1.3/PKG-INFO` & `red-postgres-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.1.3
+Version: 0.1.5
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # red-postgres
 
 Piccolo Postgres integration for Red-DiscordBot, although it could be used with any dpy bot as an easy wrapper for making postgres with cogs more modular.
 
+![Postgres 15](https://img.shields.io/badge/postgres%2015-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
+![Red-DiscordBot](https://img.shields.io/badge/Red%20DiscordBot-V3.5-red?style=for-the-badge)
+
 ![Py](https://img.shields.io/badge/python-v3.11-yellow?style=for-the-badge)
 ![black](https://img.shields.io/badge/style-black-000000?style=for-the-badge&?link=https://github.com/psf/black)
 ![license](https://img.shields.io/github/license/Vertyco/red-postgres?style=for-the-badge)
 
 ![Forks](https://img.shields.io/github/forks/Vertyco/red-postgres?style=for-the-badge&color=9cf)
 ![Stars](https://img.shields.io/github/stars/Vertyco/red-postgres?style=for-the-badge&color=yellow)
 ![Lines of code](https://img.shields.io/tokei/lines/github/Vertyco/red-postgres?color=ff69b4&label=Lines&style=for-the-badge)
```

### Comparing `red-postgres-0.1.3/README.md` & `red-postgres-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # red-postgres
 
 Piccolo Postgres integration for Red-DiscordBot, although it could be used with any dpy bot as an easy wrapper for making postgres with cogs more modular.
 
+![Postgres 15](https://img.shields.io/badge/postgres%2015-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
+![Red-DiscordBot](https://img.shields.io/badge/Red%20DiscordBot-V3.5-red?style=for-the-badge)
+
 ![Py](https://img.shields.io/badge/python-v3.11-yellow?style=for-the-badge)
 ![black](https://img.shields.io/badge/style-black-000000?style=for-the-badge&?link=https://github.com/psf/black)
 ![license](https://img.shields.io/github/license/Vertyco/red-postgres?style=for-the-badge)
 
 ![Forks](https://img.shields.io/github/forks/Vertyco/red-postgres?style=for-the-badge&color=9cf)
 ![Stars](https://img.shields.io/github/stars/Vertyco/red-postgres?style=for-the-badge&color=yellow)
 ![Lines of code](https://img.shields.io/tokei/lines/github/Vertyco/red-postgres?color=ff69b4&label=Lines&style=for-the-badge)
```

### Comparing `red-postgres-0.1.3/pyproject.toml` & `red-postgres-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "discord.py>=2.2.3",
   "piccolo[postgres]>=0.113.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "red-postgres"
-version = "0.1.3"
+version = "0.1.5"
 authors = [{ name = "Vertyco" }]
 description = "Piccolo Postgres integration for Red"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
```

### Comparing `red-postgres-0.1.3/red_postgres/engine.py` & `red-postgres-0.1.5/red_postgres/engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,111 @@
 import asyncio
+import functools
 import inspect
 import logging
+import multiprocessing as mp
 import os
 import subprocess
 from pathlib import Path
 
 from discord.ext.commands import Cog
 from piccolo.engine.postgres import PostgresEngine
 from piccolo.table import Table, create_db_tables
 
+from .errors import ConnectionTimeoutError
+
 log = logging.getLogger("red.red-postgres.engine")
 
 
 async def create_database(cog: Cog, config: dict) -> bool:
-    """Create cog's database if it doesnt exist
+    """
+    Create cog's database if it doesnt exist.
 
     Args:
         cog (Cog): Cog instance
         config (dict): Postgres connection information
 
     Returns:
         bool: whether a new database was created
     """
-    engine = await asyncio.to_thread(_acquire_db_engine, config)
+    log.debug("Acquiring engine for db creation")
+    engine = await _acquire_db_engine(config)
+    log.debug("Starting connection pool")
     await engine.start_connection_pool()
 
     # Check if the database exists
     created = False
     database_name = _root(cog).name.lower()
     databases = await engine._run_in_pool("SELECT datname FROM pg_database;")
     if database_name not in [db["datname"] for db in databases]:
         # Create the database
-        log.info(f"First time running {database_name}! Creating new database!")
+        log.info(f"New cog detected, Creating database for {database_name}")
         await engine._run_in_pool(f"CREATE DATABASE {database_name};")
         created = True
 
     # Close old database connection
     await engine.close_connection_pool()
     return created
 
 
-async def create_tables(
+async def fetch_cog_engine(
     cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
 ) -> PostgresEngine:
-    """Connect to postgres, create database/tables and return engine
+    """
+    Connect to postgres, start pool, and return engine.
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
         max_size (int): maximum number of database connections, 20 by default
 
     Returns:
         PostgresEngine instance
     """
+    log.debug("Fetching engine")
     temp_config = config.copy()
     temp_config["database"] = _root(cog).name.lower()
-    engine = await asyncio.to_thread(_acquire_db_engine, temp_config)
+    engine = await _acquire_db_engine(temp_config)
+    log.debug("Starting connection pool")
     await engine.start_connection_pool(max_size=max_size)
-
+    log.debug("Assigning engines to tables")
     # Update table engines
     for table_class in tables:
         table_class._meta.db = engine
+    return engine
+
+
+async def create_tables(
+    cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
+) -> PostgresEngine:
+    """
+    Connect to postgres, create database/tables, start pool, and return engine.
+
+    Args:
+        cog (Cog): Cog instance
+        config (dict): database connection info
+        tables (list[type[Table]]): list of piccolo table subclasses
+        max_size (int): maximum number of database connections, 20 by default
+
+    Returns:
+        PostgresEngine instance
+    """
+    engine = await fetch_cog_engine(cog, config, tables, max_size)
+
+    log.debug("Creating tables if they don't exist")
+    try:
+        task = create_db_tables(*tables, if_not_exists=True)
+        log.debug("Waiting for tables to create")
+        await asyncio.wait_for(task, timeout=10)
+    except asyncio.TimeoutError:
+        log.info("Table creation took too long")
+    except Exception as e:
+        log.info("Failed to run create tables", exc_info=e)
 
-    # Create any tables that don't already exist
-    await create_db_tables(*tables, if_not_exists=True)
     return engine
 
 
 async def run_migrations(cog: Cog, config: dict) -> str:
     """
     Run any existing migrations programatically.
 
@@ -133,26 +170,52 @@
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
         max_size (int): maximum number of database connections, 20 by default
 
     Returns:
         PostgresEngine
     """
+    log.debug(f"Registering {cog.qualified_name}")
     # Create databse under root folder name
-    await create_database(cog, config)
-    # Run any migrations
+    created = await create_database(cog, config)
+    if created:
+        # Create any tables and fetch postgres engine
+        engine = await create_tables(cog, config, tables, max_size)
+    else:
+        # Just fetch the engine
+        engine = await fetch_cog_engine(cog, config, tables, max_size)
+
+    log.debug("Running migrations, if any")
     result = await run_migrations(cog, config)
-    log.info(result)
-    # Create any tables and fetch postgres engine
-    return await create_tables(cog, config, tables, max_size)
+    result = result.replace("👍", "✓")
+    log.info(f"Migration result\n{result}")
+
+    return engine
+
 
+def _acquire(config: dict) -> PostgresEngine:
+    PostgresEngine(config=config)
 
-def _acquire_db_engine(config: dict) -> PostgresEngine:
+
+async def _acquire_db_engine(config: dict) -> PostgresEngine:
     """This is ran in executor since it blocks if connection info is bad"""
-    return PostgresEngine(config=config)
+    pool = mp.Pool()
+    try:
+        process = pool.apply_async(_acquire, args=(config,))
+        task = functools.partial(process.get, timeout=10)
+        loop = asyncio.get_running_loop()
+        new_task = loop.run_in_executor(None, task)
+        await asyncio.wait_for(new_task, timeout=10)
+    except asyncio.TimeoutError:
+        raise ConnectionTimeoutError("Database took longer than 10 seconds to connect!")
+    finally:
+        pool.close()
+
+    engine = await asyncio.to_thread(PostgresEngine, config)
+    return engine
 
 
 def _get_env(config: dict) -> dict:
     """Create mock environment for subprocess"""
     env = os.environ.copy()
     env["PICCOLO_CONF"] = "db.piccolo_conf"
     env["POSTGRES_HOST"] = config.get("host")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `red-postgres-0.1.3/red_postgres.egg-info/PKG-INFO` & `red-postgres-0.1.5/red_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.1.3
+Version: 0.1.5
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # red-postgres
 
 Piccolo Postgres integration for Red-DiscordBot, although it could be used with any dpy bot as an easy wrapper for making postgres with cogs more modular.
 
+![Postgres 15](https://img.shields.io/badge/postgres%2015-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
+![Red-DiscordBot](https://img.shields.io/badge/Red%20DiscordBot-V3.5-red?style=for-the-badge)
+
 ![Py](https://img.shields.io/badge/python-v3.11-yellow?style=for-the-badge)
 ![black](https://img.shields.io/badge/style-black-000000?style=for-the-badge&?link=https://github.com/psf/black)
 ![license](https://img.shields.io/github/license/Vertyco/red-postgres?style=for-the-badge)
 
 ![Forks](https://img.shields.io/github/forks/Vertyco/red-postgres?style=for-the-badge&color=9cf)
 ![Stars](https://img.shields.io/github/stars/Vertyco/red-postgres?style=for-the-badge&color=yellow)
 ![Lines of code](https://img.shields.io/tokei/lines/github/Vertyco/red-postgres?color=ff69b4&label=Lines&style=for-the-badge)
```

