# Comparing `tmp/datamaker-backup-0.1.3.tar.gz` & `tmp/datamaker-backup-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaker-backup-0.1.3.tar", last modified: Tue Jul 25 14:48:20 2023, max compression
+gzip compressed data, was "datamaker-backup-0.2.0.tar", last modified: Mon Aug  7 14:45:34 2023, max compression
```

## Comparing `datamaker-backup-0.1.3.tar` & `datamaker-backup-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-07-25 12:40:40.000000 datamaker-backup-0.1.3/LICENSE
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     2634 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1905 2023-07-25 14:40:09.000000 datamaker-backup-0.1.3/README.md
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/datamaker_backup/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       39 2023-07-25 12:40:40.000000 datamaker-backup-0.1.3/datamaker_backup/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     5094 2023-07-25 12:40:40.000000 datamaker-backup-0.1.3/datamaker_backup/storage.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1172 2023-07-25 14:40:09.000000 datamaker-backup-0.1.3/datamaker_backup/utils.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/datamaker_backup.egg-info/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     2634 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      324 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/SOURCES.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/dependency_links.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       52 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/requires.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       17 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/top_level.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-07-25 14:40:09.000000 datamaker-backup-0.1.3/pyproject.toml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      839 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/setup.cfg
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-08-07 14:45:34.236909 datamaker-backup-0.2.0/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-07-25 12:40:40.000000 datamaker-backup-0.2.0/LICENSE
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3611 2023-08-07 14:45:34.236909 datamaker-backup-0.2.0/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     2882 2023-08-07 14:45:26.000000 datamaker-backup-0.2.0/README.md
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-08-07 14:45:34.236909 datamaker-backup-0.2.0/datamaker_backup/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       53 2023-08-07 14:45:26.000000 datamaker-backup-0.2.0/datamaker_backup/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1663 2023-08-07 14:45:26.000000 datamaker-backup-0.2.0/datamaker_backup/connector.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     5210 2023-08-07 14:45:26.000000 datamaker-backup-0.2.0/datamaker_backup/storage.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1274 2023-08-07 14:45:26.000000 datamaker-backup-0.2.0/datamaker_backup/utils.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-08-07 14:45:34.236909 datamaker-backup-0.2.0/datamaker_backup.egg-info/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3611 2023-08-07 14:45:34.000000 datamaker-backup-0.2.0/datamaker_backup.egg-info/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      354 2023-08-07 14:45:34.000000 datamaker-backup-0.2.0/datamaker_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-08-07 14:45:34.000000 datamaker-backup-0.2.0/datamaker_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       52 2023-08-07 14:45:34.000000 datamaker-backup-0.2.0/datamaker_backup.egg-info/requires.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       17 2023-08-07 14:45:34.000000 datamaker-backup-0.2.0/datamaker_backup.egg-info/top_level.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      285 2023-08-07 14:45:26.000000 datamaker-backup-0.2.0/pyproject.toml
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      839 2023-08-07 14:45:34.236909 datamaker-backup-0.2.0/setup.cfg
```

### Comparing `datamaker-backup-0.1.3/LICENSE` & `datamaker-backup-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaker-backup-0.1.3/PKG-INFO` & `datamaker-backup-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-backup
-Version: 0.1.3
+Version: 0.2.0
 Summary: datamaker backup
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,23 +16,32 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Installation
 
+```shell
+pip install datamaker-backup
+```
+
 ## .env
 `.env.dist`에 아래 내용 추가
 
 ```dotenv
+# ENVIRONMENT
+...
+DEPLOYMENT_TARGET=development|test|production
+
 # BACKUP
 ENABLE_RESTORE=true|false
 ENABLE_BACKUP=true|false
 RESTORE_DATA_ONLY=true|false
 RESTORE_OPTIONS=do-not-set-unless-you-know-what-you-are-doing
+DBBACKUP_CLEANUP_KEEP=10
 ```
 
 ## settings.py
 
 `settings.py`에 아래 내용 추가
 
 ```python
@@ -51,14 +60,38 @@
 # datamaker-backup
 # https://github.com/datamaker-kr/datamaker-backup
 
 BACKUP_CONFIG = get_backup_settings('<repository-name>', env)
 vars().update(BACKUP_CONFIG)
 ```
 
+## postgresql
+
+PostgreSQL을 사용하는 프로젝트는 `pg_dump`, `pg_restore로` 백업 및 복원이 이루어지기 때문에 postgresql client 설치를 진행해야 합니다.
+
+### prepare to install latest postgresql
+
+```shell
+sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'
+```
+
+```shell
+wget -qO- https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo tee /etc/apt/trusted.gpg.d/pgdg.asc &>/dev/null
+```
+
+```shell
+sudo apt update
+```
+
+### install postgresql client
+
+```shell
+sudo apt install postgresql-client
+```
+
 # Usage
 
 ## 백업
 
 ### database
 
 ```shell
@@ -96,14 +129,19 @@
 python manage.py mediarestore -i <backup_id>
 ```
 
 # Configuration
 
 `.env`에서 아래 설정을 필요에 따라 적용.
 
+### DEPLOYMENT_TARGET
+배포 환경 이름. 주로 `development` | `test` | `production`로 설정.
+
+Required: `true`
+
 ### ENABLE_RESTORE
 `true` | `false`
 
 `dbrestore`, `mediarestore` 사용 가능 여부. 주로 production 환경에서는 비활성화.
 
 Default: `false`
 
@@ -128,7 +166,12 @@
 
 Example:
 `clean,create`
 
 Default:
 - `RESTORE_DATA_ONLY`가 `true`일 때에는 `data-only,disable-triggers,exit-on-error`
 - `RESTORE_DATA_ONLY`가 `false`일 때에는 `clean,create,if-exists,exit-on-error`
+
+### DBBACKUP_CLEANUP_KEEP
+dbbackup시 지정된 숫자를 초과한 나머지 백업은 삭제됨.
+
+Default: `30`
```

### Comparing `datamaker-backup-0.1.3/datamaker_backup/storage.py` & `datamaker-backup-0.2.0/datamaker_backup/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,17 @@
         offset = 0
         for chunk in content.chunks(self.chunk_size):
             hash_md5.update(chunk)
             response = requests.put(
                 url,
                 data={'filename': name},
                 files={'file': chunk},
-                headers={'Content-Range': f'bytes {offset}-{offset + len(chunk) - 1}/{size}'},
+                headers={
+                    'Content-Range': f'bytes {offset}-{offset + len(chunk) - 1}/{size}'
+                },
             )
             response.raise_for_status()
             data = response.json()
             offset = data['offset']
             url = data['url']
 
         response = requests.post(url, data={'md5': hash_md5.hexdigest()})
@@ -123,27 +125,34 @@
         data = response.json()
         return [], [item['name'] for item in data]
 
     def delete(self, name):
         assert self.enable_backup, 'Backup is disabled'
         backup_id = name.split('_')[0]
         url = f'{self.base_url}/api/backups/{backup_id}/'
-        response = requests.delete(url, params={'repository': self.repository, 'environment': self.environment})
+        response = requests.delete(
+            url, params={'repository': self.repository, 'environment': self.environment}
+        )
         response.raise_for_status()
 
     @staticmethod
     def get_schema():
         loader = MigrationLoader(None, ignore_no_migrations=True)
-        sources = [inspect.getsource(migration.__class__) for migration in loader.disk_migrations.values()]
+        sources = [
+            inspect.getsource(migration.__class__)
+            for migration in loader.disk_migrations.values()
+        ]
         sources.sort()
         return hashlib.md5(''.join(sources).encode('utf-8')).hexdigest()
 
     @staticmethod
     def get_content_type(name):
-        name = name.split('.')[0].removesuffix('-'.join([dbbackup_settings.HOSTNAME, filename_to_datestring(name)]))
+        name = name.split('.')[0].removesuffix(
+            '-'.join([dbbackup_settings.HOSTNAME, filename_to_datestring(name)])
+        )
 
         if name:
             name = name.removesuffix('-')
             if name in settings.DATABASES:
                 return 'database', name
             else:
                 raise ValueError('Unknown backup category')
```

### Comparing `datamaker-backup-0.1.3/datamaker_backup.egg-info/PKG-INFO` & `datamaker-backup-0.2.0/datamaker_backup.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-backup
-Version: 0.1.3
+Version: 0.2.0
 Summary: datamaker backup
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,23 +16,32 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Installation
 
+```shell
+pip install datamaker-backup
+```
+
 ## .env
 `.env.dist`에 아래 내용 추가
 
 ```dotenv
+# ENVIRONMENT
+...
+DEPLOYMENT_TARGET=development|test|production
+
 # BACKUP
 ENABLE_RESTORE=true|false
 ENABLE_BACKUP=true|false
 RESTORE_DATA_ONLY=true|false
 RESTORE_OPTIONS=do-not-set-unless-you-know-what-you-are-doing
+DBBACKUP_CLEANUP_KEEP=10
 ```
 
 ## settings.py
 
 `settings.py`에 아래 내용 추가
 
 ```python
@@ -51,14 +60,38 @@
 # datamaker-backup
 # https://github.com/datamaker-kr/datamaker-backup
 
 BACKUP_CONFIG = get_backup_settings('<repository-name>', env)
 vars().update(BACKUP_CONFIG)
 ```
 
+## postgresql
+
+PostgreSQL을 사용하는 프로젝트는 `pg_dump`, `pg_restore로` 백업 및 복원이 이루어지기 때문에 postgresql client 설치를 진행해야 합니다.
+
+### prepare to install latest postgresql
+
+```shell
+sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'
+```
+
+```shell
+wget -qO- https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo tee /etc/apt/trusted.gpg.d/pgdg.asc &>/dev/null
+```
+
+```shell
+sudo apt update
+```
+
+### install postgresql client
+
+```shell
+sudo apt install postgresql-client
+```
+
 # Usage
 
 ## 백업
 
 ### database
 
 ```shell
@@ -96,14 +129,19 @@
 python manage.py mediarestore -i <backup_id>
 ```
 
 # Configuration
 
 `.env`에서 아래 설정을 필요에 따라 적용.
 
+### DEPLOYMENT_TARGET
+배포 환경 이름. 주로 `development` | `test` | `production`로 설정.
+
+Required: `true`
+
 ### ENABLE_RESTORE
 `true` | `false`
 
 `dbrestore`, `mediarestore` 사용 가능 여부. 주로 production 환경에서는 비활성화.
 
 Default: `false`
 
@@ -128,7 +166,12 @@
 
 Example:
 `clean,create`
 
 Default:
 - `RESTORE_DATA_ONLY`가 `true`일 때에는 `data-only,disable-triggers,exit-on-error`
 - `RESTORE_DATA_ONLY`가 `false`일 때에는 `clean,create,if-exists,exit-on-error`
+
+### DBBACKUP_CLEANUP_KEEP
+dbbackup시 지정된 숫자를 초과한 나머지 백업은 삭제됨.
+
+Default: `30`
```

### Comparing `datamaker-backup-0.1.3/setup.cfg` & `datamaker-backup-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = datamaker-backup
-version = 0.1.3
+version = 0.2.0
 description = datamaker backup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.datamaker.io
 author = datamaker
 author_email = developer@datamaker.io
 license = MIT
```

