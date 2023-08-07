# Comparing `tmp/microsoft_kiota_http-0.4.4.tar.gz` & `tmp/microsoft_kiota_http-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_http-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_http-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_http-0.4.4.tar` & `microsoft_kiota_http-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
--rw-r--r--   0        0        0      117 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1804 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.gitignore
--rw-r--r--   0        0        0    15946 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.pylintrc
--rw-r--r--   0        0        0     1216 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/LICENSE
--rw-r--r--   0        0        0     2376 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/README.md
--rw-r--r--   0        0        0     2757 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/SUPPORT.md
--rw-r--r--   0        0        0      121 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/__init__.py
--rw-r--r--   0        0        0       23 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/_version.py
--rw-r--r--   0        0        0    14637 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/httpx_request_adapter.py
--rw-r--r--   0        0        0     5189 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/kiota_client_factory.py
--rw-r--r--   0        0        0      327 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/__init__.py
--rw-r--r--   0        0        0      652 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/async_kiota_transport.py
--rw-r--r--   0        0        0     2011 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/middleware.py
--rw-r--r--   0        0        0      377 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/__init__.py
--rw-r--r--   0        0        0     1621 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
--rw-r--r--   0        0        0     2127 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/redirect_handler_option.py
--rw-r--r--   0        0        0      858 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/response_handler_option.py
--rw-r--r--   0        0        0     3067 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/retry_handler_option.py
--rw-r--r--   0        0        0      714 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/telemetry_handler_option.py
--rw-r--r--   0        0        0     1344 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/url_replace_option.py
--rw-r--r--   0        0        0     2303 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     8588 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/redirect_handler.py
--rw-r--r--   0        0        0     8057 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/retry_handler.py
--rw-r--r--   0        0        0     2307 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/url_replace_handler.py
--rw-r--r--   0        0        0     1286 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      885 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0     4882 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/conftest.py
--rw-r--r--   0        0        0      114 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/helpers/__init__.py
--rw-r--r--   0        0        0     4498 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/helpers/mock_response_object.py
--rw-r--r--   0        0        0      105 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/helpers/office_location.py
--rw-r--r--   0        0        0        0 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/__init__.py
--rw-r--r--   0        0        0      989 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     2207 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_redirect_handler.py
--rw-r--r--   0        0        0     4324 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_retry_handler.py
--rw-r--r--   0        0        0     1681 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_url_replace_handler.py
--rw-r--r--   0        0        0    10952 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/test_httpx_request_adapter.py
--rw-r--r--   0        0        0     3355 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/test_kiota_client_factory.py
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft_kiota_http-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-08-07 11:22:01.032894 microsoft_kiota_http-0.5.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-08-07 11:22:01.032894 microsoft_kiota_http-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1717 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/.gitignore
+-rw-r--r--   0        0        0    15946 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/.pylintrc
+-rw-r--r--   0        0        0     1402 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/LICENSE
+-rw-r--r--   0        0        0      327 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/Makefile
+-rw-r--r--   0        0        0     2376 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/README.md
+-rw-r--r--   0        0        0     2757 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/SUPPORT.md
+-rw-r--r--   0        0        0      121 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/__init__.py
+-rw-r--r--   0        0        0       23 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/_version.py
+-rw-r--r--   0        0        0    15065 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/httpx_request_adapter.py
+-rw-r--r--   0        0        0     5652 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/kiota_client_factory.py
+-rw-r--r--   0        0        0      376 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/__init__.py
+-rw-r--r--   0        0        0      652 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/async_kiota_transport.py
+-rw-r--r--   0        0        0     2011 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/middleware.py
+-rw-r--r--   0        0        0      439 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/__init__.py
+-rw-r--r--   0        0        0     1621 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
+-rw-r--r--   0        0        0     2127 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/redirect_handler_option.py
+-rw-r--r--   0        0        0      873 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/response_handler_option.py
+-rw-r--r--   0        0        0     3027 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/retry_handler_option.py
+-rw-r--r--   0        0        0      714 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/telemetry_handler_option.py
+-rw-r--r--   0        0        0     1344 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/url_replace_option.py
+-rw-r--r--   0        0        0     1688 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/options/user_agent_handler_option.py
+-rw-r--r--   0        0        0     2172 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     8496 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/redirect_handler.py
+-rw-r--r--   0        0        0     7994 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/retry_handler.py
+-rw-r--r--   0        0        0     2189 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/url_replace_handler.py
+-rw-r--r--   0        0        0     1211 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/kiota_http/middleware/user_agent_handler.py
+-rw-r--r--   0        0        0     1286 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      887 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     4882 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      114 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     4498 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/helpers/mock_response_object.py
+-rw-r--r--   0        0        0      105 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/helpers/office_location.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/middleware_tests/__init__.py
+-rw-r--r--   0        0        0      989 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/middleware_tests/test_parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     2207 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/middleware_tests/test_redirect_handler.py
+-rw-r--r--   0        0        0     4324 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/middleware_tests/test_retry_handler.py
+-rw-r--r--   0        0        0     1681 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/middleware_tests/test_url_replace_handler.py
+-rw-r--r--   0        0        0      572 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/middleware_tests/test_user_agent_handler.py
+-rw-r--r--   0        0        0    11346 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/test_httpx_request_adapter.py
+-rw-r--r--   0        0        0     3430 2023-08-07 11:22:01.036894 microsoft_kiota_http-0.5.0/tests/test_kiota_client_factory.py
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft_kiota_http-0.5.0/PKG-INFO
```

### Comparing `microsoft_kiota_http-0.4.4/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_http-0.5.0/.github/workflows/auto-merge-dependabot.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.5.1
+        uses: dependabot/fetch-metadata@v1.6.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft_kiota_http-0.4.4/.github/workflows/build_publish.yml` & `microsoft_kiota_http-0.5.0/.github/workflows/build_publish.yml`

 * *Files 26% similar despite different names*

```diff
@@ -19,31 +19,30 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pipenv
-          pipenv install -r requirements-dev.txt
+          pip install -r requirements-dev.txt
       - name: Check code format
         run: |
-          pipenv run yapf -dr kiota_http
+          yapf -dr kiota_http
       - name: Check import order
         run: |
-          pipenv run isort kiota_http
+          isort kiota_http
       - name: Lint with Pylint
         run: |
-          pipenv run pylint kiota_http --disable=W --rcfile=.pylintrc
+          pylint kiota_http --disable=W --rcfile=.pylintrc
       - name: Static type checking with Mypy
         run: |
-          pipenv run mypy kiota_http
+          mypy kiota_http
       - name: Run tests with Pytest
         run: |
-          pipenv run pytest
+          pytest
 
   publish:
     name: Publish distribution to PyPI
     if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
     runs-on: ubuntu-latest
     environment: pypi_prod
     needs: [build]
```

### Comparing `microsoft_kiota_http-0.4.4/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_http-0.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_http-0.5.0/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/.gitignore` & `microsoft_kiota_http-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/.pylintrc` & `microsoft_kiota_http-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/CHANGELOG.md` & `microsoft_kiota_http-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.5.0] - 2023-07-27
+
+### Added
+
+- Added a translator method to change a `RequestInformation` object into a HTTPX client request object.
+- Enabled backing store support
+
+### Changed
+
 ## [0.4.4] - 2023-05-31
 
 ### Added
 
 - Added a url replace handler for replacing url segments.
 
 ### Changed
```

### Comparing `microsoft_kiota_http-0.4.4/LICENSE` & `microsoft_kiota_http-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/README.md` & `microsoft_kiota_http-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/SECURITY.md` & `microsoft_kiota_http-0.5.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/SUPPORT.md` & `microsoft_kiota_http-0.5.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/httpx_request_adapter.py` & `microsoft_kiota_http-0.5.0/kiota_http/httpx_request_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, Dict, List, Optional, TypeVar, Union
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 
 import httpx
 from kiota_abstractions.api_client_builder import (
     enable_backing_store_for_parse_node_factory,
     enable_backing_store_for_serialization_writer_factory,
 )
 from kiota_abstractions.api_error import APIError
@@ -24,15 +24,15 @@
 from .kiota_client_factory import KiotaClientFactory
 from .middleware.options import ResponseHandlerOption
 
 ResponseType = Union[str, int, float, bool, datetime, bytes]
 ModelType = TypeVar("ModelType", bound=Parsable)
 
 
-class HttpxRequestAdapter(RequestAdapter):
+class HttpxRequestAdapter(RequestAdapter, Generic[ModelType]):
 
     def __init__(
         self,
         authentication_provider: AuthenticationProvider,
         parse_node_factory: ParseNodeFactory = ParseNodeFactoryRegistry(),
         serialization_writer_factory:
         SerializationWriterFactory = SerializationWriterFactoryRegistry(),
@@ -88,22 +88,22 @@
             return None
         segments = header.lower().split(';')
         if not segments:
             return None
         return segments[0]
 
     async def send_async(
-        self, request_info: RequestInformation, model_type: ParsableFactory,
+        self, request_info: RequestInformation, parsable_factory: ParsableFactory,
         error_map: Dict[str, ParsableFactory]
     ) -> Optional[ModelType]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized response model.
         Args:
             request_info (RequestInformation): the request info to execute.
-            model_type (ParsableFactory): the class of the response model 
+            parsable_factory (ParsableFactory): the class of the response model 
             to deserialize the response into.
             error_map (Dict[str, ParsableFactory]): the error dict to use in
             case of a failed request.
 
         Returns:
             ModelType: the deserialized response model.
         """
@@ -116,26 +116,26 @@
         if response_handler:
             return await response_handler.handle_response_async(response, error_map)
 
         await self.throw_failed_responses(response, error_map)
         if self._should_return_none(response):
             return None
         root_node = await self.get_root_parse_node(response)
-        result = root_node.get_object_value(model_type)
+        result = root_node.get_object_value(parsable_factory)
         return result
 
     async def send_collection_async(
-        self, request_info: RequestInformation, model_type: ParsableFactory,
+        self, request_info: RequestInformation, parsable_factory: ParsableFactory,
         error_map: Dict[str, ParsableFactory]
     ) -> Optional[List[ModelType]]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized response model collection.
         Args:
             request_info (RequestInformation): the request info to execute.
-            model_type (ParsableFactory): the class of the response model
+            parsable_factory (ParsableFactory): the class of the response model
             to deserialize the response into.
             error_map (Dict[str, ParsableFactory]): the error dict to use in
             case of a failed request.
 
         Returns:
             ModelType: the deserialized response model collection.
         """
@@ -147,15 +147,15 @@
         if response_handler:
             return await response_handler.handle_response_async(response, error_map)
 
         await self.throw_failed_responses(response, error_map)
         if self._should_return_none(response):
             return None
         root_node = await self.get_root_parse_node(response)
-        result = root_node.get_collection_of_object_values(model_type)
+        result = root_node.get_collection_of_object_values(parsable_factory)
         return result
 
     async def send_collection_of_primitive_async(
         self, request_info: RequestInformation, response_type: ResponseType,
         error_map: Dict[str, ParsableFactory]
     ) -> Optional[List[ResponseType]]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
@@ -222,15 +222,15 @@
             return root_node.get_int_value()
         if response_type == "float":
             return root_node.get_float_value()
         if response_type == "bool":
             return root_node.get_bool_value()
         if response_type == "datetime":
             return root_node.get_datetime_value()
-        raise Exception("Found unexpected type to deserialize")
+        raise TypeError(f"Unable to deserialize type: {response_type!r}")
 
     async def send_no_response_content_async(
         self, request_info: RequestInformation, error_map: Dict[str, ParsableFactory]
     ) -> None:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized primitive response model.
         Args:
@@ -256,18 +256,18 @@
         """
         self._parse_node_factory = enable_backing_store_for_parse_node_factory(
             self._parse_node_factory
         )
         self._serialization_writer_factory = enable_backing_store_for_serialization_writer_factory(
             self._serialization_writer_factory
         )
-        if not (self._serialization_writer_factory or self._parse_node_factory):
+        if not any([self._serialization_writer_factory, self._parse_node_factory]):
             raise Exception("Unable to enable backing store")
-        if backing_store_factory:
-            BackingStoreFactorySingleton.__instance = backing_store_factory
+
+        BackingStoreFactorySingleton(backing_store_factory=backing_store_factory)
 
     async def get_root_parse_node(self, response: httpx.Response) -> ParseNode:
         payload = response.content
         response_content_type = self.get_response_content_type(response)
         if not response_content_type:
             raise Exception("No response content type found for deserialization")
 
@@ -285,23 +285,23 @@
         response_status_code = response.status_code
         response_status_code_str = str(response_status_code)
         response_headers = response.headers
 
         if not error_map:
             raise APIError(
                 "The server returned an unexpected status code and no error class is registered"
-                f" for this code {response_status_code}", response_headers, response_status_code
+                f" for this code {response_status_code}", response_status_code, response_headers
             )
         if (response_status_code_str not in error_map) and (
             (400 <= response_status_code < 500 and '4XX' not in error_map) or
             (500 <= response_status_code < 600 and '5XX' not in error_map)
         ):
             raise APIError(
                 "The server returned an unexpected status code and no error class is registered"
-                f" for this code {response_status_code}", response_headers, response_status_code
+                f" for this code {response_status_code}", response_status_code, response_headers
             )
 
         error_class = None
         if response_status_code_str in error_map:
             error_class = error_map[response_status_code_str]
         elif 400 <= response_status_code < 500:
             error_class = error_map['4XX']
@@ -312,15 +312,15 @@
         error = root_node.get_object_value(error_class)
 
         if isinstance(error, APIError):
             error.response_headers = response_headers
             error.response_status_code = response_status_code
             raise error
         raise APIError(
-            f"Unexpected error type: {type(error)}", response_headers, response_status_code
+            f"Unexpected error type: {type(error)}", response_status_code, response_headers
         )
 
     async def get_http_response_message(self, request_info: RequestInformation) -> httpx.Response:
         self.set_base_url_for_request_information(request_info)
         await self._authentication_provider.authenticate_request(request_info)
 
         request = self.get_request_from_request_information(request_info)
@@ -343,7 +343,16 @@
             method=request_info.http_method.value,
             url=request_info.url,
             headers=request_info.request_headers,
             content=request_info.content,
         )
         request.options = request_info.request_options  # type:ignore
         return request
+
+    async def convert_to_native_async(self, request_info: RequestInformation) -> httpx.Request:
+        if request_info is None:
+            raise ValueError("request information must be provided")
+
+        await self._authentication_provider.authenticate_request(request_info)
+
+        request = self.get_request_from_request_information(request_info)
+        return request
```

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/kiota_client_factory.py` & `microsoft_kiota_http-0.5.0/kiota_http/kiota_client_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 from typing import Dict, List, Optional
 
 import httpx
 from kiota_abstractions.request_option import RequestOption
 
+from kiota_http.middleware.options.user_agent_handler_option import UserAgentHandlerOption
+from kiota_http.middleware.user_agent_handler import UserAgentHandler
+
 from .middleware import (
     AsyncKiotaTransport,
     BaseMiddleware,
     MiddlewarePipeline,
     ParametersNameDecodingHandler,
     RedirectHandler,
     RetryHandler,
@@ -93,14 +96,15 @@
         Helper method that returns a list of default middleware instantiated with
         appropriate options
         """
         redirect_handler = RedirectHandler()
         retry_handler = RetryHandler()
         parameters_name_decoding_handler = ParametersNameDecodingHandler()
         url_replace_handler = UrlReplaceHandler()
+        user_agent_handler = UserAgentHandler()
 
         if options:
             redirect_handler_options = options.get(RedirectHandlerOption.get_key())
             if redirect_handler_options:
                 redirect_handler = RedirectHandler(options=redirect_handler_options)
 
             retry_handler_options = options.get(RetryHandlerOption.get_key())
@@ -115,16 +119,21 @@
                     options=parameters_name_decoding_handler_options
                 )
 
             url_replace_handler_options = options.get(UrlReplaceHandlerOption.get_key())
             if url_replace_handler_options:
                 url_replace_handler = UrlReplaceHandler(options=url_replace_handler_options)
 
+            user_agent_handler_options = options.get(UserAgentHandlerOption.get_key())
+            if user_agent_handler_options:
+                user_agent_handler = UserAgentHandler(options=user_agent_handler_options)
+
         middleware = [
-            redirect_handler, retry_handler, parameters_name_decoding_handler, url_replace_handler
+            redirect_handler, retry_handler, parameters_name_decoding_handler, url_replace_handler,
+            user_agent_handler
         ]
         return middleware
 
     @staticmethod
     def create_middleware_pipeline(
         middleware: Optional[List[BaseMiddleware]], transport: httpx.AsyncBaseTransport
     ) -> MiddlewarePipeline:
```

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/async_kiota_transport.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/async_kiota_transport.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/middleware.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/parameters_name_decoding_handler_option.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/options/parameters_name_decoding_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/redirect_handler_option.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/options/redirect_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/response_handler_option.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/options/response_handler_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any
+from typing import Union
 
 from kiota_abstractions.request_option import RequestOption
 from kiota_abstractions.response_handler import ResponseHandler
 
 
 class ResponseHandlerOption(RequestOption):
     """ Adds a ResponseHandler as a RequestOption for the request."""
 
     RESPONSE_HANDLER_OPTION_KEY = "ResponseHandler"
 
-    def __init__(self, response_handler: ResponseHandler = None) -> None:
+    def __init__(self, response_handler: Union[ResponseHandler, None] = None) -> None:
         """To create an instance of ResponseHandlerOption
 
         Args:
             response_handler (ResponseHandler): - The response handler instance
         """
         self._response_handler = response_handler
```

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/retry_handler_option.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/options/retry_handler_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import FrozenSet, Set
-
 from kiota_abstractions.request_option import RequestOption
 
 
 class RetryHandlerOption(RequestOption):
     """The retry request option class
     """
 
@@ -38,48 +36,48 @@
         if delay > self.MAX_DELAY:
             raise ValueError(f'MaxLimitExceeded. Delay should not be more than ${self.MAX_DELAY}')
         if max_retries > self.MAX_MAX_RETRIES:
             raise ValueError(
                 f'MaxLimitExceeded. MaxRetries should not be more than ${self.MAX_MAX_RETRIES}'
             )
         if delay < 0 and max_retries < 0:
-            raise ValueError(f'InvalidMinValue. Delay and MaxRetries should not be negative')
+            raise ValueError('InvalidMinValue. Delay and MaxRetries should not be negative')
         if delay < 0:
-            raise ValueError(f'InvalidMinValue. Delay should not be negative')
+            raise ValueError('InvalidMinValue. Delay should not be negative')
         if max_retries < 0:
-            raise ValueError(f'InvalidMinValue. MaxRetries should not be negative')
+            raise ValueError('InvalidMinValue. MaxRetries should not be negative')
 
         self._max_retry: int = min(max_retries, self.MAX_MAX_RETRIES)
         self._max_delay: float = min(delay, self.MAX_DELAY)
         self._should_retry: bool = should_retry
 
     @property
     def max_delay(self) -> float:
         return self._max_delay
 
     @max_delay.setter
     def max_delay(self, value: float) -> None:
         if value > self.MAX_DELAY:
             raise ValueError(f'MaxLimitExceeded. Delay should not be more than ${self.MAX_DELAY}')
         if value < 0:
-            raise ValueError(f'InvalidMinValue. Delay should not be negative')
+            raise ValueError('InvalidMinValue. Delay should not be negative')
         self._max_delay = value
 
     @property
     def max_retry(self) -> int:
         return self._max_retry
 
     @max_retry.setter
     def max_retry(self, value: int) -> None:
         if value > self.MAX_MAX_RETRIES:
             raise ValueError(
                 f'MaxLimitExceeded. MaxRetries should not be more than ${self.MAX_MAX_RETRIES}'
             )
         if value < 0:
-            raise ValueError(f'InvalidMinValue. MaxRetries should not be negative')
+            raise ValueError('InvalidMinValue. MaxRetries should not be negative')
         self._max_retry = value
 
     @property
     def should_retry(self) -> bool:
         return self._should_retry
 
     @should_retry.setter
```

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/telemetry_handler_option.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/options/telemetry_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/url_replace_option.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/options/url_replace_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/parameters_name_decoding_handler.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/parameters_name_decoding_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import json
 from urllib.parse import unquote
 
 import httpx
+from kiota_abstractions.request_option import RequestOption
 
 from .middleware import BaseMiddleware
 from .options import ParametersNameDecodingHandlerOption
 
 
 class ParametersNameDecodingHandler(BaseMiddleware):
 
     def __init__(
         self,
-        options: ParametersNameDecodingHandlerOption = ParametersNameDecodingHandlerOption(),
-        **kwargs
+        options: RequestOption = ParametersNameDecodingHandlerOption(),
     ):
         """Create an instance of ParametersNameDecodingHandler
 
         Args:
             options (ParametersNameDecodingHandlerOption, optional): The parameters name
             decoding handler options value.
             Defaults to ParametersNameDecodingHandlerOption
@@ -35,17 +34,19 @@
 
         Returns:
             Response: The response object.
         """
         current_options = self._get_current_options(request)
 
         updated_url: str = str(request.url)  #type: ignore
-        if (
-            current_options and current_options.enabled and '%' in updated_url
-            and current_options.characters_to_decode
+        if all(
+            [
+                current_options, current_options.enabled, '%' in updated_url,
+                current_options.characters_to_decode
+            ]
         ):
             updated_url = unquote(updated_url)
         request.url = httpx.URL(updated_url)
         response = await super().send(request, transport)
         return response
 
     def _get_current_options(self, request: httpx.Request) -> ParametersNameDecodingHandlerOption:
@@ -54,16 +55,11 @@
 
         Args:
             request (httpx.Request): The prepared request object
 
         Returns:
             ParametersNameDecodingHandlerOption: The options to used.
         """
-        current_options = self.options
-        request_options = request.options.get(              # type:ignore
-            ParametersNameDecodingHandlerOption.get_key()
+        current_options =request.options.get( # type:ignore
+            ParametersNameDecodingHandlerOption.get_key(), self.options
         )
-        # Override default options with request options
-        if request_options:
-            current_options = request_options
-
         return current_options
```

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/redirect_handler.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/redirect_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing
 
 import httpx
+from kiota_abstractions.request_option import RequestOption
 
 from .middleware import BaseMiddleware
 from .options import RedirectHandlerOption
 
 
 class RedirectHandler(BaseMiddleware):
     """Middlware that allows us to define the redirect policy for all requests
@@ -17,15 +18,15 @@
         307,  # Temporary Permanently
         308,  # Moved Permanently
     }
     STATUS_CODE_SEE_OTHER: int = 303
     LOCATION_HEADER: str = "Location"
     AUTHORIZATION_HEADER: str = "Authorization"
 
-    def __init__(self, options: RedirectHandlerOption = RedirectHandlerOption()) -> None:
+    def __init__(self, options: RequestOption = RedirectHandlerOption()) -> None:
         super().__init__()
         self.options = options
         self.redirect_on_status_codes: typing.Set[int] = self.DEFAULT_REDIRECT_STATUS_CODES
         self.history: typing.List[httpx.Request] = []
 
     def increment(self, response, max_redirect) -> bool:
         """Increment the redirect attempts for this request.
@@ -82,20 +83,16 @@
 
         Args:
             request (httpx.Request): The prepared request object
 
         Returns:
             RedirectHandlerOption: The options to used.
         """
-        current_options = self.options
-        request_options = request.options.get(RedirectHandlerOption.get_key())  # type:ignore
-        # Override default options with request options
-        if request_options:
-            current_options = request_options
-
+        current_options = request.options.get( # type:ignore
+            RedirectHandlerOption.get_key(), self.options)
         return current_options
 
     def _build_redirect_request(
         self, request: httpx.Request, response: httpx.Response
     ) -> httpx.Request:
         """
         Given a request and a redirect response, return a new request that
```

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/retry_handler.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/retry_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import random
 import time
 from email.utils import parsedate_to_datetime
-from typing import FrozenSet, Set
+from typing import FrozenSet, Set, Type
 
 import httpx
+from kiota_abstractions.request_option import RequestOption
 
 from .middleware import BaseMiddleware
 from .options import RetryHandlerOption
 
 
 class RetryHandler(BaseMiddleware):
     """
@@ -48,21 +49,21 @@
     # 504 - Gateway timeout
     DEFAULT_RETRY_STATUS_CODES: Set[int] = {429, 503, 504}
 
     DEFAULT_ALLOWED_METHODS: FrozenSet[str] = frozenset(
         ['HEAD', 'GET', 'POST', 'PUT', 'PATCH', 'DELETE', 'OPTIONS']
     )
 
-    def __init__(self, options: RetryHandlerOption = RetryHandlerOption()) -> None:
+    def __init__(self, options: RequestOption = RetryHandlerOption()) -> None:
         super().__init__()
         self.allowed_methods: FrozenSet[str] = self.DEFAULT_ALLOWED_METHODS
         self.backoff_factor: float = self.DEFAULT_BACKOFF_FACTOR
         self.backoff_max: int = self.MAXIMUM_BACKOFF
         self.options = options
-        self.respect_retry_after_header: bool = options.DEFAULT_SHOULD_RETRY
+        self.respect_retry_after_header: bool = self.options.DEFAULT_SHOULD_RETRY  # type:ignore
         self.retry_on_status_codes: Set[int] = self.DEFAULT_RETRY_STATUS_CODES
 
     async def send(self, request: httpx.Request, transport: httpx.AsyncBaseTransport):
         """
         Sends the http request object to the next middleware or retries the request if necessary.
         """
         current_options = self._get_current_options(request)
@@ -103,20 +104,16 @@
 
         Args:
             request (httpx.Request): The prepared request object
 
         Returns:
             RetryHandlerOption: The options to used.
         """
-        current_options = self.options
-        request_options = request.options.get(RetryHandlerOption.get_key())  # type:ignore
-        # Override default options with request options
-        if request_options:
-            current_options = request_options
-
+        current_options = request.options.get( # type:ignore
+            RetryHandlerOption.get_key(), self.options)
         return current_options
 
     def should_retry(self, request, options, response):
         """
         Determines whether the request should be retried
         Checks if the request method is in allowed methods
         Checks if the response status code is in retryable status codes.
```

### Comparing `microsoft_kiota_http-0.4.4/kiota_http/middleware/url_replace_handler.py` & `microsoft_kiota_http-0.5.0/kiota_http/middleware/url_replace_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import httpx
+from kiota_abstractions.request_option import RequestOption
 
 from .middleware import BaseMiddleware
 from .options import UrlReplaceHandlerOption
 
 
 class UrlReplaceHandler(BaseMiddleware):
 
-    def __init__(self, options: UrlReplaceHandlerOption = UrlReplaceHandlerOption(), **kwargs):
+    def __init__(self, options: RequestOption = UrlReplaceHandlerOption()):
         """Create an instance of UrlReplaceHandler
 
         Args:
             options (UrlReplaceHandlerOption, optional): The url replacement
             options to pass to the handler.
             Defaults to UrlReplaceHandlerOption
         """
@@ -43,22 +44,17 @@
 
         Args:
             request (httpx.Request): The prepared request object
 
         Returns:
             UrlReplaceHandlerOption: The options to be used.
         """
-        current_options = self.options
-        request_options = request.options.get(  # type:ignore
-            UrlReplaceHandlerOption.get_key()
+        current_options =request.options.get(  # type:ignore
+            UrlReplaceHandlerOption.get_key(), self.options
         )
-        # Override default options with request options
-        if request_options:
-            current_options = request_options
-
         return current_options
 
     def replace_url_segment(self, url_str: str, current_options: UrlReplaceHandlerOption) -> str:
-        if (current_options and current_options.is_enabled and current_options.replacement_pairs):
+        if all([current_options, current_options.is_enabled, current_options.replacement_pairs]):
             for k, v in current_options.replacement_pairs.items():
                 url_str = url_str.replace(k, v, 1)
         return url_str
```

### Comparing `microsoft_kiota_http-0.4.4/pyproject.toml` & `microsoft_kiota_http-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/requirements-dev.txt` & `microsoft_kiota_http-0.5.0/requirements-dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 -i https://pypi.org/simple
 
-astroid==2.15.5
+astroid==2.15.6
 
 asyncmock==0.4.2
 
-certifi==2023.5.7
+certifi==2023.7.22
 
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
 
 colorama==0.4.6
 
 coverage[toml]==7.2.7
 
-dill==0.3.6
+dill==0.3.7
 
 docutils==0.20.1
 
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
 
 flit==3.9.0
 
 flit-core==3.9.0
 
 idna==3.4
 
@@ -28,69 +28,69 @@
 
 isort==5.12.0
 
 lazy-object-proxy==1.9.0
 
 mccabe==0.7.0
 
-mock==5.0.2
+mock==5.1.0
 
-mypy==1.3.0
+mypy==1.4.1
 
 mypy-extensions==1.0.0
 
 packaging==23.1
 
-platformdirs==3.5.1
+platformdirs==3.10.0
 
-pluggy==1.0.0
+pluggy==1.2.0
 
-pylint==2.17.4
+pylint==2.17.5
 
-pytest==7.3.1
+pytest==7.4.0
 
-pytest-asyncio==0.21.0
+pytest-asyncio==0.21.1
 
 pytest-cov==4.1.0
 
-pytest-mock==3.10.0
+pytest-mock==3.11.1
 
 requests==2.31.0
 
 toml==0.10.2
 
 tomli==2.0.1
 
 tomli-w==1.0.0
 
-tomlkit==0.11.8
+tomlkit==0.12.1
 
-types-python-dateutil==2.8.19.13
+types-python-dateutil==2.8.19.14
 
-typing-extensions==4.6.3
+typing-extensions==4.7.1
 
-urllib3==2.0.3
+urllib3==2.0.4
 
 wrapt==1.15.0
 
-yapf==0.33.0
+yapf==0.40.1
 
-anyio==3.7.0
+anyio==3.7.1
 
 h11==0.14.0
 
 h2==4.1.0
 
 hpack==4.0.0
 
-httpcore==0.17.2
+httpcore==0.17.3
 
 httpx[http2]==0.24.1
 
 hyperframe==6.0.1
 
-microsoft-kiota-abstractions==0.5.1
+microsoft-kiota-abstractions==0.7.0
 
 sniffio==1.3.0
 
 uritemplate==4.1.1
```

### Comparing `microsoft_kiota_http-0.4.4/tests/conftest.py` & `microsoft_kiota_http-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/tests/helpers/mock_response_object.py` & `microsoft_kiota_http-0.5.0/tests/helpers/mock_response_object.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/tests/middleware_tests/test_parameters_name_decoding_handler.py` & `microsoft_kiota_http-0.5.0/tests/middleware_tests/test_parameters_name_decoding_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/tests/middleware_tests/test_redirect_handler.py` & `microsoft_kiota_http-0.5.0/tests/middleware_tests/test_redirect_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/tests/middleware_tests/test_retry_handler.py` & `microsoft_kiota_http-0.5.0/tests/middleware_tests/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/tests/middleware_tests/test_url_replace_handler.py` & `microsoft_kiota_http-0.5.0/tests/middleware_tests/test_url_replace_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.4/tests/test_httpx_request_adapter.py` & `microsoft_kiota_http-0.5.0/tests/test_httpx_request_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     assert simple_error_response.text == '{"error": "not found"}'
     assert simple_error_response.status_code == 404
     content_type = request_adapter.get_response_content_type(simple_error_response)
     assert content_type == 'application/json'
 
     with pytest.raises(APIError) as e:
         await request_adapter.throw_failed_responses(simple_error_response, None)
-    assert str(e.value) == "The server returned an unexpected status code and"\
+    assert str(e.value.message) == "The server returned an unexpected status code and"\
             " no error class is registered for this code 404"
     assert e.value.response_status_code == 404
 
 
 @pytest.mark.asyncio
 async def test_throw_failed_responses_no_error_class(
     request_adapter, simple_error_response, mock_error_map
@@ -125,15 +125,15 @@
     assert simple_error_response.text == '{"error": "not found"}'
     assert simple_error_response.status_code == 404
     content_type = request_adapter.get_response_content_type(simple_error_response)
     assert content_type == 'application/json'
 
     with pytest.raises(APIError) as e:
         await request_adapter.throw_failed_responses(simple_error_response, mock_error_map)
-    assert str(e.value) == "The server returned an unexpected status code and"\
+    assert str(e.value.message) == "The server returned an unexpected status code and"\
             " no error class is registered for this code 404"
     assert e.value.response_status_code == 404
 
 
 @pytest.mark.asyncio
 async def test_throw_failed_responses_not_apierror(
     request_adapter, mock_error_map, mock_error_object
@@ -142,28 +142,28 @@
     resp = httpx.Response(status_code=500, headers={"Content-Type": "application/json"})
     assert resp.status_code == 500
     content_type = request_adapter.get_response_content_type(resp)
     assert content_type == 'application/json'
 
     with pytest.raises(Exception) as e:
         await request_adapter.throw_failed_responses(resp, mock_error_map)
-    assert str(e.value) == "Unexpected error type: <class 'Exception'>"
+    assert str(e.value.message) == "Unexpected error type: <class 'Exception'>"
 
 
 @pytest.mark.asyncio
 async def test_throw_failed_responses(request_adapter, mock_apierror_map, mock_error_object):
     request_adapter.get_root_parse_node = AsyncMock(return_value=mock_error_object)
     resp = httpx.Response(status_code=500, headers={"Content-Type": "application/json"})
     assert resp.status_code == 500
     content_type = request_adapter.get_response_content_type(resp)
     assert content_type == 'application/json'
 
     with pytest.raises(APIError) as e:
         await request_adapter.throw_failed_responses(resp, mock_apierror_map)
-    assert str(e.value) == "Custom Internal Server Error"
+    assert str(e.value.message) == "Custom Internal Server Error"
 
 
 @pytest.mark.asyncio
 async def test_send_async(request_adapter, request_info, mock_user_response, mock_user):
     request_adapter.get_http_response_message = AsyncMock(return_value=mock_user_response)
     request_adapter.get_root_parse_node = AsyncMock(return_value=mock_user)
     resp = await request_adapter.get_http_response_message(request_info)
@@ -214,29 +214,43 @@
 ):
     request_adapter.get_http_response_message = AsyncMock(return_value=mock_primitive_response)
     request_adapter.get_root_parse_node = AsyncMock(return_value=mock_primitive)
     resp = await request_adapter.get_http_response_message(request_info)
     assert resp.headers.get("content-type") == 'application/json'
     final_result = await request_adapter.send_primitive_async(request_info, "float", {})
     assert final_result == 22.3
-    
+
+
 @pytest.mark.asyncio
 async def test_send_primitive_async_bytes(
     request_adapter, request_info, mock_primitive_response_bytes, mock_primitive
 ):
-    request_adapter.get_http_response_message = AsyncMock(return_value=mock_primitive_response_bytes)
+    request_adapter.get_http_response_message = AsyncMock(
+        return_value=mock_primitive_response_bytes
+    )
     request_adapter.get_root_parse_node = AsyncMock(return_value=mock_primitive)
     resp = await request_adapter.get_http_response_message(request_info)
-    assert resp.headers.get("content-type") == 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'
+    assert resp.headers.get(
+        "content-type"
+    ) == 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'
     final_result = await request_adapter.send_primitive_async(request_info, "bytes", {})
     assert final_result == b'Hello World'
 
 
 @pytest.mark.asyncio
 async def test_send_primitive_async_no_content(
     request_adapter, request_info, mock_no_content_response
 ):
     request_adapter.get_http_response_message = AsyncMock(return_value=mock_no_content_response)
     resp = await request_adapter.get_http_response_message(request_info)
     assert resp.headers.get("content-type") == 'application/json'
     final_result = await request_adapter.send_primitive_async(request_info, float, {})
     assert final_result is None
+
+
+@pytest.mark.asyncio
+async def test_convert_to_native_async(request_adapter, request_info):
+    request_info.http_method = Method.GET
+    request_info.url = BASE_URL
+    request_info.content = bytes('hello world', 'utf_8')
+    req = await request_adapter.convert_to_native_async(request_info)
+    assert isinstance(req, httpx.Request)
```

### Comparing `microsoft_kiota_http-0.4.4/tests/test_kiota_client_factory.py` & `microsoft_kiota_http-0.5.0/tests/test_kiota_client_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import httpx
 import pytest
 
-from kiota_http import middleware
 from kiota_http.kiota_client_factory import KiotaClientFactory
 from kiota_http.middleware import (
-    AsyncKiotaTransport,
-    MiddlewarePipeline,
-    ParametersNameDecodingHandler,
-    RedirectHandler,
-    RetryHandler,
-    UrlReplaceHandler
+    AsyncKiotaTransport, MiddlewarePipeline, ParametersNameDecodingHandler, RedirectHandler,
+    RetryHandler, UrlReplaceHandler
 )
 from kiota_http.middleware.options import RedirectHandlerOption, RetryHandlerOption
+from kiota_http.middleware.user_agent_handler import UserAgentHandler
 
 
 def test_create_with_default_middleware():
     """Test creation of HTTP Client using default middleware"""
     client = KiotaClientFactory.create_with_default_middleware()
 
     assert isinstance(client, httpx.AsyncClient)
@@ -50,33 +46,34 @@
     assert isinstance(pipeline._first_middleware, RetryHandler)
 
 
 def test_get_default_middleware():
     """Test fetching of default middleware with no custom options passed"""
     middleware = KiotaClientFactory.get_default_middleware(None)
 
-    assert len(middleware) == 4
+    assert len(middleware) == 5
     assert isinstance(middleware[0], RedirectHandler)
     assert isinstance(middleware[1], RetryHandler)
     assert isinstance(middleware[2], ParametersNameDecodingHandler)
     assert isinstance(middleware[3], UrlReplaceHandler)
+    assert isinstance(middleware[4], UserAgentHandler)
 
 
 def test_get_default_middleware_with_options():
     """Test fetching of default middleware with custom options passed"""
     retry_options = RetryHandlerOption(max_retries=7)
     redirect_options = RedirectHandlerOption(should_redirect=False)
     options = {
         f'{retry_options.get_key()}': retry_options,
         f'{redirect_options.get_key()}': redirect_options
     }
 
     middleware = KiotaClientFactory.get_default_middleware(options=options)
 
-    assert len(middleware) == 4
+    assert len(middleware) == 5
     assert isinstance(middleware[0], RedirectHandler)
     assert middleware[0].options.should_redirect is False
     assert isinstance(middleware[1], RetryHandler)
     assert middleware[1].options.max_retry == 7
     assert isinstance(middleware[2], ParametersNameDecodingHandler)
```

### Comparing `microsoft_kiota_http-0.4.4/PKG-INFO` & `microsoft_kiota_http-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-http
-Version: 0.4.4
+Version: 0.5.0
 Summary: Kiota http request adapter implementation for httpx library
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

