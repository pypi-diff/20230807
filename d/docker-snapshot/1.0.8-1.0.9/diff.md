# Comparing `tmp/docker-snapshot-1.0.8.tar.gz` & `tmp/docker_snapshot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-snapshot-1.0.8.tar", max compression
+gzip compressed data, was "docker_snapshot-1.0.9.tar", max compression
```

## Comparing `docker-snapshot-1.0.8.tar` & `docker_snapshot-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1975 2021-08-16 11:55:00.475434 docker-snapshot-1.0.8/README.md
--rw-r--r--   0        0        0     4144 2022-07-12 14:44:58.991802 docker-snapshot-1.0.8/docker_snapshot/__init__.py
--rw-r--r--   0        0        0     5083 2022-07-13 09:27:33.229355 docker-snapshot-1.0.8/docker_snapshot/container.py
--rw-r--r--   0        0        0        0 2021-08-16 11:55:00.475434 docker-snapshot-1.0.8/docker_snapshot/images/__init__.py
--rw-r--r--   0        0        0       95 2021-08-16 11:55:00.475434 docker-snapshot-1.0.8/docker_snapshot/images/rsync
--rw-r--r--   0        0        0     1102 2021-08-18 15:04:23.785545 docker-snapshot-1.0.8/docker_snapshot/settings.py
--rw-r--r--   0        0        0     3437 2022-07-13 09:30:26.608365 docker-snapshot-1.0.8/docker_snapshot/snapshot.py
--rw-r--r--   0        0        0      263 2021-08-16 11:55:00.475434 docker-snapshot-1.0.8/docker_snapshot/utils.py
--rw-r--r--   0        0        0      658 2022-07-13 09:31:52.564520 docker-snapshot-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3060 2022-07-13 09:32:33.906953 docker-snapshot-1.0.8/setup.py
--rw-r--r--   0        0        0     2771 2022-07-13 09:32:33.908197 docker-snapshot-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1976 2023-02-09 08:19:42.093056 docker_snapshot-1.0.9/README.md
+-rw-r--r--   0        0        0     4144 2022-07-12 14:44:58.991802 docker_snapshot-1.0.9/docker_snapshot/__init__.py
+-rw-r--r--   0        0        0     5083 2022-07-13 09:27:33.229355 docker_snapshot-1.0.9/docker_snapshot/container.py
+-rw-r--r--   0        0        0        0 2021-08-16 11:55:00.475434 docker_snapshot-1.0.9/docker_snapshot/images/__init__.py
+-rw-r--r--   0        0        0       95 2021-08-16 11:55:00.475434 docker_snapshot-1.0.9/docker_snapshot/images/rsync
+-rw-r--r--   0        0        0     1102 2021-08-18 15:04:23.785545 docker_snapshot-1.0.9/docker_snapshot/settings.py
+-rw-r--r--   0        0        0     3437 2022-07-13 09:30:26.608365 docker_snapshot-1.0.9/docker_snapshot/snapshot.py
+-rw-r--r--   0        0        0      263 2021-08-16 11:55:00.475434 docker_snapshot-1.0.9/docker_snapshot/utils.py
+-rw-r--r--   0        0        0      658 2023-08-07 13:37:37.532006 docker_snapshot-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 docker_snapshot-1.0.9/PKG-INFO
```

### Comparing `docker-snapshot-1.0.8/README.md` & `docker_snapshot-1.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Personally I use it to quickly save the state of my development database, try out something that mutates the state - a data migration or user interaction - and return to the initial state. Often repeatedly, because trial and error is essential. You can probably use it on any sort of stored data, probably. 
 
 Note: This repository is still a work in progress.
 
 ## Installing
 ```bash
-# Note: excutable will be called `ds`
+# Note: executable will be called `ds`
 pip install docker-snapshot
 ```
 
 Shell completion:
 ```bash
 # For Bash, add this to ~/.bashrc:
 eval "$(_DS_COMPLETE=source_bash ds)"
```

### Comparing `docker-snapshot-1.0.8/docker_snapshot/__init__.py` & `docker_snapshot-1.0.9/docker_snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-snapshot-1.0.8/docker_snapshot/container.py` & `docker_snapshot-1.0.9/docker_snapshot/container.py`

 * *Files identical despite different names*

### Comparing `docker-snapshot-1.0.8/docker_snapshot/settings.py` & `docker_snapshot-1.0.9/docker_snapshot/settings.py`

 * *Files identical despite different names*

### Comparing `docker-snapshot-1.0.8/docker_snapshot/snapshot.py` & `docker_snapshot-1.0.9/docker_snapshot/snapshot.py`

 * *Files identical despite different names*

### Comparing `docker-snapshot-1.0.8/pyproject.toml` & `docker_snapshot-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "docker-snapshot"
 homepage = "https://github.com/occamz/ds"
 documentation = "https://github.com/occamz/ds"
-version = "1.0.8"
+version = "1.0.9"
 description = "`ds` is a development utility for managing snapshots inside a docker container."
 authors = ["occamz"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-click = "^8.0.1"
+click = "^8.1.6"
 click-aliases = "^1.0.1"
-colorama = "^0.4.4"
+colorama = "^0.4.6"
 hruid = "^0.0.3"
-rich = "^10.7.0"
-PyYAML = "^5.4.1"
-docker = "^5.0.0"
+rich = "^13.5.2"
+PyYAML = "^6.0.1"
+docker = "^6.1.3"
 six = "^1.16.0"
 
 [tool.poetry.scripts]
 ds = "docker_snapshot:execute_cli"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `docker-snapshot-1.0.8/setup.py` & `docker_snapshot-1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,113 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: docker-snapshot
+Version: 1.0.9
+Summary: `ds` is a development utility for managing snapshots inside a docker container.
+Home-page: https://github.com/occamz/ds
+Author: occamz
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: click (>=8.1.6,<9.0.0)
+Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: docker (>=6.1.3,<7.0.0)
+Requires-Dist: hruid (>=0.0.3,<0.0.4)
+Requires-Dist: rich (>=13.5.2,<14.0.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
+Project-URL: Documentation, https://github.com/occamz/ds
+Description-Content-Type: text/markdown
+
+# ds - docker snapshot
+
+`ds` is a development utility for managing snapshots inside a docker container.
+
+Personally I use it to quickly save the state of my development database, try out something that mutates the state - a data migration or user interaction - and return to the initial state. Often repeatedly, because trial and error is essential. You can probably use it on any sort of stored data, probably. 
+
+Note: This repository is still a work in progress.
+
+## Installing
+```bash
+# Note: executable will be called `ds`
+pip install docker-snapshot
+```
+
+Shell completion:
+```bash
+# For Bash, add this to ~/.bashrc:
+eval "$(_DS_COMPLETE=source_bash ds)"
+
+# For Zsh, add this to ~/.zshrc:
+eval "$(_DS_COMPLETE=source_zsh ds)"
+```
+
+
+## Usage
+
+Create a snapshot
+```bash
+ds create name-goes-here
+# or auto-generate a name
+ds create 
+```
+
+Restore a snapshot
+```bash
+ds restore name-goes-here
+# or restore the latest snapshot
+ds restore
+```
+
+List snapshots
+```bash
+ds ls
+```
+
+Delete snapshots
+```bash
+ds delete name-goes-here
+```
+
+## Example project setup
+In this example we use `ds` to create and restore database snapshots in our development environment. The projects `docker-compose.yml` file could look something like this:
+```
+version: "3.8"
+services:
+  db:
+    container_name: db
+    restart: always
+    image: postgres:13
+    env_file: .env
+    ports:
+      - 5432:5432
+    volumes:
+      - db-volume:/var/lib/postgresql/data
+  ...
+```
+
+1) Browse to your project root
+```bash
+cd code/your-awesome-project
+```
+
+2) Create `ds.yaml` template file
+```bash
+ds init
+```
+
+3) Edit your `ds.yaml`
+```yaml
+# The target container
+container_name: "db"
+
+# The directory inside said container that you want to snapshot
+directory: "/var/lib/postgresql/data"
+
+# Identifier to separate projects, this allows you:
+# - To have multiple projects with the same container name
+# - To have multiple setups (ie. docker-compose / kind) for the same project
+namespace: "your-awesome-project"
+```
 
-packages = \
-['docker_snapshot', 'docker_snapshot.images']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=5.4.1,<6.0.0',
- 'click-aliases>=1.0.1,<2.0.0',
- 'click>=8.0.1,<9.0.0',
- 'colorama>=0.4.4,<0.5.0',
- 'docker>=5.0.0,<6.0.0',
- 'hruid>=0.0.3,<0.0.4',
- 'rich>=10.7.0,<11.0.0',
- 'six>=1.16.0,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['ds = docker_snapshot:execute_cli']}
-
-setup_kwargs = {
-    'name': 'docker-snapshot',
-    'version': '1.0.8',
-    'description': '`ds` is a development utility for managing snapshots inside a docker container.',
-    'long_description': '# ds - docker snapshot\n\n`ds` is a development utility for managing snapshots inside a docker container.\n\nPersonally I use it to quickly save the state of my development database, try out something that mutates the state - a data migration or user interaction - and return to the initial state. Often repeatedly, because trial and error is essential. You can probably use it on any sort of stored data, probably. \n\nNote: This repository is still a work in progress.\n\n## Installing\n```bash\n# Note: excutable will be called `ds`\npip install docker-snapshot\n```\n\nShell completion:\n```bash\n# For Bash, add this to ~/.bashrc:\neval "$(_DS_COMPLETE=source_bash ds)"\n\n# For Zsh, add this to ~/.zshrc:\neval "$(_DS_COMPLETE=source_zsh ds)"\n```\n\n\n## Usage\n\nCreate a snapshot\n```bash\nds create name-goes-here\n# or auto-generate a name\nds create \n```\n\nRestore a snapshot\n```bash\nds restore name-goes-here\n# or restore the latest snapshot\nds restore\n```\n\nList snapshots\n```bash\nds ls\n```\n\nDelete snapshots\n```bash\nds delete name-goes-here\n```\n\n## Example project setup\nIn this example we use `ds` to create and restore database snapshots in our development environment. The projects `docker-compose.yml` file could look something like this:\n```\nversion: "3.8"\nservices:\n  db:\n    container_name: db\n    restart: always\n    image: postgres:13\n    env_file: .env\n    ports:\n      - 5432:5432\n    volumes:\n      - db-volume:/var/lib/postgresql/data\n  ...\n```\n\n1) Browse to your project root\n```bash\ncd code/your-awesome-project\n```\n\n2) Create `ds.yaml` template file\n```bash\nds init\n```\n\n3) Edit your `ds.yaml`\n```yaml\n# The target container\ncontainer_name: "db"\n\n# The directory inside said container that you want to snapshot\ndirectory: "/var/lib/postgresql/data"\n\n# Identifier to separate projects, this allows you:\n# - To have multiple projects with the same container name\n# - To have multiple setups (ie. docker-compose / kind) for the same project\nnamespace: "your-awesome-project"\n```\n',
-    'author': 'occamz',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/occamz/ds',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

