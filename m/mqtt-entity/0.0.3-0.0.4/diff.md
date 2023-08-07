# Comparing `tmp/mqtt-entity-0.0.3.tar.gz` & `tmp/mqtt-entity-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-entity-0.0.3.tar", last modified: Fri May 19 12:44:55 2023, max compression
+gzip compressed data, was "mqtt-entity-0.0.4.tar", last modified: Mon Aug  7 17:53:52 2023, max compression
```

## Comparing `mqtt-entity-0.0.3.tar` & `mqtt-entity-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/mqtt_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/mqtt_entity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:52.873280 mqtt-entity-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-07 17:53:52.873280 mqtt-entity-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:52.869280 mqtt-entity-0.0.4/mqtt_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/mqtt_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/mqtt_entity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/mqtt_entity/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/mqtt_entity/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/mqtt_entity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:52.869280 mqtt-entity-0.0.4/mqtt_entity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-07 17:53:52.000000 mqtt-entity-0.0.4/mqtt_entity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-07 17:53:52.000000 mqtt-entity-0.0.4/mqtt_entity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:53:52.000000 mqtt-entity-0.0.4/mqtt_entity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-07 17:53:52.000000 mqtt-entity-0.0.4/mqtt_entity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 17:53:52.000000 mqtt-entity-0.0.4/mqtt_entity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:53:52.000000 mqtt-entity-0.0.4/mqtt_entity.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-07 17:53:52.873280 mqtt-entity-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:52.873280 mqtt-entity-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-07 17:53:40.000000 mqtt-entity-0.0.4/tests/test_helpers.py
```

### Comparing `mqtt-entity-0.0.3/LICENSE` & `mqtt-entity-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.3/PKG-INFO` & `mqtt-entity-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-entity
-Version: 0.0.3
+Version: 0.0.4
 Summary: MQTT client to manage Home Assistant entities via MQTT
 Home-page: https://github.com/kellerza/mqtt-entity/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: home-assistant,mqtt,library,discovery,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mqtt-entity-0.0.3/README.md` & `mqtt-entity-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.3/mqtt_entity/client.py` & `mqtt-entity-0.0.4/mqtt_entity/client.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.3/mqtt_entity/entities.py` & `mqtt-entity-0.0.4/mqtt_entity/entities.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,36 +59,47 @@
     unit_of_measurement: str = attrs.field(default="")
     state_class: str = attrs.field(default="")
     expire_after: int = attrs.field(default=0)
     """Unavailable if not updated."""
     enabled_by_default: bool = attrs.field(default=True)
     entity_category: str = attrs.field(default="")
     icon: str = attrs.field(default="")
-    attributes_topic: str = attrs.field(default="")
+    json_attributes_topic: str = attrs.field(default="")
     """Used by the set_attributes helper."""
 
+    discovery_extra: dict[str, Any] = attrs.field(factory=dict)
+    """Additional MQTT Discovery attributes."""
+
     _path = ""
 
     def __attrs_post_init__(self) -> None:
         """Init the class."""
         if not self._path:
             raise TypeError(f"Do not instantiate {self.__class__.__name__} directly")
         if not self.state_class and self.device_class == "energy":
             self.state_class = "total_increasing"
 
     @property
-    def asdict(self) -> dict:
+    def asdict(self) -> dict[str, Any]:
         """Represent the entity as a dictionary, without empty values and defaults."""
 
         def _filter(atrb: attrs.Attribute, value: Any) -> bool:
+            if atrb.name == "discovery_extra":
+                return False
             return (
                 bool(value) and atrb.default != value and not inspect.isfunction(value)
             )
 
-        return attrs.asdict(self, filter=_filter)
+        res = attrs.asdict(self, filter=_filter)
+        for key in self.discovery_extra:
+            if key in res and res[key] != self.discovery_extra[key]:
+                _LOGGER.debug("Overwriting %s with %s", key, self.discovery_extra[key])
+        res.update(self.discovery_extra)
+
+        return res
 
     @property
     def topic(self) -> str:
         """Discovery topic."""
         uid, did = self.unique_id, self.device.id
         if uid.startswith(did):
             uid = uid[len(did) :].strip("_")
```

### Comparing `mqtt-entity-0.0.3/mqtt_entity/helpers.py` & `mqtt-entity-0.0.4/mqtt_entity/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,14 @@
     attributes: dict[str, Any],
     *,
     entity: Entity,
     client: MQTTClient,
     retain: bool = False,
 ) -> None:
     """Set attributes helper."""
-    if not entity.attributes_topic:
-        raise ValueError(f"Entity '{entity.name}' needs an attributes_topic.")
+    if not entity.json_attributes_topic:
+        raise ValueError(f"Entity '{entity.name}' needs an json_attributes_topic.")
     await client.publish(
-        topic=entity.attributes_topic,
+        topic=entity.json_attributes_topic,
         payload=dumps(attributes),
         retain=retain,
     )
```

### Comparing `mqtt-entity-0.0.3/mqtt_entity/utils.py` & `mqtt-entity-0.0.4/mqtt_entity/utils.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.3/mqtt_entity.egg-info/PKG-INFO` & `mqtt-entity-0.0.4/mqtt_entity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-entity
-Version: 0.0.3
+Version: 0.0.4
 Summary: MQTT client to manage Home Assistant entities via MQTT
 Home-page: https://github.com/kellerza/mqtt-entity/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: home-assistant,mqtt,library,discovery,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mqtt-entity-0.0.3/setup.cfg` & `mqtt-entity-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.3/tests/conftest.py` & `mqtt-entity-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.3/tests/test_client.py` & `mqtt-entity-0.0.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.3/tests/test_entities.py` & `mqtt-entity-0.0.4/tests/test_entities.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,7 +65,35 @@
         "unique_id": "789",
         "device": {"identifiers": ["123"]},
         "availability": [{"topic": "/blah"}],
         "state_topic": "/test/a",
     }
 
     assert ent.topic == "homeassistant/sensor/123/789/config"
+
+
+def discovery_extra():
+    """Test discovery_extra."""
+    dev = Device(identifiers=["123"])
+
+    ava = Availability(topic="/blah")
+
+    ent = SensorEntity(
+        name="test1",
+        unique_id="789",
+        device=dev,
+        availability=[ava],
+        state_topic="/test/a",
+        json_attributes_topic="/test/f",
+        discovery_extra={"a": "b", "state_topic": "c"},
+    )
+    assert ent.asdict == {
+        "name": "test1",
+        "unique_id": "789",
+        "device": {"identifiers": ["123"]},
+        "availability": [{"topic": "/blah"}],
+        "json_attributes_topic": "/test/f",
+        "state_topic": "c",
+        "a": "b",
+    }
+
+    assert ent.topic == "homeassistant/sensor/123/789/config"
```

### Comparing `mqtt-entity-0.0.3/tests/test_helpers.py` & `mqtt-entity-0.0.4/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 @pytest.mark.asyncio
 async def test_set_attributes():
     """Test set_attributes."""
     dev = Device(identifiers=["test123"])
     e = SensorEntity(
-        attributes_topic="blah",
+        json_attributes_topic="blah",
         unique_id="a1",
         device=dev,
         state_topic="/st",
         name="test1",
     )
     mc = AsyncMock()
     thea = {"the": "attr"}
```

