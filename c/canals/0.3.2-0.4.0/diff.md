# Comparing `tmp/canals-0.3.2.tar.gz` & `tmp/canals-0.4.0.tar.gz`

## Comparing `canals-0.3.2.tar` & `canals-0.4.0.tar`

### file list

```diff
@@ -1,78 +1,25 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.3.2/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.3.2/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.3.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 canals-0.3.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.3.2/canals/__about__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.3.2/canals/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 canals-0.3.2/canals/errors.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.2/canals/component/__init__.py
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 canals-0.3.2/canals/component/component.py
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 canals-0.3.2/canals/component/input_output.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/__init__.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/draw.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/mermaid.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/__init__.py
--rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/connections.py
--rw-r--r--   0        0        0    31560 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/save_load.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/sockets.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/validation.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.2/canals/testing/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.3.2/canals/testing/test_component.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.2/docs/index.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 canals-0.3.2/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.3.2/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 canals-0.3.2/docs/concepts/components.md
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 canals-0.3.2/docs/concepts/concepts.md
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 canals-0.3.2/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.3.2/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.3.2/images/canals-logo-light.png
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/test/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.2/test/_helpers.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.2/test/conftest.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 canals-0.3.2/test/test_save_load.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 canals-0.3.2/test/component/test_component.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_double_loop_pipeline.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_connections.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_draw.py
--rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_input_sockets.py
--rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_output_sockets.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_pipeline.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_validation_pipeline_io.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/__init__.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_accumulate.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_add_value.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_concatenate.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_double.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_greet.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_merge_loop.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_parity.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_remainder.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_repeat.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_subtract.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_sum.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_threshold.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 canals-0.3.2/test/test_files/mermaid_mock/test_response.png
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 canals-0.3.2/test/test_files/pipeline_draw/pygraphviz.jpg
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 canals-0.3.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.3.2/LICENSE
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 canals-0.3.2/README.md
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 canals-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 canals-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.4.0/canals/__about__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 canals-0.4.0/canals/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 canals-0.4.0/canals/errors.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 canals-0.4.0/canals/type_checking.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 canals-0.4.0/canals/utils.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.4.0/canals/component/__init__.py
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 canals-0.4.0/canals/component/component.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/connections.py
+-rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/sockets.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/validation.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/draw/__init__.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/draw/draw.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/draw/graphviz.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 canals-0.4.0/canals/pipeline/draw/mermaid.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.4.0/canals/testing/__init__.py
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 canals-0.4.0/canals/testing/factory.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.4.0/canals/testing/test_component.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 canals-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 canals-0.4.0/README.md
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 canals-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 canals-0.4.0/PKG-INFO
```

### Comparing `canals-0.3.2/canals/errors.py` & `canals-0.4.0/canals/errors.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.2/canals/draw/draw.py` & `canals-0.4.0/canals/pipeline/draw/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 from typing import Literal, Optional, Dict, get_args, Any
 
 import logging
 from pathlib import Path
 
 import networkx
 
-from canals.pipeline.validation import find_pipeline_inputs, find_pipeline_outputs
-from canals.draw.graphviz import to_agraph
-from canals.draw.mermaid import to_mermaid_image, to_mermaid_text
-
+from canals.pipeline.validation import _find_pipeline_inputs, _find_pipeline_outputs
+from canals.pipeline.draw.graphviz import _to_agraph
+from canals.pipeline.draw.mermaid import _to_mermaid_image, _to_mermaid_text
+from canals.utils import _type_name
 
 logger = logging.getLogger(__name__)
 RenderingEngines = Literal["graphviz", "mermaid-img", "mermaid-text"]
 
 
-def draw(
+def _draw(
     graph: networkx.MultiDiGraph,
     path: Path,
     engine: RenderingEngines = "mermaid-img",
     style_map: Optional[Dict[str, str]] = None,
 ) -> None:
     """
     Renders the pipeline graph and saves it to file.
     """
-    converted_graph = convert(graph=graph, engine=engine, style_map=style_map)
+    converted_graph = _convert(graph=graph, engine=engine, style_map=style_map)
 
     if engine == "graphviz":
         converted_graph.draw(path)
 
     elif engine == "mermaid-img":
         with open(path, "wb") as imagefile:
             imagefile.write(converted_graph)
@@ -41,42 +41,42 @@
 
     else:
         raise ValueError(f"Unknown rendering engine '{engine}'. Choose one from: {get_args(RenderingEngines)}.")
 
     logger.debug("Pipeline diagram saved at %s", path)
 
 
-def convert_for_debug(
+def _convert_for_debug(
     graph: networkx.MultiDiGraph,
 ) -> Any:
     """
     Renders the pipeline graph with additional debug information into a text file that Mermaid can later render.
     """
     graph = _prepare_for_drawing(graph=graph, style_map={})
-    return to_mermaid_text(graph=graph)
+    return _to_mermaid_text(graph=graph)
 
 
-def convert(
+def _convert(
     graph: networkx.MultiDiGraph,
     engine: RenderingEngines = "mermaid-img",
     style_map: Optional[Dict[str, str]] = None,
 ) -> Any:
     """
     Renders the pipeline graph with the correct render and returns it.
     """
     graph = _prepare_for_drawing(graph=graph, style_map=style_map or {})
 
     if engine == "graphviz":
-        return to_agraph(graph=graph)
+        return _to_agraph(graph=graph)
 
     if engine == "mermaid-img":
-        return to_mermaid_image(graph=graph)
+        return _to_mermaid_image(graph=graph)
 
     if engine == "mermaid-text":
-        return to_mermaid_text(graph=graph)
+        return _to_mermaid_text(graph=graph)
 
     raise ValueError(f"Unknown rendering engine '{engine}'. Choose one from: {get_args(RenderingEngines)}.")
 
 
 def _prepare_for_drawing(graph: networkx.MultiDiGraph, style_map: Dict[str, str]) -> networkx.MultiDiGraph:
     """
     Prepares the graph to be drawn: adds explitic input and output nodes, labels the edges, applies the styles, etc.
@@ -89,23 +89,22 @@
     # Label the edges
     for inp, outp, key, data in graph.edges(keys=True, data=True):
         data["label"] = f"{data['from_socket'].name} -> {data['to_socket'].name}"
         graph.add_edge(inp, outp, key=key, **data)
 
     # Draw the inputs
     graph.add_node("input")
-    for node, in_sockets in find_pipeline_inputs(graph).items():
+    for node, in_sockets in _find_pipeline_inputs(graph).items():
         for in_socket in in_sockets:
-            node_instance = graph.nodes[node]["instance"]
-            socket_has_default = in_socket.name in node_instance.defaults
-            if not socket_has_default and in_socket.sender is None:
-                # If this socket has no defaults and no other component sends anything to it
-                # it must be a socket that receives input directly when running the Pipeline
-                graph.add_edge("input", node, label=in_socket.name)
+            if in_socket.sender is None:
+                # If this socket has no sender it could be a socket that receives input
+                # directly when running the Pipeline. We can't know that for sure, in doubt
+                # we draw it as receiving input directly.
+                graph.add_edge("input", node, label=in_socket.name, conn_type=_type_name(in_socket.type))
 
     # Draw the outputs
     graph.add_node("output")
-    for node, out_sockets in find_pipeline_outputs(graph).items():
+    for node, out_sockets in _find_pipeline_outputs(graph).items():
         for out_socket in out_sockets:
-            graph.add_edge(node, "output", label=out_socket.name)
+            graph.add_edge(node, "output", label=out_socket.name, conn_type=_type_name(out_socket.type))
 
     return graph
```

### Comparing `canals-0.3.2/canals/draw/graphviz.py` & `canals-0.4.0/canals/pipeline/draw/graphviz.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from networkx.drawing.nx_agraph import to_agraph as nx_to_agraph
 
 
 logger = logging.getLogger(__name__)
 
 
-def to_agraph(graph: networkx.MultiDiGraph):
+def _to_agraph(graph: networkx.MultiDiGraph):
     """
     Renders a pipeline graph using PyGraphViz. You need to install it and all its system dependencies for it to work.
     """
     try:
         import pygraphviz  # pylint: disable=unused-import,import-outside-toplevel
     except (ModuleNotFoundError, ImportError) as exc:
         raise ImportError(
```

### Comparing `canals-0.3.2/canals/pipeline/pipeline.py` & `canals-0.4.0/canals/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 import os
 import json
 import datetime
 import logging
 from pathlib import Path
 from copy import deepcopy
 from collections import OrderedDict
-from dataclasses import fields
 
 import networkx
 
 from canals.component import Component
 from canals.errors import PipelineConnectError, PipelineMaxLoops, PipelineRuntimeError, PipelineValidationError
-from canals.draw import draw, convert_for_debug, RenderingEngines
-from canals.pipeline.sockets import InputSocket, OutputSocket, find_input_sockets, find_output_sockets
-from canals.pipeline.validation import validate_pipeline_input
-from canals.pipeline.connections import parse_connection_name, find_unambiguous_connection, get_socket_type_desc
-
+from canals.pipeline.draw import _draw, _convert_for_debug, RenderingEngines
+from canals.pipeline.sockets import InputSocket, OutputSocket
+from canals.pipeline.validation import _validate_pipeline_input
+from canals.pipeline.connections import _parse_connection_name, _find_unambiguous_connection
+from canals.utils import _type_name
 
 logger = logging.getLogger(__name__)
 
 
 class Pipeline:
     """
     Components orchestration engine.
@@ -116,17 +115,19 @@
 
         # Component instances must be components
         if not hasattr(instance, "__canals_component__"):
             raise PipelineValidationError(
                 f"'{type(instance)}' doesn't seem to be a component. Is this class decorated with @component?"
             )
 
-        # Find inputs and outputs
-        input_sockets = find_input_sockets(instance)
-        output_sockets = find_output_sockets(instance)
+        # Create the component's input and output sockets
+        inputs = getattr(instance.run, "__canals_input__", {})
+        outputs = getattr(instance.run, "__canals_output__", {})
+        input_sockets = {name: InputSocket(**data) for name, data in inputs.items()}
+        output_sockets = {name: OutputSocket(**data) for name, data in outputs.items()}
 
         # Add component to the graph, disconnected
         logger.debug("Adding component '%s' (%s)", name, instance)
         self.graph.add_node(
             name,
             instance=instance,
             input_sockets=input_sockets,
@@ -150,16 +151,16 @@
             None
 
         Raises:
             PipelineConnectError: if the two components cannot be connected (for example if one of the components is
                 not present in the pipeline, or the connections don't match by type, and so on).
         """
         # Edges may be named explicitly by passing 'node_name.edge_name' to connect().
-        from_node, from_socket_name = parse_connection_name(connect_from)
-        to_node, to_socket_name = parse_connection_name(connect_to)
+        from_node, from_socket_name = _parse_connection_name(connect_from)
+        to_node, to_socket_name = _parse_connection_name(connect_to)
 
         # Get the nodes data.
         try:
             from_sockets = self.graph.nodes[from_node]["output_sockets"]
         except KeyError as exc:
             raise ValueError(f"Component named {from_node} not found in the pipeline.") from exc
 
@@ -171,34 +172,30 @@
         # If the name of either socket is given, get the socket
         if from_socket_name:
             from_socket = from_sockets.get(from_socket_name, None)
             if not from_socket:
                 raise PipelineConnectError(
                     f"'{from_node}.{from_socket_name} does not exist. "
                     f"Output connections of {from_node} are: "
-                    + ", ".join(
-                        [f"{name} (type {get_socket_type_desc(socket.type)})" for name, socket in from_sockets.items()]
-                    )
+                    + ", ".join([f"{name} (type {_type_name(socket.type)})" for name, socket in from_sockets.items()])
                 )
         if to_socket_name:
             to_socket = to_sockets.get(to_socket_name, None)
             if not to_socket:
                 raise PipelineConnectError(
                     f"'{to_node}.{to_socket_name} does not exist. "
                     f"Input connections of {to_node} are: "
-                    + ", ".join(
-                        [f"{name} (type {get_socket_type_desc(socket.type)})" for name, socket in to_sockets.items()]
-                    )
+                    + ", ".join([f"{name} (type {_type_name(socket.type)})" for name, socket in to_sockets.items()])
                 )
 
         # Look for an unambiguous connection among the possible ones.
         # Note that if there is more than one possible connection but two sockets match by name, they're paired.
         from_sockets = [from_socket] if from_socket_name else list(from_sockets.values())
         to_sockets = [to_socket] if to_socket_name else list(to_sockets.values())
-        from_socket, to_socket = find_unambiguous_connection(
+        from_socket, to_socket = _find_unambiguous_connection(
             sender_node=from_node, sender_sockets=from_sockets, receiver_node=to_node, receiver_sockets=to_sockets
         )
 
         # Connect the components on these sockets
         self._direct_connect(from_node=from_node, from_socket=from_socket, to_node=to_node, to_socket=to_socket)
 
     def _direct_connect(self, from_node: str, from_socket: OutputSocket, to_node: str, to_socket: InputSocket) -> None:
@@ -213,15 +210,22 @@
                 f"Cannot connect '{from_node}.{from_socket.name}' with '{to_node}.{to_socket.name}': "
                 f"{to_node}.{to_socket.name} is already connected to {to_socket.sender}.\n"
             )
 
         # Create the connection
         logger.debug("Connecting '%s.%s' to '%s.%s'", from_node, from_socket.name, to_node, to_socket.name)
         edge_key = f"{from_socket.name}/{to_socket.name}"
-        self.graph.add_edge(from_node, to_node, key=edge_key, from_socket=from_socket, to_socket=to_socket)
+        self.graph.add_edge(
+            from_node,
+            to_node,
+            key=edge_key,
+            conn_type=_type_name(from_socket.type),
+            from_socket=from_socket,
+            to_socket=to_socket,
+        )
 
         # Stores the name of the node that will send its output to this socket
         to_socket.sender = from_node
 
     def get_component(self, name: str) -> Component:
         """
         Returns an instance of a component.
@@ -253,15 +257,20 @@
         Returns:
             None
 
         Raises:
             ImportError: if `engine='graphviz'` and `pygraphviz` is not installed.
             HTTPConnectionError: (and similar) if the internet connection is down or other connection issues.
         """
-        draw(graph=deepcopy(self.graph), path=path, engine=engine)
+        sockets = {
+            comp: "\n".join([f"{name}: {socket}" for name, socket in data.get("input_sockets", {}).items()])
+            for comp, data in self.graph.nodes(data=True)
+        }
+        print(sockets)
+        _draw(graph=deepcopy(self.graph), path=path, engine=engine)
 
     def warm_up(self):
         """
         Make sure all nodes are warm.
 
         It's the node's responsibility to make sure this method can be called at every `Pipeline.run()`
         without re-initializing everything.
@@ -310,22 +319,22 @@
         # - Input nodes            # [e[0] for e in self.graph.in_edges(node)]
         # - Output nodes           # [e[1] for e in self.graph.out_edges(node)]
         # - Output edges           # [e[2]["label"] for e in self.graph.out_edges(node, data=True)]
         #
         # if debug:
         #     os.makedirs("debug", exist_ok=True)
 
-        data = validate_pipeline_input(self.graph, input_values=data)
+        data = _validate_pipeline_input(self.graph, input_values=data)
         self._clear_visits_count()
         self.warm_up()
 
         logger.info("Pipeline execution started.")
         inputs_buffer = OrderedDict(
             {
-                node: {key: value for key, value in input_data.__dict__.items() if value is not None}
+                node: {key: value for key, value in input_data.items() if value is not None}
                 for node, input_data in data.items()
             }
         )
         pipeline_output: Dict[str, Dict[str, Any]] = {}
 
         if debug:
             logger.info("Debug mode ON.")
@@ -399,15 +408,15 @@
         logger.info("Pipeline executed successfully.")
         return pipeline_output
 
     def _record_pipeline_step(self, step, inputs_buffer, pipeline_output):
         """
         Stores a snapshot of this step into the self.debug dictionary of the pipeline.
         """
-        mermaid_graph = convert_for_debug(deepcopy(self.graph))
+        mermaid_graph = _convert_for_debug(deepcopy(self.graph))
         self.debug[step] = {
             "time": datetime.datetime.now(),
             "inputs_buffer": list(inputs_buffer.items()),
             "pipeline_output": pipeline_output,
             "diagram": mermaid_graph,
         }
 
@@ -484,18 +493,21 @@
         input_components = {
             from_node: data["to_socket"].name for from_node, _, data in self.graph.in_edges(name, data=True)
         }
         # Sockets that have received inputs from upstream components
         received_input_sockets = set(inputs.keys())
 
         # All components inputs, whether they're connected, default or pipeline inputs
-        instance = self.graph.nodes[name]["instance"]
-        input_sockets = {f.name for f in fields(instance.__canals_input__)}
-        optional_input_sockets = set(instance.__canals_optional_inputs__)
-        mandatory_input_sockets = set(instance.__canals_mandatory_inputs__)
+        input_sockets: Dict[str, InputSocket] = self.graph.nodes[name]["input_sockets"].keys()
+        optional_input_sockets = {
+            socket.name for socket in self.graph.nodes[name]["input_sockets"].values() if socket.is_optional
+        }
+        mandatory_input_sockets = {
+            socket.name for socket in self.graph.nodes[name]["input_sockets"].values() if not socket.is_optional
+        }
 
         # Components that are in the inputs buffer and have no inputs assigned are considered skipped
         skipped_components = {n for n, v in inputs_buffer.items() if not v}
 
         # Sockets that have their upstream component marked as skipped
         skipped_optional_input_sockets = {
             sockets["to_socket"].name
@@ -617,34 +629,34 @@
         """
         self.graph.nodes[name]["visits"] += 1
         instance = self.graph.nodes[name]["instance"]
         try:
             logger.info("* Running %s (visits: %s)", name, self.graph.nodes[name]["visits"])
             logger.debug("   '%s' inputs: %s", name, inputs)
 
-            # Optional fields are defaulted to None so creation of the input dataclass doesn't fail
-            # cause we're missing some argument
-            optionals = {field: None for field in instance.__canals_optional_inputs__}
+            # # Optional fields are defaulted to None so creation of the input dataclass doesn't fail
+            # # cause we're missing some argument
+            # optionals = {field: None for field in instance.__canals_optional_inputs__}
 
             # Pass the inputs as kwargs after adding the component's own defaults to them
-            inputs = {**optionals, **instance.defaults, **inputs}
-            input_dataclass = instance.input(**inputs)
+            # inputs = {**optionals, **instance.defaults, **inputs}
+            # input_dataclass = instance.input(**inputs)
 
-            output_dataclass = instance.run(input_dataclass)
+            outputs = instance.run(**inputs)
 
             # Unwrap the output
-            logger.debug("   '%s' outputs: %s\n", name, output_dataclass.__dict__)
+            logger.debug("   '%s' outputs: %s\n", name, outputs)
 
         except Exception as e:
             raise PipelineRuntimeError(
                 f"{name} raised '{e.__class__.__name__}: {e}' \nInputs: {inputs}\n\n"
                 "See the stacktrace above for more information."
             ) from e
 
-        return output_dataclass
+        return outputs
 
     def _route_output(
         self,
         node_name: str,
         node_results: Dict[str, Any],
         inputs_buffer: OrderedDict,
     ) -> OrderedDict:
@@ -661,15 +673,15 @@
         for edge_data in self.graph.out_edges(node_name, data=True):
             to_socket = edge_data[2]["to_socket"]
             from_socket = edge_data[2]["from_socket"]
             target_node = edge_data[1]
 
             # If this is a decision node and a loop is involved, we add to the input buffer only the nodes
             # that received their expected output and we leave the others out of the queue.
-            if is_decision_node_for_loop and getattr(node_results, from_socket.name) is None:
+            if is_decision_node_for_loop and node_results.get(from_socket.name, None) is None:
                 if networkx.has_path(self.graph, target_node, node_name):
                     # In case we're choosing to leave a loop, do not put the loop's node in the buffer.
                     logger.debug(
                         "Not adding '%s' to the inputs buffer: we're leaving the loop.",
                         target_node,
                     )
                 else:
@@ -680,12 +692,12 @@
                     )
             else:
                 # In all other cases, populate the inputs buffer for all downstream nodes, setting None to any
                 # edge that did not receive input.
                 if target_node not in inputs_buffer:
                     inputs_buffer[target_node] = {}  # Create the buffer for the downstream node if it's not there yet
 
-                value_to_route = getattr(node_results, from_socket.name, None)
+                value_to_route = node_results.get(from_socket.name, None)
                 if value_to_route:
                     inputs_buffer[target_node][to_socket.name] = value_to_route
 
         return inputs_buffer
```

### Comparing `canals-0.3.2/canals/pipeline/save_load.py` & `canals-0.4.0/canals/pipeline/save_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # pylint: disable=protected-access
 
 from typing import Dict, List, Any, Tuple
 import json
 import logging
 from pathlib import Path
 
-from canals.component import component, Component
+from canals.component.component import component
 from canals.pipeline.pipeline import Pipeline
 from canals.errors import PipelineUnmarshalError
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -66,15 +66,15 @@
     Returns:
         A Python dictionary representing the Pipelines objects above, that can be written to JSON and can be reused to
         recreate the original Pipelines.
     """
     schema: Dict[str, Any] = {}
 
     # Summarize pipeline configuration
-    components: List[Tuple[str, str, Component]] = []
+    components: List[Tuple[str, str, Any]] = []
     schema["pipelines"] = {}
     for pipeline_name, pipeline in pipelines.items():
         pipeline_repr: Dict[str, Any] = {}
         pipeline_repr["metadata"] = pipeline.metadata
         pipeline_repr["max_loops_allowed"] = pipeline.max_loops_allowed
 
         # Collect components
@@ -118,15 +118,15 @@
     Returns:
         The pipelines as a dictionary of `{"pipeline-name": <pipeline object>}`.
 
     Raises PipelineUnmarshalError: if any Component class has not been imported before loading.
 
     """
     pipelines = {}
-    component_instances: Dict[str, Component] = {}
+    component_instances: Dict[str, Any] = {}
     for pipeline_name, pipeline_schema in schema["pipelines"].items():
         # Create the Pipeline object
         pipe_args = {"metadata": pipeline_schema.get("metadata", None)}
         if "max_loops_allowed" in pipeline_schema.keys():
             pipe_args["max_loops_allowed"] = pipeline_schema["max_loops_allowed"]
         pipe = Pipeline(**pipe_args)
```

### Comparing `canals-0.3.2/canals/pipeline/validation.py` & `canals-0.4.0/canals/pipeline/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from typing import List, Dict, Any
 import logging
-from dataclasses import fields
 
 import networkx
 
 from canals.errors import PipelineValidationError
 from canals.pipeline.sockets import InputSocket, OutputSocket
 
 
 logger = logging.getLogger(__name__)
 
 
-def find_pipeline_inputs(graph: networkx.MultiDiGraph) -> Dict[str, List[InputSocket]]:
+def _find_pipeline_inputs(graph: networkx.MultiDiGraph) -> Dict[str, List[InputSocket]]:
     """
     Collect components that have disconnected input sockets. Note that this method returns *ALL* disconnected
     input sockets, including all such sockets with default values.
     """
     return {
-        node: [socket for socket in data.get("input_sockets", {}).values() if not socket.sender]
-        for node, data in graph.nodes(data=True)
+        name: [socket for socket in data.get("input_sockets", {}).values() if not socket.sender]
+        for name, data in graph.nodes(data=True)
     }
 
 
-def find_pipeline_outputs(graph) -> Dict[str, List[OutputSocket]]:
+def _find_pipeline_outputs(graph) -> Dict[str, List[OutputSocket]]:
     """
     Collect components that have disconnected output sockets. They define the pipeline output.
     """
     return {
         node: list(data.get("output_sockets", {}).values())
         for node, data in graph.nodes(data=True)
         if not graph.out_edges(node)
     }
 
 
-def validate_pipeline_input(graph: networkx.MultiDiGraph, input_values: Dict[str, Any]) -> Dict[str, Any]:
+def _validate_pipeline_input(graph: networkx.MultiDiGraph, input_values: Dict[str, Any]) -> Dict[str, Any]:
     """
     Make sure the pipeline is properly built and that the input received makes sense.
     Returns the input values, validated and updated at need.
     """
-    if not any(sockets for sockets in find_pipeline_inputs(graph).values()):
+    if not any(sockets for sockets in _find_pipeline_inputs(graph).values()):
         raise PipelineValidationError("This pipeline has no inputs.")
 
     # Make sure the input keys are all nodes of the pipeline
     unknown_components = [key for key in input_values.keys() if not key in graph.nodes]
     if unknown_components:
         raise ValueError(f"Pipeline received data for unknown component(s): {', '.join(unknown_components)}")
 
@@ -59,37 +58,35 @@
 
 
 def _validate_input_sockets_are_connected(graph: networkx.MultiDiGraph, input_values: Dict[str, Any]):
     """
     Make sure all the inputs nodes are receiving all the values they need, either from the Pipeline's input or from
     other nodes.
     """
-    valid_inputs = find_pipeline_inputs(graph)
+    valid_inputs = _find_pipeline_inputs(graph)
     for node, sockets in valid_inputs.items():
         for socket in sockets:
-            node_instance = graph.nodes[node]["instance"]
-            input_in_node_defaults = hasattr(node_instance, "defaults") and socket.name in node_instance.defaults
-            inputs_for_node = input_values.get(node)
+            inputs_for_node = input_values.get(node, {})
             missing_input_value = (
                 not inputs_for_node
-                or not socket.name in [f.name for f in fields(inputs_for_node)]
-                or not getattr(inputs_for_node, socket.name)
+                or not socket.name in inputs_for_node.keys()
+                or not inputs_for_node.get(socket.name, None)
             )
-            if missing_input_value and not input_in_node_defaults:
+            if missing_input_value and not socket.is_optional:
                 raise ValueError(f"Missing input: {node}.{socket.name}")
 
 
 def _validate_nodes_receive_only_expected_input(graph: networkx.MultiDiGraph, input_values: Dict[str, Any]):
     """
     Make sure that every input node is only receiving input values from EITHER the pipeline's input or another node,
     but never from both.
     """
     for node, input_data in input_values.items():
-        for socket_name in [f.name for f in fields(input_data)]:
-            if not getattr(input_data, socket_name):
+        for socket_name in input_data.keys():
+            if not input_data.get(socket_name, None):
                 continue
             if not socket_name in graph.nodes[node]["input_sockets"].keys():
                 raise ValueError(
                     f"Component {node} is not expecting any input value called {socket_name}. "
                     "Are you using the correct Input class?"
                 )
```

### Comparing `canals-0.3.2/canals/testing/test_component.py` & `canals-0.4.0/canals/testing/test_component.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.2/.gitignore` & `canals-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.3.2/LICENSE` & `canals-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.3.2/README.md` & `canals-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `canals-0.3.2/pyproject.toml` & `canals-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,100 +5,90 @@
 [project]
 name = "canals"
 description = 'A component orchestration engine for Haystack'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
-authors = [
-  { name = "ZanSara", email = "sara.zanzottera@deepset.ai" },
-]
+authors = [{ name = "ZanSara", email = "sara.zanzottera@deepset.ai" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: Freely Distributable",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
 dependencies = [
-  "networkx",  # Pipeline graphs
+  "networkx", # Pipeline graphs
+
 ]
 
 [project.optional-dependencies]
 graphviz = [
   "pygraphviz", # Draw pipelines (requires the 'graphviz' system library)
+
 ]
 mermaid = [
   "requests", # Draw pipelines (requires internet connectivity)
+
 ]
 dev = [
   "hatch",
   "pre-commit",
   "mypy",
   "pylint==2.15.10",
   "black[jupyter]==22.6.0",
   "pytest",
   "pytest-cov",
   "requests",
   "coverage",
 ]
-docs = [
-  "mkdocs-material",
-  "mkdocstrings[python]",
-  "mkdocs-mermaid2-plugin"
-]
-
+docs = ["mkdocs-material", "mkdocstrings[python]", "mkdocs-mermaid2-plugin"]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/canals#readme"
 Issues = "https://github.com/deepset-ai/canals/issues"
 Source = "https://github.com/deepset-ai/canals"
 
 [tool.hatch.version]
 path = "canals/__about__.py"
 
+[tool.hatch.build]
+include = ["/canals/**/*.py"]
+
 [tool.hatch.envs.default]
-dependencies = [
-  "pytest",
-  "pytest-cov",
-  "requests",
-]
+dependencies = ["pytest", "pytest-cov", "requests"]
+
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report xml:coverage.xml --cov-config=pyproject.toml --cov=canals --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
-omit = [
-  "canals/__about__.py",
-]
+omit = ["canals/__about__.py"]
 
 [tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.black]
 line-length = 120
 
 [tool.pylint.'MESSAGES CONTROL']
-max-line-length=120
-good-names="e"
-max-args=10
+max-line-length = 120
+good-names = "e"
+max-args = 10
 disable = [
   "fixme",
   "line-too-long",
   "missing-class-docstring",
   "missing-module-docstring",
 ]
```

### Comparing `canals-0.3.2/PKG-INFO` & `canals-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.3.2
+Version: 0.4.0
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: canals Version: 0.3.2 Summary: A component
+Metadata-Version: 2.1 Name: canals Version: 0.4.0 Summary: A component
 orchestration engine for Haystack Project-URL: Documentation, https://
 github.com/deepset-ai/canals#readme Project-URL: Issues, https://github.com/
 deepset-ai/canals/issues Project-URL: Source, https://github.com/deepset-ai/
 canals Author-email: ZanSara
 zanzottera@deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: License :: Freely
 Distributable Classifier: License :: OSI Approved :: Apache Software License
```

