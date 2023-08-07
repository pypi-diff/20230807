# Comparing `tmp/kfp-tekton-1.7.0.tar.gz` & `tmp/kfp-tekton-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-1.7.0.tar", last modified: Mon May 15 17:56:58 2023, max compression
+gzip compressed data, was "kfp-tekton-1.7.1.tar", last modified: Tue Jun 27 21:15:29 2023, max compression
```

## Comparing `kfp-tekton-1.7.0.tar` & `kfp-tekton-1.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-15 17:56:58.990003 kfp-tekton-1.7.0/
--rw-r--r--   0 tommyli    (501) staff       (20)    11890 2023-05-15 17:56:58.989514 kfp-tekton-1.7.0/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)    16444 2023-05-15 17:54:32.000000 kfp-tekton-1.7.0/README.md
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-15 17:56:58.978821 kfp-tekton-1.7.0/kfp_tekton/
--rw-r--r--   0 tommyli    (501) staff       (20)      713 2023-05-15 17:54:32.000000 kfp-tekton-1.7.0/kfp_tekton/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    33277 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/_client.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-15 17:56:58.988643 kfp-tekton-1.7.0/kfp_tekton/compiler/
--rw-r--r--   0 tommyli    (501) staff       (20)      675 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    44521 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/_data_passing_rewriter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     7091 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/_k8s_helper.py
--rw-r--r--   0 tommyli    (501) staff       (20)    32108 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/_op_to_template.py
--rw-r--r--   0 tommyli    (501) staff       (20)    30933 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/_tekton_handler.py
--rw-r--r--   0 tommyli    (501) staff       (20)    99548 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/compiler.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4279 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/main.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4088 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/pipeline_utils.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2071 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/compiler/yaml_utils.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1311 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/k8s_client_helper.py
--rw-r--r--   0 tommyli    (501) staff       (20)    17417 2023-05-11 18:46:53.000000 kfp-tekton-1.7.0/kfp_tekton/tekton.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-15 17:56:58.981706 kfp-tekton-1.7.0/kfp_tekton.egg-info/
--rw-r--r--   0 tommyli    (501) staff       (20)    11890 2023-05-15 17:56:58.000000 kfp-tekton-1.7.0/kfp_tekton.egg-info/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)      645 2023-05-15 17:56:58.000000 kfp-tekton-1.7.0/kfp_tekton.egg-info/SOURCES.txt
--rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-05-15 17:56:58.000000 kfp-tekton-1.7.0/kfp_tekton.egg-info/dependency_links.txt
--rw-r--r--   0 tommyli    (501) staff       (20)      107 2023-05-15 17:56:58.000000 kfp-tekton-1.7.0/kfp_tekton.egg-info/entry_points.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       49 2023-05-15 17:56:58.000000 kfp-tekton-1.7.0/kfp_tekton.egg-info/requires.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       11 2023-05-15 17:56:58.000000 kfp-tekton-1.7.0/kfp_tekton.egg-info/top_level.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       38 2023-05-15 17:56:58.990156 kfp-tekton-1.7.0/setup.cfg
--rw-r--r--   0 tommyli    (501) staff       (20)     7466 2023-05-15 17:54:32.000000 kfp-tekton-1.7.0/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-06-27 21:15:29.738591 kfp-tekton-1.7.1/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11890 2023-06-27 21:15:29.738240 kfp-tekton-1.7.1/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    16444 2023-06-27 21:04:46.000000 kfp-tekton-1.7.1/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-06-27 21:15:29.728940 kfp-tekton-1.7.1/kfp_tekton/
+-rw-r--r--   0 tommyli    (501) staff       (20)      713 2023-06-27 21:02:52.000000 kfp-tekton-1.7.1/kfp_tekton/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    33277 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/_client.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-06-27 21:15:29.737683 kfp-tekton-1.7.1/kfp_tekton/compiler/
+-rw-r--r--   0 tommyli    (501) staff       (20)      675 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    44521 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/_data_passing_rewriter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7091 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/_k8s_helper.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    32108 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/_op_to_template.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    30933 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/_tekton_handler.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    99735 2023-06-26 20:55:17.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/compiler.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4279 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/main.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4296 2023-06-26 20:57:11.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/pipeline_utils.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2071 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/compiler/yaml_utils.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1311 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/k8s_client_helper.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    17417 2023-05-11 18:46:53.000000 kfp-tekton-1.7.1/kfp_tekton/tekton.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-06-27 21:15:29.731594 kfp-tekton-1.7.1/kfp_tekton.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11890 2023-06-27 21:15:29.000000 kfp-tekton-1.7.1/kfp_tekton.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)      645 2023-06-27 21:15:29.000000 kfp-tekton-1.7.1/kfp_tekton.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-06-27 21:15:29.000000 kfp-tekton-1.7.1/kfp_tekton.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)      107 2023-06-27 21:15:29.000000 kfp-tekton-1.7.1/kfp_tekton.egg-info/entry_points.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       49 2023-06-27 21:15:29.000000 kfp-tekton-1.7.1/kfp_tekton.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       11 2023-06-27 21:15:29.000000 kfp-tekton-1.7.1/kfp_tekton.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       38 2023-06-27 21:15:29.738692 kfp-tekton-1.7.1/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     7466 2023-06-27 21:03:18.000000 kfp-tekton-1.7.1/setup.py
```

### Comparing `kfp-tekton-1.7.0/PKG-INFO` & `kfp-tekton-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp-tekton
-Version: 1.7.0
+Version: 1.7.1
 Summary: Tekton Compiler for Kubeflow Pipelines
 Home-page: https://github.com/kubeflow/kfp-tekton/
 Author: kubeflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -83,15 +83,15 @@
   * `kfp_tekton.TektonClient.create_run_from_pipeline_package` runs a local
     pipeline package on Kubeflow Pipelines.
 
 
 <h2><a id="project-prerequisites">Project Prerequisites</a></h2>
 
  - Python: `3.8` or later
- - Tekton: [`v0.47.0`](https://github.com/tektoncd/pipeline/releases/tag/v0.47.0) or [later](https://github.com/tektoncd/pipeline/releases/latest)
+ - Tekton: [`v0.47.1`](https://github.com/tektoncd/pipeline/releases/tag/v0.47.1) or [later](https://github.com/tektoncd/pipeline/releases/latest)
  - Tekton CLI: [`0.30.1`](https://github.com/tektoncd/cli/releases/tag/v0.30.1)
  - Kubeflow Pipelines: [KFP with Tekton backend](https://github.com/kubeflow/kfp-tekton/blob/master/guides/kfp_tekton_install.md)
 
 Follow the instructions for [installing project prerequisites](https://github.com/kubeflow/kfp-tekton/blob/master/sdk/python/README.md#development-prerequisites)
 and take note of some important caveats.
```

### Comparing `kfp-tekton-1.7.0/README.md` & `kfp-tekton-1.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 The source code of the `kfp-tekton` compiler was created as an extension of the [`Kubeflow Pipelines SDK Compiler`](https://github.com/kubeflow/pipelines/tree/sdk/release-1.8/sdk/python/kfp/compiler).
 This approach allowed us to leverage much of the existing [Kubeflow Pipelines Python SDK code](https://www.kubeflow.org/docs/pipelines/sdk/sdk-overview/#sdk-packages),
 like the DSL and components packages, but "override" or "replace" those parts of the compiler code required to generate
 the Tekton YAML instead of Argo YAML. Since the KFP SDK was not designed and implemented to easily be extended,
 _monkey-patching_ was used to replace non-class methods and functions at runtime.
 
 In order for the _monkey patch_ to work properly, the `kfp-tekton` compiler source code has to be aligned with a
-specific version of the `kfp` SDK compiler. As of now the `kfp-tekton` SDK version is `1.7.0` which is aligned with KFP
-SDK version [`1.8.21`](https://pypi.org/project/kfp/1.8.21/).
+specific version of the `kfp` SDK compiler. As of now the `kfp-tekton` SDK version is `1.7.1` which is aligned with KFP
+SDK version [`1.8.22`](https://pypi.org/project/kfp/1.8.22/).
 
 
 ## Adding New Code
 
 The Python package structure as well as the module names and method signatures closely mirror those of the
 [`Kubeflow Pipelines Python SDK`](https://github.com/kubeflow/pipelines/tree/master/sdk/python).
 This helps keeping track of all the code that had to modified and will make merging (some of) the code back into KFP or
```

### Comparing `kfp-tekton-1.7.0/kfp_tekton/__init__.py` & `kfp-tekton-1.7.1/kfp_tekton/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.7.0'
+__version__ = '1.7.1'
 
 from ._client import TektonClient  # noqa F401
 from .k8s_client_helper import env_from_secret  # noqa F401
```

### Comparing `kfp-tekton-1.7.0/kfp_tekton/_client.py` & `kfp-tekton-1.7.1/kfp_tekton/_client.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/__init__.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/_data_passing_rewriter.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/_data_passing_rewriter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/_k8s_helper.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/_k8s_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/_op_to_template.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/_op_to_template.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/_tekton_handler.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/_tekton_handler.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/compiler.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 DEFAULT_ARTIFACT_ENDPOINT_SCHEME = env.get('DEFAULT_ARTIFACT_ENDPOINT_SCHEME', 'http://')
 # DISABLE_CEL_CONDITION should be True until CEL is officially merged into Tekton main API.
 DISABLE_CEL_CONDITION = True
 # Default finally extension is 5 minutes
 DEFAULT_FINALLY_SECONDS = 300
 
 
-def _get_super_condition_template():
+def _get_super_condition_template(image_name="python:3.9.17-alpine3.18"):
 
   python_script = textwrap.dedent('''\
     import sys
     input1=str.rstrip(sys.argv[1])
     input2=str.rstrip(sys.argv[2])
     try:
       input1=int(input1)
@@ -88,15 +88,15 @@
       {'name': 'operand2'},
       {'name': 'operator'}
     ],
     'steps': [{
       'name': 'main',
       'command': ['sh', '-ec', 'program_path=$(mktemp); printf "%s" "$0" > "$program_path";  python3 -u "$program_path" "$1" "$2"'],
       'args': [python_script, '$(inputs.params.operand1)', '$(inputs.params.operand2)'],
-      'image': 'python:alpine3.6',
+      'image': image_name,
     }]
   }
 
   return template
 
 
 def _get_cel_condition_template():
@@ -147,14 +147,15 @@
     self.security_context = None
     self.automount_service_account_token = None
     self.group_names = {}
     self.pipeline_env = {}
     self.pipeline_workspaces = {}
     self.task_workspaces = {}
     self.generate_component_spec_annotations = True
+    self.condition_image_name = "python:3.9.17-alpine3.18"
     super().__init__(**kwargs)
 
   def _set_pipeline_conf(self, tekton_pipeline_conf: TektonPipelineConf):
     self.pipeline_labels = tekton_pipeline_conf.pipeline_labels
     self.pipeline_labels['pipelines.kubeflow.org/pipelinename'] = ''
     self.pipeline_labels['pipelines.kubeflow.org/generation'] = ''
     self.pipeline_annotations = tekton_pipeline_conf.pipeline_annotations
@@ -162,14 +163,15 @@
     self.tekton_inline_spec = tekton_pipeline_conf.tekton_inline_spec
     self.resource_in_separate_yaml = tekton_pipeline_conf.resource_in_separate_yaml
     self.security_context = tekton_pipeline_conf.security_context
     self.automount_service_account_token = tekton_pipeline_conf.automount_service_account_token
     self.pipeline_env = tekton_pipeline_conf.pipeline_env
     self.pipeline_workspaces = tekton_pipeline_conf.pipeline_workspaces
     self.generate_component_spec_annotations = tekton_pipeline_conf.generate_component_spec_annotations
+    self.condition_image_name = tekton_pipeline_conf.condition_image_name
 
   def _resolve_value_or_reference(self, value_or_reference, potential_references):
     """_resolve_value_or_reference resolves values and PipelineParams, which could be task parameters or input parameters.
     Args:
       value_or_reference: value or reference to be resolved. It could be basic python types or PipelineParam
       potential_references(dict{str->str}): a dictionary of parameter names to task names
       """
@@ -970,15 +972,15 @@
     cel_conditions = {}
     condition_when_refs = {}
     condition_task_refs = {}
     string_condition_refs = {}
     for template in raw_templates:
       if template['kind'] == 'Condition':
         if DISABLE_CEL_CONDITION:
-          condition_task_spec = _get_super_condition_template()
+          condition_task_spec = _get_super_condition_template(self.condition_image_name)
         else:
           condition_task_spec = _get_cel_condition_template()
 
         condition_params = template['spec'].get('params', [])
         if condition_params:
           condition_task_ref = [{
               'name': template['metadata']['name'],
```

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/main.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/main.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/pipeline_utils.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/pipeline_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.tekton_inline_spec = True
         self.resource_in_separate_yaml = False
         self.security_context = None
         self.automount_service_account_token = None
         self.pipeline_env = {}
         self.pipeline_workspaces = {}
         self.generate_component_spec_annotations = True
+        self.condition_image_name = "python:3.9.17-alpine3.18"
         super().__init__(**kwargs)
 
     def copy(self):
         return TektonPipelineConf()\
             .set_tekton_inline_spec(self.tekton_inline_spec)\
             .set_resource_in_separate_yaml(self.resource_in_separate_yaml)\
             .set_security_context(self.security_context)\
@@ -90,7 +91,11 @@
         volumeSpec = volume if volume else volume_claim_template_spec
         self.pipeline_workspaces[workspace_name] = (volumeSpec, path_prefix)
         return self
 
     def set_generate_component_spec_annotations(self, value: bool):
         self.generate_component_spec_annotations = value
         return self
+
+    def set_condition_image_name(self, condition_image_name: str):
+        self.condition_image_name = condition_image_name
+        return self
```

### Comparing `kfp-tekton-1.7.0/kfp_tekton/compiler/yaml_utils.py` & `kfp-tekton-1.7.1/kfp_tekton/compiler/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/k8s_client_helper.py` & `kfp-tekton-1.7.1/kfp_tekton/k8s_client_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton/tekton.py` & `kfp-tekton-1.7.1/kfp_tekton/tekton.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/kfp_tekton.egg-info/PKG-INFO` & `kfp-tekton-1.7.1/kfp_tekton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp-tekton
-Version: 1.7.0
+Version: 1.7.1
 Summary: Tekton Compiler for Kubeflow Pipelines
 Home-page: https://github.com/kubeflow/kfp-tekton/
 Author: kubeflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -83,15 +83,15 @@
   * `kfp_tekton.TektonClient.create_run_from_pipeline_package` runs a local
     pipeline package on Kubeflow Pipelines.
 
 
 <h2><a id="project-prerequisites">Project Prerequisites</a></h2>
 
  - Python: `3.8` or later
- - Tekton: [`v0.47.0`](https://github.com/tektoncd/pipeline/releases/tag/v0.47.0) or [later](https://github.com/tektoncd/pipeline/releases/latest)
+ - Tekton: [`v0.47.1`](https://github.com/tektoncd/pipeline/releases/tag/v0.47.1) or [later](https://github.com/tektoncd/pipeline/releases/latest)
  - Tekton CLI: [`0.30.1`](https://github.com/tektoncd/cli/releases/tag/v0.30.1)
  - Kubeflow Pipelines: [KFP with Tekton backend](https://github.com/kubeflow/kfp-tekton/blob/master/guides/kfp_tekton_install.md)
 
 Follow the instructions for [installing project prerequisites](https://github.com/kubeflow/kfp-tekton/blob/master/sdk/python/README.md#development-prerequisites)
 and take note of some important caveats.
```

### Comparing `kfp-tekton-1.7.0/kfp_tekton.egg-info/SOURCES.txt` & `kfp-tekton-1.7.1/kfp_tekton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.7.0/setup.py` & `kfp-tekton-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # =============================================================================
 # To install the kfp_tekton project run:
 #
 #    $ pip3 install -e .
 #
 # To create a distribution for PyPi run:
 #
-#    $ export KFP_TEKTON_VERSION=1.7.0-rc1
+#    $ export KFP_TEKTON_VERSION=1.7.1-rc1
 #    $ python3 setup.py sdist
 #    $ twine check dist/kfp-tekton-${KFP_TEKTON_VERSION/-rc/rc}.tar.gz
 #    $ twine upload --repository pypi dist/kfp-tekton-${KFP_TEKTON_VERSION/-rc/rc}.tar.gz
 #
 #   ... or:
 #
-#    $ make distribution KFP_TEKTON_VERSION=1.7.0-rc1
+#    $ make distribution KFP_TEKTON_VERSION=1.7.1-rc1
 #
 # =============================================================================
 
 import logging
 import re
 import sys
 
@@ -55,15 +55,15 @@
 logger = logging.getLogger("kfp_tekton/setup.py")
 logger.setLevel(logging.INFO)
 
 
 # NOTICE, after any updates to the following, ./requirements.in should be updated
 # accordingly.
 REQUIRES = [
-    "kfp>=1.8.10,<1.8.22",
+    "kfp>=1.8.10,<1.8.23",
     "kfp-tekton-server-api>=1.5.0"
 ]
 
 TESTS_REQUIRE = [
     'pytest',
 ]
```

