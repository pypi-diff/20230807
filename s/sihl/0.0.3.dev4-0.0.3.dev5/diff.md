# Comparing `tmp/sihl-0.0.3.dev4.tar.gz` & `tmp/sihl-0.0.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.3.dev4.tar", max compression
+gzip compressed data, was "sihl-0.0.3.dev5.tar", max compression
```

## Comparing `sihl-0.0.3.dev4.tar` & `sihl-0.0.3.dev5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-08-01 15:49:47.829813 sihl-0.0.3.dev4/LICENSE
--rw-r--r--   0        0        0      894 2023-08-01 15:49:47.829813 sihl-0.0.3.dev4/README.md
--rw-r--r--   0        0        0     1568 2023-08-01 15:50:01.426070 sihl-0.0.3.dev4/pyproject.toml
--rw-r--r--   0        0        0   402648 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/NotoSansMono-Bold.ttf
--rw-r--r--   0        0        0      448 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/__init__.py
--rw-r--r--   0        0        0      289 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     3202 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     3884 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     4748 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0    14319 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/object_detection.py
--rw-r--r--   0        0        0      189 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/layers/__init__.py
--rw-r--r--   0        0        0     1553 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/layers/convblocks.py
--rw-r--r--   0        0        0     2711 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/layers/fpn.py
--rw-r--r--   0        0        0      514 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/layers/scalers.py
--rw-r--r--   0        0        0     5215 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/lightning_module.py
--rw-r--r--   0        0        0      549 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/sihl_model.py
--rw-r--r--   0        0        0     2797 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/timm_backbone.py
--rw-r--r--   0        0        0     6509 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1740 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/utils.py
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-07 00:26:21.459815 sihl-0.0.3.dev5/LICENSE
+-rw-r--r--   0        0        0      894 2023-08-07 00:26:21.459815 sihl-0.0.3.dev5/README.md
+-rw-r--r--   0        0        0     1568 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/pyproject.toml
+-rw-r--r--   0        0        0   402648 2023-08-07 00:26:21.463815 sihl-0.0.3.dev5/src/sihl/NotoSansMono-Bold.ttf
+-rw-r--r--   0        0        0      448 2023-08-07 00:26:21.463815 sihl-0.0.3.dev5/src/sihl/__init__.py
+-rw-r--r--   0        0        0      289 2023-08-07 00:26:21.463815 sihl-0.0.3.dev5/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     3241 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     3962 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     4942 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0    14319 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/heads/object_detection.py
+-rw-r--r--   0        0        0      189 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/__init__.py
+-rw-r--r--   0        0        0     1553 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/convblocks.py
+-rw-r--r--   0        0        0     2711 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/fpn.py
+-rw-r--r--   0        0        0      514 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/scalers.py
+-rw-r--r--   0        0        0     5215 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0      549 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/sihl_model.py
+-rw-r--r--   0        0        0     2797 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/timm_backbone.py
+-rw-r--r--   0        0        0     6509 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1740 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/utils.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev5/PKG-INFO
```

### Comparing `sihl-0.0.3.dev4/LICENSE` & `sihl-0.0.3.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/README.md` & `sihl-0.0.3.dev5/README.md`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/pyproject.toml` & `sihl-0.0.3.dev5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.3-dev4"
+version = "0.0.3-dev5"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
```

### Comparing `sihl-0.0.3.dev4/src/sihl/NotoSansMono-Bold.ttf` & `sihl-0.0.3.dev5/src/sihl/NotoSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/heads/binary_classification.py` & `sihl-0.0.3.dev5/src/sihl/heads/binary_classification.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,34 +26,35 @@
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores = torch.sigmoid(self.net(inputs[self.level])).squeeze(-1)
         return scores, scores > 0.5
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[self.level]).squeeze(-1).float()
+        logits = self.net(inputs[self.level]).squeeze(-1)
         labels = labels.to(logits.dtype).to(logits.device)
         loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, labels)
         return loss, {}
 
     def on_validation_start(self) -> None:
         self.accuracy_computer = torchmetrics.classification.BinaryAccuracy()
         self.precision_computer = torchmetrics.classification.BinaryPrecision()
         self.recall_computer = torchmetrics.classification.BinaryRecall()
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        input = inputs[self.level]
-        logits = self.net(input).squeeze(-1).float()
+        logits = self.net(inputs[self.level]).squeeze(-1)
         labels = labels.to(logits.dtype).to(logits.device)
         loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, labels)
-        self.accuracy_computer.to(input.device).update(logits, labels)
-        self.precision_computer.to(input.device).update(logits, labels)
-        self.recall_computer.to(input.device).update(logits, labels)
+        logits = logits.detach().float()
+        labels = labels.detach()
+        self.accuracy_computer.to(logits.device).update(logits, labels)
+        self.precision_computer.to(logits.device).update(logits, labels)
+        self.recall_computer.to(logits.device).update(logits, labels)
         return loss, {}
 
     def on_validation_end(self) -> dict[str, float]:
         return {
             "accuracy": self.accuracy_computer.compute().item(),
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
```

### Comparing `sihl-0.0.3.dev4/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.3.dev5/src/sihl/heads/multiclass_classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         label_weights: tuple[float, ...] | None = None,
         label_smoothing: float = 0.0,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.level = level
         self.class_names = class_names or tuple(str(_) for _ in range(num_classes))
+        assert len(self.class_names) == self.num_classes
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.label_smoothing = label_smoothing
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1),
             nn.Flatten(),
             nn.Linear(in_channels[self.level], num_classes),
         )
@@ -43,43 +44,43 @@
             torch.nn.functional.softmax(self.net(inputs[self.level]), dim=1), dim=1
         )
         return scores, classes
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[self.level]).float()
+        logits = self.net(inputs[self.level])
         loss = torch.nn.functional.cross_entropy(
             logits,
             labels.to(logits.device),
             weight=self.label_weights,
             label_smoothing=self.label_smoothing,
         )
         return loss, {}
 
     def on_validation_start(self) -> None:
-        self.accuracy_computer = MulticlassAccuracy(num_classes=self.num_classes)
-        self.precision_computer = MulticlassPrecision(num_classes=self.num_classes)
-        self.recall_computer = MulticlassRecall(num_classes=self.num_classes)
+        self.accuracy_computer = MulticlassAccuracy(self.num_classes, average="micro")
+        self.precision_computer = MulticlassPrecision(self.num_classes, average="micro")
+        self.recall_computer = MulticlassRecall(self.num_classes, average="micro")
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        input = inputs[self.level]
-        logits = self.net(input).float()
+        logits = self.net(inputs[self.level])
         labels = labels.to(logits.device)
         loss = torch.nn.functional.cross_entropy(
             logits,
             labels,
             weight=self.label_weights,
             label_smoothing=self.label_smoothing,
         )
-        self.accuracy_computer.to(input.device).update(logits, labels)
-        self.precision_computer.to(input.device).update(logits, labels)
-        self.recall_computer.to(input.device).update(logits, labels)
+        logits = logits.detach().float()
+        self.accuracy_computer.to(logits.device).update(logits, labels)
+        self.precision_computer.to(logits.device).update(logits, labels)
+        self.recall_computer.to(logits.device).update(logits, labels)
         return loss, {}
 
     def on_validation_end(self) -> dict[str, float]:
         return {
             "accuracy": self.accuracy_computer.compute().item(),
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
```

### Comparing `sihl-0.0.3.dev4/src/sihl/heads/multilabel_classification.py` & `sihl-0.0.3.dev5/src/sihl/heads/multilabel_classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         class_names: tuple[str, ...] | None = None,
         label_weights: list[float] | None = None,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.level = level
         self.class_names = class_names or tuple(str(_) for _ in range(num_classes))
+        assert len(self.class_names) == self.num_classes
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1),
             nn.Flatten(),
             nn.Linear(in_channels[self.level], num_classes),
         )
 
@@ -41,37 +42,41 @@
             torch.sigmoid(self.net(inputs[self.level])), descending=True
         )
         return scores, classes
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[self.level]).float()
+        logits = self.net(inputs[self.level])
         loss = torch.nn.functional.binary_cross_entropy_with_logits(
-            logits, labels.to(logits.device), pos_weight=self.label_weights
+            logits,
+            labels.to(logits.device).to(logits.dtype),
+            pos_weight=self.label_weights,
         )
         return loss, {}
 
     def on_validation_start(self) -> None:
-        self.accuracy_computer = MultilabelAccuracy(num_labels=self.num_classes)
-        self.precision_computer = MultilabelPrecision(num_labels=self.num_classes)
-        self.recall_computer = MultilabelRecall(num_labels=self.num_classes)
+        self.accuracy_computer = MultilabelAccuracy(self.num_classes, average="micro")
+        self.precision_computer = MultilabelPrecision(self.num_classes, average="micro")
+        self.recall_computer = MultilabelRecall(self.num_classes, average="micro")
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
-        logits = self.net(input).float()
-        labels = labels.to(logits.device)
+        logits = self.net(input)
+        labels = labels.to(logits.device).to(logits.dtype)
         loss = torch.nn.functional.binary_cross_entropy_with_logits(
             logits, labels, pos_weight=self.label_weights
         )
-        self.accuracy_computer.to(input.device).update(logits, labels)
-        self.precision_computer.to(input.device).update(logits, labels)
-        self.recall_computer.to(input.device).update(logits, labels)
+        logits = logits.detach().float()
+        labels = labels.float()
+        self.accuracy_computer.to(logits.device).update(logits, labels)
+        self.precision_computer.to(logits.device).update(logits, labels)
+        self.recall_computer.to(logits.device).update(logits, labels)
         return loss, {}
 
     def on_validation_end(self) -> dict[str, float]:
         return {
             "accuracy": self.accuracy_computer.compute().item(),
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
```

### Comparing `sihl-0.0.3.dev4/src/sihl/heads/object_detection.py` & `sihl-0.0.3.dev5/src/sihl/heads/object_detection.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/layers/convblocks.py` & `sihl-0.0.3.dev5/src/sihl/layers/convblocks.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/layers/fpn.py` & `sihl-0.0.3.dev5/src/sihl/layers/fpn.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/layers/scalers.py` & `sihl-0.0.3.dev5/src/sihl/layers/scalers.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/lightning_module.py` & `sihl-0.0.3.dev5/src/sihl/lightning_module.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/sihl_model.py` & `sihl-0.0.3.dev5/src/sihl/sihl_model.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/timm_backbone.py` & `sihl-0.0.3.dev5/src/sihl/timm_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/torchvision_backbone.py` & `sihl-0.0.3.dev5/src/sihl/torchvision_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/src/sihl/utils.py` & `sihl-0.0.3.dev5/src/sihl/utils.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev4/PKG-INFO` & `sihl-0.0.3.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.3.dev4
+Version: 0.0.3.dev5
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

