# Comparing `tmp/agent_protocol-0.1.2.tar.gz` & `tmp/agent_protocol-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_protocol-0.1.2.tar", max compression
+gzip compressed data, was "agent_protocol-0.2.0.tar", max compression
```

## Comparing `agent_protocol-0.1.2.tar` & `agent_protocol-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     2398 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/README.md
--rw-r--r--   0        0        0       76 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/__init__.py
--rw-r--r--   0        0        0     4007 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/agent.py
--rw-r--r--   0        0        0      600 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/cli.py
--rw-r--r--   0        0        0      202 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/dependencies.py
--rw-r--r--   0        0        0     1683 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/models.py
--rw-r--r--   0        0        0      329 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/server.py
--rw-r--r--   0        0        0        0 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/__init__.py
--rw-r--r--   0        0        0       35 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/compliance/__init__.py
--rw-r--r--   0        0        0      449 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/compliance/conftest.py
--rw-r--r--   0        0        0     3426 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/compliance/main.py
--rw-r--r--   0        0        0      804 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 agent_protocol-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3009 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/README.md
+-rw-r--r--   0        0        0      353 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/__init__.py
+-rw-r--r--   0        0        0     5052 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/agent.py
+-rw-r--r--   0        0        0      600 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/cli.py
+-rw-r--r--   0        0        0     3592 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/db.py
+-rw-r--r--   0        0        0     2319 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/models.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/router.py
+-rw-r--r--   0        0        0      331 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/server.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/compliance/__init__.py
+-rw-r--r--   0        0        0      449 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/compliance/conftest.py
+-rw-r--r--   0        0        0     3754 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/compliance/main.py
+-rw-r--r--   0        0        0      804 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 agent_protocol-0.2.0/PKG-INFO
```

### Comparing `agent_protocol-0.1.2/README.md` & `agent_protocol-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,36 +7,69 @@
 ```sh
 pip install agent-protocol
 ```
 
 Then add the following code to your agent:
 
 ```python
-from agent_protocol import (
-    Agent,
-    StepResult,
-    StepHandler,
-)
-
-async def task_handler(task_input) -> StepHandler:
-    # TODO: Initialize code for the agent task.
-    async def step_handler(step_input) -> StepResult:
-        # TODO: Execute code for the agent step.
-        # The step could for example be a single iteration of a ReAct loop.
-
-        # TODO: Return the result of the step.
-        return StepResult(
-            output=...,
-        )
+from agent_protocol import Agent, Step, Task
+
+
+async def task_handler(task: Task) -> None:
+    # TODO: Create initial step(s) for the task
+    await Agent.db.create_step(task.task_id, ...)
+
+
+async def step_handler(step: Step) -> Step:
+    # TODO: handle next step
+    if step.name == "print":
+        print(step.input)
+        step.is_last = True
+
+    step.output = "Output from the agent"
+    return step
 
-    return step_handler
 
 if __name__ == "__main__":
     # Add the task handler and start the server
-    Agent.handle_task(task_handler).start()
+    Agent.setup_agent(task_handler, step_handler).start()
+```
+
+## Customization
+
+### Database
+
+By default the SDK stores data in memory. You can customize the database by setting db to your own database object.
+
+```python
+Agent.db = your_database
+```
+
+The database object must implement the methods from [db.py](./agent/python/db.py).
+
+### Routes
+
+You can also add your own routes to the server. For example:
+
+```python
+from agent_protocol import Agent, router
+from fastapi import APIRouter
+
+my_router = APIRouter()
+
+
+@my_router.get("/hello")
+async def hello():
+    return {"hello": "world"}
+
+my_router.include_router(router)
+
+task_handler = ...
+step_handler = ...
+Agent.setup_agent(task_handler, step_handler).start(router=my_router)
 ```
 
 ## Usage
 
 To start the server run the file where you added the code above:
 
 ```sh
@@ -83,14 +116,15 @@
   "input": null,
   "task_id": "e6d768bb-4c50-4007-9853-aeffb46c77be",
   "step_id": "8ff8ba39-2c3e-4246-8086-fbd2a897240b"
 }
 ```
 
 ## Test compliance
+
 Part of the package is also a test suite that can be used to test compliance with the protocol. To run the tests, run the following command:
 
 ```sh
 agent-protocol test --url <url>
 ```
 
 In the background it uses pytest, you can pass any pytest arguments to the command above.
```

### Comparing `agent_protocol-0.1.2/agent_protocol/cli.py` & `agent_protocol-0.2.0/agent_protocol/cli.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.1.2/agent_protocol/models.py` & `agent_protocol-0.2.0/agent_protocol/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # generated by fastapi-codegen:
-#   filename:  ../openapi.yml
-#   timestamp: 2023-07-19T12:37:58+00:00
+#   filename:  ../../openapi.yml
+#   timestamp: 2023-08-07T12:14:43+00:00
 
 from __future__ import annotations
 
+from enum import Enum
 from typing import Any, List, Optional
 
 from pydantic import BaseModel, Field
 
 
 class TaskInput(BaseModel):
     __root__: Any = Field(
         ..., description="Input parameters for the task. Any value is allowed."
     )
 
 
 class Artifact(BaseModel):
-    __root__: Any = Field(
-        ..., description="Artifact that the task has produced. Any value is allowed."
+    artifact_id: str = Field(..., description="ID of the artifact.")
+    file_name: str = Field(..., description="Filename of the artifact.")
+    relative_path: Optional[str] = Field(
+        None, description="Relative path of the artifact in the agent's workspace."
     )
 
 
 class StepInput(BaseModel):
     __root__: Any = Field(
         ..., description="Input parameters for the task step. Any value is allowed."
     )
@@ -30,34 +33,41 @@
 class StepOutput(BaseModel):
     __root__: Any = Field(
         ..., description="Output that the task step has produced. Any value is allowed."
     )
 
 
 class TaskRequestBody(BaseModel):
-    input: Optional[TaskInput] = None
+    input: Optional[str] = Field(None, description="Input prompt for the task.")
+    additional_input: Optional[TaskInput] = None
 
 
 class Task(TaskRequestBody):
     task_id: str = Field(..., description="The ID of the task.")
-    artifacts: Optional[List[Artifact]] = Field(
+    artifacts: List[Artifact] = Field(
         [], description="A list of artifacts that the task has produced."
     )
 
 
 class StepRequestBody(BaseModel):
-    input: Optional[StepInput]
+    input: Optional[str] = Field(None, description="Input prompt for the step.")
+    additional_input: Optional[StepInput] = None
+
+
+class Status(Enum):
+    created = "created"
+    completed = "completed"
 
 
-class StepResult(BaseModel):
-    output: Optional[StepOutput]
-    artifacts: Optional[List[Artifact]] = Field(
+class Step(StepRequestBody):
+    task_id: str = Field(..., description="The ID of the task this step belongs to.")
+    step_id: str = Field(..., description="The ID of the task step.")
+    name: Optional[str] = Field(None, description="The name of the task step.")
+    status: Status = Field(..., description="The status of the task step.")
+    output: Optional[str] = Field(None, description="Output of the task step.")
+    additional_output: Optional[StepOutput] = None
+    artifacts: List[Artifact] = Field(
         [], description="A list of artifacts that the step has produced."
     )
     is_last: Optional[bool] = Field(
         False, description="Whether this is the last step in the task."
     )
-
-
-class Step(StepRequestBody, StepResult):
-    task_id: str = Field(..., description="The ID of the task this step belongs to.")
-    step_id: str = Field(..., description="The ID of the task step.")
```

### Comparing `agent_protocol-0.1.2/agent_protocol/utils/compliance/main.py` & `agent_protocol-0.2.0/agent_protocol/utils/compliance/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,21 @@
         task_id = response.json()["task_id"]
         step_body = StepRequestBody(input="test")
         response = requests.post(
             f"{url}/agent/tasks/{task_id}/steps", json=step_body.dict()
         )
         assert response.status_code == 200
 
+    def test_list_artifacts(self, url):
+        response = requests.post(f"{url}/agent/tasks", json=self.task_data)
+        task_id = response.json()["task_id"]
+        response = requests.get(f"{url}/agent/tasks/{task_id}/artifacts")
+        assert response.status_code == 200
+        assert isinstance(response.json(), list)
+
     @pytest.mark.skip("There is no way to be sure any step exists")
     def test_get_agent_task_step(self, url):
         # Create task
         response = requests.post(f"{url}agent/tasks", json=self.task_data)
         task_id = response.json()["task_id"]
         # Get steps
         response = requests.get(f"{url}/agent/tasks/{task_id}/steps")
```

### Comparing `agent_protocol-0.1.2/pyproject.toml` & `agent_protocol-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent-protocol"
-version = "0.1.2"
+version = "0.2.0"
 description = "API for interacting with Agent"
 authors = ["e2b <hello@e2b.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/sdk/tree/main/agent/python/"
 packages = [{ include = "agent_protocol" }]
```

### Comparing `agent_protocol-0.1.2/PKG-INFO` & `agent_protocol-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-protocol
-Version: 0.1.2
+Version: 0.2.0
 Summary: API for interacting with Agent
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -33,36 +33,69 @@
 ```sh
 pip install agent-protocol
 ```
 
 Then add the following code to your agent:
 
 ```python
-from agent_protocol import (
-    Agent,
-    StepResult,
-    StepHandler,
-)
-
-async def task_handler(task_input) -> StepHandler:
-    # TODO: Initialize code for the agent task.
-    async def step_handler(step_input) -> StepResult:
-        # TODO: Execute code for the agent step.
-        # The step could for example be a single iteration of a ReAct loop.
-
-        # TODO: Return the result of the step.
-        return StepResult(
-            output=...,
-        )
+from agent_protocol import Agent, Step, Task
+
+
+async def task_handler(task: Task) -> None:
+    # TODO: Create initial step(s) for the task
+    await Agent.db.create_step(task.task_id, ...)
+
+
+async def step_handler(step: Step) -> Step:
+    # TODO: handle next step
+    if step.name == "print":
+        print(step.input)
+        step.is_last = True
+
+    step.output = "Output from the agent"
+    return step
 
-    return step_handler
 
 if __name__ == "__main__":
     # Add the task handler and start the server
-    Agent.handle_task(task_handler).start()
+    Agent.setup_agent(task_handler, step_handler).start()
+```
+
+## Customization
+
+### Database
+
+By default the SDK stores data in memory. You can customize the database by setting db to your own database object.
+
+```python
+Agent.db = your_database
+```
+
+The database object must implement the methods from [db.py](./agent/python/db.py).
+
+### Routes
+
+You can also add your own routes to the server. For example:
+
+```python
+from agent_protocol import Agent, router
+from fastapi import APIRouter
+
+my_router = APIRouter()
+
+
+@my_router.get("/hello")
+async def hello():
+    return {"hello": "world"}
+
+my_router.include_router(router)
+
+task_handler = ...
+step_handler = ...
+Agent.setup_agent(task_handler, step_handler).start(router=my_router)
 ```
 
 ## Usage
 
 To start the server run the file where you added the code above:
 
 ```sh
@@ -109,14 +142,15 @@
   "input": null,
   "task_id": "e6d768bb-4c50-4007-9853-aeffb46c77be",
   "step_id": "8ff8ba39-2c3e-4246-8086-fbd2a897240b"
 }
 ```
 
 ## Test compliance
+
 Part of the package is also a test suite that can be used to test compliance with the protocol. To run the tests, run the following command:
 
 ```sh
 agent-protocol test --url <url>
 ```
 
 In the background it uses pytest, you can pass any pytest arguments to the command above.
```

