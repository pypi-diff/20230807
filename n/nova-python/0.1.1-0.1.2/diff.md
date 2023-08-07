# Comparing `tmp/nova_python-0.1.1.tar.gz` & `tmp/nova_python-0.1.2.tar.gz`

## Comparing `nova_python-0.1.1.tar` & `nova_python-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 nova_python-0.1.1/Cargo.toml
--rwxrwxrwx   0     1000      998      945 2023-08-07 05:15:38.000000 nova_python-0.1.1/.gitignore
--rwxrwxrwx   0     1000      998    35184 2023-08-07 00:42:06.000000 nova_python-0.1.1/LICENSE
--rwxrwxrwx   0     1000      998     1663 2023-08-07 09:32:33.000000 nova_python-0.1.1/README.md
--rwxrwxrwx   0     1000      998      544 2023-08-07 09:37:18.000000 nova_python-0.1.1/pyproject.toml
--rwxrwxrwx   0     1000      998     6258 2023-08-07 09:16:40.000000 nova_python-0.1.1/src/lib.rs
--rwxrwxrwx   0     1000      998    30430 2023-08-07 08:57:10.000000 nova_python-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 nova_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 nova_python-0.1.2/Cargo.toml
+-rwxrwxrwx   0     1000      998      945 2023-08-07 05:15:38.000000 nova_python-0.1.2/.gitignore
+-rwxrwxrwx   0     1000      998    35184 2023-08-07 00:42:06.000000 nova_python-0.1.2/LICENSE
+-rwxrwxrwx   0     1000      998     1896 2023-08-07 11:13:33.000000 nova_python-0.1.2/README.md
+-rwxrwxrwx   0     1000      998      559 2023-08-07 11:20:31.000000 nova_python-0.1.2/pyproject.toml
+-rwxrwxrwx   0     1000      998     6666 2023-08-07 10:57:45.000000 nova_python-0.1.2/src/lib.rs
+-rwxrwxrwx   0     1000      998    30430 2023-08-07 11:03:49.000000 nova_python-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 nova_python-0.1.2/PKG-INFO
```

### Comparing `nova_python-0.1.1/.gitignore` & `nova_python-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.1/LICENSE` & `nova_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.1/README.md` & `nova_python-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -58,13 +58,16 @@
     data=[{"input": "I'm going to kill them."}]
 )
 ```
 
 
 If everything goes to plan, you'll receive a string containing JSON-Data, which you can then use in your project.  
 *Happy prompting!*
-
+<br><br>
 ## FAQ ##
 **Q:** I get an error when installing the package  
 **A:** Make you sure, that you have <a href="https://rustup.rs/">Cargo</a> installed
 
+**Q**: I keep getting `RuntimeError: error sending request for url (https://api.nova-oss.com/v1/moderations): operation timed out`  
+**A**: Try passing a higher value than 30 as `seconds_until_timeout` to `make_request` 
+
 Made with 🩸 by Leander
```

#### html2text {}

```diff
@@ -11,10 +11,14 @@
 ("YOUR_API_KEY") client.make_request( endpoint=Endpoints.CHAT_COMPLETION,
 model=Models.GPT3, data=[ {"role": "system", "content": "You are a helpful
 assistant."}, {"role": "user", "content": "Hello!"} ] ) ``` or ```python from
 nova_python import Endpoints, Models, NovaClient client = NovaClient
 ("YOUR_API_KEY") client.make_request( endpoint=Endpoints.MODERATION,
 model=Models.MODERATION_STABLE, data=[{"input": "I'm going to kill them."}] )
 ``` If everything goes to plan, you'll receive a string containing JSON-Data,
-which you can then use in your project. *Happy prompting!* ## FAQ ## **Q:** I
-get an error when installing the package **A:** Make you sure, that you have
-Cargo installed Made with ð©¸ by Leander
+which you can then use in your project. *Happy prompting!*
+
+## FAQ ## **Q:** I get an error when installing the package **A:** Make you
+sure, that you have Cargo installed **Q**: I keep getting `RuntimeError: error
+sending request for url (https://api.nova-oss.com/v1/moderations): operation
+timed out` **A**: Try passing a higher value than 30 as `seconds_until_timeout`
+to `make_request` Made with ð©¸ by Leander
```

### Comparing `nova_python-0.1.1/pyproject.toml` & `nova_python-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
-repository = "https://github.com/NovaOSS/nova-python"
+[project.urls]
+"Homepage" = "https://github.com/NovaOSS/nova-python"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
```

### Comparing `nova_python-0.1.1/src/lib.rs` & `nova_python-0.1.2/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 use pyo3::prelude::*;
 use std::collections::HashMap;
 use pyo3::types::PyDict;
 use std::time;
 
+// An enum to represent the different models
 #[pyclass(module = "nova_python", frozen)]
 #[derive(PartialEq)]
 #[derive(Clone)]
 enum Models {
     #[pyo3(name = "GPT3")]
     Gpt3,
     #[pyo3(name = "GPT4")]
     Gpt4,
     #[pyo3(name = "MODERATION_LATEST")]
     ModerationLatest,
     #[pyo3(name = "MODERATION_STABLE")]
     ModerationStable,
 }
 
+// An enum to represent the different endpoints
 #[pyclass(module = "nova_python", frozen)]
 #[derive(PartialEq)]
 #[derive(Clone)]
 enum Endpoints {
     #[pyo3(name = "CHAT_COMPLETION")]
     ChatCompletion,
     #[pyo3(name = "MODERATION")]
     Moderation,
 }
 
+// Interface to the Nova API
 #[pyclass(module = "nova_python", frozen)]
 struct NovaClient {
     #[pyo3(get)]
     api_key: String,
     url: String
 }
 
@@ -46,27 +49,32 @@
 
         Ok(NovaClient {
             api_key,
             url: String::from("https://api.nova-oss.com/v1/")
         })
     }
 
-    fn make_request(&self, endpoint: Endpoints, model: Models, data: Vec<Py<PyDict>>) -> PyResult<String> {
+    // Used to make a request to the Nova API
+    fn make_request(&self, endpoint: Endpoints, model: Models, data: Vec<Py<PyDict>>, seconds_until_timeout: Option<String>) -> PyResult<String> {
         if !model_is_compatible(&endpoint, &model) {
             return Err(NovaClient::get_endpoint_not_compatible_error());
         }
 
         let request_url = self.get_request_url(&endpoint).unwrap();
         let request_body = self.get_request_body(&endpoint, &model, data).unwrap();
 
         let rt = tokio::runtime::Runtime::new().unwrap();
-        
+        let seconds_until_timeout = match seconds_until_timeout {
+            Some(seconds_until_timeout) => seconds_until_timeout.parse::<u64>().unwrap(),
+            None => 30
+        };
+
         let response: Result<String, reqwest::Error> = rt.block_on(async {
             let client = reqwest::Client::builder()
-                .timeout(time::Duration::from_secs(10))
+                .timeout(time::Duration::from_secs(seconds_until_timeout))
                 .user_agent("Mozilla/5.0")
                 .build()
                 .unwrap();
 
             let ai_response = client.post(&request_url)
                 .header("Authorization", format!("Bearer {}", self.api_key))
                 .header("Content-Type", "application/json")
```

### Comparing `nova_python-0.1.1/Cargo.lock` & `nova_python-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,15 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "nova-python"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "pyo3",
  "reqwest",
  "tokio",
 ]
 
 [[package]]
```

### Comparing `nova_python-0.1.1/PKG-INFO` & `nova_python-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nova-python
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: 🐍 Python library for accessing the Nova API
 Author: Leander <@henceiusegentoo>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/NovaOSS/nova-python
 
 # nova-python
 🐍 Python library for accessing the Nova API
 
 ## Usage ##
 Install the module (This requires <a href="https://rustup.rs/">Cargo</a>)  
 ```sh
@@ -70,13 +71,16 @@
     data=[{"input": "I'm going to kill them."}]
 )
 ```
 
 
 If everything goes to plan, you'll receive a string containing JSON-Data, which you can then use in your project.  
 *Happy prompting!*
-
+<br><br>
 ## FAQ ##
 **Q:** I get an error when installing the package  
 **A:** Make you sure, that you have <a href="https://rustup.rs/">Cargo</a> installed
 
+**Q**: I keep getting `RuntimeError: error sending request for url (https://api.nova-oss.com/v1/moderations): operation timed out`  
+**A**: Try passing a higher value than 30 as `seconds_until_timeout` to `make_request` 
+
 Made with 🩸 by Leander
```

#### html2text {}

```diff
@@ -1,25 +1,30 @@
-Metadata-Version: 2.1 Name: nova-python Version: 0.1.1 Classifier: Programming
+Metadata-Version: 2.1 Name: nova-python Version: 0.1.2 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE Summary: ð Python library for accessing the Nova API
 Author: Leander <@henceiusegentoo> Requires-Python: >=3.7 Description-Content-
-Type: text/markdown; charset=UTF-8; variant=GFM # nova-python ð Python
-library for accessing the Nova API ## Usage ## Install the module (This
-requires Cargo) ```sh $ pip install nova-python ``` Import the module ```python
-from nova_python import Endpoints, Models, NovaClient ``` Create an instance of
-NovaClient, using your API key ```python client = NovaClient("YOUR_API_KEY")
-``` nova_python currently implements two enums: Endpoints and Models. Those
-contain: **Endpoints** * `Endpoints.CHAT_COMPLETION` * `Endpoints.MODERATION`
-**Models** * `Models.GPT3` * `Models.GPT4` * `Models.MODERATION_LATEST` *
-`Models.MODERATION_STABLE` Now, to make a request, use the `make_request`
-function. For example: ```python from nova_python import Endpoints, Models,
-NovaClient client = NovaClient("YOUR_API_KEY") client.make_request
-( endpoint=Endpoints.CHAT_COMPLETION, model=Models.GPT3, data=[ {"role":
-"system", "content": "You are a helpful assistant."}, {"role": "user",
-"content": "Hello!"} ] ) ``` or ```python from nova_python import Endpoints,
-Models, NovaClient client = NovaClient("YOUR_API_KEY") client.make_request
-( endpoint=Endpoints.MODERATION, model=Models.MODERATION_STABLE, data=[
-{"input": "I'm going to kill them."}] ) ``` If everything goes to plan, you'll
-receive a string containing JSON-Data, which you can then use in your project.
-*Happy prompting!* ## FAQ ## **Q:** I get an error when installing the package
-**A:** Make you sure, that you have Cargo installed Made with ð©¸ by Leander
+Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Homepage, https://
+github.com/NovaOSS/nova-python # nova-python ð Python library for accessing
+the Nova API ## Usage ## Install the module (This requires Cargo) ```sh $ pip
+install nova-python ``` Import the module ```python from nova_python import
+Endpoints, Models, NovaClient ``` Create an instance of NovaClient, using your
+API key ```python client = NovaClient("YOUR_API_KEY") ``` nova_python currently
+implements two enums: Endpoints and Models. Those contain: **Endpoints** *
+`Endpoints.CHAT_COMPLETION` * `Endpoints.MODERATION` **Models** * `Models.GPT3`
+* `Models.GPT4` * `Models.MODERATION_LATEST` * `Models.MODERATION_STABLE` Now,
+to make a request, use the `make_request` function. For example: ```python from
+nova_python import Endpoints, Models, NovaClient client = NovaClient
+("YOUR_API_KEY") client.make_request( endpoint=Endpoints.CHAT_COMPLETION,
+model=Models.GPT3, data=[ {"role": "system", "content": "You are a helpful
+assistant."}, {"role": "user", "content": "Hello!"} ] ) ``` or ```python from
+nova_python import Endpoints, Models, NovaClient client = NovaClient
+("YOUR_API_KEY") client.make_request( endpoint=Endpoints.MODERATION,
+model=Models.MODERATION_STABLE, data=[{"input": "I'm going to kill them."}] )
+``` If everything goes to plan, you'll receive a string containing JSON-Data,
+which you can then use in your project. *Happy prompting!*
+
+## FAQ ## **Q:** I get an error when installing the package **A:** Make you
+sure, that you have Cargo installed **Q**: I keep getting `RuntimeError: error
+sending request for url (https://api.nova-oss.com/v1/moderations): operation
+timed out` **A**: Try passing a higher value than 30 as `seconds_until_timeout`
+to `make_request` Made with ð©¸ by Leander
```

