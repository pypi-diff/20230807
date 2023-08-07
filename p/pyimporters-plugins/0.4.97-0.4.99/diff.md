# Comparing `tmp/pyimporters-plugins-0.4.97.tar.gz` & `tmp/pyimporters-plugins-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimporters-plugins-0.4.97.tar", last modified: Mon Jul 12 08:11:45 2021, max compression
+gzip compressed data, was "pyimporters-plugins-0.4.99.tar", last modified: Sat Aug 14 18:44:25 2021, max compression
```

## Comparing `pyimporters-plugins-0.4.97.tar` & `pyimporters-plugins-0.4.99.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       97 2021-04-14 08:56:13.318634 pyimporters-plugins-0.4.97/.dockerignore
--rw-r--r--   0        0        0      147 2021-04-14 13:03:38.626280 pyimporters-plugins-0.4.97/.gitignore
--rw-r--r--   0        0        0      448 2021-04-14 08:56:13.318634 pyimporters-plugins-0.4.97/Dockerfile
--rw-r--r--   0        0        0     7516 2021-07-12 07:39:31.267234 pyimporters-plugins-0.4.97/Jenkinsfile
--rw-r--r--   0        0        0      380 2021-04-14 08:56:13.318634 pyimporters-plugins-0.4.97/README.md
--rw-r--r--   0        0        0       61 2021-07-12 08:11:44.184393 pyimporters-plugins-0.4.97/pyimporters_plugins/__init__.py
--rw-r--r--   0        0        0     3606 2021-04-29 13:29:12.406576 pyimporters-plugins-0.4.97/pyimporters_plugins/base.py
--rw-r--r--   0        0        0     1849 2021-04-14 12:21:25.091583 pyimporters-plugins-0.4.97/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-14 09:43:53.296712 pyimporters-plugins-0.4.97/tests/__init__.py
--rwxr-xr-x   0        0        0     3112 2021-04-19 10:53:59.429602 pyimporters-plugins-0.4.97/tests/data/small.xml.gz
--rwxr-xr-x   0        0        0     3280 2021-04-19 10:53:59.430603 pyimporters-plugins-0.4.97/tests/data/small.zip
--rwxr-xr-x   0        0        0     3280 2021-04-19 10:53:59.430603 pyimporters-plugins-0.4.97/tests/data/small_zip
--rw-r--r--   0        0        0     1106 2021-04-19 11:03:09.741693 pyimporters-plugins-0.4.97/tests/test_base.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pyimporters-plugins-0.4.97/setup.py
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 pyimporters-plugins-0.4.97/PKG-INFO
+-rw-r--r--   0        0        0       97 2021-04-14 08:56:13.318634 pyimporters-plugins-0.4.99/.dockerignore
+-rw-r--r--   0        0        0      147 2021-04-14 13:03:38.626280 pyimporters-plugins-0.4.99/.gitignore
+-rw-r--r--   0        0        0      448 2021-04-14 08:56:13.318634 pyimporters-plugins-0.4.99/Dockerfile
+-rw-r--r--   0        0        0     7047 2021-08-14 18:43:57.428672 pyimporters-plugins-0.4.99/Jenkinsfile
+-rw-r--r--   0        0        0      380 2021-04-14 08:56:13.318634 pyimporters-plugins-0.4.99/README.md
+-rw-r--r--   0        0        0       61 2021-08-14 18:44:24.359390 pyimporters-plugins-0.4.99/pyimporters_plugins/__init__.py
+-rw-r--r--   0        0        0     3606 2021-04-29 13:29:12.406576 pyimporters-plugins-0.4.99/pyimporters_plugins/base.py
+-rw-r--r--   0        0        0     1849 2021-04-14 12:21:25.091583 pyimporters-plugins-0.4.99/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-04-14 09:43:53.296712 pyimporters-plugins-0.4.99/tests/__init__.py
+-rwxr-xr-x   0        0        0     3112 2021-04-19 10:53:59.429602 pyimporters-plugins-0.4.99/tests/data/small.xml.gz
+-rwxr-xr-x   0        0        0     3280 2021-04-19 10:53:59.430603 pyimporters-plugins-0.4.99/tests/data/small.zip
+-rwxr-xr-x   0        0        0     3280 2021-04-19 10:53:59.430603 pyimporters-plugins-0.4.99/tests/data/small_zip
+-rw-r--r--   0        0        0     1106 2021-04-19 11:03:09.741693 pyimporters-plugins-0.4.99/tests/test_base.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pyimporters-plugins-0.4.99/setup.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 pyimporters-plugins-0.4.99/PKG-INFO
```

### Comparing `pyimporters-plugins-0.4.97/Jenkinsfile` & `pyimporters-plugins-0.4.99/Jenkinsfile`

 * *Files 19% similar despite different names*

```diff
@@ -64,28 +64,20 @@
             environment name: "LAST_COMMIT_IS_TEAM", value: "1"
           }
           steps {
             script {
               println("attempt to publish ${env.JOB_NAME} with version: ${MAJOR_VERSION}.${MINOR_VERSION}.${env.BUILD_ID}")
 
               // push updates of file __init__.py
-              sh "echo '\"\"\"Sherpa knowledge import plugins\"\"\"' > pyimporters_plugins/__init__.py"
-              sh "echo '__version__ = \"${MAJOR_VERSION}.${MINOR_VERSION}.${env.BUILD_ID}\"' >> pyimporters_plugins/__init__.py"
-              sh('''
-                git config --remove-section credential >/dev/null 2>&1 || true
-                git config --remove-section user >/dev/null 2>&1 || true
-                git config --global push.default matching
-                git config user.name 'Guillaume Karcher'
-                git config user.email 'guillaume.karcher@kairntech.com'
-                git commit pyimporters_plugins/__init__.py -m "[Jenkins CI] Commit on version files" || echo "No changes to commit"
-                git config --local credential.helper "!f() { echo username=\\$GIT_AUTH_USR; echo password=\\$GIT_AUTH_PSW; }; f"
-                git push
-                git config --remove-section credential
-                git config --remove-section user
-              ''')
+              withCredentials([gitUsernamePassword(credentialsId: 'bitbucket-user', gitToolName: 'git-tool')]) {
+                sh "echo '\"\"\"Sherpa knowledge import plugins\"\"\"' > pyimporters_plugins/__init__.py"
+                sh "echo '__version__ = \"${MAJOR_VERSION}.${MINOR_VERSION}.${env.BUILD_ID}\"' >> pyimporters_plugins/__init__.py"
+                sh 'git commit pyimporters_plugins/__init__.py -m "[Jenkins CI] Commit on version files" || echo "No changes to commit"'
+                sh 'git push'
+              }
             }
           }
         }
 
       }
     }
```

### Comparing `pyimporters-plugins-0.4.97/pyimporters_plugins/base.py` & `pyimporters-plugins-0.4.99/pyimporters_plugins/base.py`

 * *Files identical despite different names*

### Comparing `pyimporters-plugins-0.4.97/pyproject.toml` & `pyimporters-plugins-0.4.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyimporters-plugins-0.4.97/tests/data/small.xml.gz` & `pyimporters-plugins-0.4.99/tests/data/small.xml.gz`

 * *Files identical despite different names*

### Comparing `pyimporters-plugins-0.4.97/tests/data/small.zip` & `pyimporters-plugins-0.4.99/tests/data/small.zip`

 * *Files identical despite different names*

### Comparing `pyimporters-plugins-0.4.97/tests/data/small_zip` & `pyimporters-plugins-0.4.99/tests/data/small_zip`

 * *Files identical despite different names*

### Comparing `pyimporters-plugins-0.4.97/tests/test_base.py` & `pyimporters-plugins-0.4.99/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pyimporters-plugins-0.4.97/setup.py` & `pyimporters-plugins-0.4.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pydantic==1.7.3', 'fastapi==0.61.2', 'pytest', 'progress']
 
 setup(name='pyimporters-plugins',
-      version='0.4.97',
+      version='0.4.99',
       description='Sherpa knowledge import plugins',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

