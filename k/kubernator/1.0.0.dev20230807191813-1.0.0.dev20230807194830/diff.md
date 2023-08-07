# Comparing `tmp/kubernator-1.0.0.dev20230807191813.tar.gz` & `tmp/kubernator-1.0.0.dev20230807194830.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernator-1.0.0.dev20230807191813.tar", last modified: Mon Aug  7 19:18:55 2023, max compression
+gzip compressed data, was "kubernator-1.0.0.dev20230807194830.tar", last modified: Mon Aug  7 19:49:24 2023, max compression
```

## Comparing `kubernator-1.0.0.dev20230807191813.tar` & `kubernator-1.0.0.dev20230807194830.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:55.889252 kubernator-1.0.0.dev20230807191813/
--rw-rw-r--   0 runner    (1001) docker     (123)       27 2023-08-07 19:18:51.000000 kubernator-1.0.0.dev20230807191813/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-08-07 19:18:55.885252 kubernator-1.0.0.dev20230807191813/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:55.885252 kubernator-1.0.0.dev20230807191813/kubernator/
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-08-07 19:18:51.000000 kubernator-1.0.0.dev20230807191813/kubernator/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/istio.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    25906 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/k8s_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/kops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:55.885252 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:18:55.889252 kubernator-1.0.0.dev20230807191813/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    11276 2023-08-07 19:18:51.000000 kubernator-1.0.0.dev20230807191813/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:49:24.568931 kubernator-1.0.0.dev20230807194830/
+-rw-rw-r--   0 runner    (1001) docker     (123)       27 2023-08-07 19:49:19.000000 kubernator-1.0.0.dev20230807194830/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-08-07 19:49:24.568931 kubernator-1.0.0.dev20230807194830/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:49:24.564931 kubernator-1.0.0.dev20230807194830/kubernator/
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-08-07 19:49:19.000000 kubernator-1.0.0.dev20230807194830/kubernator/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/istio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25906 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/k8s_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/kops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-07 19:48:13.000000 kubernator-1.0.0.dev20230807194830/kubernator/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:49:24.564931 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:49:24.000000 kubernator-1.0.0.dev20230807194830/kubernator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:49:24.568931 kubernator-1.0.0.dev20230807194830/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11295 2023-08-07 19:49:19.000000 kubernator-1.0.0.dev20230807194830/setup.py
```

### Comparing `kubernator-1.0.0.dev20230807191813/PKG-INFO` & `kubernator-1.0.0.dev20230807194830/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubernator
-Version: 1.0.0.dev20230807191813
+Version: 1.0.0.dev20230807194830
 Summary: Kubernator is the a pluggable framework for K8S provisioning
 Home-page: https://github.com/karellen/kubernator
 Author: Express Systems USA, Inc.
 Author-email: 
 Maintainer: Karellen, Inc., Arcadiy Ivanov
 Maintainer-email: supervisor@karellen.co,arcadiy@karellen.co
 License: Apache License, Version 2.0
@@ -34,15 +34,15 @@
 # Kubernator
 
 Kubernator™ (Ktor™) is an integrated solution for the Kubernetes state management. It operates on directories,
 processing their content via a collection of plugins, generating Kubernetes resources in the process, validating them,
 transforming them and then applying against the Kubernetes cluster.
 
 [![Gitter](https://img.shields.io/gitter/room/karellen/lobby?logo=gitter)](https://gitter.im/karellen/Lobby)
-[![Build Status](https://img.shields.io/github/workflow/status/karellen/kubernator/kubernator/master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/kubernator/kubernator.yml?branch=master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)
 [![Coverage Status](https://img.shields.io/coveralls/github/karellen/kubernator/master?logo=coveralls)](https://coveralls.io/r/karellen/kubernator?branch=master)
 
 [![Kubernator Version](https://img.shields.io/pypi/v/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Python Versions](https://img.shields.io/pypi/pyversions/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Downloads Per Day](https://img.shields.io/pypi/dd/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Downloads Per Week](https://img.shields.io/pypi/dw/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Downloads Per Month](https://img.shields.io/pypi/dm/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
```

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/LICENSE` & `kubernator-1.0.0.dev20230807194830/kubernator/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/__init__.py` & `kubernator-1.0.0.dev20230807194830/kubernator/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/api.py` & `kubernator-1.0.0.dev20230807194830/kubernator/api.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/app.py` & `kubernator-1.0.0.dev20230807194830/kubernator/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                                    default_includes=Globs(["*"], True),
                                    default_excludes=Globs([".*"], True),
                                    )
         context.app = dict(_repository_credentials_provider=None,
                            default_includes=Globs(context.app.default_includes),
                            default_excludes=Globs(context.app.default_excludes),
                            includes=Globs(context.app.default_includes),
-                           excludes=Globs(context.app.default_includes),
+                           excludes=Globs(context.app.default_excludes),
                            )
 
     def handle_before_dir(self, cwd: Path):
         context = self.context
         app = context.app
         app.includes = Globs(app.default_includes)
         app.excludes = Globs(app.default_excludes)
```

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/helm.py` & `kubernator-1.0.0.dev20230807194830/kubernator/helm.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/istio.py` & `kubernator-1.0.0.dev20230807194830/kubernator/istio.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,19 +70,21 @@
     def handle_start(self):
         context = self.context
         self.istio_stanza += ["--kubeconfig", os.environ.get("KUBECONFIG", os.path.expanduser("~/.kube/config"))]
 
         version_out: str = context.app.run_capturing_out(self.istio_stanza + ["version", "-o", "json"],
                                                          stderr_logger)
 
-        version = json.loads(version_out)["clientVersion"]["version"]
+        version_out_js = json.loads(version_out)
+        version = version_out_js["clientVersion"]["version"]
         logger.info("Found Istio client version %s", version)
 
-        self.client_version = version.split(".")
-        mesh_versions = set(m.value.split(".") for m in MESH_PILOT_JP.find(version_out))
+        self.client_version = tuple(version.split("."))
+        mesh_versions = set(tuple(m.value.split(".")) for m in MESH_PILOT_JP.find(version_out_js))
+
         if mesh_versions:
             self.server_version = max(mesh_versions)
 
         if not self.server_version:
             logger.info("No Istio mesh has been found and it'll be created")
             self.provision_operator = True
         elif self.server_version < self.client_version:
@@ -137,15 +139,17 @@
             logger.info("Skipping Istio as no Operator was processed")
         else:
             with tempfile.NamedTemporaryFile(mode="wt", delete=False) as operators_file:
                 yaml.safe_dump_all((r.manifest for r in self.resources.values()), operators_file)
 
             if context.app.args.command == "apply":
                 logger.info("Running Istio precheck")
-                context.app.run(self.istio_stanza + ["x", "precheck", "-f", operators_file.name],
+                context.app.run(self.istio_stanza + ["x", "precheck"],
+                                stdout_logger, stderr_logger).wait()
+                context.app.run(self.istio_stanza + ["validate", "-f", operators_file.name],
                                 stdout_logger, stderr_logger).wait()
 
                 self._operator_init(operators_file, True)
 
                 if not context.app.args.dry_run:
                     self._operator_init(operators_file, False)
```

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/k8s.py` & `kubernator-1.0.0.dev20230807194830/kubernator/k8s.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/k8s_api.py` & `kubernator-1.0.0.dev20230807194830/kubernator/k8s_api.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/kops.py` & `kubernator-1.0.0.dev20230807194830/kubernator/kops.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/proc.py` & `kubernator-1.0.0.dev20230807194830/kubernator/proc.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/template.py` & `kubernator-1.0.0.dev20230807194830/kubernator/template.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator/tf.py` & `kubernator-1.0.0.dev20230807194830/kubernator/tf.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator.egg-info/PKG-INFO` & `kubernator-1.0.0.dev20230807194830/kubernator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubernator
-Version: 1.0.0.dev20230807191813
+Version: 1.0.0.dev20230807194830
 Summary: Kubernator is the a pluggable framework for K8S provisioning
 Home-page: https://github.com/karellen/kubernator
 Author: Express Systems USA, Inc.
 Author-email: 
 Maintainer: Karellen, Inc., Arcadiy Ivanov
 Maintainer-email: supervisor@karellen.co,arcadiy@karellen.co
 License: Apache License, Version 2.0
@@ -34,15 +34,15 @@
 # Kubernator
 
 Kubernator™ (Ktor™) is an integrated solution for the Kubernetes state management. It operates on directories,
 processing their content via a collection of plugins, generating Kubernetes resources in the process, validating them,
 transforming them and then applying against the Kubernetes cluster.
 
 [![Gitter](https://img.shields.io/gitter/room/karellen/lobby?logo=gitter)](https://gitter.im/karellen/Lobby)
-[![Build Status](https://img.shields.io/github/workflow/status/karellen/kubernator/kubernator/master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/kubernator/kubernator.yml?branch=master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)
 [![Coverage Status](https://img.shields.io/coveralls/github/karellen/kubernator/master?logo=coveralls)](https://coveralls.io/r/karellen/kubernator?branch=master)
 
 [![Kubernator Version](https://img.shields.io/pypi/v/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Python Versions](https://img.shields.io/pypi/pyversions/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Downloads Per Day](https://img.shields.io/pypi/dd/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Downloads Per Week](https://img.shields.io/pypi/dw/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
 [![Kubernator Downloads Per Month](https://img.shields.io/pypi/dm/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)
```

### Comparing `kubernator-1.0.0.dev20230807191813/kubernator.egg-info/SOURCES.txt` & `kubernator-1.0.0.dev20230807194830/kubernator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 setup.py
 kubernator/LICENSE
 kubernator/__init__.py
+kubernator/__main__.py
 kubernator/api.py
 kubernator/app.py
 kubernator/helm.py
 kubernator/istio.py
 kubernator/k8s.py
 kubernator/k8s_api.py
 kubernator/kops.py
```

### Comparing `kubernator-1.0.0.dev20230807191813/setup.py` & `kubernator-1.0.0.dev20230807194830/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'kubernator',
-        version = '1.0.0.dev20230807191813',
+        version = '1.0.0.dev20230807194830',
         description = 'Kubernator is the a pluggable framework for K8S provisioning',
-        long_description = '# Kubernator\n\nKubernator™ (Ktor™) is an integrated solution for the Kubernetes state management. It operates on directories,\nprocessing their content via a collection of plugins, generating Kubernetes resources in the process, validating them,\ntransforming them and then applying against the Kubernetes cluster.\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/lobby?logo=gitter)](https://gitter.im/karellen/Lobby)\n[![Build Status](https://img.shields.io/github/workflow/status/karellen/kubernator/kubernator/master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/kubernator/master?logo=coveralls)](https://coveralls.io/r/karellen/kubernator?branch=master)\n\n[![Kubernator Version](https://img.shields.io/pypi/v/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Python Versions](https://img.shields.io/pypi/pyversions/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Day](https://img.shields.io/pypi/dd/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Week](https://img.shields.io/pypi/dw/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Month](https://img.shields.io/pypi/dm/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n\n## Notices\n\n### Beta Software\n\nWhile fully functional in the current state and used in production, this software is in **EARLY BETA**. A lot of things\nare expected to change rapidly, including main APIs, initialization procedures and some core features. Documentation at\nthis stage is basically non-existent.\n\n### License\n\nThe product is licensed under the Apache License, Version 2.0. Please see LICENSE for further details.\n\n### Warranties and Liability\n\nKubernator and its plugins are provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either\nexpress or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT,\nMERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of\nusing or redistributing Kubernator and assume any risks associated with doing so.\n\n### Trademarks\n\n"Kubernator" and "Ktor" are trademarks or registered trademarks of Express Systems USA, Inc and Karellen, Inc. All other\ntrademarks are property of their respective owners.\n\n## Problem Statement\n\n## Solution\n\n## Mode of Operation\n\nKubernator is a command line utility. Upon startup and processing of the command line arguments and initializing\nlogging, Kubernator initializes plugins. Current plugins include:\n\n0. Kubernator App\n1. Terraform\n2. kOps\n3. Kubernetes\n4. Helm\n5. Template\n\nThe order of initialization matters as it\'s the order the plugin handlers are executed!\n\nThe entire application operates in the following stages by invoking each plugin\'s stage handler in sequence:\n\n1. Plugin Init Stage\n2. Pre-start script (if specified)\n3. Plugin Start Stage\n4. For each directory in the pipeline:\n    1. Plugin Before Directory Stage\n    2. If `.kubernator.py` is present in the directory:\n        1. Plugin Before Script Stage\n        2. `.kubernator.py` script\n        3. Plugin After Script Stage\n    3. Plugin After Directory Stage\n5. Plugin End Stage\n\nEach plugin individually plays a specific role and performs a specific function which will be described in a later\nsection.\n\n## State/Context\n\nThere is a global state that is carried through as the application is running. It is a hierarchy of objects (`context`)\nthat follows the parent-child relationship as the application traverses the directory structure. For example, given the\ndirectory structure `/a/b`, `/a/c`, and `/a/c/d` any value of the context set or modified in context scoped to\ndirectory `/a` is visible in directories `/a/b`, `/a/c` and `/a/c/d`, while the same modified or set in `/a/b` is only\nvisible there, while one in `/a/c` is visible in `/a/c` and in `/a/c/d` but not `/a` or `/a/b`.\n\nAdditionally, there is a `context.globals` which is the top-most context that is available in all stages that are not\nassociated with the directory structure.\n\nNote, that in cases where the directory structure traversal moves to remote directories (that are actualized by local\ntemporary directories), such remote directory structure enters the context hierarchy as a child of the directory in\nwhich remote was registered.\n\nAlso note, that context carries not just data by references to essential functions.\n\nIn pre-start and `.kubernator.py` scripts the context is fully available as a global variable `ktor`.\n\n### Plugins\n\n#### Kubernator App Plugin\n\nThe role of the Kubernator App Plugin is to traverse the directory structure, expose essential functions through context\nand to run Kubernator scripts.\n\nIn the *After Directory Stage* Kubernator app scans the directories immediately available in the current, sorts them in\nthe alphabetic order, excludes those matching any of the patterns in `context.app.excludes` and then queues up the\nremaining directories in the order the match the patterns in `context.app.includes`.\n\nThus, for a directory content `/a/foo`, `/a/bal`, `/a/bar`, `/a/baz`, excludes `f*`, and includes `baz` and `*`, the\nresulting queue of directories to traverse will be `/a/baz`, `/a/bal`, `/a/bar`.\n\nNotice, that user can further interfere with processing order of the directory queue by asking Kubernator to walk\narbitrary paths, both local and remote.\n\n##### Context\n\n* `ktor.app.args`\n  > Namespace containing command line argument values\n* `ktor.app.walk_local(*paths: Union[Path, str, bytes])`\n  > Immediately schedules the paths to be traversed after the current directory by adding them to the queue\n  > Relative path is relative to the current directory\n* `ktor.app.walk_remote(repo, *path_prefixes: Union[Path, str, bytes])`\n  > Immediately schedules the path prefixes under the remote repo URL to be traversed after the current directory by\n  > adding them to the queue. Only Git URLs are currently supported.\n  > All absolute path prefixes are relativized based on the repository.\n* `ktor.app.repository_credentials_provider(func: Callable)`\n  > Sets a repository credentials provider function `func` that sets/overwrites credentials for URLs being specified by\n  > `walk_remote`. The callable `func` accepts a single argument containing a parsed URL in a form of tuple. The `func`\n  > is expected to return a tuple of three elements representing URL schema, username and password. If the value should\n  > not be changed it should be None. To convert from `git://repo.com/hello` to HTTPS authentication one should write\n  > a function returning `("https", "username", "password")`. The best utility is achieved by logic that allows running\n  > the plan both in CI and local environments using different authentication mechanics in different environments.\n\n#### Terraform\n\nThis is exclusively designed to pull the configuration options out of Terraform and to allow scripts and plugins to\nutilize that data.\n\n##### Context\n\n* `ktor.tf`\n  > A dictionary containing the values from Terraform output\n\n#### Kops\n\n##### Context\n\n#### Kubernetes\n\n##### Context\n\n#### Helm\n\n##### Context\n\n#### Templates\n\n##### Context\n\n## Examples\n\n### Adding Remote Directory\n\n```python\nktor.app.repository_credentials_provider(lambda r: ("ssh", "git", None))\nktor.app.walk_remote("git://repo.example.com/org/project?ref=dev", "/project")\n```\n\n### Adding Local Directory\n\n```python\nktor.app.walk_local("/home/username/local-dir")\n```\n\n### Using Transformers\n\n```python\ndef remove_replicas(resources, r: "K8SResource"):\n    if (r.group == "apps" and r.kind in ("StatefulSet", "Deployment")\n            and "replicas" in r.manifest["spec"]):\n        logger.warning("Resource %s in %s contains `replica` specification that will be removed. Use HPA!!!",\n                       r, r.source)\n        del r.manifest["spec"]["replicas"]\n\n\nktor.k8s.add_transformer(remove_replicas)\n```\n',
+        long_description = '# Kubernator\n\nKubernator™ (Ktor™) is an integrated solution for the Kubernetes state management. It operates on directories,\nprocessing their content via a collection of plugins, generating Kubernetes resources in the process, validating them,\ntransforming them and then applying against the Kubernetes cluster.\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/lobby?logo=gitter)](https://gitter.im/karellen/Lobby)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/kubernator/kubernator.yml?branch=master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/kubernator/master?logo=coveralls)](https://coveralls.io/r/karellen/kubernator?branch=master)\n\n[![Kubernator Version](https://img.shields.io/pypi/v/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Python Versions](https://img.shields.io/pypi/pyversions/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Day](https://img.shields.io/pypi/dd/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Week](https://img.shields.io/pypi/dw/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Month](https://img.shields.io/pypi/dm/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n\n## Notices\n\n### Beta Software\n\nWhile fully functional in the current state and used in production, this software is in **EARLY BETA**. A lot of things\nare expected to change rapidly, including main APIs, initialization procedures and some core features. Documentation at\nthis stage is basically non-existent.\n\n### License\n\nThe product is licensed under the Apache License, Version 2.0. Please see LICENSE for further details.\n\n### Warranties and Liability\n\nKubernator and its plugins are provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either\nexpress or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT,\nMERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of\nusing or redistributing Kubernator and assume any risks associated with doing so.\n\n### Trademarks\n\n"Kubernator" and "Ktor" are trademarks or registered trademarks of Express Systems USA, Inc and Karellen, Inc. All other\ntrademarks are property of their respective owners.\n\n## Problem Statement\n\n## Solution\n\n## Mode of Operation\n\nKubernator is a command line utility. Upon startup and processing of the command line arguments and initializing\nlogging, Kubernator initializes plugins. Current plugins include:\n\n0. Kubernator App\n1. Terraform\n2. kOps\n3. Kubernetes\n4. Helm\n5. Template\n\nThe order of initialization matters as it\'s the order the plugin handlers are executed!\n\nThe entire application operates in the following stages by invoking each plugin\'s stage handler in sequence:\n\n1. Plugin Init Stage\n2. Pre-start script (if specified)\n3. Plugin Start Stage\n4. For each directory in the pipeline:\n    1. Plugin Before Directory Stage\n    2. If `.kubernator.py` is present in the directory:\n        1. Plugin Before Script Stage\n        2. `.kubernator.py` script\n        3. Plugin After Script Stage\n    3. Plugin After Directory Stage\n5. Plugin End Stage\n\nEach plugin individually plays a specific role and performs a specific function which will be described in a later\nsection.\n\n## State/Context\n\nThere is a global state that is carried through as the application is running. It is a hierarchy of objects (`context`)\nthat follows the parent-child relationship as the application traverses the directory structure. For example, given the\ndirectory structure `/a/b`, `/a/c`, and `/a/c/d` any value of the context set or modified in context scoped to\ndirectory `/a` is visible in directories `/a/b`, `/a/c` and `/a/c/d`, while the same modified or set in `/a/b` is only\nvisible there, while one in `/a/c` is visible in `/a/c` and in `/a/c/d` but not `/a` or `/a/b`.\n\nAdditionally, there is a `context.globals` which is the top-most context that is available in all stages that are not\nassociated with the directory structure.\n\nNote, that in cases where the directory structure traversal moves to remote directories (that are actualized by local\ntemporary directories), such remote directory structure enters the context hierarchy as a child of the directory in\nwhich remote was registered.\n\nAlso note, that context carries not just data by references to essential functions.\n\nIn pre-start and `.kubernator.py` scripts the context is fully available as a global variable `ktor`.\n\n### Plugins\n\n#### Kubernator App Plugin\n\nThe role of the Kubernator App Plugin is to traverse the directory structure, expose essential functions through context\nand to run Kubernator scripts.\n\nIn the *After Directory Stage* Kubernator app scans the directories immediately available in the current, sorts them in\nthe alphabetic order, excludes those matching any of the patterns in `context.app.excludes` and then queues up the\nremaining directories in the order the match the patterns in `context.app.includes`.\n\nThus, for a directory content `/a/foo`, `/a/bal`, `/a/bar`, `/a/baz`, excludes `f*`, and includes `baz` and `*`, the\nresulting queue of directories to traverse will be `/a/baz`, `/a/bal`, `/a/bar`.\n\nNotice, that user can further interfere with processing order of the directory queue by asking Kubernator to walk\narbitrary paths, both local and remote.\n\n##### Context\n\n* `ktor.app.args`\n  > Namespace containing command line argument values\n* `ktor.app.walk_local(*paths: Union[Path, str, bytes])`\n  > Immediately schedules the paths to be traversed after the current directory by adding them to the queue\n  > Relative path is relative to the current directory\n* `ktor.app.walk_remote(repo, *path_prefixes: Union[Path, str, bytes])`\n  > Immediately schedules the path prefixes under the remote repo URL to be traversed after the current directory by\n  > adding them to the queue. Only Git URLs are currently supported.\n  > All absolute path prefixes are relativized based on the repository.\n* `ktor.app.repository_credentials_provider(func: Callable)`\n  > Sets a repository credentials provider function `func` that sets/overwrites credentials for URLs being specified by\n  > `walk_remote`. The callable `func` accepts a single argument containing a parsed URL in a form of tuple. The `func`\n  > is expected to return a tuple of three elements representing URL schema, username and password. If the value should\n  > not be changed it should be None. To convert from `git://repo.com/hello` to HTTPS authentication one should write\n  > a function returning `("https", "username", "password")`. The best utility is achieved by logic that allows running\n  > the plan both in CI and local environments using different authentication mechanics in different environments.\n\n#### Terraform\n\nThis is exclusively designed to pull the configuration options out of Terraform and to allow scripts and plugins to\nutilize that data.\n\n##### Context\n\n* `ktor.tf`\n  > A dictionary containing the values from Terraform output\n\n#### Kops\n\n##### Context\n\n#### Kubernetes\n\n##### Context\n\n#### Helm\n\n##### Context\n\n#### Templates\n\n##### Context\n\n## Examples\n\n### Adding Remote Directory\n\n```python\nktor.app.repository_credentials_provider(lambda r: ("ssh", "git", None))\nktor.app.walk_remote("git://repo.example.com/org/project?ref=dev", "/project")\n```\n\n### Adding Local Directory\n\n```python\nktor.app.walk_local("/home/username/local-dir")\n```\n\n### Using Transformers\n\n```python\ndef remove_replicas(resources, r: "K8SResource"):\n    if (r.group == "apps" and r.kind in ("StatefulSet", "Deployment")\n            and "replicas" in r.manifest["spec"]):\n        logger.warning("Resource %s in %s contains `replica` specification that will be removed. Use HPA!!!",\n                       r, r.source)\n        del r.manifest["spec"]["replicas"]\n\n\nktor.k8s.add_transformer(remove_replicas)\n```\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             'Operating System :: MacOS :: MacOS X',
```

