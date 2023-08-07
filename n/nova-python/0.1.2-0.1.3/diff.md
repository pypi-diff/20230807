# Comparing `tmp/nova_python-0.1.2.tar.gz` & `tmp/nova_python-0.1.3.tar.gz`

## Comparing `nova_python-0.1.2.tar` & `nova_python-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 nova_python-0.1.2/Cargo.toml
--rwxrwxrwx   0     1000      998      945 2023-08-07 05:15:38.000000 nova_python-0.1.2/.gitignore
--rwxrwxrwx   0     1000      998    35184 2023-08-07 00:42:06.000000 nova_python-0.1.2/LICENSE
--rwxrwxrwx   0     1000      998     1896 2023-08-07 11:13:33.000000 nova_python-0.1.2/README.md
--rwxrwxrwx   0     1000      998      559 2023-08-07 11:20:31.000000 nova_python-0.1.2/pyproject.toml
--rwxrwxrwx   0     1000      998     6666 2023-08-07 10:57:45.000000 nova_python-0.1.2/src/lib.rs
--rwxrwxrwx   0     1000      998    30430 2023-08-07 11:03:49.000000 nova_python-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 nova_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nova_python-0.1.3/Cargo.toml
+-rwxrwxrwx   0     1000      998      945 2023-08-07 12:42:57.000000 nova_python-0.1.3/.gitignore
+-rwxrwxrwx   0     1000      998    35184 2023-08-07 12:42:57.000000 nova_python-0.1.3/LICENSE
+-rwxrwxrwx   0     1000      998     2368 2023-08-07 14:14:30.000000 nova_python-0.1.3/README.md
+-rwxrwxrwx   0     1000      998      563 2023-08-07 12:42:57.000000 nova_python-0.1.3/pyproject.toml
+-rwxrwxrwx   0     1000      998     7741 2023-08-07 14:02:42.000000 nova_python-0.1.3/src/lib.rs
+-rwxrwxrwx   0     1000      998    30445 2023-08-07 14:01:36.000000 nova_python-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 nova_python-0.1.3/PKG-INFO
```

### Comparing `nova_python-0.1.2/.gitignore` & `nova_python-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.2/LICENSE` & `nova_python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.2/README.md` & `nova_python-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -32,39 +32,62 @@
 
 Now, to make a request, use the `make_request` function. For example:
 
 ```python
 from nova_python import Endpoints, Models, NovaClient
 client = NovaClient("YOUR_API_KEY")
 
-client.make_request(
+reponse = client.make_request(
     endpoint=Endpoints.CHAT_COMPLETION,
     model=Models.GPT3,
     data=[
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Hello!"}
     ]
 )
+
+...
 ```
 
 or
 
 ```python
 from nova_python import Endpoints, Models, NovaClient
 client = NovaClient("YOUR_API_KEY")
 
-client.make_request(
+reponse = client.make_request(
     endpoint=Endpoints.MODERATION,
     model=Models.MODERATION_STABLE,
     data=[{"input": "I'm going to kill them."}]
 )
+
+...
+```
+If everything goes to plan, you'll receive a string containing JSON-Data, which you can then use in your project.  
+
+Note, that when using chat completion, as special ChatResponse-Instance get's returned.  
+You can access the reponse's json.data, by casting it to a string using the `str` method, like this:
+```python
+...
+
+str(reponse)
+
+...
+```
+
+but more importantly, you can use it's `get_message_content` function, to directly get access to the chat reponse. Used like this:
+```
+...
+
+content = reponse.get_message_content()
+
+...
 ```
 
 
-If everything goes to plan, you'll receive a string containing JSON-Data, which you can then use in your project.  
 *Happy prompting!*
 <br><br>
 ## FAQ ##
 **Q:** I get an error when installing the package  
 **A:** Make you sure, that you have <a href="https://rustup.rs/">Cargo</a> installed
 
 **Q**: I keep getting `RuntimeError: error sending request for url (https://api.nova-oss.com/v1/moderations): operation timed out`
```

#### html2text {}

```diff
@@ -4,21 +4,28 @@
 NovaClient ``` Create an instance of NovaClient, using your API key ```python
 client = NovaClient("YOUR_API_KEY") ``` nova_python currently implements two
 enums: Endpoints and Models. Those contain: **Endpoints** *
 `Endpoints.CHAT_COMPLETION` * `Endpoints.MODERATION` **Models** * `Models.GPT3`
 * `Models.GPT4` * `Models.MODERATION_LATEST` * `Models.MODERATION_STABLE` Now,
 to make a request, use the `make_request` function. For example: ```python from
 nova_python import Endpoints, Models, NovaClient client = NovaClient
-("YOUR_API_KEY") client.make_request( endpoint=Endpoints.CHAT_COMPLETION,
-model=Models.GPT3, data=[ {"role": "system", "content": "You are a helpful
-assistant."}, {"role": "user", "content": "Hello!"} ] ) ``` or ```python from
-nova_python import Endpoints, Models, NovaClient client = NovaClient
-("YOUR_API_KEY") client.make_request( endpoint=Endpoints.MODERATION,
+("YOUR_API_KEY") reponse = client.make_request
+( endpoint=Endpoints.CHAT_COMPLETION, model=Models.GPT3, data=[ {"role":
+"system", "content": "You are a helpful assistant."}, {"role": "user",
+"content": "Hello!"} ] ) ... ``` or ```python from nova_python import
+Endpoints, Models, NovaClient client = NovaClient("YOUR_API_KEY") reponse =
+client.make_request( endpoint=Endpoints.MODERATION,
 model=Models.MODERATION_STABLE, data=[{"input": "I'm going to kill them."}] )
-``` If everything goes to plan, you'll receive a string containing JSON-Data,
-which you can then use in your project. *Happy prompting!*
+... ``` If everything goes to plan, you'll receive a string containing JSON-
+Data, which you can then use in your project. Note, that when using chat
+completion, as special ChatResponse-Instance get's returned. You can access the
+reponse's json.data, by casting it to a string using the `str` method, like
+this: ```python ... str(reponse) ... ``` but more importantly, you can use it's
+`get_message_content` function, to directly get access to the chat reponse.
+Used like this: ``` ... content = reponse.get_message_content() ... ``` *Happy
+prompting!*
 
 ## FAQ ## **Q:** I get an error when installing the package **A:** Make you
 sure, that you have Cargo installed **Q**: I keep getting `RuntimeError: error
 sending request for url (https://api.nova-oss.com/v1/moderations): operation
 timed out` **A**: Try passing a higher value than 30 as `seconds_until_timeout`
 to `make_request` Made with ð©¸ by Leander
```

### Comparing `nova_python-0.1.2/pyproject.toml` & `nova_python-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/NovaOSS/nova-python"
+"Repo" = "https://github.com/henceiusegentoo/nova-python"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
```

### Comparing `nova_python-0.1.2/src/lib.rs` & `nova_python-0.1.3/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -50,31 +50,31 @@
         Ok(NovaClient {
             api_key,
             url: String::from("https://api.nova-oss.com/v1/")
         })
     }
 
     // Used to make a request to the Nova API
-    fn make_request(&self, endpoint: Endpoints, model: Models, data: Vec<Py<PyDict>>, seconds_until_timeout: Option<String>) -> PyResult<String> {
+    fn make_request(&self, endpoint: Endpoints, model: Models, data: Vec<Py<PyDict>>, seconds_until_timeout: Option<usize>) -> PyResult<PyObject> {
         if !model_is_compatible(&endpoint, &model) {
             return Err(NovaClient::get_endpoint_not_compatible_error());
         }
 
         let request_url = self.get_request_url(&endpoint).unwrap();
         let request_body = self.get_request_body(&endpoint, &model, data).unwrap();
 
         let rt = tokio::runtime::Runtime::new().unwrap();
         let seconds_until_timeout = match seconds_until_timeout {
-            Some(seconds_until_timeout) => seconds_until_timeout.parse::<u64>().unwrap(),
+            Some(seconds_until_timeout) => seconds_until_timeout,
             None => 30
         };
 
-        let response: Result<String, reqwest::Error> = rt.block_on(async {
+        let unmatched_response: Result<String, reqwest::Error> = rt.block_on(async {
             let client = reqwest::Client::builder()
-                .timeout(time::Duration::from_secs(seconds_until_timeout))
+                .timeout(time::Duration::from_secs(seconds_until_timeout as u64))
                 .user_agent("Mozilla/5.0")
                 .build()
                 .unwrap();
 
             let ai_response = client.post(&request_url)
                 .header("Authorization", format!("Bearer {}", self.api_key))
                 .header("Content-Type", "application/json")
@@ -82,17 +82,33 @@
                 .send()
                 .await?;
             
             let text = ai_response.text().await?;
             Ok(text)
         });
 
-        match response {
-            Ok(response) => Ok(response),
-            Err(response) => Err(pyo3::exceptions::PyRuntimeError::new_err(response.to_string()))
+        let reponse = match unmatched_response {
+            Ok(unmatched_response) => Ok(unmatched_response),
+            Err(unmatched_response) => Err(pyo3::exceptions::PyRuntimeError::new_err(unmatched_response.to_string()))
+        }.unwrap();
+
+        if endpoint == Endpoints::ChatCompletion {
+            let final_reponse = Python::with_gil(|py| {
+                let reponse = ChatResponse::new(reponse);
+                reponse.into_py(py)
+            });
+
+            return Ok(final_reponse);
+            
+        } else {
+            let final_reponse = Python::with_gil(|py| {
+                reponse.into_py(py)
+            });
+
+            return Ok(final_reponse);
         }
     }
 
 }
 
 impl NovaClient {
     fn get_request_url(&self, endpoint: &Endpoints) -> PyResult<String> {
@@ -177,17 +193,44 @@
     fn get_invalid_endpoint_error() -> PyErr {
         pyo3::exceptions::PyValueError::new_err("Invalid endpoint")
     }
 
     fn get_invalid_model_error() -> PyErr {
         pyo3::exceptions::PyValueError::new_err("Invalid model")
     }
+}
+
+#[pyclass(module = "nova_python", frozen)]
+struct ChatResponse {
+    json: String,
+}
+
+#[pymethods]
+impl ChatResponse {
+    #[new]
+    fn new(json: String) -> Self {
+        ChatResponse {
+            json
+        }
+    }
+
+    fn get_message_content(&self) -> PyResult<String> {
+        let json = &self.json;
+        let json: serde_json::Value = serde_json::from_str(json).unwrap();
+
+        let content = json["choices"][0]["message"]["content"].as_str().unwrap();
+        Ok(content.trim().to_string())
+    }
+
+    fn __str__(&self) -> PyResult<String> {
+        Ok(self.json.clone())
+    }
 
-    fn get_request_failed_error() -> PyErr {
-        pyo3::exceptions::PyRuntimeError::new_err("Request failed for unknown reasons.")
+    fn __repr__(&self) -> PyResult<String> {
+        Ok(format!("ChatResponse(json={})", self.json))
     }
 }
 
 fn model_is_compatible(endpoint: &Endpoints, model: &Models) -> bool {
     if endpoint == &Endpoints::ChatCompletion {
         if [Models::Gpt3, Models::Gpt4].contains(model) {
             return true;
```

### Comparing `nova_python-0.1.2/Cargo.lock` & `nova_python-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -450,18 +450,19 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "nova-python"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "pyo3",
  "reqwest",
+ "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

