# Comparing `tmp/chirho-0.1.0a1.tar.gz` & `tmp/chirho-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chirho-0.1.0a1.tar", last modified: Tue Jul 11 13:43:48 2023, max compression
+gzip compressed data, was "chirho-0.1.0a2.tar", last modified: Mon Aug  7 15:33:51 2023, max compression
```

## Comparing `chirho-0.1.0a1.tar` & `chirho-0.1.0a2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-11 13:43:37.000000 chirho-0.1.0a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-11 13:43:48.524194 chirho-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-07-11 13:43:37.000000 chirho-0.1.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.520194 chirho-0.1.0a1/chirho/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/chirho/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/chirho/counterfactual/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/counterfactual/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/counterfactual/handlers/ambiguity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/counterfactual/handlers/counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/counterfactual/handlers/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/counterfactual/internals.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/counterfactual/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/chirho/indexed/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/indexed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/indexed/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/indexed/internals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/indexed/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/chirho/interventional/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/interventional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/interventional/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/interventional/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/chirho/observational/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/observational/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/chirho/observational/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/observational/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/observational/handlers/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/observational/handlers/soft_conditioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/observational/internals.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-11 13:43:37.000000 chirho-0.1.0a1/chirho/observational/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:43:48.524194 chirho-0.1.0a1/chirho.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-11 13:43:48.000000 chirho-0.1.0a1/chirho.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-11 13:43:48.000000 chirho-0.1.0a1/chirho.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:43:48.000000 chirho-0.1.0a1/chirho.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 13:43:48.000000 chirho-0.1.0a1/chirho.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 13:43:48.000000 chirho-0.1.0a1/chirho.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 13:43:48.524194 chirho-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-11 13:43:37.000000 chirho-0.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.769572 chirho-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 15:33:33.000000 chirho-0.1.0a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-07 15:33:51.769572 chirho-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-08-07 15:33:33.000000 chirho-0.1.0a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.765572 chirho-0.1.0a2/chirho/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.765572 chirho-0.1.0a2/chirho/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.769572 chirho-0.1.0a2/chirho/counterfactual/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/counterfactual/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/counterfactual/handlers/ambiguity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/counterfactual/handlers/counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/counterfactual/handlers/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/counterfactual/internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/counterfactual/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.769572 chirho-0.1.0a2/chirho/indexed/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/indexed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/indexed/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/indexed/internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/indexed/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.769572 chirho-0.1.0a2/chirho/interventional/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/interventional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/interventional/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/interventional/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.769572 chirho-0.1.0a2/chirho/observational/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/observational/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.769572 chirho-0.1.0a2/chirho/observational/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/observational/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/observational/handlers/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/observational/handlers/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/observational/handlers/soft_conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/observational/internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-07 15:33:33.000000 chirho-0.1.0a2/chirho/observational/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:33:51.765572 chirho-0.1.0a2/chirho.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-07 15:33:51.000000 chirho-0.1.0a2/chirho.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-07 15:33:51.000000 chirho-0.1.0a2/chirho.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:33:51.000000 chirho-0.1.0a2/chirho.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-07 15:33:51.000000 chirho-0.1.0a2/chirho.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 15:33:51.000000 chirho-0.1.0a2/chirho.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-07 15:33:51.769572 chirho-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-07 15:33:33.000000 chirho-0.1.0a2/setup.py
```

### Comparing `chirho-0.1.0a1/LICENSE.md` & `chirho-0.1.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/PKG-INFO` & `chirho-0.1.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chirho
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Causal reasoning
 Home-page: https://www.basis.ai/
 Author: Basis
 License: Apache 2.0
 Project-URL: Source, https://github.com/BasisResearch/chirho
 Keywords: machine learning statistics probabilistic programming bayesian modeling pytorch
 Classifier: Intended Audience :: Developers
@@ -20,18 +20,22 @@
 Requires-Python: >=3.8
 Provides-Extra: extras
 Provides-Extra: test
 License-File: LICENSE.md
 
 |Build Status|
 
+.. image:: docs/source/_static/img/chirho_logo_wide.png
+   :alt: ChiRho logo
+   :align: center
+
 .. index-inclusion-marker
 
-Causal Probabilistic Programming with ChiRho
-=================================================
+Causal Reasoning with ChiRho
+============================
 
 ChiRho is a causal extension to the Pyro probabilistic programming
 language. It was built to bridge the gap between the capabilities of
 modern probablistic programming systems, such as Pyro, and the needs of
 policymakers, scientists, and AI researchers, who often want to use
 models to answer their questions about cause-and-effect relationships.
 As a non-exhaustive set of examples, ChiRho makes it easier to
@@ -145,14 +149,18 @@
   - Causal inference with deep models and proxy variables
 - `Example: Mediation analysis and (in)direct effects <https://basisresearch.github.io/chirho/mediation.html>`_
   - Mediation analysis for path specific effects
 - `Example: Deep structural causal model counterfactuals <https://basisresearch.github.io/chirho/deepscm.html>`_
   - Counterfactuals with normalizing flows
 - `Example: Structured Latent Confounders <https://basisresearch.github.io/chirho/slc.html>`_
   - Causal effect estimation when latent confounders are shared across groups
+- `Example: Synthetic difference-in-differences <https://basisresearch.github.io/chirho/sdid.html>`_
+  - Counterfactual estimation from longitudinal data
+- `Example: Robust estimation with the DR learner <https://basisresearch.github.io/chirho/dr_learner.html>`_
+  - Heterogeneous causal effect estimation with a misspecified model
 - `Design notes <https://basisresearch.github.io/chirho/design_notes>`_
   - Technical implementation details of ChiRho using effect handlers
 
 *Note*: These tutorials and examples assume some familiarity with Pyro and
 probabilistic programming. For introductory Pyro tutorials, please see
 `Additional background reading
 material <#additional-background-reading-material>`__ below.
```

### Comparing `chirho-0.1.0a1/README.rst` & `chirho-0.1.0a2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 |Build Status|
 
+.. image:: docs/source/_static/img/chirho_logo_wide.png
+   :alt: ChiRho logo
+   :align: center
+
 .. index-inclusion-marker
 
-Causal Probabilistic Programming with ChiRho
-=================================================
+Causal Reasoning with ChiRho
+============================
 
 ChiRho is a causal extension to the Pyro probabilistic programming
 language. It was built to bridge the gap between the capabilities of
 modern probablistic programming systems, such as Pyro, and the needs of
 policymakers, scientists, and AI researchers, who often want to use
 models to answer their questions about cause-and-effect relationships.
 As a non-exhaustive set of examples, ChiRho makes it easier to
@@ -121,14 +125,18 @@
   - Causal inference with deep models and proxy variables
 - `Example: Mediation analysis and (in)direct effects <https://basisresearch.github.io/chirho/mediation.html>`_
   - Mediation analysis for path specific effects
 - `Example: Deep structural causal model counterfactuals <https://basisresearch.github.io/chirho/deepscm.html>`_
   - Counterfactuals with normalizing flows
 - `Example: Structured Latent Confounders <https://basisresearch.github.io/chirho/slc.html>`_
   - Causal effect estimation when latent confounders are shared across groups
+- `Example: Synthetic difference-in-differences <https://basisresearch.github.io/chirho/sdid.html>`_
+  - Counterfactual estimation from longitudinal data
+- `Example: Robust estimation with the DR learner <https://basisresearch.github.io/chirho/dr_learner.html>`_
+  - Heterogeneous causal effect estimation with a misspecified model
 - `Design notes <https://basisresearch.github.io/chirho/design_notes>`_
   - Technical implementation details of ChiRho using effect handlers
 
 *Note*: These tutorials and examples assume some familiarity with Pyro and
 probabilistic programming. For introductory Pyro tutorials, please see
 `Additional background reading
 material <#additional-background-reading-material>`__ below.
@@ -176,8 +184,8 @@
 
 References
 ----------
 Pearl, Judea. *Causality: Models, Reasoning and Inference*. 2nd ed. USA: Cambridge University Press, 2009.
 
 
 .. |Build Status| image:: https://github.com/BasisResearch/chirho/actions/workflows/test.yml/badge.svg
-   :target: https://github.com/BasisResearch/chirho/actions/workflows/test.yml
+   :target: https://github.com/BasisResearch/chirho/actions/workflows/test.yml
```

### Comparing `chirho-0.1.0a1/chirho/counterfactual/handlers/ambiguity.py` & `chirho-0.1.0a2/chirho/counterfactual/handlers/ambiguity.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho/counterfactual/handlers/selection.py` & `chirho-0.1.0a2/chirho/counterfactual/handlers/selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     """
 
     @staticmethod
     def get_mask(
         dist: pyro.distributions.Distribution,
         value: Optional[torch.Tensor],
         device: torch.device = torch.device("cpu"),
+        name: Optional[str] = None,
     ) -> torch.Tensor:
         indices = get_factual_indices()
         return ~indexset_as_mask(indices, device=device)  # negate == complement
 
 
 class SelectFactual(DependentMaskMessenger):
     """
@@ -58,10 +59,11 @@
     """
 
     @staticmethod
     def get_mask(
         dist: pyro.distributions.Distribution,
         value: Optional[torch.Tensor] = None,
         device: torch.device = torch.device("cpu"),
+        name: Optional[str] = None,
     ) -> torch.Tensor:
         indices = get_factual_indices()
         return indexset_as_mask(indices, device=device)
```

### Comparing `chirho-0.1.0a1/chirho/counterfactual/internals.py` & `chirho-0.1.0a2/chirho/counterfactual/internals.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho/indexed/handlers.py` & `chirho-0.1.0a2/chirho/indexed/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,24 @@
     """
 
     def get_mask(
         self,
         dist: pyro.distributions.Distribution,
         value: Optional[torch.Tensor],
         device: torch.device = torch.device("cpu"),
+        name: Optional[str] = None,
     ) -> torch.Tensor:
         raise NotImplementedError
 
     def _pyro_sample(self, msg: Dict[str, Any]) -> None:
+        if pyro.poutine.util.site_is_subsample(msg):
+            return
+
         device = get_sample_msg_device(msg["fn"], msg["value"])
-        mask = self.get_mask(msg["fn"], msg["value"], device=device)
+        name = msg["name"] if "name" in msg else None
+        mask = self.get_mask(msg["fn"], msg["value"], device=device, name=name)
         msg["mask"] = mask if msg["mask"] is None else msg["mask"] & mask
+
+        # expand distribution to make sure two copies of a variable are sampled
+        msg["fn"] = msg["fn"].expand(
+            torch.broadcast_shapes(msg["fn"].batch_shape, mask.shape)
+        )
```

### Comparing `chirho-0.1.0a1/chirho/indexed/internals.py` & `chirho-0.1.0a2/chirho/indexed/internals.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pyro
 import pyro.infer.reparam
 import torch
 from pyro.poutine.indep_messenger import CondIndepStackFrame, IndepMessenger
 
 from chirho.indexed.ops import (
     IndexSet,
+    cond,
     gather,
     get_index_plates,
     indices_of,
     scatter,
     union,
 )
 
@@ -175,14 +176,40 @@
 def _indices_of_distribution(
     value: pyro.distributions.Distribution, **kwargs
 ) -> IndexSet:
     kwargs.pop("event_dim", None)
     return indices_of(value.batch_shape, event_dim=0, **kwargs)
 
 
+@cond.register(int)
+@cond.register(float)
+@cond.register(bool)
+def _cond_number(
+    fst: Union[bool, numbers.Number],
+    snd: Union[bool, numbers.Number, torch.Tensor],
+    case: Union[bool, torch.Tensor],
+    **kwargs,
+) -> torch.Tensor:
+    return cond(
+        torch.as_tensor(fst), torch.as_tensor(snd), torch.as_tensor(case), **kwargs
+    )
+
+
+@cond.register
+def _cond_tensor(
+    fst: torch.Tensor,
+    snd: torch.Tensor,
+    case: torch.Tensor,
+    *,
+    event_dim: int = 0,
+    **kwargs,
+) -> torch.Tensor:
+    return torch.where(case[(...,) + (None,) * event_dim], snd, fst)
+
+
 class _LazyPlateMessenger(IndepMessenger):
     prefix: str = "__index_plate__"
 
     def __init__(self, name: str, *args, **kwargs):
         self._orig_name: str = name
         super().__init__(f"{self.prefix}_{name}", *args, **kwargs)
```

### Comparing `chirho-0.1.0a1/chirho/indexed/ops.py` & `chirho-0.1.0a2/chirho/indexed/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import functools
+import operator
 from typing import Dict, Hashable, Iterable, List, Optional, Set, Tuple, TypeVar, Union
 
 import pyro
 import torch
 
 T = TypeVar("T")
 
@@ -260,14 +261,62 @@
     assert len(values) > 0
     assert all(isinstance(k, IndexSet) for k in values)
     for indices, value in values.items():
         result = scatter(value, indices, result=result, **kwargs)
     return result
 
 
+@functools.singledispatch
+def cond(fst, snd, case: Optional[T] = None, **kwargs):
+    """
+    Selection operation that is the sum-type analogue of :func:`scatter`
+    in the sense that where :func:`scatter` propagates both of its arguments,
+    :func:`cond` propagates only one, depending on the value of a boolean ``case`` .
+
+    For a given ``fst`` , ``snd`` , and ``case`` , :func:`cond` returns
+    ``snd`` if the ``case`` is true, and ``fst`` otherwise,
+    analogous to a Python conditional expression ``snd if case else fst`` .
+    Unlike a Python conditional expression, however, the case may be a tensor,
+    and both branches are evaluated, as with :func:`torch.where` ::
+
+        >> fst, snd = torch.randn(2, 3), torch.randn(2, 3)
+        >> case = (fst < snd).all(-1)
+        >> x = cond(fst, snd, case, event_dim=1)
+        >> assert (x == torch.where(case[..., None], snd, fst)).all()
+
+    .. note::
+
+        :func:`cond` can be extended to new value types by registering
+        an implementation for the type using :func:`functools.singledispatch` .
+
+    :param fst: The value to return if ``case`` is ``False`` .
+    :param snd: The value to return if ``case`` is ``True`` .
+    :param case: A boolean value or tensor. If a tensor, should have event shape ``()`` .
+    :param kwargs: Additional keyword arguments used by specific implementations.
+    """
+    raise NotImplementedError(f"cond not implemented for {type(fst)}")
+
+
+@cond.register(dict)
+@pyro.poutine.runtime.effectful(type="cond_n")
+def _cond_n(values: Dict[IndexSet, T], case: Union[bool, torch.Tensor], **kwargs):
+    assert len(values) > 0
+    assert all(isinstance(k, IndexSet) for k in values.keys())
+    result: Optional[T] = None
+    for indices, value in values.items():
+        tst = torch.as_tensor(
+            functools.reduce(
+                operator.or_, [case == index for index in next(iter(indices.values()))]
+            ),
+            dtype=torch.bool,
+        )
+        result = cond(result if result is not None else value, value, tst, **kwargs)
+    return result
+
+
 @pyro.poutine.runtime.effectful(type="get_index_plates")
 def get_index_plates() -> (
     Dict[Hashable, pyro.poutine.indep_messenger.CondIndepStackFrame]
 ):
     return {}
```

### Comparing `chirho-0.1.0a1/chirho/interventional/handlers.py` & `chirho-0.1.0a2/chirho/interventional/handlers.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho/interventional/ops.py` & `chirho-0.1.0a2/chirho/interventional/ops.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho/observational/handlers/condition.py` & `chirho-0.1.0a2/chirho/observational/handlers/condition.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho/observational/handlers/soft_conditioning.py` & `chirho-0.1.0a2/chirho/observational/handlers/soft_conditioning.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho/observational/internals.py` & `chirho-0.1.0a2/chirho/observational/internals.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho/observational/ops.py` & `chirho-0.1.0a2/chirho/observational/ops.py`

 * *Files identical despite different names*

### Comparing `chirho-0.1.0a1/chirho.egg-info/PKG-INFO` & `chirho-0.1.0a2/chirho.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chirho
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Causal reasoning
 Home-page: https://www.basis.ai/
 Author: Basis
 License: Apache 2.0
 Project-URL: Source, https://github.com/BasisResearch/chirho
 Keywords: machine learning statistics probabilistic programming bayesian modeling pytorch
 Classifier: Intended Audience :: Developers
@@ -20,18 +20,22 @@
 Requires-Python: >=3.8
 Provides-Extra: extras
 Provides-Extra: test
 License-File: LICENSE.md
 
 |Build Status|
 
+.. image:: docs/source/_static/img/chirho_logo_wide.png
+   :alt: ChiRho logo
+   :align: center
+
 .. index-inclusion-marker
 
-Causal Probabilistic Programming with ChiRho
-=================================================
+Causal Reasoning with ChiRho
+============================
 
 ChiRho is a causal extension to the Pyro probabilistic programming
 language. It was built to bridge the gap between the capabilities of
 modern probablistic programming systems, such as Pyro, and the needs of
 policymakers, scientists, and AI researchers, who often want to use
 models to answer their questions about cause-and-effect relationships.
 As a non-exhaustive set of examples, ChiRho makes it easier to
@@ -145,14 +149,18 @@
   - Causal inference with deep models and proxy variables
 - `Example: Mediation analysis and (in)direct effects <https://basisresearch.github.io/chirho/mediation.html>`_
   - Mediation analysis for path specific effects
 - `Example: Deep structural causal model counterfactuals <https://basisresearch.github.io/chirho/deepscm.html>`_
   - Counterfactuals with normalizing flows
 - `Example: Structured Latent Confounders <https://basisresearch.github.io/chirho/slc.html>`_
   - Causal effect estimation when latent confounders are shared across groups
+- `Example: Synthetic difference-in-differences <https://basisresearch.github.io/chirho/sdid.html>`_
+  - Counterfactual estimation from longitudinal data
+- `Example: Robust estimation with the DR learner <https://basisresearch.github.io/chirho/dr_learner.html>`_
+  - Heterogeneous causal effect estimation with a misspecified model
 - `Design notes <https://basisresearch.github.io/chirho/design_notes>`_
   - Technical implementation details of ChiRho using effect handlers
 
 *Note*: These tutorials and examples assume some familiarity with Pyro and
 probabilistic programming. For introductory Pyro tutorials, please see
 `Additional background reading
 material <#additional-background-reading-material>`__ below.
```

### Comparing `chirho-0.1.0a1/chirho.egg-info/SOURCES.txt` & `chirho-0.1.0a2/chirho.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 chirho/interventional/handlers.py
 chirho/interventional/ops.py
 chirho/observational/__init__.py
 chirho/observational/internals.py
 chirho/observational/ops.py
 chirho/observational/handlers/__init__.py
 chirho/observational/handlers/condition.py
+chirho/observational/handlers/cut.py
 chirho/observational/handlers/soft_conditioning.py
```

### Comparing `chirho-0.1.0a1/setup.py` & `chirho-0.1.0a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from setuptools import find_packages, setup
 
-VERSION = "0.1.0-alpha1"
+VERSION = "0.1.0-alpha2"
 
 try:
     long_description = open("README.rst", encoding="utf-8").read()
 except Exception as e:
     sys.stderr.write("Failed to read README: {}\n".format(e))
     sys.stderr.flush()
     long_description = ""
```

