# Comparing `tmp/pytest-playwright-0.3.3.tar.gz` & `tmp/pytest-playwright-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-0.3.3.tar", last modified: Mon Apr 24 19:29:19 2023, max compression
+gzip compressed data, was "pytest-playwright-0.4.0.tar", last modified: Mon Aug  7 09:02:44 2023, max compression
```

## Comparing `pytest-playwright-0.3.3.tar` & `pytest-playwright-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/local-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/pytest_playwright/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/pytest_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright/_repo_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/pytest_playwright/pytest_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/pytest_playwright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/tests/assets/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/assets/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/assets/django/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/assets/django/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/test_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.209586 pytest-playwright-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.209586 pytest-playwright-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/local-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/pytest_playwright/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/pytest_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright/_repo_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/pytest_playwright/pytest_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/pytest_playwright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 09:02:44.000000 pytest-playwright-0.4.0/pytest_playwright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.209586 pytest-playwright-0.4.0/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:44.213586 pytest-playwright-0.4.0/tests/assets/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/assets/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/assets/django/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/assets/django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-08-07 09:02:22.000000 pytest-playwright-0.4.0/tests/test_playwright.py
```

### Comparing `pytest-playwright-0.3.3/.gitignore` & `pytest-playwright-0.4.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -135,10 +135,13 @@
 
 # pytype static type analyzer
 .pytype/
 
 # End of https://www.toptal.com/developers/gitignore/api/python
 .vscode
 
+# Jetbrains IDEs
+.idea
+
 _repo_version.py
 .DS_Store
 /test-results/
```

### Comparing `pytest-playwright-0.3.3/.pre-commit-config.yaml` & `pytest-playwright-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.3/CONTRIBUTING.md` & `pytest-playwright-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.3/LICENSE` & `pytest-playwright-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.3/PKG-INFO` & `pytest-playwright-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.3.3
+Version: 0.4.0
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pytest plugin for Playwright [![PyPI](https://img.shields.io/pypi/v/pytest-playwright)](https://pypi.org/project/pytest-playwright/)
 
 Write end-to-end tests for your web apps with [Playwright](https://github.com/microsoft/playwright-python) and [pytest](https://docs.pytest.org/en/stable/).
```

### Comparing `pytest-playwright-0.3.3/README.md` & `pytest-playwright-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.3/SECURITY.md` & `pytest-playwright-0.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.3/pytest_playwright/pytest_playwright.py` & `pytest-playwright-0.4.0/pytest_playwright/pytest_playwright.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,18 @@
 def pytest_configure(config: Any) -> None:
     config.addinivalue_line(
         "markers", "skip_browser(name): mark test to be skipped a specific browser"
     )
     config.addinivalue_line(
         "markers", "only_browser(name): mark test to run only on a specific browser"
     )
+    config.addinivalue_line(
+        "markers",
+        "browser_context_args(**kwargs): provide additional arguments to browser.new_context()",
+    )
 
 
 # Making test result information available in fixtures
 # https://docs.pytest.org/en/latest/example/simple.html#making-test-result-information-available-in-fixtures
 @pytest.hookimpl(tryfirst=True, hookwrapper=True)
 def pytest_runtest_makereport(item: Any) -> Generator[None, Any, None]:
     # execute all other hooks to obtain the report object
@@ -223,14 +227,19 @@
 def context(
     browser: Browser,
     browser_context_args: Dict,
     pytestconfig: Any,
     request: pytest.FixtureRequest,
 ) -> Generator[BrowserContext, None, None]:
     pages: List[Page] = []
+
+    context_args_marker = next(request.node.iter_markers("browser_context_args"), None)
+    additional_context_args = context_args_marker.kwargs if context_args_marker else {}
+    browser_context_args.update(additional_context_args)
+
     context = browser.new_context(**browser_context_args)
     context.on("page", lambda page: pages.append(page))
 
     tracing_option = pytestconfig.getoption("--tracing")
     capture_trace = tracing_option in ["on", "retain-on-failure"]
     if capture_trace:
         context.tracing.start(
@@ -238,15 +247,15 @@
             screenshots=True,
             snapshots=True,
             sources=True,
         )
 
     yield context
 
-    # If requst.node is missing rep_call, then some error happened during execution
+    # If request.node is missing rep_call, then some error happened during execution
     # that prevented teardown, but should still be counted as a failure
     failed = request.node.rep_call.failed if hasattr(request.node, "rep_call") else True
 
     if capture_trace:
         retain_trace = tracing_option == "on" or (
             failed and tracing_option == "retain-on-failure"
         )
@@ -263,15 +272,19 @@
     if capture_screenshot:
         for index, page in enumerate(pages):
             human_readable_status = "failed" if failed else "finished"
             screenshot_path = _build_artifact_test_folder(
                 pytestconfig, request, f"test-{human_readable_status}-{index+1}.png"
             )
             try:
-                page.screenshot(timeout=5000, path=screenshot_path)
+                page.screenshot(
+                    timeout=5000,
+                    path=screenshot_path,
+                    full_page=pytestconfig.getoption("--full-page-screenshot"),
+                )
             except Error:
                 pass
 
     context.close()
 
     video_option = pytestconfig.getoption("--video")
     preserve_video = video_option == "on" or (
@@ -388,7 +401,13 @@
     )
     group.addoption(
         "--screenshot",
         default="off",
         choices=["on", "off", "only-on-failure"],
         help="Whether to automatically capture a screenshot after each test.",
     )
+    group.addoption(
+        "--full-page-screenshot",
+        action="store_true",
+        default=False,
+        help="Whether to take a full page screenshot",
+    )
```

### Comparing `pytest-playwright-0.3.3/pytest_playwright.egg-info/PKG-INFO` & `pytest-playwright-0.4.0/pytest_playwright.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.3.3
+Version: 0.4.0
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pytest plugin for Playwright [![PyPI](https://img.shields.io/pypi/v/pytest-playwright)](https://pypi.org/project/pytest-playwright/)
 
 Write end-to-end tests for your web apps with [Playwright](https://github.com/microsoft/playwright-python) and [pytest](https://docs.pytest.org/en/stable/).
```

### Comparing `pytest-playwright-0.3.3/pytest_playwright.egg-info/SOURCES.txt` & `pytest-playwright-0.4.0/pytest_playwright.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
 SECURITY.md
+conda_build_config.yaml
 local-requirements.txt
+meta.yaml
 setup.cfg
 setup.py
 .github/workflows/ci.yml
 .github/workflows/python-publish.yml
 pytest_playwright/__init__.py
 pytest_playwright/_repo_version.py
 pytest_playwright/pytest_playwright.py
```

### Comparing `pytest-playwright-0.3.3/setup.py` & `pytest-playwright-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,23 @@
         "pytest>=6.2.4,<8.0.0",
         "pytest-base-url>=1.0.0,<3.0.0",
         "python-slugify>=6.0.0,<9.0.0",
     ],
     entry_points={"pytest11": ["playwright = pytest_playwright.pytest_playwright"]},
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Framework :: Pytest",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     use_scm_version={
         "version_scheme": "post-release",
         "write_to": "pytest_playwright/_repo_version.py",
         "write_to_template": 'version = "{version}"\n',
     },
     setup_requires=["setuptools_scm"],
 )
```

### Comparing `pytest-playwright-0.3.3/tests/assets/django/settings.py` & `pytest-playwright-0.4.0/tests/assets/django/settings.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.3/tests/conftest.py` & `pytest-playwright-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.3/tests/test_playwright.py` & `pytest-playwright-0.4.0/tests/test_playwright.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,38 @@
             assert page.evaluate("window.navigator.userAgent") == "foobar"
     """
     )
     result = testdir.runpytest()
     result.assert_outcomes(passed=1)
 
 
+def test_user_defined_browser_context_args(testdir: pytest.Testdir) -> None:
+    testdir.makeconftest(
+        """
+        import pytest
+
+        @pytest.fixture(scope="session")
+        def browser_context_args():
+            return {"user_agent": "foobar"}
+    """
+    )
+    testdir.makepyfile(
+        """
+        import pytest
+
+        @pytest.mark.browser_context_args(user_agent="overwritten", locale="new-locale")
+        def test_browser_context_args(page):
+            assert page.evaluate("window.navigator.userAgent") == "overwritten"
+            assert page.evaluate("window.navigator.languages") == ["new-locale"]
+    """
+    )
+    result = testdir.runpytest()
+    result.assert_outcomes(passed=1)
+
+
 def test_chromium(testdir: pytest.Testdir) -> None:
     testdir.makepyfile(
         """
         def test_is_chromium(page, browser_name, is_chromium, is_firefox, is_webkit):
             assert browser_name == "chromium"
             assert is_chromium
             assert is_firefox is False
@@ -688,7 +712,29 @@
             else:
                 assert os.path.isfile(os.path.join(root, file["name"]))
         if isinstance(file["name"], re.Pattern):
             assert any([file["name"].match(item) for item in os.listdir(root)])
             assert "children" not in file
         if "children" in file:
             _assert_folder_tree(os.path.join(root, file["name"]), file["children"])
+
+
+def test_is_able_to_set_expect_timeout_via_conftest(testdir: pytest.Testdir) -> None:
+    testdir.makeconftest(
+        """
+        from playwright.sync_api import expect
+        expect.set_options(timeout=1111)
+    """
+    )
+    testdir.makepyfile(
+        """
+        from playwright.sync_api import expect
+
+        def test_small_timeout(page):
+            page.goto("data:text/html,")
+            expect(page.locator("#A")).to_be_visible()
+    """
+    )
+    result = testdir.runpytest()
+    result.assert_outcomes(passed=0, failed=1, skipped=0)
+    result.stdout.fnmatch_lines("*AssertionError: Locator expected to be visible*")
+    result.stdout.fnmatch_lines("*LocatorAssertions.to_be_visible with timeout 1111ms*")
```

