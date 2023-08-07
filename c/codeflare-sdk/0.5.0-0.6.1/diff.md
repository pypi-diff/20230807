# Comparing `tmp/codeflare_sdk-0.5.0.tar.gz` & `tmp/codeflare_sdk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflare_sdk-0.5.0.tar", max compression
+gzip compressed data, was "codeflare_sdk-0.6.1.tar", max compression
```

## Comparing `codeflare_sdk-0.5.0.tar` & `codeflare_sdk-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-07-06 19:46:30.609866 codeflare_sdk-0.5.0/LICENSE
--rw-r--r--   0        0        0     3488 2023-07-06 19:46:30.609866 codeflare_sdk-0.5.0/README.md
--rw-r--r--   0        0        0      859 2023-07-06 19:46:45.658588 codeflare_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/__init__.py
--rw-r--r--   0        0        0     4434 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/auth.py
--rw-r--r--   0        0        0     3931 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/awload.py
--rw-r--r--   0        0        0    18065 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/cluster.py
--rw-r--r--   0        0        0     1802 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/config.py
--rw-r--r--   0        0        0     2141 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/model.py
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/job/__init__.py
--rw-r--r--   0        0        0     6618 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/job/jobs.py
--rw-r--r--   0        0        0    15130 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/templates/base-template.yaml
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/__init__.py
--rw-r--r--   0        0        0     5697 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_cert.py
--rwxr-xr-x   0        0        0    15433 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_yaml.py
--rw-r--r--   0        0        0     6778 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/pretty_print.py
--rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 codeflare_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-07 18:23:06.859560 codeflare_sdk-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3488 2023-08-07 18:23:06.859560 codeflare_sdk-0.6.1/README.md
+-rw-r--r--   0        0        0      994 2023-08-07 18:23:23.211436 codeflare_sdk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/__init__.py
+-rw-r--r--   0        0        0     6149 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/auth.py
+-rw-r--r--   0        0        0     3400 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/awload.py
+-rw-r--r--   0        0        0    21924 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/cluster.py
+-rw-r--r--   0        0        0     1692 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/config.py
+-rw-r--r--   0        0        0     2159 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/model.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/job/__init__.py
+-rw-r--r--   0        0        0     6660 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/job/jobs.py
+-rw-r--r--   0        0        0    15130 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/templates/base-template.yaml
+-rw-r--r--   0        0        0        0 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     5766 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/utils/generate_cert.py
+-rwxr-xr-x   0        0        0    13435 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/utils/generate_yaml.py
+-rw-r--r--   0        0        0     1556 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/utils/kube_api_helpers.py
+-rw-r--r--   0        0        0     6663 2023-08-07 18:23:06.875560 codeflare_sdk-0.6.1/src/codeflare_sdk/utils/pretty_print.py
+-rw-r--r--   0        0        0     4593 1970-01-01 00:00:00.000000 codeflare_sdk-0.6.1/PKG-INFO
```

### Comparing `codeflare_sdk-0.5.0/LICENSE` & `codeflare_sdk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/README.md` & `codeflare_sdk-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/pyproject.toml` & `codeflare_sdk-0.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeflare-sdk"
-version = "0.5.0"
+version = "0.6.1"
 description = "Python SDK for codeflare client"
 
 license = "Apache-2.0"
 
 authors = [
     "Michael Clifford <mcliffor@redhat.com>",
     "Mustafa Eyceoz <meyceoz@redhat.com>",
@@ -19,17 +19,24 @@
 
 keywords = ['codeflare', 'python', 'sdk', 'client', 'batch', 'scale']
 
 [tool.poetry.dependencies]
 python = "^3.7"
 openshift-client = "1.0.18"
 rich = "^12.5"
-ray = {version = "2.1.0", extras = ["default"]}
+ray = {version = "2.5.0", extras = ["default"]}
 kubernetes = ">= 25.3.0, < 27"
 codeflare-torchx = "0.6.0.dev0"
 cryptography = "40.0.2"
+executing = "1.2.0"
+pydantic = "< 2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 pdoc3 = "0.10.0"
+
+[tool.poetry.group.test.dependencies]
+pytest = "7.4.0"
+coverage = "7.2.7"
+pytest-mock = "3.11.1"
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/cluster.py` & `codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/cluster.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 
 """
 The cluster sub-module contains the definition of the Cluster object, which represents
 the resources requested by the user. It also contains functions for checking the
 cluster setup queue, a list of all existing clusters, and the user's working namespace.
 """
 
-from os import stat
 from time import sleep
 from typing import List, Optional, Tuple, Dict
 
-import openshift as oc
 from ray.job_submission import JobSubmissionClient
 
+from .auth import config_check, api_config_handler
 from ..utils import pretty_print
 from ..utils.generate_yaml import generate_appwrapper
+from ..utils.kube_api_helpers import _kube_api_error_handling
 from .config import ClusterConfiguration
 from .model import (
     AppWrapper,
     AppWrapperStatus,
     CodeFlareClusterStatus,
     RayCluster,
     RayClusterStatus,
 )
+from kubernetes import client, config
+import yaml
+import os
 
 
 class Cluster:
     """
     An object for requesting, bringing up, and taking down resources.
     Can also be used for seeing the resource cluster status and details.
 
@@ -61,28 +64,30 @@
     def create_app_wrapper(self):
         """
         Called upon cluster object creation, creates an AppWrapper yaml based on
         the specifications of the ClusterConfiguration.
         """
 
         if self.config.namespace is None:
-            self.config.namespace = oc.get_project_name()
-            if type(self.config.namespace) is not str:
+            self.config.namespace = get_current_namespace()
+            if self.config.namespace is None:
+                print("Please specify with namespace=<your_current_namespace>")
+            elif type(self.config.namespace) is not str:
                 raise TypeError(
                     f"Namespace {self.config.namespace} is of type {type(self.config.namespace)}. Check your Kubernetes Authentication."
                 )
 
         name = self.config.name
         namespace = self.config.namespace
         min_cpu = self.config.min_cpus
         max_cpu = self.config.max_cpus
         min_memory = self.config.min_memory
         max_memory = self.config.max_memory
-        gpu = self.config.gpu
-        workers = self.config.max_worker
+        gpu = self.config.num_gpus
+        workers = self.config.num_workers
         template = self.config.template
         image = self.config.image
         instascale = self.config.instascale
         instance_types = self.config.machine_types
         env = self.config.envs
         local_interactive = self.config.local_interactive
         image_pull_secrets = self.config.image_pull_secrets
@@ -108,48 +113,46 @@
     def up(self):
         """
         Applies the AppWrapper yaml, pushing the resource request onto
         the MCAD queue.
         """
         namespace = self.config.namespace
         try:
-            with oc.project(namespace):
-                oc.invoke("apply", ["-f", self.app_wrapper_yaml])
-        except oc.OpenShiftPythonException as osp:  # pragma: no cover
-            error_msg = osp.result.err()
-            if "Unauthorized" in error_msg:
-                raise PermissionError(
-                    "Action not permitted, have you put in correct/up-to-date auth credentials?"
-                )
-            raise osp
+            config_check()
+            api_instance = client.CustomObjectsApi(api_config_handler())
+            with open(self.app_wrapper_yaml) as f:
+                aw = yaml.load(f, Loader=yaml.FullLoader)
+            api_instance.create_namespaced_custom_object(
+                group="mcad.ibm.com",
+                version="v1beta1",
+                namespace=namespace,
+                plural="appwrappers",
+                body=aw,
+            )
+        except Exception as e:  # pragma: no cover
+            return _kube_api_error_handling(e)
 
     def down(self):
         """
         Deletes the AppWrapper yaml, scaling-down and deleting all resources
         associated with the cluster.
         """
         namespace = self.config.namespace
         try:
-            with oc.project(namespace):
-                oc.invoke("delete", ["AppWrapper", self.app_wrapper_name])
-        except oc.OpenShiftPythonException as osp:  # pragma: no cover
-            error_msg = osp.result.err()
-            if (
-                'the server doesn\'t have a resource type "AppWrapper"' in error_msg
-                or "forbidden" in error_msg
-                or "Unauthorized" in error_msg
-                or "Missing or incomplete configuration" in error_msg
-            ):
-                raise PermissionError(
-                    "Action not permitted, have you run auth.login()/cluster.up() yet?"
-                )
-            elif "not found" in error_msg:
-                print("Cluster not found, have you run cluster.up() yet?")
-            else:
-                raise osp
+            config_check()
+            api_instance = client.CustomObjectsApi(api_config_handler())
+            api_instance.delete_namespaced_custom_object(
+                group="mcad.ibm.com",
+                version="v1beta1",
+                namespace=namespace,
+                plural="appwrappers",
+                name=self.app_wrapper_name,
+            )
+        except Exception as e:  # pragma: no cover
+            return _kube_api_error_handling(e)
 
     def status(
         self, print_to_console: bool = True
     ) -> Tuple[CodeFlareClusterStatus, bool]:
         """
         Returns the requested cluster's status, as well as whether or not
         it is ready for use.
@@ -169,17 +172,23 @@
             elif appwrapper.status in [
                 AppWrapperStatus.FAILED,
                 AppWrapperStatus.DELETED,
             ]:
                 ready = False
                 status = CodeFlareClusterStatus.FAILED  # should deleted be separate
                 return status, ready  # exit early, no need to check ray status
-            elif appwrapper.status in [AppWrapperStatus.PENDING]:
+            elif appwrapper.status in [
+                AppWrapperStatus.PENDING,
+                AppWrapperStatus.QUEUEING,
+            ]:
                 ready = False
-                status = CodeFlareClusterStatus.QUEUED
+                if appwrapper.status == AppWrapperStatus.PENDING:
+                    status = CodeFlareClusterStatus.QUEUED
+                else:
+                    status = CodeFlareClusterStatus.QUEUEING
                 if print_to_console:
                     pretty_print.print_app_wrappers_status([appwrapper])
                 return (
                     status,
                     ready,
                 )  # no need to check the ray status since still in queue
 
@@ -194,15 +203,15 @@
                 RayClusterStatus.FAILED,
             ]:
                 ready = False
                 status = CodeFlareClusterStatus.FAILED
 
             if print_to_console:
                 # overriding the number of gpus with requested
-                cluster.worker_gpu = self.config.gpu
+                cluster.worker_gpu = self.config.num_gpus
                 pretty_print.print_cluster_status(cluster)
         elif print_to_console:
             if status == CodeFlareClusterStatus.UNKNOWN:
                 pretty_print.print_no_resources_found()
             else:
                 pretty_print.print_app_wrappers_status([appwrapper], starting=True)
 
@@ -243,24 +252,29 @@
         return f"ray://{self.config.name}-head-svc.{self.config.namespace}.svc:10001"
 
     def cluster_dashboard_uri(self) -> str:
         """
         Returns a string containing the cluster's dashboard URI.
         """
         try:
-            with oc.project(self.config.namespace):
-                route = oc.invoke(
-                    "get", ["route", "-o", "jsonpath='{$.items[*].spec.host}'"]
-                )
-                route = route.out().split(" ")
-                route = [x for x in route if f"ray-dashboard-{self.config.name}" in x]
-                route = route[0].strip().strip("'")
-            return f"http://{route}"
-        except:
-            return "Dashboard route not available yet, have you run cluster.up()?"
+            config_check()
+            api_instance = client.CustomObjectsApi(api_config_handler())
+            routes = api_instance.list_namespaced_custom_object(
+                group="route.openshift.io",
+                version="v1",
+                namespace=self.config.namespace,
+                plural="routes",
+            )
+        except Exception as e:  # pragma: no cover
+            return _kube_api_error_handling(e)
+
+        for route in routes["items"]:
+            if route["metadata"]["name"] == f"ray-dashboard-{self.config.name}":
+                return f"http://{route['spec']['host']}"
+        return "Dashboard route not available yet, have you run cluster.up()?"
 
     def list_jobs(self) -> List:
         """
         This method accesses the head ray node in your cluster and lists the running jobs.
         """
         dashboard_route = self.cluster_dashboard_uri()
         client = JobSubmissionClient(dashboard_route)
@@ -292,14 +306,63 @@
         }
         if working_dir:
             to_return["working_dir"] = working_dir
         if requirements:
             to_return["requirements"] = requirements
         return to_return
 
+    def from_k8_cluster_object(rc):
+        machine_types = (
+            rc["metadata"]["labels"]["orderedinstance"].split("_")
+            if "orderedinstance" in rc["metadata"]["labels"]
+            else []
+        )
+        local_interactive = (
+            "volumeMounts"
+            in rc["spec"]["workerGroupSpecs"][0]["template"]["spec"]["containers"][0]
+        )
+        cluster_config = ClusterConfiguration(
+            name=rc["metadata"]["name"],
+            namespace=rc["metadata"]["namespace"],
+            machine_types=machine_types,
+            num_workers=rc["spec"]["workerGroupSpecs"][0]["minReplicas"],
+            min_cpus=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"][
+                "containers"
+            ][0]["resources"]["requests"]["cpu"],
+            max_cpus=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"][
+                "containers"
+            ][0]["resources"]["limits"]["cpu"],
+            min_memory=int(
+                rc["spec"]["workerGroupSpecs"][0]["template"]["spec"]["containers"][0][
+                    "resources"
+                ]["requests"]["memory"][:-1]
+            ),
+            max_memory=int(
+                rc["spec"]["workerGroupSpecs"][0]["template"]["spec"]["containers"][0][
+                    "resources"
+                ]["limits"]["memory"][:-1]
+            ),
+            num_gpus=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"][
+                "containers"
+            ][0]["resources"]["limits"]["nvidia.com/gpu"],
+            instascale=True if machine_types else False,
+            image=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"]["containers"][
+                0
+            ]["image"],
+            local_interactive=local_interactive,
+        )
+        return Cluster(cluster_config)
+
+    def local_client_url(self):
+        if self.config.local_interactive == True:
+            ingress_domain = _get_ingress_domain()
+            return f"ray://rayclient-{self.config.name}-{self.config.namespace}.{ingress_domain}"
+        else:
+            return "None"
+
 
 def list_all_clusters(namespace: str, print_to_console: bool = True):
     """
     Returns (and prints by default) a list of all clusters in a given namespace.
     """
     clusters = _get_ray_clusters(namespace)
     if print_to_console:
@@ -316,175 +379,221 @@
         namespace, filter=[AppWrapperStatus.RUNNING, AppWrapperStatus.PENDING]
     )
     if print_to_console:
         pretty_print.print_app_wrappers_status(app_wrappers)
     return app_wrappers
 
 
+def get_current_namespace():  # pragma: no cover
+    if api_config_handler() != None:
+        if os.path.isfile("/var/run/secrets/kubernetes.io/serviceaccount/namespace"):
+            try:
+                file = open(
+                    "/var/run/secrets/kubernetes.io/serviceaccount/namespace", "r"
+                )
+                active_context = file.readline().strip("\n")
+                return active_context
+            except Exception as e:
+                print("Unable to find current namespace")
+                return None
+        else:
+            print("Unable to find current namespace")
+            return None
+    else:
+        try:
+            _, active_context = config.list_kube_config_contexts(config_check())
+        except Exception as e:
+            return _kube_api_error_handling(e)
+        try:
+            return active_context["context"]["namespace"]
+        except KeyError:
+            return None
+
+
+def get_cluster(cluster_name: str, namespace: str = "default"):
+    try:
+        config.load_kube_config()
+        api_instance = client.CustomObjectsApi()
+        rcs = api_instance.list_namespaced_custom_object(
+            group="ray.io",
+            version="v1alpha1",
+            namespace=namespace,
+            plural="rayclusters",
+        )
+    except Exception as e:
+        return _kube_api_error_handling(e)
+
+    for rc in rcs["items"]:
+        if rc["metadata"]["name"] == cluster_name:
+            return Cluster.from_k8_cluster_object(rc)
+    raise FileNotFoundError(
+        f"Cluster {cluster_name} is not found in {namespace} namespace"
+    )
+
+
 # private methods
+def _get_ingress_domain():
+    try:
+        config.load_kube_config()
+        api_client = client.CustomObjectsApi(api_config_handler())
+        ingress = api_client.get_cluster_custom_object(
+            "config.openshift.io", "v1", "ingresses", "cluster"
+        )
+    except Exception as e:  # pragma: no cover
+        return _kube_api_error_handling(e)
+    return ingress["spec"]["domain"]
 
 
 def _app_wrapper_status(name, namespace="default") -> Optional[AppWrapper]:
-    cluster = None
     try:
-        with oc.project(namespace), oc.timeout(10 * 60):
-            cluster = oc.selector(f"appwrapper/{name}").object()
-    except oc.OpenShiftPythonException as osp:  # pragma: no cover
-        msg = osp.msg
-        if "Expected a single object, but selected 0" in msg:
-            return cluster
-        error_msg = osp.result.err()
-        if not (
-            'the server doesn\'t have a resource type "appwrapper"' in error_msg
-            or "forbidden" in error_msg
-            or "Unauthorized" in error_msg
-            or "Missing or incomplete configuration" in error_msg
-        ):
-            raise osp
-
-    if cluster:
-        return _map_to_app_wrapper(cluster)
+        config_check()
+        api_instance = client.CustomObjectsApi(api_config_handler())
+        aws = api_instance.list_namespaced_custom_object(
+            group="mcad.ibm.com",
+            version="v1beta1",
+            namespace=namespace,
+            plural="appwrappers",
+        )
+    except Exception as e:  # pragma: no cover
+        return _kube_api_error_handling(e)
 
-    return cluster
+    for aw in aws["items"]:
+        if aw["metadata"]["name"] == name:
+            return _map_to_app_wrapper(aw)
+    return None
 
 
 def _ray_cluster_status(name, namespace="default") -> Optional[RayCluster]:
-    cluster = None
     try:
-        with oc.project(namespace), oc.timeout(10 * 60):
-            cluster = oc.selector(f"rayclusters/{name}").object()
-    except oc.OpenShiftPythonException as osp:  # pragma: no cover
-        msg = osp.msg
-        if "Expected a single object, but selected 0" in msg:
-            return cluster
-        error_msg = osp.result.err()
-        if not (
-            'the server doesn\'t have a resource type "rayclusters"' in error_msg
-            or "forbidden" in error_msg
-            or "Unauthorized" in error_msg
-            or "Missing or incomplete configuration" in error_msg
-        ):
-            raise osp
-
-    if cluster:
-        return _map_to_ray_cluster(cluster)
+        config_check()
+        api_instance = client.CustomObjectsApi(api_config_handler())
+        rcs = api_instance.list_namespaced_custom_object(
+            group="ray.io",
+            version="v1alpha1",
+            namespace=namespace,
+            plural="rayclusters",
+        )
+    except Exception as e:  # pragma: no cover
+        return _kube_api_error_handling(e)
 
-    return cluster
+    for rc in rcs["items"]:
+        if rc["metadata"]["name"] == name:
+            return _map_to_ray_cluster(rc)
+    return None
 
 
 def _get_ray_clusters(namespace="default") -> List[RayCluster]:
     list_of_clusters = []
     try:
-        with oc.project(namespace), oc.timeout(10 * 60):
-            ray_clusters = oc.selector("rayclusters").objects()
-    except oc.OpenShiftPythonException as osp:  # pragma: no cover
-        error_msg = osp.result.err()
-        if (
-            'the server doesn\'t have a resource type "rayclusters"' in error_msg
-            or "forbidden" in error_msg
-            or "Unauthorized" in error_msg
-            or "Missing or incomplete configuration" in error_msg
-        ):
-            raise PermissionError(
-                "Action not permitted, have you put in correct/up-to-date auth credentials?"
-            )
-        else:
-            raise osp
+        config_check()
+        api_instance = client.CustomObjectsApi(api_config_handler())
+        rcs = api_instance.list_namespaced_custom_object(
+            group="ray.io",
+            version="v1alpha1",
+            namespace=namespace,
+            plural="rayclusters",
+        )
+    except Exception as e:  # pragma: no cover
+        return _kube_api_error_handling(e)
 
-    for cluster in ray_clusters:
-        list_of_clusters.append(_map_to_ray_cluster(cluster))
+    for rc in rcs["items"]:
+        list_of_clusters.append(_map_to_ray_cluster(rc))
     return list_of_clusters
 
 
 def _get_app_wrappers(
     namespace="default", filter=List[AppWrapperStatus]
 ) -> List[AppWrapper]:
     list_of_app_wrappers = []
 
     try:
-        with oc.project(namespace), oc.timeout(10 * 60):
-            app_wrappers = oc.selector("appwrappers").objects()
-    except oc.OpenShiftPythonException as osp:  # pragma: no cover
-        error_msg = osp.result.err()
-        if (
-            'the server doesn\'t have a resource type "appwrappers"' in error_msg
-            or "forbidden" in error_msg
-            or "Unauthorized" in error_msg
-            or "Missing or incomplete configuration" in error_msg
-        ):
-            raise PermissionError(
-                "Action not permitted, have you put in correct/up-to-date auth credentials?"
-            )
-        else:
-            raise osp
+        config_check()
+        api_instance = client.CustomObjectsApi(api_config_handler())
+        aws = api_instance.list_namespaced_custom_object(
+            group="mcad.ibm.com",
+            version="v1beta1",
+            namespace=namespace,
+            plural="appwrappers",
+        )
+    except Exception as e:  # pragma: no cover
+        return _kube_api_error_handling(e)
 
-    for item in app_wrappers:
+    for item in aws["items"]:
         app_wrapper = _map_to_app_wrapper(item)
         if filter and app_wrapper.status in filter:
             list_of_app_wrappers.append(app_wrapper)
         else:
             # Unsure what the purpose of the filter is
             list_of_app_wrappers.append(app_wrapper)
     return list_of_app_wrappers
 
 
-def _map_to_ray_cluster(cluster) -> Optional[RayCluster]:
-    cluster_model = cluster.model
-    if type(cluster_model.status.state) == oc.model.MissingModel:
-        status = RayClusterStatus.UNKNOWN
+def _map_to_ray_cluster(rc) -> Optional[RayCluster]:
+    if "state" in rc["status"]:
+        status = RayClusterStatus(rc["status"]["state"].lower())
     else:
-        status = RayClusterStatus(cluster_model.status.state.lower())
+        status = RayClusterStatus.UNKNOWN
 
-    with oc.project(cluster.namespace()), oc.timeout(10 * 60):
-        route = (
-            oc.selector(f"route/ray-dashboard-{cluster.name()}")
-            .object()
-            .model.spec.host
-        )
+    config_check()
+    api_instance = client.CustomObjectsApi(api_config_handler())
+    routes = api_instance.list_namespaced_custom_object(
+        group="route.openshift.io",
+        version="v1",
+        namespace=rc["metadata"]["namespace"],
+        plural="routes",
+    )
+    ray_route = None
+    for route in routes["items"]:
+        if route["metadata"]["name"] == f"ray-dashboard-{rc['metadata']['name']}":
+            ray_route = route["spec"]["host"]
 
     return RayCluster(
-        name=cluster.name(),
+        name=rc["metadata"]["name"],
         status=status,
         # for now we are not using autoscaling so same replicas is fine
-        min_workers=cluster_model.spec.workerGroupSpecs[0].replicas,
-        max_workers=cluster_model.spec.workerGroupSpecs[0].replicas,
-        worker_mem_max=cluster_model.spec.workerGroupSpecs[0]
-        .template.spec.containers[0]
-        .resources.limits.memory,
-        worker_mem_min=cluster_model.spec.workerGroupSpecs[0]
-        .template.spec.containers[0]
-        .resources.requests.memory,
-        worker_cpu=cluster_model.spec.workerGroupSpecs[0]
-        .template.spec.containers[0]
-        .resources.limits.cpu,
+        workers=rc["spec"]["workerGroupSpecs"][0]["replicas"],
+        worker_mem_max=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"][
+            "containers"
+        ][0]["resources"]["limits"]["memory"],
+        worker_mem_min=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"][
+            "containers"
+        ][0]["resources"]["requests"]["memory"],
+        worker_cpu=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"]["containers"][
+            0
+        ]["resources"]["limits"]["cpu"],
         worker_gpu=0,  # hard to detect currently how many gpus, can override it with what the user asked for
-        namespace=cluster.namespace(),
-        dashboard=route,
+        namespace=rc["metadata"]["namespace"],
+        dashboard=ray_route,
     )
 
 
-def _map_to_app_wrapper(cluster) -> AppWrapper:
-    cluster_model = cluster.model
+def _map_to_app_wrapper(aw) -> AppWrapper:
+    if "status" in aw and "canrun" in aw["status"]:
+        return AppWrapper(
+            name=aw["metadata"]["name"],
+            status=AppWrapperStatus(aw["status"]["state"].lower()),
+            can_run=aw["status"]["canrun"],
+            job_state=aw["status"]["queuejobstate"],
+        )
     return AppWrapper(
-        name=cluster.name(),
-        status=AppWrapperStatus(cluster_model.status.state.lower()),
-        can_run=cluster_model.status.canrun,
-        job_state=cluster_model.status.queuejobstate,
+        name=aw["metadata"]["name"],
+        status=AppWrapperStatus("queueing"),
+        can_run=False,
+        job_state="Still adding to queue",
     )
 
 
 def _copy_to_ray(cluster: Cluster) -> RayCluster:
     ray = RayCluster(
         name=cluster.config.name,
         status=cluster.status(print_to_console=False)[0],
-        min_workers=cluster.config.min_worker,
-        max_workers=cluster.config.max_worker,
+        workers=cluster.config.num_workers,
         worker_mem_min=cluster.config.min_memory,
         worker_mem_max=cluster.config.max_memory,
         worker_cpu=cluster.config.min_cpus,
-        worker_gpu=cluster.config.gpu,
+        worker_gpu=cluster.config.num_gpus,
         namespace=cluster.config.namespace,
         dashboard=cluster.cluster_dashboard_uri(),
     )
     if ray.status == CodeFlareClusterStatus.READY:
         ray.status = RayClusterStatus.READY
     return ray
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/config.py` & `codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 """
 The config sub-module contains the definition of the ClusterConfiguration dataclass,
 which is used to specify resource requirements and other details when creating a
 Cluster object.
 """
 
 from dataclasses import dataclass, field
-from .auth import Authentication
 import pathlib
-import openshift
 
 dir = pathlib.Path(__file__).parent.parent.resolve()
 
 
 @dataclass
 class ClusterConfiguration:
     """
@@ -35,18 +33,17 @@
 
     name: str
     namespace: str = None
     head_info: list = field(default_factory=list)
     machine_types: list = field(default_factory=list)  # ["m4.xlarge", "g4dn.xlarge"]
     min_cpus: int = 1
     max_cpus: int = 1
-    min_worker: int = 1
-    max_worker: int = 1
+    num_workers: int = 1
     min_memory: int = 2
     max_memory: int = 2
-    gpu: int = 0
+    num_gpus: int = 0
     template: str = f"{dir}/templates/base-template.yaml"
     instascale: bool = False
     envs: dict = field(default_factory=dict)
-    image: str = "ghcr.io/foundation-model-stack/base:ray2.1.0-py38-gpu-pytorch1.12.0cu116-20221213-193103"
+    image: str = "quay.io/project-codeflare/ray:2.5.0-py38-cu116"
     local_interactive: bool = False
     image_pull_secrets: list = field(default_factory=list)
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/model.py` & `codeflare_sdk-0.6.1/src/codeflare_sdk/cluster/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 
 class AppWrapperStatus(Enum):
     """
     Defines the possible reportable states of an AppWrapper.
     """
 
+    QUEUEING = "queueing"
     PENDING = "pending"
     RUNNING = "running"
     FAILED = "failed"
     DELETED = "deleted"
     COMPLETED = "completed"
     RUNNING_HOLD_COMPLETION = "runningholdcompletion"
 
@@ -51,28 +52,28 @@
     """
     Defines the possible reportable states of a Codeflare cluster.
     """
 
     READY = 1
     STARTING = 2
     QUEUED = 3
-    FAILED = 4
-    UNKNOWN = 5
+    QUEUEING = 4
+    FAILED = 5
+    UNKNOWN = 6
 
 
 @dataclass
 class RayCluster:
     """
     For storing information about a Ray cluster.
     """
 
     name: str
     status: RayClusterStatus
-    min_workers: int
-    max_workers: int
+    workers: int
     worker_mem_min: str
     worker_mem_max: str
     worker_cpu: int
     worker_gpu: int
     namespace: str
     dashboard: str
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/job/jobs.py` & `codeflare_sdk-0.6.1/src/codeflare_sdk/job/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # limitations under the License.
 
 
 import abc
 from typing import TYPE_CHECKING, Optional, Dict, List
 from pathlib import Path
 
-import openshift as oc
 from torchx.components.dist import ddp
 from torchx.runner import get_runner
 from torchx.specs import AppHandle, parse_app_handle, AppDryRunInfo
 
 if TYPE_CHECKING:
     from ..cluster.cluster import Cluster
+from ..cluster.cluster import get_current_namespace
 
 all_jobs: List["Job"] = []
 torchx_runner = get_runner()
 
 
 class JobDefinition(metaclass=abc.ABCMeta):
     def _dry_run(self, cluster: "Cluster"):
@@ -87,24 +87,24 @@
         self.scheduler_args: Dict[str, str] = (
             scheduler_args if scheduler_args is not None else dict()
         )
         self.image = image
         self.workspace = workspace
 
     def _dry_run(self, cluster: "Cluster"):
-        j = f"{cluster.config.max_worker}x{max(cluster.config.gpu, 1)}"  # # of proc. = # of gpus
+        j = f"{cluster.config.num_workers}x{max(cluster.config.num_gpus, 1)}"  # # of proc. = # of gpus
         return torchx_runner.dryrun(
             app=ddp(
                 *self.script_args,
                 script=self.script,
                 m=self.m,
                 name=self.name,
                 h=self.h,
                 cpu=self.cpu if self.cpu is not None else cluster.config.max_cpus,
-                gpu=self.gpu if self.gpu is not None else cluster.config.gpu,
+                gpu=self.gpu if self.gpu is not None else cluster.config.num_gpus,
                 memMB=self.memMB
                 if self.memMB is not None
                 else cluster.config.max_memory * 1024,
                 j=self.j if self.j is not None else j,
                 env=self.env,
                 max_retries=self.max_retries,
                 rdzv_port=self.rdzv_port,
@@ -120,15 +120,15 @@
 
     def _missing_spec(self, spec: str):
         raise ValueError(f"Job definition missing arg: {spec}")
 
     def _dry_run_no_cluster(self):
         if self.scheduler_args is not None:
             if self.scheduler_args.get("namespace") is None:
-                self.scheduler_args["namespace"] = oc.get_project_name()
+                self.scheduler_args["namespace"] = get_current_namespace()
         return torchx_runner.dryrun(
             app=ddp(
                 *self.script_args,
                 script=self.script,
                 m=self.m,
                 name=self.name if self.name is not None else self._missing_spec("name"),
                 h=self.h,
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/templates/base-template.yaml` & `codeflare_sdk-0.6.1/src/codeflare_sdk/templates/base-template.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_cert.py` & `codeflare_sdk-0.6.1/src/codeflare_sdk/utils/generate_cert.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import base64
 import os
 from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 import datetime
+from ..cluster.auth import config_check, api_config_handler
 from kubernetes import client, config
 
 
 def generate_ca_cert(days: int = 30):
     # Generate base64 encoded ca.key and ca.cert
     # Similar to:
     # openssl req -x509 -nodes -newkey rsa:2048 -keyout ca.key -days 1826 -out ca.crt -subj '/CN=root-ca'
@@ -78,16 +79,16 @@
     tls_dir = os.path.join(os.getcwd(), f"tls-{cluster_name}-{namespace}")
     if not os.path.exists(tls_dir):
         os.makedirs(tls_dir)
 
     # Similar to:
     # oc get secret ca-secret-<cluster-name> -o template='{{index .data "ca.key"}}'
     # oc get secret ca-secret-<cluster-name> -o template='{{index .data "ca.crt"}}'|base64 -d > ${TLSDIR}/ca.crt
-    config.load_kube_config()
-    v1 = client.CoreV1Api()
+    config_check()
+    v1 = client.CoreV1Api(api_config_handler())
     secret = v1.read_namespaced_secret(f"ca-secret-{cluster_name}", namespace).data
     ca_cert = secret.get("ca.crt")
     ca_key = secret.get("ca.key")
 
     with open(os.path.join(tls_dir, "ca.crt"), "w") as f:
         f.write(base64.b64decode(ca_cert).decode("utf-8"))
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_yaml.py` & `codeflare_sdk-0.6.1/src/codeflare_sdk/utils/generate_yaml.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 (in the cluster sub-module) for AppWrapper generation.
 """
 
 import yaml
 import sys
 import argparse
 import uuid
-import openshift as oc
+from kubernetes import client, config
+from .kube_api_helpers import _kube_api_error_handling
+from ..cluster.auth import api_config_handler
 
 
 def read_template(template):
     with open(template, "r") as stream:
         try:
             return yaml.safe_load(stream)
         except yaml.YAMLError as exc:
@@ -244,47 +246,86 @@
     ][0]["env"][1]["value"] = "1"
     # update_init_container
     command = item["generictemplate"]["spec"]["headGroupSpec"]["template"]["spec"][
         "initContainers"
     ][0].get("command")[2]
 
     command = command.replace("deployment-name", cluster_name)
-
-    server_name = (
-        oc.whoami("--show-server").split(":")[1].split("//")[1].replace("api", "apps")
-    )
-
-    command = command.replace("server-name", server_name)
+    try:
+        config.load_kube_config()
+        api_client = client.CustomObjectsApi(api_config_handler())
+        ingress = api_client.get_cluster_custom_object(
+            "config.openshift.io", "v1", "ingresses", "cluster"
+        )
+    except Exception as e:  # pragma: no cover
+        return _kube_api_error_handling(e)
+    domain = ingress["spec"]["domain"]
+    command = command.replace("server-name", domain)
 
     item["generictemplate"]["spec"]["headGroupSpec"]["template"]["spec"][
         "initContainers"
     ][0].get("command")[2] = command
 
 
 def disable_raycluster_tls(resources):
-    del resources["GenericItems"][0]["generictemplate"]["spec"]["headGroupSpec"][
-        "template"
-    ]["spec"]["volumes"]
-    del resources["GenericItems"][0]["generictemplate"]["spec"]["headGroupSpec"][
-        "template"
-    ]["spec"]["containers"][0]["volumeMounts"]
-    del resources["GenericItems"][0]["generictemplate"]["spec"]["headGroupSpec"][
-        "template"
-    ]["spec"]["initContainers"]
-    del resources["GenericItems"][0]["generictemplate"]["spec"]["workerGroupSpecs"][0][
-        "template"
-    ]["spec"]["volumes"]
-    del resources["GenericItems"][0]["generictemplate"]["spec"]["workerGroupSpecs"][0][
-        "template"
-    ]["spec"]["containers"][0]["volumeMounts"]
-    del resources["GenericItems"][0]["generictemplate"]["spec"]["workerGroupSpecs"][0][
-        "template"
-    ]["spec"]["initContainers"][1]
-    del resources["GenericItems"][3]  # rayclient route
-    del resources["GenericItems"][2]  # ca-secret
+    generic_template_spec = resources["GenericItems"][0]["generictemplate"]["spec"]
+
+    if "volumes" in generic_template_spec["headGroupSpec"]["template"]["spec"]:
+        del generic_template_spec["headGroupSpec"]["template"]["spec"]["volumes"]
+
+    if (
+        "volumeMounts"
+        in generic_template_spec["headGroupSpec"]["template"]["spec"]["containers"][0]
+    ):
+        del generic_template_spec["headGroupSpec"]["template"]["spec"]["containers"][0][
+            "volumeMounts"
+        ]
+
+    if "initContainers" in generic_template_spec["headGroupSpec"]["template"]["spec"]:
+        del generic_template_spec["headGroupSpec"]["template"]["spec"]["initContainers"]
+
+    if "volumes" in generic_template_spec["workerGroupSpecs"][0]["template"]["spec"]:
+        del generic_template_spec["workerGroupSpecs"][0]["template"]["spec"]["volumes"]
+
+    if (
+        "volumeMounts"
+        in generic_template_spec["workerGroupSpecs"][0]["template"]["spec"][
+            "containers"
+        ][0]
+    ):
+        del generic_template_spec["workerGroupSpecs"][0]["template"]["spec"][
+            "containers"
+        ][0]["volumeMounts"]
+
+    for i in range(
+        len(
+            generic_template_spec["workerGroupSpecs"][0]["template"]["spec"][
+                "initContainers"
+            ]
+        )
+    ):
+        if (
+            generic_template_spec["workerGroupSpecs"][0]["template"]["spec"][
+                "initContainers"
+            ][i]["name"]
+            == "create-cert"
+        ):
+            del generic_template_spec["workerGroupSpecs"][0]["template"]["spec"][
+                "initContainers"
+            ][i]
+
+    updated_items = []
+    for i in resources["GenericItems"][:]:
+        if "rayclient-deployment-name" in i["generictemplate"]["metadata"]["name"]:
+            continue
+        if "ca-secret-deployment-name" in i["generictemplate"]["metadata"]["name"]:
+            continue
+        updated_items.append(i)
+
+    resources["GenericItems"] = updated_items
 
 
 def write_user_appwrapper(user_yaml, output_file_name):
     with open(output_file_name, "w") as outfile:
         yaml.dump(user_yaml, outfile, default_flow_style=False)
     print(f"Written to: {output_file_name}")
 
@@ -334,135 +375,7 @@
     if local_interactive:
         enable_local_interactive(resources, cluster_name, namespace)
     else:
         disable_raycluster_tls(resources["resources"])
     outfile = appwrapper_name + ".yaml"
     write_user_appwrapper(user_yaml, outfile)
     return outfile
-
-
-def main():  # pragma: no cover
-    parser = argparse.ArgumentParser(description="Generate user AppWrapper")
-    parser.add_argument(
-        "--name",
-        required=False,
-        default="",
-        help="User selected name for AppWrapper and Ray Cluster (auto-generated if not provided)",
-    )
-    parser.add_argument(
-        "--min-cpu",
-        type=int,
-        required=True,
-        help="min number of CPU(s) in a worker required for running job",
-    )
-    parser.add_argument(
-        "--max-cpu",
-        type=int,
-        required=True,
-        help="max number of CPU(s) in a worker required for running job",
-    )
-    parser.add_argument(
-        "--min-memory",
-        type=int,
-        required=True,
-        help="min RAM required in a worker for running job, in GB",
-    )
-    parser.add_argument(
-        "--max-memory",
-        type=int,
-        required=True,
-        help="max RAM required in a worker for running job, in GB",
-    )
-    parser.add_argument(
-        "--gpu",
-        type=int,
-        required=True,
-        help="GPU(s) required in a worker for running job",
-    )
-    parser.add_argument(
-        "--workers",
-        type=int,
-        required=True,
-        help="How many workers are required in the cluster",
-    )
-    parser.add_argument(
-        "--template", required=True, help="Template AppWrapper yaml file"
-    )
-    parser.add_argument(
-        "--image",
-        required=False,
-        default="rayproject/ray:latest",
-        help="Ray image to be used (defaults to rayproject/ray:latest)",
-    )
-    parser.add_argument(
-        "--instascale",
-        default=False,
-        required=False,
-        action="store_true",
-        help="Indicates that instascale is installed on the cluster",
-    )
-    parser.add_argument(
-        "--instance-types",
-        type=str,
-        nargs="+",
-        default=[],
-        required=False,
-        help="Head,worker instance types (space separated)",
-    )
-    parser.add_argument(
-        "--namespace",
-        required=False,
-        default="default",
-        help="Set the kubernetes namespace you want to deploy your cluster to. Default. If left blank, uses the 'default' namespace",
-    )
-    parser.add_argument(
-        "--local-interactive",
-        required=False,
-        default=False,
-        help="Enable local interactive mode",
-    )
-    parser.add_argument(
-        "--image-pull-secrets",
-        required=False,
-        default=[],
-        help="Set image pull secrets for private registries",
-    )
-
-    args = parser.parse_args()
-    name = args.name
-    min_cpu = args.min_cpu
-    max_cpu = args.max_cpu
-    min_memory = args.min_memory
-    max_memory = args.max_memory
-    gpu = args.gpu
-    workers = args.workers
-    template = args.template
-    image = args.image
-    instascale = args.instascale
-    instance_types = args.instance_types
-    namespace = args.namespace
-    local_interactive = args.local_interactive
-    env = {}
-    image_pull_secrets = args.image_pull_secrets
-
-    outfile = generate_appwrapper(
-        name,
-        namespace,
-        min_cpu,
-        max_cpu,
-        min_memory,
-        max_memory,
-        gpu,
-        workers,
-        template,
-        image,
-        instascale,
-        instance_types,
-        local_interactive,
-        env,
-        image_pull_secrets,
-    )
-    return outfile
-
-
-if __name__ == "__main__":  # pragma: no cover
-    main()
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/utils/pretty_print.py` & `codeflare_sdk-0.6.1/src/codeflare_sdk/utils/pretty_print.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,16 +111,15 @@
         status = (
             "Active :white_heavy_check_mark:"
             if cluster.status == RayClusterStatus.READY
             else "Inactive :x:"
         )
         name = cluster.name
         dashboard = cluster.dashboard
-        mincount = str(cluster.min_workers)
-        maxcount = str(cluster.max_workers)
+        workers = str(cluster.workers)
         memory = str(cluster.worker_mem_min) + "~" + str(cluster.worker_mem_max)
         cpu = str(cluster.worker_cpu)
         gpu = str(cluster.worker_gpu)
         # owned = bool(cluster["userOwned"])
         owned = True
 
         #'table0' to display the cluster name, status, url, and dashboard link
@@ -138,18 +137,17 @@
         table0.add_row()
         table0.add_row(f"[link={dashboard} blue underline]Dashboard:link:[/link]")
         table0.add_row("")  # empty row for spacing
 
         #'table1' to display the worker counts
         table1 = Table(box=None)
         table1.add_row()
-        table1.add_column("Min", style="cyan", no_wrap=True)
-        table1.add_column("Max", style="magenta")
+        table1.add_column("# Workers", style="magenta")
         table1.add_row()
-        table1.add_row(mincount, maxcount)
+        table1.add_row(workers)
         table1.add_row()
 
         #'table2' to display the worker resources
         table2 = Table(box=None)
         table2.add_column("Memory", style="cyan", no_wrap=True, min_width=10)
         table2.add_column("CPU", style="magenta", min_width=10)
         table2.add_column("GPU", style="magenta", min_width=10)
```

### Comparing `codeflare_sdk-0.5.0/PKG-INFO` & `codeflare_sdk-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflare-sdk
-Version: 0.5.0
+Version: 0.6.1
 Summary: Python SDK for codeflare client
 Home-page: https://github.com/project-codeflare/codeflare-sdk
 License: Apache-2.0
 Keywords: codeflare,python,sdk,client,batch,scale
 Author: Michael Clifford
 Author-email: mcliffor@redhat.com
 Requires-Python: >=3.7,<4.0
@@ -13,17 +13,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: codeflare-torchx (==0.6.0.dev0)
 Requires-Dist: cryptography (==40.0.2)
+Requires-Dist: executing (==1.2.0)
 Requires-Dist: kubernetes (>=25.3.0,<27)
 Requires-Dist: openshift-client (==1.0.18)
-Requires-Dist: ray[default] (==2.1.0)
+Requires-Dist: pydantic (<2)
+Requires-Dist: ray[default] (==2.5.0)
 Requires-Dist: rich (>=12.5,<13.0)
 Project-URL: Repository, https://github.com/project-codeflare/codeflare-sdk
 Description-Content-Type: text/markdown
 
 # Codeflare-SDK
 
 [![Python application](https://github.com/project-codeflare/codeflare-sdk/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/project-codeflare/codeflare-sdk/actions/workflows/python-app.yml)
```

