# Comparing `tmp/stackedup-0.0.8.tar.gz` & `tmp/stackedup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackedup-0.0.8.tar", last modified: Thu Mar 18 16:57:38 2021, max compression
+gzip compressed data, was "stackedup-0.0.9.tar", last modified: Wed Dec  7 19:22:57 2022, max compression
```

## Comparing `stackedup-0.0.8.tar` & `stackedup-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2021-03-18 16:57:38.686837 stackedup-0.0.8/
--rw-r--r--   0 axolx     (1000) axolx     (1000)     7752 2021-03-18 16:57:38.686837 stackedup-0.0.8/PKG-INFO
--rw-r--r--   0 axolx     (1000) axolx     (1000)     5931 2021-03-18 16:57:11.000000 stackedup-0.0.8/README.md
--rw-r--r--   0 axolx     (1000) axolx     (1000)       38 2021-03-18 16:57:38.686837 stackedup-0.0.8/setup.cfg
--rw-r--r--   0 axolx     (1000) axolx     (1000)     1110 2021-03-18 16:57:37.000000 stackedup-0.0.8/setup.py
-drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2021-03-18 16:57:38.686837 stackedup-0.0.8/stackedup.egg-info/
--rw-r--r--   0 axolx     (1000) axolx     (1000)     7752 2021-03-18 16:57:38.000000 stackedup-0.0.8/stackedup.egg-info/PKG-INFO
--rw-r--r--   0 axolx     (1000) axolx     (1000)      608 2021-03-18 16:57:38.000000 stackedup-0.0.8/stackedup.egg-info/SOURCES.txt
--rw-r--r--   0 axolx     (1000) axolx     (1000)        1 2021-03-18 16:57:38.000000 stackedup-0.0.8/stackedup.egg-info/dependency_links.txt
--rw-r--r--   0 axolx     (1000) axolx     (1000)      265 2021-03-18 16:57:38.000000 stackedup-0.0.8/stackedup.egg-info/entry_points.txt
--rw-r--r--   0 axolx     (1000) axolx     (1000)       48 2021-03-18 16:57:38.000000 stackedup-0.0.8/stackedup.egg-info/requires.txt
--rw-r--r--   0 axolx     (1000) axolx     (1000)        7 2021-03-18 16:57:38.000000 stackedup-0.0.8/stackedup.egg-info/top_level.txt
-drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2021-03-18 16:57:38.686837 stackedup-0.0.8/stacks/
--rw-r--r--   0 axolx     (1000) axolx     (1000)       16 2019-10-29 20:37:46.000000 stackedup-0.0.8/stacks/__init__.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     2092 2021-01-31 04:46:11.000000 stackedup-0.0.8/stacks/cluster.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     2354 2021-03-18 16:26:15.000000 stackedup-0.0.8/stacks/command.py
-drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2021-03-18 16:57:38.686837 stackedup-0.0.8/stacks/commands/
--rw-r--r--   0 axolx     (1000) axolx     (1000)        0 2019-11-03 02:49:58.000000 stackedup-0.0.8/stacks/commands/__init__.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)      796 2019-11-19 22:51:47.000000 stackedup-0.0.8/stacks/commands/assume_role.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     4611 2021-03-18 16:49:03.000000 stackedup-0.0.8/stacks/commands/container_shell.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     2242 2021-01-30 03:31:06.000000 stackedup-0.0.8/stacks/commands/database_shell.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     1687 2021-03-18 16:26:15.000000 stackedup-0.0.8/stacks/commands/stack_details.py
--rwxr-xr-x   0 axolx     (1000) axolx     (1000)     1906 2020-03-03 19:44:42.000000 stackedup-0.0.8/stacks/commands/stack_launch.py
--rwxr-xr-x   0 axolx     (1000) axolx     (1000)     1902 2020-01-31 21:43:50.000000 stackedup-0.0.8/stacks/commands/stack_update.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     2531 2020-03-03 19:39:31.000000 stackedup-0.0.8/stacks/config.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     5857 2021-03-18 16:52:35.000000 stackedup-0.0.8/stacks/stack.py
-drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2021-03-18 16:57:38.686837 stackedup-0.0.8/stacks/test/
--rw-r--r--   0 axolx     (1000) axolx     (1000)        0 2019-10-29 20:37:46.000000 stackedup-0.0.8/stacks/test/__init__.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     1294 2020-03-03 19:45:23.000000 stackedup-0.0.8/stacks/test/test_config.py
--rw-r--r--   0 axolx     (1000) axolx     (1000)     2274 2020-01-31 21:41:54.000000 stackedup-0.0.8/stacks/test/test_stack.py
+drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2022-12-07 19:22:57.123975 stackedup-0.0.9/
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     7784 2022-12-07 19:22:57.123975 stackedup-0.0.9/PKG-INFO
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     5939 2021-03-18 16:59:54.000000 stackedup-0.0.9/README.md
+-rw-r--r--   0 axolx     (1000) axolx     (1000)       38 2022-12-07 19:22:57.123975 stackedup-0.0.9/setup.cfg
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     1110 2022-12-07 19:22:41.000000 stackedup-0.0.9/setup.py
+drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2022-12-07 19:22:57.123975 stackedup-0.0.9/stackedup.egg-info/
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     7784 2022-12-07 19:22:57.000000 stackedup-0.0.9/stackedup.egg-info/PKG-INFO
+-rw-r--r--   0 axolx     (1000) axolx     (1000)      608 2022-12-07 19:22:57.000000 stackedup-0.0.9/stackedup.egg-info/SOURCES.txt
+-rw-r--r--   0 axolx     (1000) axolx     (1000)        1 2022-12-07 19:22:57.000000 stackedup-0.0.9/stackedup.egg-info/dependency_links.txt
+-rw-r--r--   0 axolx     (1000) axolx     (1000)      265 2022-12-07 19:22:57.000000 stackedup-0.0.9/stackedup.egg-info/entry_points.txt
+-rw-r--r--   0 axolx     (1000) axolx     (1000)       48 2022-12-07 19:22:57.000000 stackedup-0.0.9/stackedup.egg-info/requires.txt
+-rw-r--r--   0 axolx     (1000) axolx     (1000)        7 2022-12-07 19:22:57.000000 stackedup-0.0.9/stackedup.egg-info/top_level.txt
+drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2022-12-07 19:22:57.123975 stackedup-0.0.9/stacks/
+-rw-r--r--   0 axolx     (1000) axolx     (1000)       16 2019-10-29 20:37:46.000000 stackedup-0.0.9/stacks/__init__.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     2092 2021-01-31 04:46:11.000000 stackedup-0.0.9/stacks/cluster.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     2354 2021-03-18 16:26:15.000000 stackedup-0.0.9/stacks/command.py
+drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2022-12-07 19:22:57.123975 stackedup-0.0.9/stacks/commands/
+-rw-r--r--   0 axolx     (1000) axolx     (1000)        0 2019-11-03 02:49:58.000000 stackedup-0.0.9/stacks/commands/__init__.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)      796 2019-11-19 22:51:47.000000 stackedup-0.0.9/stacks/commands/assume_role.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     4618 2022-12-07 19:20:09.000000 stackedup-0.0.9/stacks/commands/container_shell.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     2242 2021-01-30 03:31:06.000000 stackedup-0.0.9/stacks/commands/database_shell.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     1687 2021-03-18 16:26:15.000000 stackedup-0.0.9/stacks/commands/stack_details.py
+-rwxr-xr-x   0 axolx     (1000) axolx     (1000)     1906 2020-03-03 19:44:42.000000 stackedup-0.0.9/stacks/commands/stack_launch.py
+-rwxr-xr-x   0 axolx     (1000) axolx     (1000)     1902 2020-01-31 21:43:50.000000 stackedup-0.0.9/stacks/commands/stack_update.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     2531 2020-03-03 19:39:31.000000 stackedup-0.0.9/stacks/config.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     5857 2021-03-18 16:52:35.000000 stackedup-0.0.9/stacks/stack.py
+drwxr-xr-x   0 axolx     (1000) axolx     (1000)        0 2022-12-07 19:22:57.123975 stackedup-0.0.9/stacks/test/
+-rw-r--r--   0 axolx     (1000) axolx     (1000)        0 2019-10-29 20:37:46.000000 stackedup-0.0.9/stacks/test/__init__.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     1294 2020-03-03 19:45:23.000000 stackedup-0.0.9/stacks/test/test_config.py
+-rw-r--r--   0 axolx     (1000) axolx     (1000)     2274 2020-01-31 21:41:54.000000 stackedup-0.0.9/stacks/test/test_stack.py
```

### Comparing `stackedup-0.0.8/PKG-INFO` & `stackedup-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackedup
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tooling to help manage CloudFormation stacks
 Home-page: https://github.com/ombu/stacks
 Author: OMBU
 Author-email: martin@ombuweb.com
 License: UNKNOWN
 Description: # Stackedup
         
@@ -18,19 +18,19 @@
         - **account**: An AWS account used by the application
         - **cluster**: A collection of AWS resources where applications run, such as
           compute capacity, database, networking configuration, etc that allows running
           one more instances
         - **instance**: An instance of an application, such as testing or production
         - **service**: An application service, such as an API or a web UI
         
-        As much as possible, stackedup aims to get out of  the way between you and your
-        CloudFormation Stacks.  Clusters, instances and services are plain
-        CloudFormation stacks. stackedup helps you launch and update them, recording
-        state and current parameters in an instance manifest, a YAML file usually named
-        `config.yaml.  A common instance  manifest, may look like this:
+        As much as possible, stackedup aims to get out of the way between you and your
+        CloudFormation Stacks. Clusters, instances and services are plain CloudFormation
+        stacks. stackedup helps you launch and update them, recording state and current
+        parameters in an instance manifest, a YAML file usually named `config.yaml. A
+        common instance manifest, may look like this:
         
         ```yaml
         ---
         project_name: my-project
         
         # The types of stacks supported in this project
         stack_types:
@@ -87,24 +87,26 @@
         
         ## Installation
         
         Stacked up is distributed in the Python Package Index (PyPI). To install it:
         
             pip install stackedup
         
-        This will install the current version of stackedup. Older projects may depend on specific versions, so stacked up is
-        usually installed as part of the project Python requirements. In a project with a `requirements.txt` file:
+        This will install the current version of stackedup. Older projects may depend on
+        specific versions, so stacked up is usually installed as part of the project
+        Python requirements. In a project with a `requirements.txt` file:
         
             pip install -r requirements.txt
         
         ## Usage
         
-        To run any stackedup command, your AWS CLI environment must be configured such that you are able to
-        assume the roles included in the accounts section of the instance manifest. When running commands, stacked
-        up will attempt to assume these roles.
+        To run any stackedup command, your AWS CLI environment must be configured such
+        that you are able to assume the roles included in the accounts section of the
+        instance manifest. When running commands, stacked up will attempt to assume
+        these roles.
         
         ### Launching stacks
         
         For a cluster:
         
             stack-launch cluster <cluster-name>
         
@@ -116,45 +118,45 @@
         
         For a cluster:
         
             stack-details cluster <cluster-name>
         
             stack-details <service> <instance>
         
-        
         ### Updating stacks
         
         After updating the parameters for an existing stack in the instance manifest
-        (often _config.yaml`), update the instance:
+        (often \_config.yaml`), update the instance:
         
             stack-update <service> <instance>
         
         ### Opening a shell session in a service container (==experimental==)
         
-        For service stacks that run [ECS
-        Services]([https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html))
+        For service stacks that run
+        [ECS Services](<[https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html)>)
         stacked up includes an experimental command to start a shell session in one of
         the service containers:
         
             $ container-shell <instance> <service> <service-name> <container>
             ssh -t -i <ssh-key> ec2-user@ec2-54-218-12-133... docker exec -it 380f02d109d9a038e1e1909e0f31e85a6491312d3c29726b269bde8621ce1212 sh
         
-        The command returns an SSH command, so it's often ran in backticks as command substitution:
+        The command returns an SSH command, so it's often ran in backticks as command
+        substitution:
         
             $ `container-shell <instance> <service> <service-name> <container>`
             #    (← you are in container bash session)
         
         ## AWS accounts
         
         stackedup can manage instances across AWS accounts, through IAM roles. The AWS
-        accounts their IAM roles for a project are defined in the `accounts:` section
-        of the instance manifest (usually a file named `config.yaml`). stackedup
-        commands automatically switch roles into the right account when performing
-        stack operations. One can also use the information in the instance manifest to
-        assume a role for a desired account in the AWS console:
+        accounts their IAM roles for a project are defined in the `accounts:` section of
+        the instance manifest (usually a file named `config.yaml`). stackedup commands
+        automatically switch roles into the right account when performing stack
+        operations. One can also use the information in the instance manifest to assume
+        a role for a desired account in the AWS console:
         
         1. Log into the AWS console for the master AWS account and open the _Switch
            Role_ view
            ([screenshot](https://tickets.ombuweb.com/attachments/download/8875/20200310-1038-aws-switch-role-1.png))
         
         2. Obtain the desired AWS account ID and role name for the target role from the
            instance manifest and enter it into the _Switch Role_ view:
@@ -169,18 +171,19 @@
         ```
         
         ### Packaged and distribute
         
         Edit `setup.py` with the desired target version. Then:
         
         ```console
-        pip install wheel
+        pip install wheel twine
         python setup.py sdist bdist_wheel
         python -m twine upload dist/stackedup-<tag>*
         
+        ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `stackedup-0.0.8/README.md` & `stackedup-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 - **account**: An AWS account used by the application
 - **cluster**: A collection of AWS resources where applications run, such as
   compute capacity, database, networking configuration, etc that allows running
   one more instances
 - **instance**: An instance of an application, such as testing or production
 - **service**: An application service, such as an API or a web UI
 
-As much as possible, stackedup aims to get out of  the way between you and your
-CloudFormation Stacks.  Clusters, instances and services are plain
-CloudFormation stacks. stackedup helps you launch and update them, recording
-state and current parameters in an instance manifest, a YAML file usually named
-`config.yaml.  A common instance  manifest, may look like this:
+As much as possible, stackedup aims to get out of the way between you and your
+CloudFormation Stacks. Clusters, instances and services are plain CloudFormation
+stacks. stackedup helps you launch and update them, recording state and current
+parameters in an instance manifest, a YAML file usually named `config.yaml. A
+common instance manifest, may look like this:
 
 ```yaml
 ---
 project_name: my-project
 
 # The types of stacks supported in this project
 stack_types:
@@ -79,24 +79,26 @@
 
 ## Installation
 
 Stacked up is distributed in the Python Package Index (PyPI). To install it:
 
     pip install stackedup
 
-This will install the current version of stackedup. Older projects may depend on specific versions, so stacked up is
-usually installed as part of the project Python requirements. In a project with a `requirements.txt` file:
+This will install the current version of stackedup. Older projects may depend on
+specific versions, so stacked up is usually installed as part of the project
+Python requirements. In a project with a `requirements.txt` file:
 
     pip install -r requirements.txt
 
 ## Usage
 
-To run any stackedup command, your AWS CLI environment must be configured such that you are able to
-assume the roles included in the accounts section of the instance manifest. When running commands, stacked
-up will attempt to assume these roles.
+To run any stackedup command, your AWS CLI environment must be configured such
+that you are able to assume the roles included in the accounts section of the
+instance manifest. When running commands, stacked up will attempt to assume
+these roles.
 
 ### Launching stacks
 
 For a cluster:
 
     stack-launch cluster <cluster-name>
 
@@ -108,45 +110,45 @@
 
 For a cluster:
 
     stack-details cluster <cluster-name>
 
     stack-details <service> <instance>
 
-
 ### Updating stacks
 
 After updating the parameters for an existing stack in the instance manifest
-(often _config.yaml`), update the instance:
+(often \_config.yaml`), update the instance:
 
     stack-update <service> <instance>
 
 ### Opening a shell session in a service container (==experimental==)
 
-For service stacks that run [ECS
-Services]([https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html))
+For service stacks that run
+[ECS Services](<[https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html)>)
 stacked up includes an experimental command to start a shell session in one of
 the service containers:
 
     $ container-shell <instance> <service> <service-name> <container>
     ssh -t -i <ssh-key> ec2-user@ec2-54-218-12-133... docker exec -it 380f02d109d9a038e1e1909e0f31e85a6491312d3c29726b269bde8621ce1212 sh
 
-The command returns an SSH command, so it's often ran in backticks as command substitution:
+The command returns an SSH command, so it's often ran in backticks as command
+substitution:
 
     $ `container-shell <instance> <service> <service-name> <container>`
     #    (← you are in container bash session)
 
 ## AWS accounts
 
 stackedup can manage instances across AWS accounts, through IAM roles. The AWS
-accounts their IAM roles for a project are defined in the `accounts:` section
-of the instance manifest (usually a file named `config.yaml`). stackedup
-commands automatically switch roles into the right account when performing
-stack operations. One can also use the information in the instance manifest to
-assume a role for a desired account in the AWS console:
+accounts their IAM roles for a project are defined in the `accounts:` section of
+the instance manifest (usually a file named `config.yaml`). stackedup commands
+automatically switch roles into the right account when performing stack
+operations. One can also use the information in the instance manifest to assume
+a role for a desired account in the AWS console:
 
 1. Log into the AWS console for the master AWS account and open the _Switch
    Role_ view
    ([screenshot](https://tickets.ombuweb.com/attachments/download/8875/20200310-1038-aws-switch-role-1.png))
 
 2. Obtain the desired AWS account ID and role name for the target role from the
    instance manifest and enter it into the _Switch Role_ view:
@@ -161,11 +163,12 @@
 ```
 
 ### Packaged and distribute
 
 Edit `setup.py` with the desired target version. Then:
 
 ```console
-pip install wheel
+pip install wheel twine
 python setup.py sdist bdist_wheel
 python -m twine upload dist/stackedup-<tag>*
 
+```
```

### Comparing `stackedup-0.0.8/setup.py` & `stackedup-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stackedup",
-    version="0.0.8",
+    version="0.0.9",
     author="OMBU",
     author_email="martin@ombuweb.com",
     url="https://github.com/ombu/stacks",
     description="Tooling to help manage CloudFormation stacks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

### Comparing `stackedup-0.0.8/stackedup.egg-info/PKG-INFO` & `stackedup-0.0.9/stackedup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackedup
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tooling to help manage CloudFormation stacks
 Home-page: https://github.com/ombu/stacks
 Author: OMBU
 Author-email: martin@ombuweb.com
 License: UNKNOWN
 Description: # Stackedup
         
@@ -18,19 +18,19 @@
         - **account**: An AWS account used by the application
         - **cluster**: A collection of AWS resources where applications run, such as
           compute capacity, database, networking configuration, etc that allows running
           one more instances
         - **instance**: An instance of an application, such as testing or production
         - **service**: An application service, such as an API or a web UI
         
-        As much as possible, stackedup aims to get out of  the way between you and your
-        CloudFormation Stacks.  Clusters, instances and services are plain
-        CloudFormation stacks. stackedup helps you launch and update them, recording
-        state and current parameters in an instance manifest, a YAML file usually named
-        `config.yaml.  A common instance  manifest, may look like this:
+        As much as possible, stackedup aims to get out of the way between you and your
+        CloudFormation Stacks. Clusters, instances and services are plain CloudFormation
+        stacks. stackedup helps you launch and update them, recording state and current
+        parameters in an instance manifest, a YAML file usually named `config.yaml. A
+        common instance manifest, may look like this:
         
         ```yaml
         ---
         project_name: my-project
         
         # The types of stacks supported in this project
         stack_types:
@@ -87,24 +87,26 @@
         
         ## Installation
         
         Stacked up is distributed in the Python Package Index (PyPI). To install it:
         
             pip install stackedup
         
-        This will install the current version of stackedup. Older projects may depend on specific versions, so stacked up is
-        usually installed as part of the project Python requirements. In a project with a `requirements.txt` file:
+        This will install the current version of stackedup. Older projects may depend on
+        specific versions, so stacked up is usually installed as part of the project
+        Python requirements. In a project with a `requirements.txt` file:
         
             pip install -r requirements.txt
         
         ## Usage
         
-        To run any stackedup command, your AWS CLI environment must be configured such that you are able to
-        assume the roles included in the accounts section of the instance manifest. When running commands, stacked
-        up will attempt to assume these roles.
+        To run any stackedup command, your AWS CLI environment must be configured such
+        that you are able to assume the roles included in the accounts section of the
+        instance manifest. When running commands, stacked up will attempt to assume
+        these roles.
         
         ### Launching stacks
         
         For a cluster:
         
             stack-launch cluster <cluster-name>
         
@@ -116,45 +118,45 @@
         
         For a cluster:
         
             stack-details cluster <cluster-name>
         
             stack-details <service> <instance>
         
-        
         ### Updating stacks
         
         After updating the parameters for an existing stack in the instance manifest
-        (often _config.yaml`), update the instance:
+        (often \_config.yaml`), update the instance:
         
             stack-update <service> <instance>
         
         ### Opening a shell session in a service container (==experimental==)
         
-        For service stacks that run [ECS
-        Services]([https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html))
+        For service stacks that run
+        [ECS Services](<[https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html)>)
         stacked up includes an experimental command to start a shell session in one of
         the service containers:
         
             $ container-shell <instance> <service> <service-name> <container>
             ssh -t -i <ssh-key> ec2-user@ec2-54-218-12-133... docker exec -it 380f02d109d9a038e1e1909e0f31e85a6491312d3c29726b269bde8621ce1212 sh
         
-        The command returns an SSH command, so it's often ran in backticks as command substitution:
+        The command returns an SSH command, so it's often ran in backticks as command
+        substitution:
         
             $ `container-shell <instance> <service> <service-name> <container>`
             #    (← you are in container bash session)
         
         ## AWS accounts
         
         stackedup can manage instances across AWS accounts, through IAM roles. The AWS
-        accounts their IAM roles for a project are defined in the `accounts:` section
-        of the instance manifest (usually a file named `config.yaml`). stackedup
-        commands automatically switch roles into the right account when performing
-        stack operations. One can also use the information in the instance manifest to
-        assume a role for a desired account in the AWS console:
+        accounts their IAM roles for a project are defined in the `accounts:` section of
+        the instance manifest (usually a file named `config.yaml`). stackedup commands
+        automatically switch roles into the right account when performing stack
+        operations. One can also use the information in the instance manifest to assume
+        a role for a desired account in the AWS console:
         
         1. Log into the AWS console for the master AWS account and open the _Switch
            Role_ view
            ([screenshot](https://tickets.ombuweb.com/attachments/download/8875/20200310-1038-aws-switch-role-1.png))
         
         2. Obtain the desired AWS account ID and role name for the target role from the
            instance manifest and enter it into the _Switch Role_ view:
@@ -169,18 +171,19 @@
         ```
         
         ### Packaged and distribute
         
         Edit `setup.py` with the desired target version. Then:
         
         ```console
-        pip install wheel
+        pip install wheel twine
         python setup.py sdist bdist_wheel
         python -m twine upload dist/stackedup-<tag>*
         
+        ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `stackedup-0.0.8/stackedup.egg-info/SOURCES.txt` & `stackedup-0.0.9/stackedup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/cluster.py` & `stackedup-0.0.9/stacks/cluster.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/command.py` & `stackedup-0.0.9/stacks/command.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/commands/assume_role.py` & `stackedup-0.0.9/stacks/commands/assume_role.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/commands/container_shell.py` & `stackedup-0.0.9/stacks/commands/container_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class ContainerShellCommand(InstanceCommand):
     def __init__(self):
         super().__init__()
         stack_type = "application"
         stack_config_instance = config_get_stack_config(
-            self.config, stack_type, self.args.name
+            self.config, self.args.service, self.args.name
         )
         self.stack = Stack(
             project_name=self.project_name,
             stack_type=stack_type,
             name=self.args.name,
             stack_config=stack_config_instance,
             region=config_get_stack_region(self.config, stack_type, self.args.name),
```

### Comparing `stackedup-0.0.8/stacks/commands/database_shell.py` & `stackedup-0.0.9/stacks/commands/database_shell.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/commands/stack_details.py` & `stackedup-0.0.9/stacks/commands/stack_details.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/commands/stack_launch.py` & `stackedup-0.0.9/stacks/commands/stack_launch.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/commands/stack_update.py` & `stackedup-0.0.9/stacks/commands/stack_update.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/config.py` & `stackedup-0.0.9/stacks/config.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/stack.py` & `stackedup-0.0.9/stacks/stack.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/test/test_config.py` & `stackedup-0.0.9/stacks/test/test_config.py`

 * *Files identical despite different names*

### Comparing `stackedup-0.0.8/stacks/test/test_stack.py` & `stackedup-0.0.9/stacks/test/test_stack.py`

 * *Files identical despite different names*

